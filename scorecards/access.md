---
layout: default
title: Unlock All Scorecards
permalink: /scorecards/access/
---
<section class="hero">
  <h1>Unlock All Scorecards</h1>
  <p><strong>Enter your info once to get instant access to every Maven scorecard and assessment.</strong></p>
</section>

<div class="card" style="padding:22px; max-width:600px; margin:0 auto;">
  <iframe id="ziframe_335311" aria-label="Maximo Resource Access Form" frameborder="0" style="height:500px;width:99%;border:none;transition:all 0.3s ease;" src="https://forms.zohopublic.com/mavenassetmanagement1/form/MaximoResourceAccessForm/formperma/Tlj13YNyv63v-3XDiHZzviZD-pA_lFDrmJr3VLpi5I4">
  </iframe>
</div>

<script>
(function() {
  var params = new URLSearchParams(window.location.search);
  var redirect = params.get('redirect') || '{{ "/scorecards/" | relative_url }}';
  var iframe = document.getElementById('ziframe_335311');

  window.addEventListener('message', function(event) {
    try {
      // Auto-resize handler: Zoho sends "permalink|heightInPx" as a plain string
      if (typeof event.data === 'string' && event.data.indexOf('|') > -1) {
        var parts = event.data.split('|');
        var perma = parts[0];
        var newHeight = (parseInt(parts[1], 10) + 15) + 'px';
        if (iframe.src.indexOf('formperma') > 0 && iframe.src.indexOf(perma) > 0) {
          iframe.style.height = newHeight;
        }
        return;
      }

      // Submission handler: Zoho's GTM postMessage tracking
      var u = new URL(event.origin);
      if (u.host !== "forms.zohopublic.com") return;

      var evntData = event.data;
      if (evntData && evntData.constructor === Object && evntData.type === "zf_gtm") {
        var payload = evntData.payload;
        if (payload && payload.e === "zf_submitform") {
          localStorage.setItem('maven_scorecard_unlocked', 'true');
          window.location.href = redirect;
        }
      }
    } catch (error) {
      // ignore malformed messages
    }
  }, false);
})();
</script>

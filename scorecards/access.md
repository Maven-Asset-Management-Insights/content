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
  <div id="zoho-form-wrapper"></div>
</div>

<script>
(function() {
  var params = new URLSearchParams(window.location.search);
  var redirect = params.get('redirect') || '{{ "/scorecards/" | relative_url }}';

  var baseSrc = "PASTE_YOUR_ZOHO_IFRAME_SRC_HERE";
  var src = baseSrc + "?redirect=" + encodeURIComponent(redirect);

  var iframe = document.createElement('iframe');
  iframe.src = src;
  iframe.style.width = "100%";
  iframe.style.height = "600px";
  iframe.style.border = "none";
  document.getElementById('zoho-form-wrapper').appendChild(iframe);
})();
</script>

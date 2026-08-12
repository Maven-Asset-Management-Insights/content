---
layout: default
title: Access Granted
permalink: /scorecards/unlocked/
---

<section class="hero">
  <h1>You're all set!</h1>
  <p><strong>Redirecting you to your scorecard...</strong></p>
</section>

<div class="card" style="padding:22px; max-width:520px; margin:0 auto; text-align:center;">
  <p>If you're not redirected automatically in a few seconds, <a id="manual-redirect-link" href="{{ "/scorecards/" | relative_url }}">click here</a>.</p>
</div>

<script>
(function() {
  localStorage.setItem('maven_scorecard_unlocked', Date.now());

  var params = new URLSearchParams(window.location.search);
  var redirect = params.get('redirect') || '{{ "/scorecards/" | relative_url }}';

  var link = document.getElementById('manual-redirect-link');
  if (link) { link.setAttribute('href', redirect); }

var scorecardLabels = {
  '{{ "/scorecards/data-readiness-check/" | relative_url }}': 'Maximo Data Readiness Check',
  '{{ "/scorecards/work-management-assessment/" | relative_url }}': 'Maximo Work Management Value Assessment',
  '{{ "/scorecards/planning-value-assessment/" | relative_url }}': 'Maximo Planning Value Assessment',
  '{{ "/scorecards/scheduling-value-assessment/" | relative_url }}': 'Maximo Scheduling Value Assessment',
  '{{ "/scorecards/reliability-value-assessment/" | relative_url }}': 'Maximo Reliability Value Assessment',
  '{{ "/scorecards/asset-health-value-assessment/" | relative_url }}': 'Maximo Asset Health Value Assessment',
  '{{ "/scorecards/iot-value-assessment/" | relative_url }}': 'Maximo IoT Value Assessment',
  '{{ "/scorecards/time-management-value-assessment/" | relative_url }}': 'Maximo Time Management Value Assessment',
  '{{ "/scorecards/capability-assessment/" | relative_url }}': 'Maximo Capability Assessment',
  '{{ "/scorecards/hse-readiness-assessment/" | relative_url }}': 'Maximo HS&E Readiness Assessment',
  '{{ "/field-kits/maximo-readiness-scorecard.html" | relative_url }}': 'Maximo Readiness Scorecard (Printable)'
};
  var scorecardLabel = scorecardLabels[redirect] || redirect;

  if (typeof gtag === 'function') {
    gtag('event', 'scorecard_unlock', { 'scorecard_name': scorecardLabel, 'redirect_target': redirect });
  }

  window.location.href = redirect;
})();
</script>

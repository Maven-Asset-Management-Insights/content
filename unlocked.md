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
  <p>If you're not redirected automatically in a few seconds, <a id="manual-redirect-link" href="/scorecards/">click here</a>.</p>
</div>

<script>
(function() {
  // Mark this visitor as unlocked
  localStorage.setItem('maven_scorecard_unlocked', Date.now());

  // Figure out where they were headed
  var params = new URLSearchParams(window.location.search);
  var redirect = params.get('redirect') || '/scorecards/';

  // Update the manual fallback link in case JS redirect is delayed/blocked
  var link = document.getElementById('manual-redirect-link');
  if (link) {
    link.setAttribute('href', redirect);
  }

  // Map redirect paths to friendly scorecard names for analytics
  var scorecardLabels = {
    '/scorecards/data-readiness-check/': 'Maximo Data Readiness Check',
    '/scorecards/work-management-assessment/': 'Maximo Work Management Value Assessment',
    '/scorecards/hse-readiness-assessment/': 'Maximo HS&E Readiness Assessment',
    '/field-kits/maximo-readiness-scorecard.html': 'Maximo Readiness Scorecard (Printable)',
    '/scorecards/ai-readiness-assessment/': 'AI Readiness Assessment'
  };
  var scorecardLabel = scorecardLabels[redirect] || redirect;

  // Fire a GA4 event so gate conversions are trackable separately, by scorecard
  if (typeof gtag === 'function') {
    gtag('event', 'scorecard_unlock', {
      'scorecard_name': scorecardLabel,
      'redirect_target': redirect
    });
  }

  // Redirect to the requested scorecard
  window.location.href = redirect;
})();
</script>

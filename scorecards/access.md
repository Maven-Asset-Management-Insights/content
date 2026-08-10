---
layout: default
title: Unlock All Scorecards
permalink: /scorecards/access/
---
<section class="hero">
  <h1>Unlock All Scorecards</h1>
  <p><strong>Enter your info once to get instant access to every Maven scorecard and assessment.</strong></p>
</section>

<div class="card" style="padding:22px; max-width:480px; margin:0 auto;">
  <form id="accessForm">
    <div style="display:flex; gap:12px; margin-bottom:14px;">
      <div style="flex:1;">
        <label style="display:block; font-weight:600; margin-bottom:6px;">First Name</label>
        <input type="text" id="firstNameField" style="width:100%; padding:10px; border:1px solid #ccc; border-radius:6px;" />
      </div>
      <div style="flex:1;">
        <label style="display:block; font-weight:600; margin-bottom:6px;">Last Name</label>
        <input type="text" id="lastNameField" style="width:100%; padding:10px; border:1px solid #ccc; border-radius:6px;" />
      </div>
    </div>
    <div style="margin-bottom:14px;">
      <label style="display:block; font-weight:600; margin-bottom:6px;">Company *</label>
      <input type="text" id="companyField" required style="width:100%; padding:10px; border:1px solid #ccc; border-radius:6px;" />
    </div>
    <div style="margin-bottom:18px;">
      <label style="display:block; font-weight:600; margin-bottom:6px;">Work Email *</label>
      <input type="email" id="emailField" required style="width:100%; padding:10px; border:1px solid #ccc; border-radius:6px;" />
    </div>
    <button type="submit" class="button" style="width:100%; cursor:pointer;">Unlock Scorecards</button>
    <p id="formError" style="color:#C0392B; font-size:0.9rem; margin-top:10px; display:none;"></p>
  </form>
</div>

<script>
(function() {
  var params = new URLSearchParams(window.location.search);
  var redirect = params.get('redirect') || '{{ "/scorecards/" | relative_url }}';

  var FORM_ACTION = "https://docs.google.com/forms/d/e/1FAIpQLSfMx_zeTRqnk0hl78ED_EIb8iLghxBwUHwpCFYyjMxK9hKXWQ/formResponse";
  var FIRST_NAME_ENTRY = "entry.1773261783";
  var LAST_NAME_ENTRY = "entry.1478130085";
  var COMPANY_ENTRY = "entry.1072261245";
  var EMAIL_ENTRY = "entry.1057769451";

  var BLOCKED_DOMAINS = [
    "gmail.com", "yahoo.com", "hotmail.com", "outlook.com", "aol.com",
    "icloud.com", "live.com", "msn.com", "protonmail.com", "mail.com",
    "gmx.com", "yandex.com", "zoho.com"
  ];

  var form = document.getElementById('accessForm');
  var errorMsg = document.getElementById('formError');

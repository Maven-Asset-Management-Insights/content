---
layout: default
title: Unlock All Scorecards
permalink: /scorecards/access/
---
<section class="hero">
  <h1>Unlock All Scorecards</h1>
  <p><strong>Enter your info once to get instant access to every Maven scorecard and assessment.</strong></p>
</section>

<div class="card" style="padding:26px; max-width:560px; margin:0 auto;">
<form action='https://forms.zohopublic.com/mavenassetmanagement1/form/MaximoResourceAccessForm/formperma/0B6AVXJGZI3vmGvv1KhcFFpJ6bM4E_XUhrtioLROo-I/htmlRecords/submit' name='form' id='form' method='POST' accept-charset='UTF-8' enctype='multipart/form-data' onsubmit="return zf_ValidateForm();">
<input type="hidden" name="zf_referrer_name" value="MavenScorecardsGate">
<input type="hidden" name="zf_redirect_url" id="zf_redirect_url_field" value="">
<input type="hidden" name="zc_gad" value="">

<div style="margin-bottom:16px;">
  <label style="display:block; font-weight:600; margin-bottom:6px;">Full Name <span style="color:#C0392B;">*</span></label>
  <div style="display:flex; gap:12px;">
    <div style="flex:1;">
      <input type="text" maxlength="255" name="Name_First" fieldType=7 placeholder="First Name" style="width:100%; padding:10px; border:1px solid #ccc; border-radius:6px;" />
    </div>
    <div style="flex:1;">
      <input type="text" maxlength="255" name="Name_Last" fieldType=7 placeholder="Last Name" style="width:100%; padding:10px; border:1px solid #ccc; border-radius:6px;" />
    </div>
  </div>
  <p id="Name_error" style="color:#C0392B; font-size:0.9rem; margin-top:6px; display:none;">Please enter your first and last name.</p>
</div>

<div style="margin-bottom:16px;">
  <label style="display:block; font-weight:600; margin-bottom:6px;">Work Email Address <span style="color:#C0392B;">*</span></label>
  <input type="text" maxlength="255" name="Email" id="Email_field" value="" fieldType=9 placeholder="you@company.com" style="width:100%; padding:10px; border:1px solid #ccc; border-radius:6px;" />
  <p id="Email_error" style="color:#C0392B; font-size:0.9rem; margin-top:6px; display:none;"></p>
</div>

<div style="margin-bottom:16px;">
  <label style="display:block; font-weight:600; margin-bottom:6px;">Job Title</label>
  <input type="text" name="SingleLine" value="" fieldType=1 maxlength="255" placeholder="" style="width:100%; padding:10px; border:1px solid #ccc; border-radius:6px;" />
</div>

<div style="margin-bottom:20px;">
  <label style="display:block; font-weight:600; margin-bottom:8px;">What are you hoping to accomplish?</label>
  <div style="display:flex; flex-direction:column; gap:8px;">
    <label style="font-weight:400;"><input type="checkbox" id="Checkbox_1" name="Checkbox" value="Improve an existing Maximo system" /> Improve an existing Maximo system</label>
    <label style="font-weight:400;"><input type="checkbox" id="Checkbox_2" name="Checkbox" value="Upgrade to MAS" /> Upgrade to MAS</label>
    <label style="font-weight:400;"><input type="checkbox" id="Checkbox_3" name="Checkbox" value="Implement Maximo" /> Implement Maximo</label>
    <label style="font-weight:400;"><input type="checkbox" id="Checkbox_4" name="Checkbox" value="Improve maintenance processes" /> Improve maintenance processes</label>
    <label style="font-weight:400;"><input type="checkbox" id="Checkbox_5" name="Checkbox" value="Learn Maximo best practices" /> Learn Maximo best practices</label>
    <label style="font-weight:400;"><input id="Checkbox_others" type="checkbox" value="zfs-others-zfs" name="Checkbox" /> Other</label>
    <input name="Checkbox_allow_others_text" type="text" maxlength="150" style="padding:8px; border:1px solid #ccc; border-radius:6px;" />
  </div>
</div>

<button type="submit" class="button" style="width:100%; border:none; cursor:pointer;">Submit</button>
</form>
</div>

<script>
var BLOCKED_DOMAINS = [
  "gmail.com", "yahoo.com", "hotmail.com", "outlook.com", "aol.com",
  "icloud.com", "live.com", "msn.com", "protonmail.com", "mail.com",
  "gmx.com", "yandex.com", "zoho.com"
];

// Set the dynamic redirect target in case Zoho ever honors the hidden field
(function() {
  var params = new URLSearchParams(window.location.search);
  var target = params.get('redirect') || '{{ "/scorecards/" | relative_url }}';
  var bridgeUrl = window.location.origin + '{{ "/scorecards/unlocked/" | relative_url }}' + '?redirect=' + encodeURIComponent(target);
  document.getElementById('zf_redirect_url_field').value = bridgeUrl;
})();

function zf_ValidateForm() {
  var first = document.forms.form["Name_First"].value.trim();
  var last = document.forms.form["Name_Last"].value.trim();
  var email = document.getElementById('Email_field').value.trim();
  var nameError = document.getElementById('Name_error');
  var emailError = document.getElementById('Email_error');

  nameError.style.display = 'none';
  emailError.style.display = 'none';

  if (!first || !last) {
    nameError.style.display = 'block';
    return false;
  }

  var emailValid = /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
  if (!emailValid) {
    emailError.textContent = 'Please enter a valid email address.';
    emailError.style.display = 'block';
    return false;
  }

  var domain = email.substring(email.indexOf('@') + 1).toLowerCase();
  if (BLOCKED_DOMAINS.indexOf(domain) !== -1) {
    emailError.textContent = 'Please use your work email address.';
    emailError.style.display = 'block';
    return false;
  }

  return true;
}
</script>

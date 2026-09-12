<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AI Readiness Assessment — Result</title>
<style>
  :root{
    --navy:#292C75;
    --blue:#3E67B1;
    --gray:#545454;
    --offwhite:#FAFAF9;
    --red:#C94C3D;
    --amber:#E8A33D;
    --green:#2E9E5B;
    --tint:#E9EDF7;
  }
  *{box-sizing:border-box;}
  body{
    margin:0;
    background:var(--offwhite);
    font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;
    color:var(--gray);
    display:flex;
    justify-content:center;
    padding:32px 16px 64px;
  }
  .screen{
    width:100%;
    max-width:600px;
    background:#fff;
    border-radius:4px;
    overflow:hidden;
    box-shadow:0 1px 3px rgba(41,44,117,0.12);
  }
  .header{
    background:linear-gradient(120deg,var(--navy) 60%,var(--blue));
    color:#fff;
    padding:22px 28px;
  }
  .eyebrow{
    font-size:11px;
    letter-spacing:1.5px;
    text-transform:uppercase;
    color:#B9C2E8;
    font-weight:700;
    margin:0 0 4px;
  }
  .header h1{
    margin:0 0 8px;
    font-size:21px;
    font-weight:700;
    line-height:1.3;
  }
  .header .badge{
    display:inline-block;
    font-size:11.5px;
    font-weight:700;
    letter-spacing:0.3px;
    color:#292C75;
    background:#fff;
    padding:4px 10px;
    border-radius:999px;
  }

  .panel{ padding:32px 28px 8px; }

  /* Gauge */
  .gauge-wrap{ text-align:center; margin-bottom:8px; }
  .tier-row{
    display:flex;
    justify-content:space-between;
    max-width:320px;
    margin:6px auto 0;
    font-size:11px;
    font-weight:700;
    letter-spacing:0.4px;
  }
  .tier-row span:nth-child(1){color:var(--red);}
  .tier-row span:nth-child(2){color:var(--amber);}
  .tier-row span:nth-child(3){color:var(--green);}
  .score-num{
    font-size:34px;
    font-weight:900;
    color:var(--navy);
    margin:10px 0 0;
  }
  .score-num small{ font-size:16px; font-weight:400; color:var(--gray); }

  .result-label{
    text-align:center;
    margin:18px 0 6px;
  }
  .result-label .tag{
    display:inline-block;
    font-size:11px;
    letter-spacing:1px;
    text-transform:uppercase;
    color:#8A90B8;
    font-weight:700;
    margin-bottom:4px;
  }
  .result-label .tier{
    font-size:26px;
    font-weight:900;
    color:var(--amber);
  }
  .result-copy{
    font-size:15px;
    line-height:1.55;
    text-align:center;
    max-width:440px;
    margin:0 auto 24px;
  }

  /* Benchmark strip */
  .benchmark{
    background:var(--tint);
    border-radius:6px;
    padding:16px 20px;
    display:flex;
    align-items:center;
    gap:16px;
    margin:0 0 26px;
  }
  .benchmark .stat{
    font-size:28px;
    font-weight:900;
    color:var(--blue);
    line-height:1;
    white-space:nowrap;
  }
  .benchmark p{
    margin:0;
    font-size:13.5px;
    line-height:1.4;
    color:var(--navy);
  }

  /* Recommended next scorecard */
  .next-up{
    border:1px solid #DCE1F2;
    border-radius:6px;
    padding:20px;
    margin-bottom:26px;
    position:relative;
  }
  .next-up .flag{
    font-size:11px;
    font-weight:700;
    letter-spacing:0.4px;
    text-transform:uppercase;
    color:var(--blue);
    margin:0 0 8px;
  }
  .next-up h3{
    margin:0 0 8px;
    font-size:17px;
    color:var(--navy);
  }
  .preview-line{
    filter:blur(3.5px);
    user-select:none;
    font-size:13.5px;
    color:#9096B8;
    line-height:1.5;
    margin:0 0 4px;
  }
  .lock-row{
    display:flex;
    align-items:center;
    gap:6px;
    margin-top:10px;
    font-size:12.5px;
    color:var(--gray);
    font-weight:700;
  }
  .lock-row svg{ width:13px; height:13px; }

  /* Library strip */
  .library{ margin:0 0 28px; }
  .library h4{
    font-size:12px;
    letter-spacing:0.6px;
    text-transform:uppercase;
    color:var(--navy);
    margin:0 0 10px;
  }
  .chip-grid{
    display:flex;
    flex-wrap:wrap;
    gap:8px;
  }
  .chip{
    display:flex;
    align-items:center;
    gap:6px;
    background:var(--tint);
    color:var(--navy);
    font-size:12.5px;
    font-weight:600;
    padding:7px 12px;
    border-radius:999px;
  }
  .chip svg{
    width:11px;
    height:11px;
    flex:none;
    color:#8A90B8;
  }

  /* Unlock list */
  .unlock{
    margin:0 0 28px;
  }
  .unlock h4{
    font-size:12px;
    letter-spacing:0.6px;
    text-transform:uppercase;
    color:var(--navy);
    margin:0 0 10px;
  }
  .unlock ul{
    list-style:none;
    margin:0;
    padding:0;
  }
  .unlock li{
    display:flex;
    gap:10px;
    align-items:flex-start;
    font-size:14px;
    line-height:1.5;
    margin-bottom:8px;
  }
  .unlock li svg{
    flex:none;
    width:15px;
    height:15px;
    margin-top:2px;
    color:var(--green);
  }

  /* Capture form */
  .capture{
    background:var(--navy);
    margin:0 -28px;
    padding:26px 28px 30px;
  }
  .capture h3{
    color:#fff;
    font-size:16px;
    margin:0 0 4px;
  }
  .capture p.sub{
    color:#B9C2E8;
    font-size:13px;
    margin:0 0 16px;
  }
  .capture form{
    display:flex;
    gap:8px;
  }
  .capture input[type=email]{
    flex:1;
    padding:12px 14px;
    border-radius:4px;
    border:none;
    font-size:14px;
    font-family:inherit;
  }
  .capture button{
    background:#fff;
    color:var(--navy);
    border:none;
    border-radius:4px;
    padding:12px 18px;
    font-size:14px;
    font-weight:700;
    cursor:pointer;
    white-space:nowrap;
  }
  .capture button:hover{ background:var(--tint); }
  .trust{
    color:#8A90B8;
    font-size:11.5px;
    margin:10px 0 0;
  }

  .footer-links{
    text-align:center;
    padding:18px 28px 26px;
    font-size:12.5px;
  }
  .footer-links a{
    color:var(--blue);
    text-decoration:none;
  }
  .footer-links a:hover{ text-decoration:underline; }
</style>
</head>
<body>

<div class="screen">

  <div class="header">
    <p class="eyebrow">Maven Asset Management &middot; Free, no sign-up</p>
    <h1>AI Readiness Assessment for Maximo &amp; EAM Programs</h1>
    <span class="badge">15 Questions &middot; 30 Points</span>
  </div>

  <div class="panel">

    <div class="gauge-wrap">
      <svg width="220" height="120" viewBox="0 0 220 120">
        <path d="M20,110 A90,90 0 0,1 65,32" fill="none" stroke="#C94C3D" stroke-width="14" stroke-linecap="round"/>
        <path d="M65,32 A90,90 0 0,1 155,32" fill="none" stroke="#E8A33D" stroke-width="14" stroke-linecap="round"/>
        <path d="M155,32 A90,90 0 0,1 200,110" fill="none" stroke="#2E9E5B" stroke-width="14" stroke-linecap="round"/>
        <line x1="110" y1="110" x2="103" y2="46" stroke="#292C75" stroke-width="4" stroke-linecap="round"/>
        <circle cx="110" cy="110" r="7" fill="#292C75"/>
      </svg>
      <div class="tier-row">
        <span>Foundation First</span><span>Proceed</span><span>Ready to Scale</span>
      </div>
      <p class="score-num">14<small> / 30</small></p>
    </div>

    <div class="result-label">
      <p class="tag">Your Result</p>
      <p class="tier">Proceed</p>
    </div>
    <p class="result-copy">Your foundation has real gaps, but you're not starting from zero. AI pilots can work in isolated cases. Scaling past the pilot stage means shoring up the data and integration work first.</p>

    <div class="benchmark">
      <div class="stat">58%</div>
      <p>of Maximo teams land in Foundation First or Proceed on this check. Data foundation is the category most teams underestimate.</p>
    </div>

    <div class="next-up">
      <p class="flag">Recommended next, based on your data foundation answers</p>
      <h3>Maximo Data Readiness Check</h3>
      <p class="preview-line">"When technicians close a work order, how do they record what went..."</p>
      <div class="lock-row">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>
        8 questions &middot; unlocks with sign-up
      </div>
    </div>

    <div class="library">
      <h4>Plus the rest of the library</h4>
      <div class="chip-grid">
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>Work Management</span>
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>Planning</span>
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>Scheduling</span>
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>Reliability</span>
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>Asset Health</span>
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>IoT</span>
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>Time Management</span>
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>Capability</span>
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>HS&amp;E Readiness</span>
        <span class="chip"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="5" y="11" width="14" height="9" rx="1.5"/><path d="M8 11V7a4 4 0 0 1 8 0v4"/></svg>Readiness Scorecard</span>
      </div>
    </div>

    <div class="unlock">
      <h4>What signing up gets you</h4>
      <ul>
        <li><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path d="M20 6 9 17l-5-5"/></svg> All 11 remaining scorecards, unlocked right now</li>
        <li><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path d="M20 6 9 17l-5-5"/></svg> Every new scorecard we publish, automatically</li>
        <li><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path d="M20 6 9 17l-5-5"/></svg> A downloadable PDF of each result</li>
      </ul>
    </div>

  </div>

  <div class="capture">
    <h3>Unlock the rest with one email</h3>
    <p class="sub">Starting with the Maximo Data Readiness Check, matched to what you just told us.</p>
    <form onsubmit="return false;">
      <input type="email" placeholder="you@company.com" required>
      <button type="submit">Unlock my results</button>
    </form>
    <p class="trust">No spam, ever — just access. Unsubscribe anytime.</p>
  </div>

  <div class="footer-links">
    <a href="#">Talk to Maven</a> &nbsp;&middot;&nbsp; <a href="#">Download this result only</a>
  </div>

</div>

</body>
</html>

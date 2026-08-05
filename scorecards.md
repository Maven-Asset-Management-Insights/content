---
layout: default
title: Scorecards & Assessments
permalink: /scorecards/
---

<style>
  .scorecard-visual {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 14px;
  }
  .scorecard-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 48px;
    height: 48px;
    min-width: 48px;
    border-radius: 10px;
    background: var(--scorecard-icon-bg, #EAF2F6);
  }
  .scorecard-icon svg {
    width: 26px;
    height: 26px;
    stroke: var(--scorecard-icon-color, #1B6B93);
    fill: none;
    stroke-width: 1.8;
    stroke-linecap: round;
    stroke-linejoin: round;
  }
  .scorecard-badge {
    display: inline-block;
    padding: 4px 10px;
    border-radius: 999px;
    background: var(--scorecard-badge-bg, #FFF4E5);
    color: var(--scorecard-badge-color, #B9691E);
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.02em;
    text-transform: uppercase;
    white-space: nowrap;
  }
  .scorecard-visual .scorecard-meta {
    display: flex;
    flex-direction: column;
    gap: 4px;
  }
  .scorecard-kicker {
    letter-spacing: .08em;
    text-transform: uppercase;
    font-size: .85rem;
    opacity: .75;
  }
</style>

<section class="hero">
  <h1>Scorecards &amp; Assessments</h1>
  <p><strong>Interactive and printable tools to quickly assess where your Maximo program stands — and where to focus next.</strong></p>
</section>

<!-- FEATURED SCORECARD -->
<div class="card" style="padding:22px; margin-bottom:18px;">
  <div class="scorecard-visual">
    <div class="scorecard-icon">
      <!-- AI / circuit-brain icon -->
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M9 4.5a2.5 2.5 0 0 0-2.5 2.5v.2A2.8 2.8 0 0 0 4.5 10v1a2.8 2.8 0 0 0 2 2.68V15a2.5 2.5 0 0 0 2.5 2.5" />
        <path d="M15 4.5a2.5 2.5 0 0 1 2.5 2.5v.2a2.8 2.8 0 0 1 2 2.8v1a2.8 2.8 0 0 1-2 2.68V15a2.5 2.5 0 0 1-2.5 2.5" />
        <path d="M9 4.5h6" />
        <path d="M9 17.5h6" />
        <circle cx="9" cy="9.5" r="0.9" fill="var(--scorecard-icon-color, #1B6B93)" stroke="none" />
        <circle cx="15" cy="9.5" r="0.9" fill="var(--scorecard-icon-color, #1B6B93)" stroke="none" />
        <circle cx="12" cy="13" r="0.9" fill="var(--scorecard-icon-color, #1B6B93)" stroke="none" />
        <path d="M9 9.5h2.3M15 9.5h-2.3M12 13v-1.7" />
      </svg>
    </div>
    <div class="scorecard-meta">
      <div class="scorecard-kicker">Featured Scorecard</div>
      <span class="scorecard-badge">15 Questions · 30 Points</span>
    </div>
  </div>

  <h2 style="margin-top:0;">AI Readiness Assessment for Maximo &amp; EAM Programs</h2>
  <div style="margin-top:10px;">
    <a class="button" href="{{ "/scorecards/ai-readiness-assessment/" | relative_url }}">Take the assessment</a>
  </div>
  <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
    A 15-question interactive scorecard that scores whether your data foundation, integration architecture, and use case clarity are ready to support meaningful AI investment in Maximo and MAS. 30 points total.
  </p>
  <div style="margin-top:14px; opacity:.8;">
    Best for: EAM program owners, operations leaders, IT leads, and reliability teams evaluating AI or MAS analytics capabilities
  </div>
  <div style="margin-top:10px; color:#27AE60; font-weight:600; font-size:0.95rem;">
    Get a feel for our scorecards with this one first — open access, no email needed. Then sign up once to unlock the full library, including every scorecard we add going forward.
  </div>
</div>

<!-- INTERACTIVE SCORECARDS GRID -->
<div class="grid">

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Database icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <ellipse cx="12" cy="5.5" rx="7" ry="2.5" />
          <path d="M5 5.5v13c0 1.38 3.13 2.5 7 2.5s7-1.12 7-2.5v-13" />
          <path d="M5 11.5c0 1.38 3.13 2.5 7 2.5s7-1.12 7-2.5" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">8 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo Data Readiness Check</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/data-readiness-check/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      An interactive 8-question assessment that scores how ready your Maximo data is for AI and agentic capabilities — covering item master governance, failure coding, work order data, and data ownership.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: EAM program owners, IT leads, and reliability teams evaluating AI or MAS analytics capabilities
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Clipboard-check icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <rect x="5" y="4.5" width="14" height="17" rx="2" />
          <path d="M9 4.5V3.8A1.8 1.8 0 0 1 10.8 2h2.4A1.8 1.8 0 0 1 15 3.8v.7" />
          <path d="M8.5 12.5l2.2 2.2L15.5 10" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">14 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo Work Management Value Assessment</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/work-management-assessment/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 14-question interactive scorecard that scores how effectively your work management process is driving maintenance decisions — covering prioritization, planning, maintenance history, work flow efficiency, and data-driven decision making.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: Maintenance managers, reliability teams, and EAM program owners evaluating work management maturity
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Calendar/map icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <rect x="4" y="5" width="16" height="15" rx="2" />
          <path d="M4 9.5h16" />
          <path d="M8 3v3M16 3v3" />
          <path d="M8.5 13.5h2M13.5 13.5h2M8.5 16.5h2M13.5 16.5h2" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">12 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo Planning Value Assessment</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/planning-value-assessment/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 12-question interactive scorecard that scores whether your planning function is reducing field delays, producing reusable plans, and creating measurable value — covering plan accuracy, standardization, productivity impact, and outcome measurement.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: Maintenance planners, reliability teams, and EAM program owners evaluating planning maturity
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Clock icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <circle cx="12" cy="12.5" r="8" />
          <path d="M12 8v4.5l3 2" />
          <path d="M9 2.5h6" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">12 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo Scheduling Value Assessment</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/scheduling-value-assessment/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 12-question interactive scorecard that scores whether your scheduling process is realistic, uses labor effectively, improves execution, and earns leadership's trust — covering schedule compliance, labor balancing, idle time reduction, and workload predictability.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: Maintenance schedulers, operations leaders, and EAM program owners evaluating scheduling maturity
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Shield-check icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M12 2.5l7 3v6c0 5-3 8.5-7 10-4-1.5-7-5-7-10v-6l7-3z" />
          <path d="M8.5 12l2.3 2.3L15.5 9.5" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">12 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo Reliability Value Assessment</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/reliability-value-assessment/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 12-question interactive scorecard that scores whether failures are becoming less common, maintenance strategy is improving, and reliability gains can be demonstrated with data — covering failure reduction, strategy refinement, measurement discipline, and continuous improvement.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: Reliability engineers, maintenance managers, and EAM program owners evaluating reliability program maturity
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Heart-pulse icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M12 20.5s-7.5-4.6-9.7-9.4C1 7.8 2.6 4.5 6 4c2.2-.3 4 .9 6 3.2C14 4.9 15.8 3.7 18 4c3.4.5 5 3.8 3.7 7.1C19.5 15.9 12 20.5 12 20.5z" />
          <path d="M4.5 12h3l1.5-3 2 5 1.5-3h3.5" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">12 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo Asset Health Value Assessment</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/asset-health-value-assessment/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 12-question interactive scorecard that scores whether asset health scoring is catching declining assets early, is trusted, and is delivering measurable business value — covering early detection, data trust, behavioral impact, and business outcomes.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: Reliability engineers, maintenance managers, and EAM program owners evaluating asset health program maturity
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Wifi/sensor icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M4 9.5a11.5 11.5 0 0 1 16 0" />
          <path d="M7 13a7 7 0 0 1 10 0" />
          <path d="M10 16.5a2.8 2.8 0 0 1 4 0" />
          <circle cx="12" cy="19.5" r="1" fill="var(--scorecard-icon-color, #1B6B93)" stroke="none" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">12 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo IoT Value Assessment</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/iot-value-assessment/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 12-question interactive scorecard that scores whether sensor data is driving action, improving visibility, and delivering ROI — covering alert quality, real-time visibility, maintenance impact, and business value.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: IT leads, reliability engineers, and EAM program owners evaluating IoT and condition monitoring maturity
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Stopwatch icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <circle cx="12" cy="13.5" r="7.5" />
          <path d="M12 9.5v4l2.5 1.5" />
          <path d="M9.5 2.5h5" />
          <path d="M12 4.5v2" />
          <path d="M18.5 6l1.2-1.2" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">12 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo Time Management Value Assessment</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/time-management-value-assessment/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 12-question interactive scorecard that scores whether technician time is visible, trusted, and driving staffing decisions — covering labor visibility, data trust, planning accuracy, and workforce decision-making.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: Maintenance supervisors, workforce planners, and EAM program owners evaluating labor management maturity
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Gauge/dial icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M4 15.5a8 8 0 1 1 16 0" />
          <path d="M12 15.5l4-5" />
          <circle cx="12" cy="15.5" r="1" fill="var(--scorecard-icon-color, #1B6B93)" stroke="none" />
          <path d="M4 15.5h1.5M18.5 15.5H20" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">10 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo Capability Assessment</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/capability-assessment/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 10-question interactive scorecard that scores whether Maximo is helping your organization make better decisions — covering information-driven decision-making, reduced administrative effort, and measurable operational improvement.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: EAM program owners, operations leaders, and IT leadership evaluating Maximo's overall business impact
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Hard hat / safety icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path d="M3.5 16.5a8.5 6 0 0 1 17 0z" />
          <path d="M12 8v-2" />
          <path d="M9.5 6.5h5" />
          <path d="M3.5 16.5h17v1.5a1 1 0 0 1-1 1h-15a1 1 0 0 1-1-1v-1.5z" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Interactive Scorecard</div>
        <span class="scorecard-badge">24 Questions</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo HS&amp;E Readiness Assessment</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/scorecards/hse-readiness-assessment/" | relative_url }}">Take the assessment</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 24-question interactive scorecard to evaluate how effectively your organization is leveraging IBM Maximo Health, Safety &amp; Environment (HS&amp;E) — covering incident management, permit to work, MOC, investigations, regulatory compliance, and personnel certification tracking.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: EHS managers, operations leaders, Maximo administrators, and safety program owners
    </div>
  </div>

  <div class="card" style="padding:22px; margin-bottom:18px;">
    <div class="scorecard-visual">
      <div class="scorecard-icon">
        <!-- Printable checklist / star icon -->
        <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <rect x="4.5" y="3" width="15" height="18" rx="1.5" />
          <path d="M8 7.5h8M8 11h8M8 14.5h5" />
          <path d="M17.5 17.2l.7 1.4 1.5.2-1.1 1.1.3 1.5-1.4-.7-1.4.7.3-1.5-1.1-1.1 1.5-.2z" fill="var(--scorecard-icon-color, #1B6B93)" stroke="none" />
        </svg>
      </div>
      <div class="scorecard-meta">
        <div class="scorecard-kicker">Printable Scorecard</div>
        <span class="scorecard-badge">20 Points</span>
      </div>
    </div>

    <h2 style="margin-top:0;">Maximo Readiness Scorecard</h2>

    <div style="margin-top:10px;">
      <a class="button" href="{{ "/field-kits/maximo-readiness-scorecard.html" | relative_url }}">View scorecard</a>
    </div>

    <p style="font-size:1.05rem; line-height:1.55; margin-top:14px;">
      A 20-point scorecard to quickly assess whether Maximo is positioned to drive performance across strategy, reliability execution, and data governance.
    </p>

    <div style="margin-top:14px; opacity:.8;">
      Best for: EAM owners, operations leaders, and IT leadership evaluating overall Maximo program health
    </div>
  </div>

</div>

<p class="section-title">Why use a scorecard?</p>
<div class="card">
  <p>
    Scorecards give teams a shared, honest starting point. They surface gaps that are easy to overlook when you're close to the work, and they make it easier to prioritize where to focus — whether you're preparing for an AI initiative, evaluating your HS&amp;E program, or assessing overall Maximo program health. Start with the AI Readiness Assessment above, no form required, then sign up once to unlock our full library of scorecards.
  </p>
</div>

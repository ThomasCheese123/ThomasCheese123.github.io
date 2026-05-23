<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>USC Summer Study Plan 2025</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=IBM+Plex+Mono:wght@400;500&family=IBM+Plex+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --usc-cardinal: #990000;
    --usc-gold: #FFC72C;
    --usc-dark: #1a1009;
    --bg: #faf7f2;
    --surface: #ffffff;
    --surface2: #f4ede0;
    --text: #1a1009;
    --muted: #7a6652;
    --math: #c0392b;
    --chem: #1a6b3c;
    --cs: #1a3a6b;
    --math-light: #fdf0ef;
    --chem-light: #eef7f2;
    --cs-light: #eef2f9;
    --border: #e0d4c0;
    --shadow: 0 2px 16px rgba(26,16,9,0.08);
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'IBM Plex Sans', sans-serif;
    background: var(--bg);
    color: var(--text);
    font-size: 15px;
    line-height: 1.6;
  }

  /* HEADER */
  header {
    background: var(--usc-cardinal);
    color: white;
    padding: 0;
    position: relative;
    overflow: hidden;
  }

  .header-texture {
    position: absolute; inset: 0;
    background-image: repeating-linear-gradient(
      45deg,
      transparent,
      transparent 20px,
      rgba(255,199,44,0.07) 20px,
      rgba(255,199,44,0.07) 21px
    );
    pointer-events: none;
  }

  .header-inner {
    position: relative;
    max-width: 960px;
    margin: 0 auto;
    padding: 48px 32px 36px;
  }

  .usc-badge {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: rgba(255,199,44,0.15);
    border: 1px solid rgba(255,199,44,0.4);
    border-radius: 4px;
    padding: 6px 14px;
    margin-bottom: 20px;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.12em;
    color: var(--usc-gold);
    text-transform: uppercase;
  }

  .usc-badge span { font-size: 16px; }

  header h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(28px, 5vw, 44px);
    font-weight: 900;
    line-height: 1.1;
    margin-bottom: 12px;
    color: white;
  }

  header h1 em {
    color: var(--usc-gold);
    font-style: normal;
  }

  header p {
    color: rgba(255,255,255,0.75);
    font-size: 15px;
    max-width: 560px;
  }

  .header-meta {
    display: flex;
    gap: 24px;
    margin-top: 28px;
    flex-wrap: wrap;
  }

  .meta-pill {
    background: rgba(255,255,255,0.1);
    border: 1px solid rgba(255,255,255,0.2);
    border-radius: 100px;
    padding: 6px 16px;
    font-size: 13px;
    color: white;
    font-family: 'IBM Plex Mono', monospace;
  }

  /* COURSE LEGEND */
  .legend {
    max-width: 960px;
    margin: 32px auto 0;
    padding: 0 32px;
    display: flex;
    gap: 16px;
    flex-wrap: wrap;
  }

  .legend-item {
    display: flex;
    align-items: center;
    gap: 10px;
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 10px 18px;
    box-shadow: var(--shadow);
    flex: 1;
    min-width: 180px;
  }

  .legend-dot {
    width: 14px; height: 14px;
    border-radius: 50%;
    flex-shrink: 0;
  }

  .legend-item strong {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 13px;
  }

  .legend-item small {
    color: var(--muted);
    font-size: 12px;
    display: block;
    line-height: 1.2;
  }

  /* OVERVIEW STATS */
  .stats-bar {
    max-width: 960px;
    margin: 20px auto;
    padding: 0 32px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
    gap: 12px;
  }

  .stat-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 16px;
    text-align: center;
    box-shadow: var(--shadow);
  }

  .stat-num {
    font-family: 'Playfair Display', serif;
    font-size: 28px;
    font-weight: 700;
    color: var(--usc-cardinal);
    line-height: 1;
  }

  .stat-label {
    font-size: 11px;
    color: var(--muted);
    text-transform: uppercase;
    letter-spacing: 0.08em;
    margin-top: 4px;
    font-family: 'IBM Plex Mono', monospace;
  }

  /* TIPS SECTION */
  .tips-section {
    max-width: 960px;
    margin: 0 auto 24px;
    padding: 0 32px;
  }

  .tips-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 14px;
  }

  .tip-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-left: 4px solid var(--usc-cardinal);
    border-radius: 8px;
    padding: 16px;
    box-shadow: var(--shadow);
  }

  .tip-card h4 {
    font-size: 13px;
    font-weight: 600;
    margin-bottom: 6px;
    color: var(--usc-cardinal);
    font-family: 'IBM Plex Mono', monospace;
  }

  .tip-card p {
    font-size: 13px;
    color: var(--muted);
    line-height: 1.5;
  }

  /* MAIN CONTENT */
  main {
    max-width: 960px;
    margin: 0 auto;
    padding: 0 32px 60px;
  }

  .section-label {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 16px;
    padding-bottom: 8px;
    border-bottom: 1px solid var(--border);
  }

  /* WEEK BLOCK */
  .week-block {
    margin-bottom: 36px;
    border: 1px solid var(--border);
    border-radius: 12px;
    overflow: hidden;
    box-shadow: var(--shadow);
    background: var(--surface);
  }

  .week-header {
    background: var(--usc-dark);
    color: white;
    padding: 16px 24px;
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    gap: 16px;
    flex-wrap: wrap;
    cursor: pointer;
    user-select: none;
  }

  .week-header:hover { background: #2a1f10; }

  .week-title-group { flex: 1; }

  .week-num {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    color: var(--usc-gold);
    letter-spacing: 0.12em;
    text-transform: uppercase;
    margin-bottom: 4px;
  }

  .week-title {
    font-family: 'Playfair Display', serif;
    font-size: 18px;
    font-weight: 700;
    color: white;
  }

  .week-goal {
    font-size: 12px;
    color: rgba(255,255,255,0.6);
    margin-top: 4px;
    line-height: 1.4;
    max-width: 480px;
  }

  .week-toggle {
    font-size: 20px;
    color: var(--usc-gold);
    transition: transform 0.3s;
    flex-shrink: 0;
    margin-top: 2px;
  }

  .week-toggle.open { transform: rotate(180deg); }

  .week-days {
    display: none;
    padding: 0 20px 20px;
  }

  .week-days.open { display: block; }

  /* CHECKPOINT BAR */
  .checkpoint {
    background: linear-gradient(135deg, #fff8e6, #fff3d4);
    border: 1px solid #ffc72c55;
    border-left: 4px solid var(--usc-gold);
    border-radius: 8px;
    padding: 12px 16px;
    margin: 16px 0 8px;
    font-size: 13px;
  }

  .checkpoint strong {
    color: #8a6200;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    display: block;
    margin-bottom: 4px;
  }

  /* DAY CARD */
  .day-card {
    border: 1px solid var(--border);
    border-radius: 8px;
    margin-top: 12px;
    overflow: hidden;
  }

  .day-header {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 10px 16px;
    background: var(--surface2);
    border-bottom: 1px solid var(--border);
  }

  .day-name {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 12px;
    font-weight: 500;
    color: var(--muted);
    text-transform: uppercase;
    letter-spacing: 0.08em;
    min-width: 90px;
  }

  .day-date {
    font-size: 12px;
    color: var(--muted);
  }

  .day-hours {
    margin-left: auto;
    background: var(--usc-cardinal);
    color: white;
    font-size: 11px;
    font-family: 'IBM Plex Mono', monospace;
    padding: 3px 10px;
    border-radius: 100px;
  }

  .day-body {
    padding: 12px 16px;
    display: flex;
    flex-direction: column;
    gap: 8px;
  }

  /* SUBJECT ENTRY */
  .subject-entry {
    display: flex;
    gap: 10px;
    align-items: flex-start;
    border-radius: 6px;
    padding: 8px 10px;
  }

  .subject-entry.math { background: var(--math-light); border-left: 3px solid var(--math); }
  .subject-entry.chem { background: var(--chem-light); border-left: 3px solid var(--chem); }
  .subject-entry.cs   { background: var(--cs-light);   border-left: 3px solid var(--cs); }
  .subject-entry.review { background: #f9f4ff; border-left: 3px solid #7c3aed; }
  .subject-entry.rest { background: #f0f9ff; border-left: 3px solid #0ea5e9; }

  .subject-tag {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 10px;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 0.06em;
    padding: 2px 7px;
    border-radius: 4px;
    flex-shrink: 0;
    margin-top: 1px;
  }

  .subject-entry.math .subject-tag { background: var(--math); color: white; }
  .subject-entry.chem .subject-tag { background: var(--chem); color: white; }
  .subject-entry.cs   .subject-tag { background: var(--cs);   color: white; }
  .subject-entry.review .subject-tag { background: #7c3aed; color: white; }
  .subject-entry.rest .subject-tag { background: #0ea5e9; color: white; }

  .subject-content { flex: 1; }

  .subject-topic {
    font-size: 13px;
    font-weight: 500;
    color: var(--text);
    line-height: 1.35;
  }

  .subject-method {
    font-size: 12px;
    color: var(--muted);
    margin-top: 2px;
    line-height: 1.4;
  }

  /* REVIEW DAY */
  .review-day-card {
    background: linear-gradient(135deg, #f9f4ff, #f3eeff);
    border: 1px solid #c4b5fd;
    border-radius: 8px;
    margin-top: 12px;
    padding: 14px 16px;
  }

  .review-day-header {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    color: #7c3aed;
    margin-bottom: 8px;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .review-day-header span { font-size: 14px; }

  .review-tasks {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .review-tag {
    background: white;
    border: 1px solid #c4b5fd;
    border-radius: 4px;
    padding: 4px 10px;
    font-size: 12px;
    color: #5b21b6;
  }

  /* RESOURCES */
  .resources-section {
    margin-top: 36px;
  }

  .resources-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 16px;
  }

  .resource-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 18px;
    box-shadow: var(--shadow);
  }

  .resource-card h4 {
    font-family: 'Playfair Display', serif;
    font-size: 16px;
    font-weight: 700;
    margin-bottom: 12px;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .resource-card.math h4 { color: var(--math); }
  .resource-card.chem h4 { color: var(--chem); }
  .resource-card.cs h4   { color: var(--cs); }
  .resource-card.gen h4  { color: var(--usc-cardinal); }

  .resource-list { list-style: none; }
  .resource-list li {
    font-size: 13px;
    padding: 5px 0;
    border-bottom: 1px solid var(--border);
    color: var(--text);
    display: flex;
    gap: 8px;
    align-items: flex-start;
  }
  .resource-list li:last-child { border-bottom: none; }
  .resource-list li::before {
    content: '→';
    color: var(--muted);
    flex-shrink: 0;
    margin-top: 1px;
  }

  /* FOOTER */
  footer {
    background: var(--usc-dark);
    color: rgba(255,255,255,0.5);
    text-align: center;
    padding: 24px;
    font-size: 12px;
    font-family: 'IBM Plex Mono', monospace;
  }

  footer strong { color: var(--usc-gold); }

  /* RESPONSIVE */
  @media (max-width: 600px) {
    .header-inner, .legend, .stats-bar, .tips-section, main { padding-left: 16px; padding-right: 16px; }
    .legend { gap: 10px; }
    .legend-item { min-width: 140px; }
  }
</style>
</head>
<body>

<header>
  <div class="header-texture"></div>
  <div class="header-inner">
    <div class="usc-badge"><span>✦</span> University of Southern California</div>
    <h1>Summer <em>Study Plan</em><br>July 1 – August 10, 2026</h1>
    <p>A structured 6-week preparation plan for incoming freshmen covering Calculus I, General Chemistry, and Intro to Computing.</p>
    <div class="header-meta">
      <div class="meta-pill">📐 MATH 125</div>
      <div class="meta-pill">⚗️ CHEM 105a</div>
      <div class="meta-pill">💻 CSCI 102</div>
      <div class="meta-pill">6 Weeks · 3–4 hrs/day</div>
    </div>
  </div>
</header>

<!-- LEGEND -->
<div class="legend">
  <div class="legend-item">
    <div class="legend-dot" style="background:var(--math)"></div>
    <div>
      <strong>MATH 125</strong>
      <small>Calculus I</small>
    </div>
  </div>
  <div class="legend-item">
    <div class="legend-dot" style="background:var(--chem)"></div>
    <div>
      <strong>CHEM 105a</strong>
      <small>General Chemistry</small>
    </div>
  </div>
  <div class="legend-item">
    <div class="legend-dot" style="background:var(--cs)"></div>
    <div>
      <strong>CSCI 102</strong>
      <small>Intro to Computing</small>
    </div>
  </div>
  <div class="legend-item">
    <div class="legend-dot" style="background:#7c3aed"></div>
    <div>
      <strong>Review Day</strong>
      <small>Consolidation & practice</small>
    </div>
  </div>
</div>

<!-- STATS -->
<div class="stats-bar">
  <div class="stat-card">
    <div class="stat-num">6</div>
    <div class="stat-label">Weeks</div>
  </div>
  <div class="stat-card">
    <div class="stat-num">41</div>
    <div class="stat-label">Study Days</div>
  </div>
  <div class="stat-card">
    <div class="stat-num">3–4</div>
    <div class="stat-label">Hrs / Day</div>
  </div>
  <div class="stat-card">
    <div class="stat-num">~140</div>
    <div class="stat-label">Total Hours</div>
  </div>
  <div class="stat-card">
    <div class="stat-num">3</div>
    <div class="stat-label">Courses</div>
  </div>
</div>

<!-- USC TIPS -->
<div class="tips-section" style="margin-top:24px;">
  <div class="section-label">📌 How to Prepare for USC-Level Work</div>
  <div class="tips-grid">
    <div class="tip-card">
      <h4>Don't Just Watch — Do</h4>
      <p>USC professors expect you to actively problem-solve. Read examples, then close the book and re-do them from scratch. Passive reading won't cut it.</p>
    </div>
    <div class="tip-card">
      <h4>Spaced Repetition</h4>
      <p>Revisit concepts 1, 3, and 7 days after learning them. Use Anki for chemistry formulas and CS definitions. This is how you retain at USC's pace.</p>
    </div>
    <div class="tip-card">
      <h4>Simulate Exam Conditions</h4>
      <p>Do timed practice problems without notes. USC exams are fast-paced. Training under pressure builds speed and confidence.</p>
    </div>
    <div class="tip-card">
      <h4>Build Office-Hours Habits Now</h4>
      <p>USC professors hold office hours that most students never use. Practice articulating your questions clearly — start now so it feels natural in semester.</p>
    </div>
    <div class="tip-card">
      <h4>One Subject Deep Each Day</h4>
      <p>Rotate which subject gets your peak focus (morning). Don't split your attention across all three every day — deep work beats scattered review.</p>
    </div>
    <div class="tip-card">
      <h4>Track What You Don't Know</h4>
      <p>Keep a "confusion log" — a running list of concepts that tripped you up. Review it weekly. This is your priority list, not the syllabus.</p>
    </div>
  </div>
</div>

<!-- WEEK BLOCKS -->
<main>
  <div class="section-label" style="margin-bottom:20px;">📅 Week-by-Week Plan — Click a week to expand</div>

  <!-- WEEK 1 -->
  <div class="week-block">
    <div class="week-header" onclick="toggleWeek(this)">
      <div class="week-title-group">
        <div class="week-num">Week 01 · July 1–6</div>
        <div class="week-title">Building the Foundations</div>
        <div class="week-goal">Goal: Activate prior knowledge. Get comfortable with pre-calc math, atomic theory basics, and your first Python/terminal session.</div>
      </div>
      <div class="week-toggle">▼</div>
    </div>
    <div class="week-days">

      <div class="day-card">
        <div class="day-header">
          <div class="day-name">Tuesday</div>
          <div class="day-date">July 1</div>
          <div class="day-hours">3 hrs</div>
        </div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Pre-Calculus Review: Functions, Domains, & Graphs</div>
              <div class="subject-method">Read notes / Khan Academy · Draw and label 8 function graphs by hand · Identify domain & range</div>
            </div>
          </div>
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Atomic Structure: Protons, Neutrons, Electrons, Isotopes</div>
              <div class="subject-method">Watch CrashCourse Chemistry Ep. 1–2 · Make flashcards for atomic number, mass number, and isotope notation</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header">
          <div class="day-name">Wednesday</div>
          <div class="day-date">July 2</div>
          <div class="day-hours">3.5 hrs</div>
        </div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Algebra Fluency: Factoring, Exponents, Radicals</div>
              <div class="subject-method">Complete 20 factoring problems · Practice exponent rules with timed drill (no calculator)</div>
            </div>
          </div>
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">What is Computing? Binary & Number Systems</div>
              <div class="subject-method">Read CS Principles intro · Convert 10 decimal numbers to binary by hand · Watch "How Computers Work" (Code.org)</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header">
          <div class="day-name">Thursday</div>
          <div class="day-date">July 3</div>
          <div class="day-hours">3 hrs</div>
        </div>
        <div class="day-body">
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">The Periodic Table: Periods, Groups, Trends</div>
              <div class="subject-method">Memorize Group 1, 2, 17, 18 + transition metals · Practice locating elements by property · Khan Academy periodic trends</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Trigonometry Review: Unit Circle, Sine, Cosine, Tangent</div>
              <div class="subject-method">Draw unit circle 3 times from memory · Solve 15 basic trig equations</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header">
          <div class="day-name">Friday</div>
          <div class="day-date">July 4</div>
          <div class="day-hours">2 hrs (holiday)</div>
        </div>
        <div class="day-body">
          <div class="subject-entry rest">
            <div class="subject-tag">Light</div>
            <div class="subject-content">
              <div class="subject-topic">Independence Day — Light review only</div>
              <div class="subject-method">Review your week's flashcards (20 min) · Watch 1 CrashCourse video of your choice · Rest and recharge</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header">
          <div class="day-name">Saturday</div>
          <div class="day-date">July 5</div>
          <div class="day-hours">4 hrs</div>
        </div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">First Python Session: Install, Print, Variables, Data Types</div>
              <div class="subject-method">Install Python + VS Code · Write 10 small programs from prompts · CS50P Week 0 (Harvard, free)</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Limits: Intuitive Introduction</div>
              <div class="subject-method">Read textbook §1.1–1.2 · Use Desmos to visualize limit behavior · Watch 3Blue1Brown "Essence of Calculus" Ep. 1</div>
            </div>
          </div>
        </div>
      </div>

      <div class="review-day-card">
        <div class="review-day-header"><span>🔁</span> Sunday July 6 — Week 1 Review Day (2 hrs)</div>
        <div class="review-tasks">
          <div class="review-tag">Quiz yourself on the unit circle</div>
          <div class="review-tag">Re-do 5 hardest problems from the week</div>
          <div class="review-tag">Review Chem flashcards (Anki)</div>
          <div class="review-tag">Confirm Python installs and run first script again</div>
          <div class="review-tag">Update your confusion log</div>
        </div>
      </div>

      <div class="checkpoint">
        <strong>✦ Week 1 Checkpoint</strong>
        Can you sketch the unit circle from memory? Identify any element's period and group? Run a Python script that prints your name and performs arithmetic? If yes — you're on track!
      </div>

    </div>
  </div>

  <!-- WEEK 2 -->
  <div class="week-block">
    <div class="week-header" onclick="toggleWeek(this)">
      <div class="week-title-group">
        <div class="week-num">Week 02 · July 7–13</div>
        <div class="week-title">Limits, Bonds & Logic</div>
        <div class="week-goal">Goal: Master the limit concept and limit laws (MATH). Learn chemical bonding and naming (CHEM). Write conditionals and loops in Python (CS).</div>
      </div>
      <div class="week-toggle">▼</div>
    </div>
    <div class="week-days">

      <div class="day-card">
        <div class="day-header"><div class="day-name">Monday</div><div class="day-date">July 7</div><div class="day-hours">3.5 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Limit Laws & Evaluating Limits Algebraically</div>
              <div class="subject-method">Practice 20 limit evaluation problems · Substitution, factoring, rationalization techniques</div>
            </div>
          </div>
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Ionic vs. Covalent Bonding</div>
              <div class="subject-method">Draw 10 Lewis dot structures · Identify bond type from electronegativity differences</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Tuesday</div><div class="day-date">July 8</div><div class="day-hours">3.5 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Conditionals: if / elif / else Logic</div>
              <div class="subject-method">Write a grade calculator, a number guesser, and a simple chatbot · CS50P Week 1</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">One-Sided Limits & Continuity</div>
              <div class="subject-method">Graph 6 piecewise functions · Check continuity at each break point</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Wednesday</div><div class="day-date">July 9</div><div class="day-hours">3 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Naming Ionic & Covalent Compounds</div>
              <div class="subject-method">Complete 30 naming exercises · Use ACS nomenclature guidelines · Quizlet for polyatomic ions</div>
            </div>
          </div>
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Loops: while and for — Iteration Patterns</div>
              <div class="subject-method">FizzBuzz, prime finder, multiplication table — implement all three from scratch</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Thursday</div><div class="day-date">July 10</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Limits at Infinity & Asymptotes</div>
              <div class="subject-method">Identify horizontal/vertical asymptotes for 12 rational functions · Confirm with Desmos</div>
            </div>
          </div>
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Mole Concept & Molar Mass</div>
              <div class="subject-method">Practice 15 mole ↔ gram ↔ molecule conversions · This is the cornerstone of all stoichiometry</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Friday</div><div class="day-date">July 11</div><div class="day-hours">3.5 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Functions: Defining, Calling, Return Values, Scope</div>
              <div class="subject-method">Refactor your Week 1 programs to use functions · Write a temperature converter and a factorial calculator</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Squeeze Theorem & Special Limits (sin x / x)</div>
              <div class="subject-method">Prove sin x / x → 1 geometrically · 8 practice problems with these special cases</div>
            </div>
          </div>
        </div>
      </div>

      <div class="review-day-card">
        <div class="review-day-header"><span>🔁</span> Weekend July 12–13 — Review & Practice (3 hrs total)</div>
        <div class="review-tasks">
          <div class="review-tag">10-problem limit quiz (self-timed)</div>
          <div class="review-tag">Name 20 compounds from formula</div>
          <div class="review-tag">Write a Python program using loops + functions</div>
          <div class="review-tag">Anki deck review: Chem formulas</div>
          <div class="review-tag">Rest Sunday afternoon</div>
        </div>
      </div>

      <div class="checkpoint">
        <strong>✦ Week 2 Checkpoint</strong>
        Can you evaluate limits using all three algebraic techniques? Name ionic and covalent compounds confidently? Write a Python function that uses a loop and returns a value? If yes — excellent momentum!
      </div>

    </div>
  </div>

  <!-- WEEK 3 -->
  <div class="week-block">
    <div class="week-header" onclick="toggleWeek(this)">
      <div class="week-title-group">
        <div class="week-num">Week 03 · July 14–20</div>
        <div class="week-title">The Derivative Arrives</div>
        <div class="week-goal">Goal: Understand and compute derivatives from definition and rules (MATH). Master stoichiometry and reactions (CHEM). Build data structures: lists, dicts, strings (CS).</div>
      </div>
      <div class="week-toggle">▼</div>
    </div>
    <div class="week-days">

      <div class="day-card">
        <div class="day-header"><div class="day-name">Monday</div><div class="day-date">July 14</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">The Derivative: Definition via Limits (first principles)</div>
              <div class="subject-method">Derive f'(x) from scratch for x², x³, and √x · 10 definition-based derivative problems</div>
            </div>
          </div>
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Balancing Chemical Equations</div>
              <div class="subject-method">Balance 20 equations systematically · Check atom counts on both sides · No shortcuts yet</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Tuesday</div><div class="day-date">July 15</div><div class="day-hours">3.5 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Power Rule, Constant Rule, Sum/Difference Rule</div>
              <div class="subject-method">Drill 30 problems with these rules · Speed is the goal today — aim for <30 sec per problem</div>
            </div>
          </div>
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Lists: Indexing, Slicing, Common Methods</div>
              <div class="subject-method">CS50P Week 2 · Build a to-do list app in the terminal · Practice list comprehensions</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Wednesday</div><div class="day-date">July 16</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Stoichiometry: Mole Ratios & Mass-to-Mass Problems</div>
              <div class="subject-method">Complete 15 stoichiometry problems end-to-end · Show unit conversion chain explicitly</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Product Rule & Quotient Rule</div>
              <div class="subject-method">15 product rule + 15 quotient rule problems · Derive both rules yourself before applying</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Thursday</div><div class="day-date">July 17</div><div class="day-hours">3.5 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Dictionaries & String Manipulation</div>
              <div class="subject-method">Build a word-frequency counter · Practice .split(), .strip(), .join() · Write a simple cipher</div>
            </div>
          </div>
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Limiting Reagent & Percent Yield</div>
              <div class="subject-method">10 limiting reagent problems · Understand why this is the hardest stoichiometry concept</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Friday</div><div class="day-date">July 18</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Chain Rule: Composite Function Derivatives</div>
              <div class="subject-method">20 chain rule problems with trig, polynomial, and mixed composites · Identify "inside" and "outside" functions</div>
            </div>
          </div>
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">File I/O: Reading & Writing Text Files in Python</div>
              <div class="subject-method">Write a contact book that saves/loads from a .txt file · Practice open(), read(), write(), close()</div>
            </div>
          </div>
        </div>
      </div>

      <div class="review-day-card">
        <div class="review-day-header"><span>🔁</span> Weekend July 19–20 — Deep Review (4 hrs total)</div>
        <div class="review-tasks">
          <div class="review-tag">Timed derivative quiz: 20 problems, 25 min</div>
          <div class="review-tag">Stoichiometry practice test (Khan Academy)</div>
          <div class="review-tag">Rebuild your to-do app from scratch (no notes)</div>
          <div class="review-tag">Confusion log review</div>
          <div class="review-tag">Plan your study schedule for Week 4</div>
        </div>
      </div>

      <div class="checkpoint">
        <strong>✦ Week 3 Checkpoint</strong>
        Can you differentiate any polynomial, product, or quotient quickly? Solve a full stoichiometry problem with a limiting reagent? Write a Python program that uses lists, dicts, and file I/O? Strong week!
      </div>

    </div>
  </div>

  <!-- WEEK 4 -->
  <div class="week-block">
    <div class="week-header" onclick="toggleWeek(this)">
      <div class="week-title-group">
        <div class="week-num">Week 04 · July 21–27</div>
        <div class="week-title">Applications & Deeper Concepts</div>
        <div class="week-goal">Goal: Apply derivatives to real problems (MATH). Study solutions, reactions, gas laws (CHEM). Learn algorithmic thinking and error handling (CS).</div>
      </div>
      <div class="week-toggle">▼</div>
    </div>
    <div class="week-days">

      <div class="day-card">
        <div class="day-header"><div class="day-name">Monday</div><div class="day-date">July 21</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Implicit Differentiation</div>
              <div class="subject-method">15 implicit differentiation problems including circles and ellipses · Find tangent line slopes</div>
            </div>
          </div>
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Solutions: Molarity, Dilution, Concentration</div>
              <div class="subject-method">Practice M₁V₁ = M₂V₂ · 12 molarity calculation problems · Real lab context examples</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Tuesday</div><div class="day-date">July 22</div><div class="day-hours">3.5 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Algorithmic Thinking: Pseudocode & Flowcharts</div>
              <div class="subject-method">Plan 5 problems in pseudocode before coding · Draw flowchart for a login system · CS50 Week 0 concept review</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Related Rates Problems</div>
              <div class="subject-method">Ladder, balloon, and shadow problems · Identify variables, write equations, differentiate with respect to time</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Wednesday</div><div class="day-date">July 23</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Gas Laws: Boyle's, Charles's, Ideal Gas Law (PV=nRT)</div>
              <div class="subject-method">15 gas law problems · Convert all units before solving · Understand each variable's physical meaning</div>
            </div>
          </div>
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Exceptions & Error Handling: try / except</div>
              <div class="subject-method">Add error handling to all previous programs · Understand ValueError, TypeError, FileNotFoundError</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Thursday</div><div class="day-date">July 24</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">L'Hôpital's Rule & Indeterminate Forms</div>
              <div class="subject-method">10 0/0 form problems · 10 ∞/∞ form problems · Verify with limit evaluation first</div>
            </div>
          </div>
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Thermochemistry: Enthalpy, Hess's Law, Calorimetry</div>
              <div class="subject-method">10 enthalpy calculation problems · Draw energy diagrams for exo- vs endothermic reactions</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Friday</div><div class="day-date">July 25</div><div class="day-hours">3.5 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Classes & Object-Oriented Programming Intro</div>
              <div class="subject-method">Build a Student class with name, grade, GPA attributes and a method · CS50P Week 8</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Curve Sketching: Critical Points, Increasing/Decreasing Intervals</div>
              <div class="subject-method">Sketch 6 functions using f' and f'' analysis · Identify local max/min without graphing calculator first</div>
            </div>
          </div>
        </div>
      </div>

      <div class="review-day-card">
        <div class="review-day-header"><span>🔁</span> Weekend July 26–27 — Mixed Practice Sprint (4 hrs total)</div>
        <div class="review-tasks">
          <div class="review-tag">Derivative applications test (related rates + implicit)</div>
          <div class="review-tag">Gas law problem set (10 problems)</div>
          <div class="review-tag">Build a small OOP Python project</div>
          <div class="review-tag">Full Chem Anki deck review</div>
          <div class="review-tag">Compare confusion logs: what's improving?</div>
        </div>
      </div>

      <div class="checkpoint">
        <strong>✦ Week 4 Checkpoint</strong>
        Can you solve a related rates problem end-to-end? Apply the ideal gas law with unit conversions? Write a Python class with attributes and methods? You're in the second half — strong!
      </div>

    </div>
  </div>

  <!-- WEEK 5 -->
  <div class="week-block">
    <div class="week-header" onclick="toggleWeek(this)">
      <div class="week-title-group">
        <div class="week-num">Week 05 · July 28 – Aug 3</div>
        <div class="week-title">Integration, Equilibrium & Algorithms</div>
        <div class="week-goal">Goal: Enter integral calculus (MATH). Study chemical equilibrium and acids/bases (CHEM). Master searching, sorting, and complexity (CS).</div>
      </div>
      <div class="week-toggle">▼</div>
    </div>
    <div class="week-days">

      <div class="day-card">
        <div class="day-header"><div class="day-name">Monday</div><div class="day-date">July 28</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Antiderivatives & Indefinite Integrals</div>
              <div class="subject-method">Reverse all derivative rules · 25 antiderivative problems · Always check by differentiating your answer</div>
            </div>
          </div>
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Chemical Equilibrium: Keq, Le Chatelier's Principle</div>
              <div class="subject-method">Calculate K for 10 reactions · Predict shifts from 5 disturbance scenarios</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Tuesday</div><div class="day-date">July 29</div><div class="day-hours">3.5 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Searching & Sorting Algorithms: Linear, Binary, Bubble, Selection</div>
              <div class="subject-method">Implement all 4 from scratch · Compare performance · CS50 Week 3 (Algorithms)</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Riemann Sums & Area Under a Curve (intro)</div>
              <div class="subject-method">Use Desmos to visualize left/right Riemann sums · Calculate by hand for simple polynomials</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Wednesday</div><div class="day-date">July 30</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Acids & Bases: pH Scale, Strong vs. Weak, Buffers</div>
              <div class="subject-method">Calculate pH from [H⁺] and Ka · Titration concept overview · 12 acid-base problems</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">The Fundamental Theorem of Calculus (Parts I & II)</div>
              <div class="subject-method">This is THE most important theorem in Calc I — derive it, state it, apply it 10 times each way</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Thursday</div><div class="day-date">July 31</div><div class="day-hours">3.5 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Big-O Notation & Computational Complexity</div>
              <div class="subject-method">Classify each sort/search by time complexity · Watch "Big O Notation" — NeetCode on YouTube</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">U-Substitution for Definite & Indefinite Integrals</div>
              <div class="subject-method">20 u-sub problems · Remember to change limits for definite integrals · This is the chain rule in reverse</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Friday</div><div class="day-date">Aug 1</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Electrochemistry Intro: Oxidation States, Redox Reactions</div>
              <div class="subject-method">Assign oxidation states to 20 compounds · Balance 8 redox equations in acidic solution</div>
            </div>
          </div>
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Recursion: Thinking in Base Cases and Recursive Steps</div>
              <div class="subject-method">Implement factorial, Fibonacci, binary search recursively · Draw call stacks by hand</div>
            </div>
          </div>
        </div>
      </div>

      <div class="review-day-card">
        <div class="review-day-header"><span>🔁</span> Weekend Aug 2–3 — Integration Blitz (4 hrs total)</div>
        <div class="review-tasks">
          <div class="review-tag">20-problem integral sprint (30 min)</div>
          <div class="review-tag">Acid-base & equilibrium practice test</div>
          <div class="review-tag">Implement merge sort (stretch goal)</div>
          <div class="review-tag">Full Anki review: all three subjects</div>
          <div class="review-tag">Write down 3 things you want to go deeper on in Week 6</div>
        </div>
      </div>

      <div class="checkpoint">
        <strong>✦ Week 5 Checkpoint</strong>
        Can you evaluate a definite integral using FTC and u-substitution? Explain Le Chatelier's principle with examples? Implement a binary search recursively? You're nearly there — outstanding!
      </div>

    </div>
  </div>

  <!-- WEEK 6 -->
  <div class="week-block">
    <div class="week-header" onclick="toggleWeek(this)">
      <div class="week-title-group">
        <div class="week-num">Week 06 · Aug 4–10</div>
        <div class="week-title">Final Review & Semester Readiness</div>
        <div class="week-goal">Goal: Simulate exam conditions across all subjects. Fill remaining gaps. Build confidence and a semester study system before Day 1 at USC.</div>
      </div>
      <div class="week-toggle">▼</div>
    </div>
    <div class="week-days">

      <div class="day-card">
        <div class="day-header"><div class="day-name">Monday</div><div class="day-date">Aug 4</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Calculus I Full Practice Exam (Limits + Derivatives)</div>
              <div class="subject-method">Set a 75-minute timer, closed notes · Use a real AP Calculus AB or MIT 18.01 practice exam · Grade yourself honestly</div>
            </div>
          </div>
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Error Review & Targeted Drilling</div>
              <div class="subject-method">Identify every mistake category from the exam · Do 3× more problems of each weak type</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Tuesday</div><div class="day-date">Aug 5</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">Chemistry Full Practice Exam</div>
              <div class="subject-method">Cover: atomic structure, bonding, stoichiometry, gas laws, equilibrium, acids/bases · 90-minute timed exam · Use Khan AP Chemistry practice</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Wednesday</div><div class="day-date">Aug 6</div><div class="day-hours">4 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">CS Final Project: Build a Complete Python Application</div>
              <div class="subject-method">Choose: a budget tracker, a quiz game, or a simple inventory system · Use OOP, file I/O, error handling, and lists — all in one project</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Thursday</div><div class="day-date">Aug 7</div><div class="day-hours">3 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry math">
            <div class="subject-tag">Math</div>
            <div class="subject-content">
              <div class="subject-topic">Integration Applications: Area Between Curves, Average Value</div>
              <div class="subject-method">Preview what's coming early in MATH 125 · 8 area problems · Read §5.1–5.2 of textbook</div>
            </div>
          </div>
          <div class="subject-entry chem">
            <div class="subject-tag">Chem</div>
            <div class="subject-content">
              <div class="subject-topic">CHEM 105a Concept Map Review</div>
              <div class="subject-method">Draw a single concept map connecting all major topics from scratch — this is one of the most powerful review methods</div>
            </div>
          </div>
        </div>
      </div>

      <div class="day-card">
        <div class="day-header"><div class="day-name">Friday</div><div class="day-date">Aug 8</div><div class="day-hours">3 hrs</div></div>
        <div class="day-body">
          <div class="subject-entry cs">
            <div class="subject-tag">CS</div>
            <div class="subject-content">
              <div class="subject-topic">Preview USC CSCI 102: Data Structures & Pointers Intro</div>
              <div class="subject-method">Read about arrays vs. linked lists · Watch "Pointers in C" (if C is used at USC) or preview CS102 syllabus online</div>
            </div>
          </div>
          <div class="subject-entry review">
            <div class="subject-tag">System</div>
            <div class="subject-content">
              <div class="subject-topic">Build Your Semester Study System</div>
              <div class="subject-method">Set up Notion or Obsidian for notes · Create Anki decks for semester use · Block study hours on your calendar before classes start</div>
            </div>
          </div>
        </div>
      </div>

      <div class="review-day-card">
        <div class="review-day-header"><span>🎓</span> Final Weekend Aug 9–10 — Celebration & Orientation Prep (2 hrs light)</div>
        <div class="review-tasks">
          <div class="review-tag">Light Anki review all decks</div>
          <div class="review-tag">Review your confusion log — celebrate how much it shrank</div>
          <div class="review-tag">Read your USC syllabi (if available)</div>
          <div class="review-tag">Rest. You've earned it.</div>
          <div class="review-tag">Explore campus maps, find classrooms</div>
        </div>
      </div>

      <div class="checkpoint">
        <strong>✦ Final Checkpoint — You're Ready!</strong>
        You've built a 6-week foundation in calculus, chemistry, and programming. You know how to study, how to drill weaknesses, and how to think like a scientist and a programmer. Trust your preparation and enjoy USC. Fight on! ✌️
      </div>

    </div>
  </div>

  <!-- RESOURCES -->
  <div class="resources-section">
    <div class="section-label">📚 Recommended Resources</div>
    <div class="resources-grid">

      <div class="resource-card math">
        <h4>📐 MATH 125 Resources</h4>
        <ul class="resource-list">
          <li>3Blue1Brown — "Essence of Calculus" (YouTube, free)</li>
          <li>Prof. Leonard — Full Calculus I lectures (YouTube)</li>
          <li>Stewart's Calculus (textbook, 8th ed.) — standard at USC</li>
          <li>Desmos Graphing Calculator (desmos.com) — visualize everything</li>
          <li>Paul's Online Math Notes (tutorial.math.lamar.edu)</li>
          <li>MIT 18.01 OpenCourseWare — free practice exams</li>
          <li>WolframAlpha — check your work, not do your work</li>
        </ul>
      </div>

      <div class="resource-card chem">
        <h4>⚗️ CHEM 105a Resources</h4>
        <ul class="resource-list">
          <li>CrashCourse Chemistry (YouTube, free, 46 episodes)</li>
          <li>Khan Academy Chemistry — full course with exercises</li>
          <li>Zumdahl's "Chemistry" — common USC general chem text</li>
          <li>ChemLibreTexts (chem.libretexts.org) — free textbook</li>
          <li>Anki — for nomenclature and formula flashcards</li>
          <li>Tyler DeWitt (YouTube) — excellent for beginners</li>
          <li>AP Chemistry practice tests (College Board)</li>
        </ul>
      </div>

      <div class="resource-card cs">
        <h4>💻 CSCI 102 Resources</h4>
        <ul class="resource-list">
          <li>CS50P (Harvard, edx.org/cs50) — free Python course</li>
          <li>CS50x — broader intro to CS concepts (also free)</li>
          <li>Python.org official tutorial (docs.python.org)</li>
          <li>Automate the Boring Stuff (automatetheboringstuff.com)</li>
          <li>Replit.com — browser-based Python coding environment</li>
          <li>LeetCode Easy problems — algorithmic thinking practice</li>
          <li>NeetCode (YouTube) — algorithms explained clearly</li>
        </ul>
      </div>

      <div class="resource-card gen">
        <h4>🎓 General Study Tools</h4>
        <ul class="resource-list">
          <li>Anki (apps.ankiweb.net) — spaced repetition flashcards</li>
          <li>Notion or Obsidian — organized note-taking with links</li>
          <li>Pomodoro Timer — 50 min focus / 10 min break rhythm</li>
          <li>USC Libraries (online access, free) — digital textbooks</li>
          <li>Wolfram Problem Generator — math practice sets</li>
          <li>Khan Academy — all three subjects at foundational level</li>
          <li>Trello or Google Calendar — block-schedule your weeks</li>
        </ul>
      </div>

    </div>
  </div>

</main>

<footer>
  <strong>Fight On! ✌️</strong> · University of Southern California · Class of 2030<br>
  Study plan prepared for incoming freshmen · MATH 125 · CHEM 105a · CSCI 102
</footer>

<script>
  function toggleWeek(header) {
    const days = header.nextElementSibling;
    const toggle = header.querySelector('.week-toggle');
    const isOpen = days.classList.contains('open');
    days.classList.toggle('open', !isOpen);
    toggle.classList.toggle('open', !isOpen);
  }

  // Open week 1 by default
  document.addEventListener('DOMContentLoaded', () => {
    const firstHeader = document.querySelector('.week-header');
    if (firstHeader) toggleWeek(firstHeader);
  });
</script>

</body>
</html>

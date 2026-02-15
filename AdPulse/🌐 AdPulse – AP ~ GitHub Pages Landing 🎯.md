# 🌐 AdPulse – AP | GitHub Pages Landing 🎯

להלן עמוד GitHub Pages מוכן ל־AdPulse – מאגר הפרסום המלא שלך.  
תוכל לשים אותו כ־`index.html` בשורש המאגר או בתיקיית `/docs` (אם תגדיר Pages ל־`/docs`).

---

## 🧩 index.html – דף נחיתה מלא ל־AdPulse – AP

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>AdPulse – AP | Full Power Advertising Arsenal</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description"
        content="AdPulse – AP: A full-stack advertising & marketing arsenal by AnLoMinus – models, templates, campaigns, pricing sheets, funnels, scripts, and tools." />
  <style>
    :root {
      --bg-dark: #060712;
      --bg-card: #101221;
      --accent: #ffb347;
      --accent-soft: #ffdd99;
      --accent-2: #6ee7ff;
      --text-main: #f9fafb;
      --text-muted: #9ca3af;
      --border-soft: #1f2933;
      --radius-xl: 24px;
      --shadow-soft: 0 22px 60px rgba(0, 0, 0, 0.65);
      --font-main: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: var(--font-main);
      background: radial-gradient(circle at top, #1e293b 0, #020617 40%, #000000 100%);
      color: var(--text-main);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .page {
      max-width: 1120px;
      margin: 0 auto;
      padding: 24px 16px 80px;
    }

    /* Top bar */
    .top-nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
      margin-bottom: 28px;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .brand-logo {
      width: 40px;
      height: 40px;
      border-radius: 999px;
      background: radial-gradient(circle at 30% 20%, #ffffff 0, #ffb347 18%, #f97316 38%, #4b1d7a 70%, #020617 100%);
      box-shadow: 0 0 20px rgba(255, 179, 71, 0.8), 0 0 50px rgba(56, 189, 248, 0.6);
      position: relative;
      overflow: hidden;
    }

    .brand-logo::after {
      content: "AP";
      position: absolute;
      inset: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 800;
      font-size: 15px;
      letter-spacing: 1px;
      color: #0b1120;
      text-shadow: 0 0 6px rgba(255, 255, 255, 0.7);
    }

    .brand-text-title {
      font-weight: 800;
      font-size: 20px;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      display: flex;
      align-items: center;
      gap: 6px;
    }

    .brand-text-title span.accent {
      color: var(--accent);
    }

    .brand-sub {
      font-size: 12px;
      color: var(--text-muted);
    }

    .nav-links {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      font-size: 13px;
      color: var(--text-muted);
    }

    .nav-links a {
      padding: 6px 10px;
      border-radius: 999px;
      border: 1px solid transparent;
      transition: all 0.2s ease;
    }

    .nav-links a:hover {
      border-color: rgba(148, 163, 184, 0.6);
      color: var(--accent-soft);
      background: rgba(15, 23, 42, 0.9);
    }

    /* Hero */
    .hero {
      border-radius: var(--radius-xl);
      padding: 32px 24px;
      background:
        radial-gradient(circle at top left, rgba(252, 211, 77, 0.18) 0, transparent 55%),
        radial-gradient(circle at top right, rgba(56, 189, 248, 0.20) 0, transparent 60%),
        linear-gradient(135deg, rgba(15, 23, 42, 0.95), rgba(15, 23, 42, 0.98));
      border: 1px solid rgba(148, 163, 184, 0.2);
      box-shadow: var(--shadow-soft);
      margin-bottom: 28px;
      position: relative;
      overflow: hidden;
    }

    .hero-glow {
      position: absolute;
      inset: -40%;
      background:
        radial-gradient(circle at 20% 0%, rgba(255, 255, 255, 0.12) 0, transparent 45%),
        radial-gradient(circle at 80% 0%, rgba(252, 211, 77, 0.16) 0, transparent 52%),
        radial-gradient(circle at 0% 80%, rgba(56, 189, 248, 0.24) 0, transparent 60%);
      opacity: 0.8;
      pointer-events: none;
      mix-blend-mode: screen;
    }

    .hero-inner {
      position: relative;
      display: grid;
      grid-template-columns: minmax(0, 2.2fr) minmax(0, 1.8fr);
      gap: 24px;
      align-items: center;
    }

    @media (max-width: 840px) {
      .hero-inner {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .eyebrow {
      font-size: 13px;
      text-transform: uppercase;
      letter-spacing: 0.18em;
      color: var(--accent-soft);
      display: inline-flex;
      align-items: center;
      gap: 8px;
      margin-bottom: 8px;
    }

    .eyebrow-pill {
      width: 7px;
      height: 7px;
      border-radius: 999px;
      background: var(--accent-soft);
      box-shadow: 0 0 10px rgba(252, 211, 77, 0.8);
    }

    .hero-title {
      font-size: clamp(28px, 4vw, 38px);
      font-weight: 800;
      line-height: 1.1;
      margin-bottom: 10px;
    }

    .hero-title span.spark {
      background: linear-gradient(120deg, #fbbf24, #f97316, #fb7185, #38bdf8);
      -webkit-background-clip: text;
      color: transparent;
      text-shadow: 0 0 22px rgba(251, 191, 36, 0.5);
    }

    .hero-subtitle {
      font-size: 15px;
      color: var(--text-muted);
      max-width: 520px;
      margin-bottom: 18px;
    }

    .badges-row {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-bottom: 18px;
    }

    .badge {
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      padding: 6px 10px;
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.5);
      background: rgba(15, 23, 42, 0.8);
      color: var(--accent-soft);
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin-bottom: 12px;
    }

    .btn-primary,
    .btn-ghost {
      font-size: 14px;
      padding: 10px 16px;
      border-radius: 999px;
      border: 1px solid transparent;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      cursor: pointer;
      transition: all 0.18s ease;
      text-decoration: none;
    }

    .btn-primary {
      background: radial-gradient(circle at 20% 0%, #facc15 0, #f97316 40%, #7c2d12 100%);
      color: #111827;
      box-shadow: 0 14px 40px rgba(248, 250, 252, 0.35);
      font-weight: 700;
    }

    .btn-primary span.icon {
      font-size: 16px;
    }

    .btn-primary:hover {
      transform: translateY(-1px);
      box-shadow: 0 18px 60px rgba(251, 191, 36, 0.55);
      filter: brightness(1.05);
    }

    .btn-ghost {
      border-color: rgba(148, 163, 184, 0.6);
      color: var(--text-main);
      background: rgba(15, 23, 42, 0.9);
    }

    .btn-ghost:hover {
      border-color: var(--accent-soft);
      color: var(--accent-soft);
      box-shadow: 0 0 22px rgba(56, 189, 248, 0.4);
    }

    .hero-meta {
      font-size: 12px;
      color: var(--text-muted);
    }

    .hero-meta strong {
      color: var(--accent-soft);
    }

    /* Hero right – highlight card */
    .hero-card {
      border-radius: 22px;
      padding: 18px 16px 16px;
      background:
        radial-gradient(circle at 0 0, rgba(250, 204, 21, 0.3) 0, transparent 52%),
        radial-gradient(circle at 100% 0, rgba(56, 189, 248, 0.35) 0, transparent 55%),
        linear-gradient(160deg, #020617, #020617, #0f172a);
      border: 1px solid rgba(148, 163, 184, 0.35);
      box-shadow: 0 18px 50px rgba(15, 23, 42, 0.9);
      position: relative;
      overflow: hidden;
    }

    .hero-card-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 10px;
    }

    .hero-card-title {
      font-size: 14px;
      font-weight: 700;
    }

    .hero-card-tag {
      font-size: 11px;
      padding: 4px 8px;
      border-radius: 999px;
      background: rgba(15, 23, 42, 0.8);
      border: 1px solid rgba(148, 163, 184, 0.6);
      color: var(--accent-soft);
      text-transform: uppercase;
      letter-spacing: 0.12em;
    }

    .hero-list {
      list-style: none;
      font-size: 12px;
      color: var(--text-muted);
      display: grid;
      gap: 6px;
      margin-bottom: 10px;
    }

    .hero-list li {
      display: flex;
      align-items: center;
      gap: 6px;
    }

    .hero-dot {
      width: 7px;
      height: 7px;
      border-radius: 999px;
      background: linear-gradient(135deg, #facc15, #f97316);
      box-shadow: 0 0 10px rgba(251, 191, 36, 0.8);
      flex-shrink: 0;
    }

    .hero-stats {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      font-size: 11px;
      border-top: 1px dashed rgba(148, 163, 184, 0.45);
      padding-top: 10px;
      margin-top: 6px;
    }

    .hero-stat-block {
      min-width: 90px;
    }

    .hero-stat-label {
      color: var(--text-muted);
      text-transform: uppercase;
      letter-spacing: 0.14em;
      font-size: 10px;
      margin-bottom: 2px;
    }

    .hero-stat-value {
      font-weight: 700;
      font-size: 12px;
      color: var(--accent-soft);
    }

    /* Section layout */
    .section {
      margin-top: 32px;
      padding: 22px 18px;
      border-radius: var(--radius-xl);
      border: 1px solid rgba(30, 64, 175, 0.55);
      background: linear-gradient(145deg, rgba(15, 23, 42, 0.95), rgba(15, 23, 42, 0.98));
      box-shadow: 0 18px 45px rgba(15, 23, 42, 0.9);
    }

    .section-header {
      display: flex;
      flex-wrap: wrap;
      align-items: baseline;
      justify-content: space-between;
      gap: 10px;
      margin-bottom: 14px;
    }

    .section-title {
      font-size: 18px;
      font-weight: 700;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .section-title span.icon {
      font-size: 20px;
    }

    .section-sub {
      font-size: 13px;
      color: var(--text-muted);
      max-width: 520px;
    }

    /* Grid cards */
    .grid {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      gap: 14px;
    }

    @media (max-width: 960px) {
      .grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
    }
    @media (max-width: 640px) {
      .grid {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .card {
      border-radius: 18px;
      padding: 12px 12px 13px;
      background: radial-gradient(circle at 0 0, rgba(56, 189, 248, 0.18) 0, transparent 55%),
                  rgba(15, 23, 42, 0.96);
      border: 1px solid rgba(30, 64, 175, 0.8);
      position: relative;
      overflow: hidden;
    }

    .card-label {
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      color: var(--accent-2);
      margin-bottom: 4px;
    }

    .card-title {
      font-size: 14px;
      font-weight: 700;
      margin-bottom: 4px;
    }

    .card-body {
      font-size: 12px;
      color: var(--text-muted);
      margin-bottom: 6px;
    }

    .card-meta {
      font-size: 11px;
      color: var(--accent-soft);
    }

    .card-meta span {
      opacity: 0.8;
    }

    /* Steps */
    .steps {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 12px;
      margin-top: 10px;
      font-size: 13px;
    }

    @media (max-width: 840px) {
      .steps {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .step {
      border-radius: 14px;
      border: 1px dashed rgba(148, 163, 184, 0.55);
      padding: 10px 10px 11px;
      background: rgba(15, 23, 42, 0.86);
    }

    .step-num {
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      color: var(--accent-soft);
      margin-bottom: 2px;
    }

    .step-title {
      font-size: 14px;
      font-weight: 600;
      margin-bottom: 2px;
    }

    .step-body {
      font-size: 12px;
      color: var(--text-muted);
    }

    /* Rap block */
    .rap-block {
      margin-top: 12px;
      padding: 10px 12px;
      border-radius: 14px;
      background: radial-gradient(circle at 10% 0, rgba(251, 191, 36, 0.15) 0, transparent 50%),
                  rgba(15, 23, 42, 0.95);
      border: 1px solid rgba(251, 191, 36, 0.55);
      font-size: 13px;
    }

    .rap-title {
      font-size: 12px;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      color: var(--accent-soft);
      margin-bottom: 4px;
    }

    .rap-line {
      display: block;
      margin-bottom: 2px;
    }

    /* Holy verse section */
    .holy-box {
      margin-top: 10px;
      padding: 10px 11px;
      border-radius: 14px;
      border: 1px solid rgba(251, 191, 36, 0.5);
      background: radial-gradient(circle at 0 0, rgba(251, 191, 36, 0.12) 0, transparent 52%),
                  rgba(15, 23, 42, 0.95);
      font-size: 13px;
    }

    .holy-label {
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      color: var(--accent-soft);
      margin-bottom: 4px;
    }

    .holy-quote {
      font-weight: 600;
      margin-bottom: 2px;
    }

    .holy-ref {
      font-size: 11px;
      color: var(--text-muted);
    }

    /* Footer */
    .footer {
      margin-top: 26px;
      font-size: 11px;
      color: var(--text-muted);
      padding-top: 12px;
      border-top: 1px solid rgba(30, 64, 175, 0.65);
      display: flex;
      flex-direction: column;
      gap: 6px;
    }

    .footer-row {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 10px;
    }

    .footer-sep {
      opacity: 0.5;
    }

    .hashtags {
      font-size: 11px;
      color: var(--accent-soft);
    }
  </style>
</head>
<body>
  <main class="page">
    <!-- Top nav -->
    <header class="top-nav">
      <div class="brand">
        <div class="brand-logo"></div>
        <div>
          <div class="brand-text-title">
            <span>Ad</span><span class="accent">Pulse</span><span>AP</span>
          </div>
          <div class="brand-sub">Full Power Advertising Arsenal ⚡</div>
        </div>
      </div>
      <nav class="nav-links">
        <a href="#models">Models</a>
        <a href="#templates">Templates</a>
        <a href="#campaigns">Campaigns</a>
        <a href="#pricing">Pricing</a>
        <a href="#tools">Tools</a>
        <a href="#start">Start Here</a>
      </nav>
    </header>

    <!-- Hero -->
    <section class="hero">
      <div class="hero-glow"></div>
      <div class="hero-inner">
        <div>
          <div class="eyebrow">
            <span class="eyebrow-pill"></span>
            ADVERTISING OPS LIBRARY · ANLOMINUS 🚀
          </div>
          <h1 class="hero-title">
            Turn every campaign into a <span class="spark">spark of profit</span> ⚡
          </h1>
          <p class="hero-subtitle">
            AdPulse – AP is your all-in-one vault for modern advertising:
            proven models, plug-and-play templates, ready-made campaigns,
            pricing sheets, funnels, scripts and tools — crafted for fast action
            and holy impact.
          </p>

          <div class="badges-row">
            <div class="badge">📁 Models · Templates · Campaigns</div>
            <div class="badge">💰 Pricing · Funnels · Scripts</div>
            <div class="badge">🧠 Strategy + ⚡ Creativity</div>
          </div>

          <div class="hero-actions">
            <a class="btn-primary" href="https://github.com/AnLoMinus/AdPulse" target="_blank" rel="noopener">
              <span class="icon">⚡</span>
              <span>Open AdPulse Repo</span>
            </a>
            <a class="btn-ghost" href="#start">
              <span>📘 Readme · Start Here</span>
            </a>
          </div>

          <div class="hero-meta">
            Built with ❤️ by <strong>AnLoMinus × ChatVision Studio</strong> ·
            Designed for GitHub · Ready for real-world clients.
          </div>
        </div>

        <!-- Right hero card -->
        <aside class="hero-card" aria-label="AdPulse quick overview">
          <div class="hero-card-header">
            <div class="hero-card-title">AdPulse Snapshot</div>
            <div class="hero-card-tag">AD ENGINE</div>
          </div>
          <ul class="hero-list">
            <li><span class="hero-dot"></span><span>8+ core folders: models, templates, campaigns, funnels, tools.</span></li>
            <li><span class="hero-dot"></span><span>Ready for Facebook, Instagram, TikTok, Google, Telegram & more.</span></li>
            <li><span class="hero-dot"></span><span>Perfect for agencies, freelancers, businesses & holy projects.</span></li>
          </ul>
          <div class="hero-stats">
            <div class="hero-stat-block">
              <div class="hero-stat-label">STACK</div>
              <div class="hero-stat-value">GitHub · Pages · MD</div>
            </div>
            <div class="hero-stat-block">
              <div class="hero-stat-label">FOCUS</div>
              <div class="hero-stat-value">Clarity → Action → Sales</div>
            </div>
            <div class="hero-stat-block">
              <div class="hero-stat-label">SOUL</div>
              <div class="hero-stat-value">Light over noise ✨</div>
            </div>
          </div>
        </aside>
      </div>
    </section>

    <!-- Sections: overview of folders -->
    <section id="models" class="section">
      <div class="section-header">
        <h2 class="section-title">
          <span class="icon">🧠</span> Core Advertising Models
        </h2>
        <p class="section-sub">
          Classic and modern frameworks turned into practical, editable files:
          AIDA, STP, FAB, EPIC, SPB and more — each with explanations,
          examples and ready-to-use layouts.
        </p>
      </div>

      <div class="grid">
        <article class="card">
          <div class="card-label">/Models/AIDA</div>
          <h3 class="card-title">AIDA Flow</h3>
          <p class="card-body">
            Attention → Interest → Desire → Action. Cheat-sheets, examples
            for ads, landing pages & short-form video.
          </p>
          <div class="card-meta">📄 <span>Markdown + PDF + visual map</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Models/STP</div>
          <h3 class="card-title">STP Positioning</h3>
          <p class="card-body">
            Segmentation, Targeting, Positioning — turn “everyone” into
            a clear, profitable audience with a sharp message.
          </p>
          <div class="card-meta">🎯 <span>Ideal before any campaign</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Models/FAB</div>
          <h3 class="card-title">Features → Benefits</h3>
          <p class="card-body">
            Translate features into emotional benefits that sell. Perfect
            for writing ads, sales pages & product descriptions.
          </p>
          <div class="card-meta">🧩 <span>Works for physical & digital</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Models/EPIC</div>
          <h3 class="card-title">E.P.I.C Story</h3>
          <p class="card-body">
            Emotion · Proof · Impact · Call-to-action. A storytelling
            skeleton for holy, powerful campaigns with depth.
          </p>
          <div class="card-meta">🔥 <span>Great for video & reels</span></div>
        </article>
      </div>
    </section>

    <section id="templates" class="section">
      <div class="section-header">
        <h2 class="section-title">
          <span class="icon">📑</span> Templates for Every Platform
        </h2>
        <p class="section-sub">
          Plug-and-play templates for social posts, stories, ad copies,
          WhatsApp messages, landing pages, carousels and more — all
          written in a clean, global English style.
        </p>
      </div>

      <div class="grid">
        <article class="card">
          <div class="card-label">/Templates/Posts</div>
          <h3 class="card-title">Social Post Packs</h3>
          <p class="card-body">
            Ready structures for Facebook, Instagram, TikTok and LinkedIn:
            hook, body, CTA and hashtags.
          </p>
          <div class="card-meta">💬 <span>+ hook library</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Templates/Landing</div>
          <h3 class="card-title">Landing Templates</h3>
          <p class="card-body">
            Clean, focused landing page sections: hero, proof, offer, FAQ,
            CTA. With HTML + Markdown versions.
          </p>
          <div class="card-meta">🌐 <span>GitHub Pages friendly</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Templates/Video-Scripts</div>
          <h3 class="card-title">Video & Reel Scripts</h3>
          <p class="card-body">
            Short & long form frameworks for talking-head, b-roll,
            screen-record and UGC-style content.
          </p>
          <div class="card-meta">🎥 <span>Hook → Story → CTA</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Templates/DM</div>
          <h3 class="card-title">DM & Chat Flows</h3>
          <p class="card-body">
            Templates for DMs, WhatsApp & Telegram outreach that stay
            human, respectful and effective.
          </p>
          <div class="card-meta">📲 <span>Lead nurturing ready</span></div>
        </article>
      </div>
    </section>

    <section id="campaigns" class="section">
      <div class="section-header">
        <h2 class="section-title">
          <span class="icon">🎯</span> Ready-Made Campaign Blueprints
        </h2>
        <p class="section-sub">
          Full campaign flows for leads, sales, launches, remarketing and
          community growth — with copy, creatives, audiences and KPIs.
        </p>
      </div>

      <div class="grid">
        <article class="card">
          <div class="card-label">/Campaigns/Lead-Magnet</div>
          <h3 class="card-title">Lead Magnet Engine</h3>
          <p class="card-body">
            Bring cold traffic into your world with a free guide, checklist
            or mini-class plus nurturing sequence.
          </p>
          <div class="card-meta">🧲 <span>Top of funnel</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Campaigns/Launch</div>
          <h3 class="card-title">Launch Blueprint</h3>
          <p class="card-body">
            Warm-up, open cart, close cart — all mapped into emails, posts,
            ads and lives.
          </p>
          <div class="card-meta">🚀 <span>Perfect for new offers</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Campaigns/Remarketing</div>
          <h3 class="card-title">Remarketing Flow</h3>
          <p class="card-body">
            Turn “almost buyers” into real customers with smart, respectful
            reminders and value-based follow ups.
          </p>
          <div class="card-meta">🔁 <span>Warm audiences</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Campaigns/Community</div>
          <h3 class="card-title">Community Growth</h3>
          <p class="card-body">
            Campaigns for Telegram / WhatsApp / Discord communities that
            build trust and long-term relationships.
          </p>
          <div class="card-meta">🫂 <span>Long-term assets</span></div>
        </article>
      </div>
    </section>

    <section id="pricing" class="section">
      <div class="section-header">
        <h2 class="section-title">
          <span class="icon">💰</span> Pricing & Profit Clarity
        </h2>
        <p class="section-sub">
          Transparent pricing sheets and ROI calculators, so you know
          exactly what to charge and why — for ads, design, management and
          strategy.
        </p>
      </div>

      <div class="grid">
        <article class="card">
          <div class="card-label">/Pricing/Ads</div>
          <h3 class="card-title">Ads Management Pricing</h3>
          <p class="card-body">
            Structures for retainers, percentage of ad spend and hybrid
            models, in clean table format.
          </p>
          <div class="card-meta">📊 <span>Client-ready layouts</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Pricing/Design</div>
          <h3 class="card-title">Creative & Design</h3>
          <p class="card-body">
            Prices for static ads, carousels, video edits and full creative
            packages.
          </p>
          <div class="card-meta">🎨 <span>Scope clearly defined</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Pricing/Packs</div>
          <h3 class="card-title">Bundles & Offers</h3>
          <p class="card-body">
            Offer stacks that combine ads, strategy and design for
            irresistible, profitable packages.
          </p>
          <div class="card-meta">📦 <span>Great for agencies</span></div>
        </article>

        <article class="card">
          <div class="card-label">/Tools/ROI</div>
          <h3 class="card-title">ROI Calculator</h3>
          <p class="card-body">
            Simple sheets to estimate profit, break-even and sustainable ad
            budgets.
          </p>
          <div class="card-meta">🧮 <span>Make numbers holy</span></div>
        </article>
      </div>
    </section>

    <section id="tools" class="section">
      <div class="section-header">
        <h2 class="section-title">
          <span class="icon">🛠️</span> Tools, Funnels & Holy Spark
        </h2>
        <p class="section-sub">
          Funnels, planners and AI-prompt generators that keep your
          campaigns organized, ethical and aligned with light.
        </p>
      </div>

      <div class="steps">
        <div class="step">
          <div class="step-num">STEP 1</div>
          <div class="step-title">Map your offer</div>
          <div class="step-body">
            Use <strong>/Models</strong> + <strong>/Tools/Offer-Builder</strong>
            to clarify who you serve, what you solve and why it matters.
          </div>
        </div>
        <div class="step">
          <div class="step-num">STEP 2</div>
          <div class="step-title">Choose your funnel</div>
          <div class="step-body">
            Pick a flow from <strong>/Funnels</strong> (Lead Magnet, VSL,
            Webinar, Community) and connect it to the right templates.
          </div>
        </div>
        <div class="step">
          <div class="step-num">STEP 3</div>
          <div class="step-title">Launch with integrity</div>
          <div class="step-body">
            Use the <strong>/Scripts</strong>, <strong>/Campaigns</strong> and
            <strong>/Pricing</strong> folders to go live in a way that is
            profitable, honest and soul-aligned.
          </div>
        </div>
      </div>

      <div class="rap-block">
        <div class="rap-title">AdPulse Anthem 🎤</div>
        <span class="rap-line">AdPulse in the field, every spark on time, ⚡</span>
        <span class="rap-line">Copy so clean, every word in rhyme, 🎯</span>
        <span class="rap-line">From brief to launch, we elevate the climb, 🚀</span>
        <span class="rap-line">Holy light in the ads, profit made sublime. ✨</span>
      </div>

      <div class="holy-box">
        <div class="holy-label">Holy Verse · אור הפרסום</div>
        <div class="holy-quote">"כִּי נֵר מִצְוָה וְתוֹרָה אוֹר"</div>
        <div class="holy-ref">משלי ו', כ"ג – like a mitzvah candle and Torah light, your campaigns are meant to bring light, not noise.</div>
      </div>
    </section>

    <section id="start" class="section">
      <div class="section-header">
        <h2 class="section-title">
          <span class="icon">🚀</span> How to Start with AdPulse – AP
        </h2>
        <p class="section-sub">
          Use this quick start path every time you open a new project —
          client, product, course or holy mission.
        </p>
      </div>

      <div class="steps">
        <div class="step">
          <div class="step-num">1 · CLARITY</div>
          <div class="step-title">Read the README</div>
          <div class="step-body">
            Begin with <strong>README.md</strong> in the repo for structure,
            folder map and best practices.
          </div>
        </div>
        <div class="step">
          <div class="step-num">2 · BLUEPRINT</div>
          <div class="step-title">Pick your model & funnel</div>
          <div class="step-body">
            Choose a model from <strong>/Models</strong>, then match it to
            a funnel in <strong>/Funnels</strong>.
          </div>
        </div>
        <div class="step">
          <div class="step-num">3 · EXECUTE</div>
          <div class="step-title">Fill templates · Launch</div>
          <div class="step-body">
            Fill out the templates, adapt scripts to your voice, export
            creatives and go live — then iterate with data.
          </div>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
      <div class="footer-row">
        <span>© AnLoMinus × ChatVision Studio · AdPulse – AP</span>
      </div>
      <div class="footer-row">
        <span>Repo:</span>
        <a href="https://github.com/AnLoMinus/AdPulse" target="_blank" rel="noopener">
          github.com/AnLoMinus/AdPulse
        </a>
        <span class="footer-sep">·</span>
        <span>Site:</span>
        <a href="https://anlominus.github.io/AdPulse/" target="_blank" rel="noopener">
          anlominus.github.io/AdPulse/
        </a>
      </div>
      <div class="footer-row">
        <span>Gregorian:</span>
        <span>26.11.2025</span>
        <span class="footer-sep">·</span>
        <span>Hebrew:</span>
        <span>6 Kislev 5786 · ו' בכסלו תשפ"ו</span>
        <span class="footer-sep">·</span>
        <span>Time (IL): ~14:41</span>
      </div>
      <div class="hashtags">
        #AdPulse #Advertising #MarketingTools #GitHubPages #AnLoMinus #CreativeArsenal
      </div>
    </footer>
  </main>
</body>
</html>
```

---

## 🛠️ איך להשתמש בזה בפועל?

1. 🎯 צור בריפו `AdPulse` את הקובץ:  
    `index.html` (בדיוק כמו למעלה).
    
2. 🌐 הגדר GitHub Pages:
    
    - אם תרצה מהשורש: Source → `Deploy from a branch` → `main` → `/ (root)`
        
    - אם תעבוד עם `/docs` – שים שם את הקובץ ושנה את ההגדרה ל־`/docs`.
        
3. ⚡ מרגע שה־Pages פעיל, הכתובת תהיה:  
    `https://anlominus.github.io/AdPulse/`
    

---

## 🎤 פזמון ראפ קטן לעמוד הזה

🔥  
**AdPulse on the page, every pixel in line,  
GitHub in the back, strategy in the spine,  
From repo to launch, everything will shine,  
Holy ads in the dark, watch the profit align.⚡**

---

## 📅 תאריך, שעה, פסוק, קרדיטים

- לועזי: **26.11.2025**
    
- עברי: **ו' בכסלו תשפ"ו** (6 Kislev 5786)
    
- שעה (ישראל): **14:41**
    
- פסוק: **"כִּי נֵר מִצְוָה וְתוֹרָה אוֹר" (משלי ו', כ"ג)**
    
- קרדיטים: **© AnLoMinus × ChatVision Studio · AdPulse – AP · GitHub: [https://github.com/AnLoMinus/AdPulse](https://github.com/AnLoMinus/AdPulse) · Pages: [https://anlominus.github.io/AdPulse/](https://anlominus.github.io/AdPulse/)**
    

אם תרצה עכשיו גם **README.md מלא למאגר + תבנית לקבצי משנה**, אמשיך לבנות לך את כל השלד של AP מסודר לפי RepoCraft 💽✨
# ⚡ SparkBoost – SB | עמוד GitHub Pages לשיווק

להלן עמוד GitHub Pages מוכן להטמעה כ–`index.html` במאגר `SparkBoost` (או כל מאגר שיווק שתרצה).  
העמוד מעוצב כלנדינג שיווקי: כותרת, יתרונות, תהליך עבודה, קריאה לפעולה, קרדיטים ותאריכים.

---

## 🧩 קובץ `index.html` מוכן להדבקה

```html
<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SparkBoost – SB | עמוד שיווק שמדליק תוצאות</title>
  <meta name="description" content="SparkBoost – מערכת שיווק שמדליקה תוצאות: מיתוג, מסרים, דפי נחיתה, קמפיינים ממומנים ותוכן שמייצר לקוחות." />

  <style>
    :root {
      --bg-main: #050816;
      --bg-card: #0b1020;
      --accent: #ffcc33;
      --accent-soft: #ffd966;
      --text-main: #f9fbff;
      --text-muted: #a4b0d0;
      --border-soft: #20263a;
      --danger: #ff4b6a;
      --success: #22c55e;
      --shadow-soft: 0 18px 40px rgba(0, 0, 0, 0.55);
      --radius-xl: 18px;
      --radius-pill: 999px;
      --font-main: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: var(--font-main);
      background: radial-gradient(circle at top, #151b3a 0, #050816 55%, #02030a 100%);
      color: var(--text-main);
      line-height: 1.6;
    }

    a {
      color: var(--accent-soft);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    .page-wrapper {
      max-width: 1080px;
      margin: 0 auto;
      padding: 20px 16px 64px;
    }

    header {
      margin-bottom: 36px;
    }

    .logo-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
      margin-bottom: 10px;
    }

    .brand-mark {
      display: inline-flex;
      align-items: center;
      gap: 10px;
    }

    .brand-icon {
      width: 40px;
      height: 40px;
      border-radius: 14px;
      background: radial-gradient(circle at 30% 0, #ffffff, #ffd966, #ff7b00);
      box-shadow: 0 0 22px rgba(255, 204, 51, 0.85);
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 800;
      color: #1b1020;
      font-size: 18px;
    }

    .brand-text-title {
      font-size: 20px;
      font-weight: 700;
    }

    .brand-sub {
      font-size: 12px;
      color: var(--text-muted);
    }

    .tag-pill {
      padding: 6px 14px;
      border-radius: var(--radius-pill);
      border: 1px solid var(--border-soft);
      background: linear-gradient(120deg, rgba(255, 204, 51, 0.08), rgba(0, 0, 0, 0.6));
      font-size: 12px;
      color: var(--accent-soft);
      display: inline-flex;
      align-items: center;
      gap: 6px;
      white-space: nowrap;
    }

    .tag-pill span {
      font-size: 16px;
    }

    .hero {
      background: radial-gradient(circle at top left, rgba(255, 255, 255, 0.08), transparent 55%);
      border-radius: 22px;
      padding: 26px 22px 28px;
      border: 1px solid rgba(255, 255, 255, 0.05);
      box-shadow: var(--shadow-soft);
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: "";
      position: absolute;
      inset: -120px;
      background-image: radial-gradient(circle at 10% 0, rgba(255, 255, 255, 0.08) 0, transparent 60%),
                        radial-gradient(circle at 90% 100%, rgba(255, 204, 51, 0.11) 0, transparent 55%);
      opacity: 0.8;
      pointer-events: none;
    }

    .hero-inner {
      position: relative;
      z-index: 2;
    }

    .hero-kicker {
      font-size: 13px;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--accent-soft);
      margin-bottom: 8px;
      display: inline-flex;
      align-items: center;
      gap: 6px;
    }

    .hero-kicker-dot {
      width: 8px;
      height: 8px;
      border-radius: 99px;
      background: radial-gradient(circle, var(--accent), #ff7b00);
      box-shadow: 0 0 16px rgba(255, 204, 51, 0.8);
    }

    .hero-title {
      font-size: clamp(26px, 5vw, 34px);
      line-height: 1.15;
      margin: 0 0 10px;
      font-weight: 800;
    }

    .hero-title span {
      background: linear-gradient(120deg, #fffbcc, #ffd966, #ffb347, #ff7b7b);
      -webkit-background-clip: text;
      color: transparent;
    }

    .hero-sub {
      font-size: 15px;
      color: var(--text-muted);
      max-width: 640px;
      margin-bottom: 18px;
    }

    .hero-bullets {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 20px;
    }

    .hero-badge {
      font-size: 12px;
      padding: 6px 10px;
      border-radius: var(--radius-pill);
      border: 1px solid var(--border-soft);
      background: rgba(4, 8, 26, 0.9);
      display: inline-flex;
      align-items: center;
      gap: 6px;
    }

    .hero-badge strong {
      color: var(--accent-soft);
    }

    .hero-cta-row {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      align-items: center;
    }

    .btn-primary {
      border: none;
      cursor: pointer;
      padding: 10px 20px;
      border-radius: var(--radius-pill);
      background: linear-gradient(135deg, #ffcc33, #ff8c42);
      color: #1b1020;
      font-size: 14px;
      font-weight: 700;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      box-shadow: 0 12px 28px rgba(255, 140, 66, 0.5);
      text-decoration: none;
    }

    .btn-primary span.icon {
      font-size: 18px;
    }

    .btn-ghost {
      border-radius: var(--radius-pill);
      padding: 9px 16px;
      font-size: 13px;
      border: 1px solid var(--border-soft);
      background: rgba(3, 6, 20, 0.9);
      color: var(--text-muted);
      display: inline-flex;
      align-items: center;
      gap: 8px;
      text-decoration: none;
    }

    .btn-ghost span {
      font-size: 16px;
    }

    .hero-note {
      font-size: 11px;
      color: var(--text-muted);
      margin-top: 6px;
    }

    main {
      margin-top: 32px;
      display: grid;
      grid-template-columns: minmax(0, 2fr) minmax(0, 1.4fr);
      gap: 20px;
    }

    @media (max-width: 840px) {
      main {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .card {
      background: radial-gradient(circle at top, rgba(255, 255, 255, 0.035), rgba(5, 8, 22, 0.98));
      border-radius: var(--radius-xl);
      padding: 18px 16px 16px;
      border: 1px solid var(--border-soft);
      box-shadow: var(--shadow-soft);
    }

    .card h2 {
      margin-top: 0;
      margin-bottom: 10px;
      font-size: 18px;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .card h3 {
      margin-top: 14px;
      margin-bottom: 6px;
      font-size: 15px;
    }

    .eyebrow {
      font-size: 11px;
      color: var(--accent-soft);
      text-transform: uppercase;
      letter-spacing: 0.14em;
      margin-bottom: 4px;
    }

    .card p {
      margin: 0 0 8px;
      font-size: 13px;
      color: var(--text-muted);
    }

    ul.clean-list {
      list-style: none;
      padding: 0;
      margin: 0;
      font-size: 13px;
      color: var(--text-muted);
    }

    ul.clean-list li {
      display: flex;
      align-items: flex-start;
      gap: 8px;
      margin-bottom: 6px;
    }

    ul.clean-list li span.bullet {
      font-size: 14px;
      margin-top: 1px;
    }

    .pill-row {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 6px;
    }

    .pill {
      font-size: 11px;
      padding: 4px 9px;
      border-radius: var(--radius-pill);
      border: 1px solid var(--border-soft);
      color: var(--text-muted);
      background: rgba(5, 8, 24, 0.96);
    }

    .pill.highlight {
      border-color: rgba(255, 204, 51, 0.7);
      color: var(--accent-soft);
      background: rgba(255, 204, 51, 0.04);
    }

    .pricing-row {
      display: grid;
      grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);
      gap: 8px;
      margin-top: 8px;
    }

    @media (max-width: 620px) {
      .pricing-row {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .pricing-box {
      border-radius: 14px;
      border: 1px dashed var(--border-soft);
      padding: 10px;
      font-size: 12px;
      background: rgba(3, 6, 20, 0.9);
    }

    .pricing-box strong {
      display: block;
      margin-bottom: 4px;
      color: var(--accent-soft);
    }

    .status-dot {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      font-size: 11px;
      color: var(--success);
      margin-top: 4px;
    }

    .status-dot span.dot {
      width: 9px;
      height: 9px;
      border-radius: 50%;
      background: radial-gradient(circle, #4ade80, #16a34a);
      box-shadow: 0 0 10px rgba(34, 197, 94, 0.9);
    }

    .rap-block {
      margin-top: 10px;
      padding: 10px 12px;
      border-radius: 14px;
      border: 1px solid rgba(148, 163, 184, 0.4);
      background: radial-gradient(circle at top, rgba(148, 163, 184, 0.12), rgba(3, 6, 20, 0.95));
      font-size: 12px;
      font-style: italic;
      white-space: pre-line;
    }

    footer {
      margin-top: 28px;
      padding-top: 18px;
      border-top: 1px solid rgba(31, 41, 55, 0.9);
      font-size: 11px;
      color: var(--text-muted);
    }

    .footer-top {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 8px;
    }

    .footer-links {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      align-items: center;
    }

    .footer-links a {
      font-size: 11px;
    }

    .dates-row {
      margin-bottom: 4px;
    }

    .pasuk {
      margin-top: 6px;
      font-size: 11px;
      color: #e5e7eb;
    }

    .midot {
      margin-top: 4px;
      font-size: 11px;
      color: var(--text-muted);
    }
  </style>
</head>
<body>
  <div class="page-wrapper">
    <header>
      <div class="logo-row">
        <div class="brand-mark">
          <div class="brand-icon">SB</div>
          <div>
            <div class="brand-text-title">SparkBoost – SB</div>
            <div class="brand-sub">שיווק שמדליק תנועה, לידים ותוצאות 🚀</div>
          </div>
        </div>
        <div class="tag-pill">
          <span>⚡</span>
          <span>Marketing Engine • Landing Page</span>
        </div>
      </div>
    </header>

    <section class="hero">
      <div class="hero-inner">
        <div class="hero-kicker">
          <span class="hero-kicker-dot"></span>
          <span>שיווק ממוקד תוצאה • מיתוג • משפכים • קמפיינים</span>
        </div>
        <h1 class="hero-title">
          שיווק שמדליק <span>לבבות ותוצאות</span> – בלי רעש מיותר.
        </h1>
        <p class="hero-sub">
          SparkBoost – מערכת שיווק חכמה שמחברת בין מסר מדויק, עיצוב חד וזרימת לקוחות קבועה.
          זה לא עוד "פוסט בפייסבוק" – זו אסטרטגיה שלמה שמלווה את הלקוח מהפגישה הראשונה ועד לסגירה.
        </p>

        <div class="hero-bullets">
          <div class="hero-badge">🎯 <strong>אסטרטגיה</strong> – מי הקהל, מה המסר, איפה מופיעים</div>
          <div class="hero-badge">📲 <strong>דפי נחיתה</strong> – עמודים שמייצרים פניות אמיתיות</div>
          <div class="hero-badge">💸 <strong>קמפיינים ממומנים</strong> – תכנון, בקרה, אופטימיזציה</div>
          <div class="hero-badge">🧲 <strong>תוכן שיווקי</strong> – פוסטים, מיילים, סרטונים, רילסים</div>
        </div>

        <div class="hero-cta-row">
          <a href="mailto:anlominus+sparkboost@gmail.com?subject=SparkBoost%20–%20שיווק" class="btn-primary">
            <span class="icon">🚀</span>
            <span>בוא נדליק את השיווק שלך</span>
          </a>

          <a href="https://github.com/AnLoMinus/SparkBoost" class="btn-ghost" target="_blank" rel="noopener">
            <span>📂</span>
            <span>מאגר SparkBoost ב-GitHub</span>
          </a>
        </div>

        <div class="hero-note">
          ⚡ אפשר להתאים את העמוד לכל עסק: מצית קליפר, קלפים, קורסים, מרכז גמילה, מותג אישי ועוד.
        </div>
      </div>
    </section>

    <main>
      <!-- צד שמאל – מה מקבלים -->
      <section class="card">
        <div class="eyebrow">מה מקבלים • VALUE</div>
        <h2>💼 חבילת שיווק חכמה לעסקים</h2>
        <p>
          מטרת SparkBoost היא ליצור לך שיווק שמרגיש <strong>מסודר, מדויק ועקבי</strong> –
          במקום לנסות "עוד פוסט" בלי כיוון. כל החבילה בנויה סביב שלושה צירים:
          <strong>ברנד • מסר • מערכת.</strong>
        </p>

        <h3>🔹 1. מיתוג והצבת זהות</h3>
        <ul class="clean-list">
          <li><span class="bullet">✨</span><span>אפיון מותג – מה הסיפור, למה אתה קיים, מה הייחוד שלך.</span></li>
          <li><span class="bullet">🎨</span><span>שפה גרפית – צבעים, טיפוגרפיה, לוגו, אווירה ויזואלית.</span></li>
          <li><span class="bullet">🧭</span><span>מסר על – משפט אחד ברור שהעסק שלך עומד עליו.</span></li>
        </ul>

        <h3>🔹 2. מערכת תוכן ופרסום</h3>
        <ul class="clean-list">
          <li><span class="bullet">📅</span><span>לו"ז תוכן חודשי – פוסטים, רילסים, סטוריז, מיילים.</span></li>
          <li><span class="bullet">📢</span><span>קמפיינים ממומנים (פייסבוק, אינסטגרם, טיקטוק, גוגל, טלגרם).</span></li>
          <li><span class="bullet">🧲</span><span>דפי נחיתה המותאמים למודעות – לכל קמפיין שער משלו.</span></li>
        </ul>

        <h3>🔹 3. שיפור מתמיד (Optimization)</h3>
        <ul class="clean-list">
          <li><span class="bullet">📊</span><span>בדיקות A/B לכותרות, תמונות וקריאות לפעולה.</span></li>
          <li><span class="bullet">📈</span><span>מעקב המרות – כמה נכנסו, כמה פנו, כמה סגרו.</span></li>
          <li><span class="bullet">♻</span><span>שיפור שבועי – לא מנחשים, עובדים לפי נתונים.</span></li>
        </ul>

        <div class="pill-row">
          <div class="pill highlight">🔥 ממוקד תוצאה</div>
          <div class="pill">💬 שפה אנושית, בלי בולשיט</div>
          <div class="pill">⚡ אפשר לחבר לשאר המאגרים שלך ב-GitHub</div>
        </div>

        <div class="rap-block">
          🎤 פזמון ראפ – SparkBoost Flow:

          אני מדליק את העסק, מעלה אותו גבוה,  
          לקוח נכנס לפאנל – מרגיש שהוא בבית פה,  
          שיווק עם נשמה, לא עוד מודעה ריקה,  
          SparkBoost על ההגה – הטיסה כבר מתחילה. ⚡
        </div>
      </section>

      <!-- צד ימין – תהליך, תמחור, לינקים -->
      <aside class="card">
        <div class="eyebrow">תהליך • FLOW</div>
        <h2>🧬 איך זה עובד בפועל?</h2>
        <p>
          לא סתם "שיווק". זה מסע בנוי היטב, שלב אחרי שלב –
          כדי שתדע תמיד מה קורה, מה נבדק ומה מתעדכן.
        </p>

        <h3>1️⃣ שיחת מיקוד</h3>
        <p>היכרות, הבנת העסק, הקהל, היעדים והחזון. מגדירים מטרות חדות.</p>

        <h3>2️⃣ בניית מעטפת</h3>
        <p>מיתוג, מסר, עיצוב ראשוני, דף נחיתה ליבה + בסיס לקמפיין.</p>

        <h3>3️⃣ יציאה לאוויר</h3>
        <p>חיבור לפלטפורמות, הקמת מודעות, קביעת תקציב ומדדי הצלחה.</p>

        <h3>4️⃣ מדידה ושיפור</h3>
        <p>מעקב שבועי, שיפורים קטנים שעושים שינוי גדול לאורך זמן.</p>

        <div class="pricing-row">
          <div class="pricing-box">
            <strong>💡 סטארטר – עסקים בתחילת הדרך</strong>
            כולל: דף נחיתה, תבנית פוסטים, קמפיין אחד ממומן בסיסי.  
            <em>מתאים למי שרוצה להתחיל לזוז בלי להישרף בתקציבים.</em>
          </div>
          <div class="pricing-box">
            <strong>🚀 Pro – מערכת שיווק רצה</strong>
            כולל: מיתוג, כמה דפי נחיתה, מספר קמפיינים, ליווי חודשי.  
            <em>למי שרוצה להפוך שיווק ממקרי למערכת.</em>
          </div>
        </div>

        <div class="status-dot">
          <span class="dot"></span>
          <span>קבלת לקוחות לשיתופי פעולה – בעדיפות לעסקים עם לב ושליחות.</span>
        </div>

        <h3>🔗 קישורים רשמיים</h3>
        <ul class="clean-list">
          <li>
            <span class="bullet">📂</span>
            <span>
              מאגר GitHub:
              <a href="https://github.com/AnLoMinus/SparkBoost" target="_blank" rel="noopener">
                github.com/AnLoMinus/SparkBoost
              </a>
            </span>
          </li>
          <li>
            <span class="bullet">🌐</span>
            <span>
              אתר GitHub Pages:
              <a href="https://anlominus.github.io/SparkBoost/" target="_blank" rel="noopener">
                anlominus.github.io/SparkBoost/
              </a>
            </span>
          </li>
          <li>
            <span class="bullet">📧</span>
            <span>
              יצירת קשר:
              <a href="mailto:anlominus+sparkboost@gmail.com">anlominus+sparkboost@gmail.com</a>
            </span>
          </li>
        </ul>
      </aside>
    </main>

    <footer>
      <div class="footer-top">
        <div>
          © 2025 AnLoMinus × SparkBoost Studio · All Rights Reserved
        </div>
        <div class="footer-links">
          <span>⚡ Built for: Creative Marketing • GitHub Pages</span>
        </div>
      </div>

      <div class="dates-row">
        <div>📅 תאריך לועזי: 26/11/2025</div>
        <div>📅 תאריך עברי (נא לאמת בלוח): סביב כ"ו בחשוון תשפ"ו</div>
        <div>⏰ שעה מקומית (Asia/Jerusalem): 14:52</div>
      </div>

      <div class="pasuk">
        פסוק השראה: <strong>"וְהוּא יַצְלִיחַ דַּרְכֶּךָ" (תהילים ל"ז)</strong> – כשאתה עושה, הוא פותח לך שערים.
      </div>

      <div class="midot">
        מידות מלוות: חסד • גבורה • תפארת • נצח • הוד • יסוד • מלכות
      </div>
    </footer>
  </div>
</body>
</html>
```

---

## 🛠️ איך להשתמש בעמוד

1. צור מאגר חדש ב-GitHub בשם למשל: `SparkBoost`
    
2. צור קובץ בשם `index.html` והדבק בו את כל הקוד שלמעלה.
    
3. ב־GitHub, היכנס ל־**Settings → Pages**
    
    - Source: בחר `Deploy from a branch`
        
    - Branch: `main` / `master` + `/root`
        
4. הכתובת תהיה:  
    `https://anlominus.github.io/SparkBoost/` (או לפי שם המאגר שתבחר).
    

---

## 🎤 פזמון ראפ לנושא (מחוץ לקוד, לפוסטים / רילס)

אני מדליק את המותג, שם אותו על המפה,  
כל פוסט הוא ניצוץ, כל ליד עוד קפיצה,  
שיווק עם לב, לא עוד הצגה ריקה,  
SparkBoost בתמונה – והאש כבר נדלקה. ⚡

---

## 🔖 האשטאגים מוצעים

`#SparkBoost #SB #Marketing #DigitalMarketing #GitHubPages #Branding #LandingPage #AnLoMinus #CreativeEngine #PaidAds #ContentMarketing #BusinessGrowth`

אם תרצה עכשיו גרסת **מחירון שיווק** (לפי חבילות, כולל טלגרם, פייסבוק, אינסטה וכו’) – אבנה לך דף נפרד/סקשן נוסף בתוך אותו עמוד.
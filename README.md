<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Apple — Personal Page</title>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600&family=DM+Serif+Display:ital@0;1&display=swap" rel="stylesheet"/>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --green-50: #EAF3DE;
      --green-200: #97C459;
      --green-600: #3B6D11;
      --green-800: #27500A;
      --red-50: #FCEBEB;
      --red-400: #E24B4A;
      --amber-50: #FAEEDA;
      --amber-400: #BA7517;
      --text-primary: #1a1a18;
      --text-secondary: #5F5E5A;
      --text-muted: #888780;
      --bg: #FAFAF7;
      --bg-card: #ffffff;
      --border: rgba(0,0,0,0.1);
    }

    body {
      font-family: 'DM Sans', sans-serif;
      background: var(--bg);
      color: var(--text-primary);
      min-height: 100vh;
    }

    /* Hero */
    .hero {
      max-width: 680px;
      margin: 0 auto;
      padding: 5rem 2rem 3rem;
      text-align: center;
    }

    .apple-emoji {
      font-size: 80px;
      display: block;
      margin-bottom: 1.5rem;
      animation: bob 3s ease-in-out infinite;
    }

    @keyframes bob {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-8px); }
    }

    .hero h1 {
      font-family: 'DM Serif Display', serif;
      font-size: 48px;
      font-weight: 400;
      color: var(--text-primary);
      margin-bottom: 1rem;
      line-height: 1.15;
    }

    .hero h1 em {
      font-style: italic;
      color: var(--green-600);
    }

    .hero .bio {
      font-size: 17px;
      color: var(--text-secondary);
      line-height: 1.75;
      max-width: 420px;
      margin: 0 auto 2rem;
    }

    .tags {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      justify-content: center;
    }

    .tag {
      background: var(--green-50);
      color: var(--green-600);
      font-size: 13px;
      font-weight: 500;
      padding: 5px 14px;
      border-radius: 99px;
    }

    /* Divider */
    .divider {
      border: none;
      border-top: 1px solid var(--border);
      max-width: 640px;
      margin: 2.5rem auto;
    }

    /* Sections */
    .section {
      max-width: 680px;
      margin: 0 auto;
      padding: 0 2rem 2.5rem;
    }

    .section-label {
      font-size: 11px;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--text-muted);
      margin-bottom: 1.25rem;
    }

    /* Quote */
    .quote {
      border-left: 3px solid var(--green-200);
      padding: 1rem 1.5rem;
      background: var(--green-50);
      border-radius: 0 10px 10px 0;
    }

    .quote p {
      font-family: 'DM Serif Display', serif;
      font-style: italic;
      font-size: 18px;
      line-height: 1.65;
      color: var(--green-800);
    }

    /* Cards */
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
      gap: 12px;
    }

    .card {
      background: var(--bg-card);
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 1.1rem;
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }

    .card:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 24px rgba(0,0,0,0.07);
    }

    .card-icon { font-size: 26px; margin-bottom: 10px; display: block; }
    .card h3 { font-size: 14px; font-weight: 600; margin-bottom: 4px; }
    .card p { font-size: 13px; color: var(--text-secondary); line-height: 1.5; }

    /* Links */
    .links {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
      padding: 0 2rem 4rem;
      max-width: 680px;
      margin: 0 auto;
    }

    .link-btn {
      display: inline-flex;
      align-items: center;
      gap: 7px;
      font-size: 14px;
      font-weight: 500;
      color: var(--text-secondary);
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 9px 18px;
      text-decoration: none;
      background: var(--bg-card);
      transition: background 0.15s, color 0.15s;
    }

    .link-btn:hover {
      background: var(--green-50);
      color: var(--green-600);
      border-color: var(--green-200);
    }

    /* Footer */
    footer {
      text-align: center;
      font-size: 12px;
      color: var(--text-muted);
      padding-bottom: 2rem;
    }

    @media (max-width: 480px) {
      .hero h1 { font-size: 36px; }
      .hero { padding-top: 3rem; }
    }
  </style>
</head>
<body>

  <div class="hero">
    <span class="apple-emoji">🍎</span>
    <h1>Hey, I'm <em>Apple</em> 👋</h1>
    <p class="bio">Welcome to my little corner of the internet. I love good vibes, simple things, and fresh starts.</p>
    <div class="tags">
      <span class="tag">🎵 Music lover</span>
      <span class="tag">🌿 Nature fan</span>
      <span class="tag">📸 Photographer</span>
      <span class="tag">☕ Coffee addict</span>
    </div>
  </div>

  <hr class="divider"/>

  <div class="section">
    <div class="section-label">About me</div>
    <div class="quote">
      <p>"Just a person trying to enjoy life one day at a time — like a fresh apple, crisp and full of good things."</p>
    </div>
  </div>

  <div class="section">
    <div class="section-label">Things I enjoy</div>
    <div class="cards">
      <div class="card">
        <span class="card-icon">🎶</span>
        <h3>Music</h3>
        <p>Always have something playing in the background.</p>
      </div>
      <div class="card">
        <span class="card-icon">🌄</span>
        <h3>Exploring</h3>
        <p>Love discovering new places, big or small.</p>
      </div>
      <div class="card">
        <span class="card-icon">📖</span>
        <h3>Reading</h3>
        <p>Books, blogs, anything with good words.</p>
      </div>
      <div class="card">
        <span class="card-icon">🍕</span>
        <h3>Food</h3>
        <p>Trying new foods is basically a hobby.</p>
      </div>
    </div>
  </div>

  <hr class="divider"/>

  <div class="links">
    <a href="#" class="link-btn">📸 Instagram</a>
    <a href="#" class="link-btn">✉️ Email me</a>
    <a href="#" class="link-btn">🐦 Twitter</a>
  </div>

  <footer>made with 🍎 by Apple</footer>

</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Convrt — Roofing Landing Pages That Convert</title>
<meta name="description" content="High-converting landing pages for UK roofing companies. Turn website visitors into quote requests. Fixed price £349. Delivered in 3–5 days.">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;900&display=swap" rel="stylesheet">
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }
  :root {
    --gold: #F5C842;
    --gold-dim: #C49E1E;
    --dark: #0A0A0F;
    --dark2: #111118;
    --dark3: #1A1A24;
    --dark4: #22222E;
    --white: #F4F4F0;
    --muted: #888897;
    --border: rgba(255,255,255,0.08);
  }
  body {
    font-family: 'Inter', sans-serif;
    background: var(--dark);
    color: var(--white);
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
  }

  /* NAV */
  nav {
    display: flex; align-items: center; justify-content: space-between;
    padding: 1.25rem 2.5rem;
    border-bottom: 1px solid var(--border);
    position: sticky; top: 0; z-index: 100;
    background: rgba(10,10,15,0.92);
    backdrop-filter: blur(12px);
  }
  .nav-logo {
    display: flex; align-items: center; gap: 10px;
  }
  .nav-logo svg { width: 32px; height: 32px; }
  .nav-logo-text {
    font-size: 18px; font-weight: 900;
    letter-spacing: -0.03em; color: var(--white);
  }
  .nav-cta {
    background: var(--gold); color: #000;
    font-size: 13px; font-weight: 700;
    padding: 0.55rem 1.25rem; border-radius: 6px;
    text-decoration: none; letter-spacing: 0.01em;
    transition: opacity 0.2s;
  }
  .nav-cta:hover { opacity: 0.88; }

  /* HERO */
  .hero {
    padding: 7rem 2.5rem 5rem;
    text-align: center;
    max-width: 820px; margin: 0 auto;
  }
  .hero-badge {
    display: inline-flex; align-items: center; gap: 6px;
    background: rgba(245,200,66,0.1);
    border: 1px solid rgba(245,200,66,0.25);
    color: var(--gold);
    font-size: 12px; font-weight: 600;
    padding: 0.35rem 0.9rem; border-radius: 100px;
    margin-bottom: 2rem; letter-spacing: 0.06em; text-transform: uppercase;
  }
  .hero-badge::before {
    content: ''; width: 6px; height: 6px;
    background: var(--gold); border-radius: 50%;
    animation: pulse 2s infinite;
  }
  @keyframes pulse {
    0%, 100% { opacity: 1; } 50% { opacity: 0.3; }
  }
  h1 {
    font-size: clamp(2.4rem, 5vw, 3.8rem);
    font-weight: 900; line-height: 1.08;
    letter-spacing: -0.03em;
    margin-bottom: 1.5rem;
  }
  h1 em { font-style: normal; color: var(--gold); }
  .hero-sub {
    font-size: 1.1rem; color: var(--muted);
    max-width: 520px; margin: 0 auto 2.5rem;
    line-height: 1.7;
  }
  .hero-cta-row {
    display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap;
  }
  .btn-primary {
    background: var(--gold); color: #000;
    font-size: 15px; font-weight: 700;
    padding: 0.85rem 2rem; border-radius: 8px;
    text-decoration: none; transition: opacity 0.2s;
  }
  .btn-primary:hover { opacity: 0.88; }
  .btn-ghost {
    background: transparent; color: var(--white);
    font-size: 15px; font-weight: 500;
    padding: 0.85rem 1.75rem; border-radius: 8px;
    text-decoration: none; border: 1px solid var(--border);
    transition: border-color 0.2s;
  }
  .btn-ghost:hover { border-color: rgba(255,255,255,0.2); }

  /* ROI STRIP */
  .roi-strip {
    border-top: 1px solid var(--border);
    border-bottom: 1px solid var(--border);
    padding: 2.5rem;
    display: flex; justify-content: center;
    flex-wrap: wrap;
  }
  .roi-item {
    flex: 1; min-width: 160px; max-width: 220px;
    text-align: center; padding: 0.5rem 1rem;
    border-right: 1px solid var(--border);
  }
  .roi-item:last-child { border-right: none; }
  .roi-num {
    font-size: 2rem; font-weight: 900;
    letter-spacing: -0.04em; color: var(--gold); line-height: 1;
  }
  .roi-label {
    font-size: 12px; color: var(--muted);
    margin-top: 4px; text-transform: uppercase; letter-spacing: 0.07em;
  }

  /* SECTIONS */
  section {
    max-width: 860px; margin: 0 auto;
    padding: 5rem 2.5rem;
  }
  .section-label {
    font-size: 11px; font-weight: 700;
    color: var(--gold); letter-spacing: 0.12em;
    text-transform: uppercase; margin-bottom: 1rem;
  }
  h2 {
    font-size: clamp(1.6rem, 3.5vw, 2.4rem);
    font-weight: 900; letter-spacing: -0.02em;
    line-height: 1.15; margin-bottom: 1rem;
  }
  .section-sub {
    font-size: 1rem; color: var(--muted);
    max-width: 500px; line-height: 1.7; margin-bottom: 3rem;
  }

  /* PROBLEM CARDS */
  .problem-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 1px;
    background: var(--border);
    border: 1px solid var(--border);
    border-radius: 12px; overflow: hidden;
  }
  .prob-card { background: var(--dark2); padding: 1.5rem; }
  .prob-icon {
    width: 36px; height: 36px;
    background: rgba(255,255,255,0.05);
    border-radius: 8px; margin-bottom: 1rem;
    display: flex; align-items: center; justify-content: center;
  }
  .prob-icon svg { width: 18px; height: 18px; stroke: var(--muted); fill: none; stroke-width: 1.5; stroke-linecap: round; stroke-linejoin: round; }
  .prob-title { font-size: 14px; font-weight: 600; margin-bottom: 0.4rem; }
  .prob-desc { font-size: 13px; color: var(--muted); line-height: 1.6; }

  /* OFFER */
  .offer-box {
    background: var(--dark2);
    border: 1px solid var(--border);
    border-radius: 16px; overflow: hidden;
  }
  .offer-header {
    padding: 2rem 2rem 1.5rem;
    border-bottom: 1px solid var(--border);
    display: flex; align-items: flex-start; justify-content: space-between; gap: 1rem; flex-wrap: wrap;
  }
  .offer-title { font-size: 1.2rem; font-weight: 800; }
  .offer-price {
    font-size: 2.5rem; font-weight: 900;
    color: var(--gold); letter-spacing: -0.04em; line-height: 1;
  }
  .offer-price span { font-size: 1rem; color: var(--muted); font-weight: 400; }
  .offer-items {
    padding: 1.5rem 2rem;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 0.75rem;
  }
  .offer-item { display: flex; align-items: flex-start; gap: 10px; font-size: 14px; }
  .offer-item svg { width: 18px; height: 18px; flex-shrink: 0; margin-top: 2px; stroke: var(--gold); fill: none; stroke-width: 2; stroke-linecap: round; stroke-linejoin: round; }
  .offer-item strong { display: block; font-weight: 600; }
  .offer-item span { color: var(--muted); font-size: 12px; }
  .offer-footer {
    padding: 1.5rem 2rem;
    border-top: 1px solid var(--border);
    display: flex; align-items: center; justify-content: space-between; flex-wrap: wrap; gap: 1rem;
  }
  .offer-note { font-size: 13px; color: var(--muted); }
  .offer-note strong { color: var(--white); }

  /* PROCESS */
  .steps {
    display: flex; flex-direction: column;
    border: 1px solid var(--border); border-radius: 12px; overflow: hidden;
  }
  .step {
    display: flex; gap: 1.5rem;
    padding: 1.5rem 1.75rem;
    border-bottom: 1px solid var(--border);
    background: var(--dark2);
    align-items: flex-start;
  }
  .step:last-child { border-bottom: none; }
  .step-num { font-size: 11px; font-weight: 800; color: var(--gold); letter-spacing: 0.05em; width: 28px; flex-shrink: 0; padding-top: 2px; }
  .step-content h4 { font-size: 14px; font-weight: 700; margin-bottom: 3px; }
  .step-content p { font-size: 13px; color: var(--muted); line-height: 1.6; }

  /* PROOF */
  .proof-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 12px;
  }
  .proof-card {
    background: var(--dark2);
    border: 1px solid var(--border);
    border-radius: 12px; padding: 1.5rem;
  }
  .stars { color: var(--gold); font-size: 13px; margin-bottom: 0.75rem; letter-spacing: 2px; }
  .proof-text { font-size: 14px; line-height: 1.65; margin-bottom: 1rem; }
  .proof-author { font-size: 12px; color: var(--muted); }
  .proof-author strong { color: var(--white); display: block; }

  /* FINAL CTA */
  .final-cta {
    text-align: center;
    padding: 5rem 2.5rem;
    border-top: 1px solid var(--border);
  }
  .final-cta h2 { font-size: clamp(1.8rem, 4vw, 3rem); margin-bottom: 1rem; }
  .final-cta p { color: var(--muted); margin-bottom: 2.5rem; font-size: 1rem; }
  .final-cta .btn-primary { font-size: 17px; padding: 1rem 2.5rem; }

  footer {
    padding: 1.5rem 2.5rem;
    border-top: 1px solid var(--border);
    text-align: center;
    font-size: 12px; color: var(--muted);
  }

  @media (max-width: 600px) {
    nav { padding: 1rem 1.25rem; }
    .hero { padding: 4rem 1.25rem 3rem; }
    section { padding: 3rem 1.25rem; }
    .roi-strip { padding: 1.5rem 1.25rem; }
    .roi-item { border-right: none; border-bottom: 1px solid var(--border); }
    .roi-item:last-child { border-bottom: none; }
    .offer-header, .offer-footer { flex-direction: column; }
    .final-cta { padding: 3rem 1.25rem; }
  }
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="nav-logo">
    <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
      <rect width="40" height="40" rx="9" fill="#F5C842"/>
      <polyline points="11,29 11,13 29,13" stroke="#0A0A0F" stroke-width="4.5" stroke-linecap="round" stroke-linejoin="round"/>
      <line x1="11" y1="13" x2="29" y2="29" stroke="#0A0A0F" stroke-width="4.5" stroke-linecap="round"/>
    </svg>
    <span class="nav-logo-text">convrt</span>
  </div>
  <a href="#contact" class="nav-cta">Get your page →</a>
</nav>

<!-- HERO -->
<div class="hero">
  <div class="hero-badge">Built for UK roofers</div>
  <h1>Turn website visitors into <em>quote requests</em></h1>
  <p class="hero-sub">One sharp, fast-loading page built to convert — so every visitor becomes a lead, not a missed job worth £10k.</p>
  <div class="hero-cta-row">
    <a href="#offer" class="btn-primary">See what's included</a>
    <a href="#how" class="btn-ghost">How it works</a>
  </div>
</div>

<!-- ROI STRIP -->
<div class="roi-strip">
  <div class="roi-item">
    <div class="roi-num">£349</div>
    <div class="roi-label">One-off, fixed price</div>
  </div>
  <div class="roi-item">
    <div class="roi-num">3–5</div>
    <div class="roi-label">Days to delivery</div>
  </div>
  <div class="roi-item">
    <div class="roi-num">£15k</div>
    <div class="roi-label">Avg roofing job value</div>
  </div>
  <div class="roi-item">
    <div class="roi-num">1 job</div>
    <div class="roi-label">Pays for this 40× over</div>
  </div>
</div>

<!-- PROBLEM -->
<section>
  <div class="section-label">The problem</div>
  <h2>Most roofers lose leads before the first call</h2>
  <p class="section-sub">You've got traffic — from Google Ads, referrals, local searches. But your site isn't built to convert it.</p>
  <div class="problem-grid">
    <div class="prob-card">
      <div class="prob-icon">
        <svg viewBox="0 0 24 24"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
      </div>
      <div class="prob-title">Referrals dry up</div>
      <div class="prob-desc">Word-of-mouth is unpredictable. When referrals slow, jobs slow. You need a second channel that runs 24/7.</div>
    </div>
    <div class="prob-card">
      <div class="prob-icon">
        <svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/></svg>
      </div>
      <div class="prob-title">No clear CTA</div>
      <div class="prob-desc">Visitors land and don't know what to do next. No phone, no form, no WhatsApp. They bounce to a competitor.</div>
    </div>
    <div class="prob-card">
      <div class="prob-icon">
        <svg viewBox="0 0 24 24"><rect x="5" y="2" width="14" height="20" rx="2"/><line x1="12" y1="18" x2="12.01" y2="18"/></svg>
      </div>
      <div class="prob-title">Not mobile-optimised</div>
      <div class="prob-desc">70%+ of UK local searches happen on mobile. A slow or broken mobile site kills the lead before you even know it existed.</div>
    </div>
    <div class="prob-card">
      <div class="prob-icon">
        <svg viewBox="0 0 24 24"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
      </div>
      <div class="prob-title">No trust signals</div>
      <div class="prob-desc">No reviews, no photos, no guarantee. Homeowners won't request a quote from someone they can't verify.</div>
    </div>
  </div>
</section>

<!-- OFFER -->
<section id="offer" style="padding-top:0;">
  <div class="section-label">The offer</div>
  <h2>Everything you need. Nothing you don't.</h2>
  <p class="section-sub">A single, focused landing page built to get quote requests — fully done for you.</p>
  <div class="offer-box">
    <div class="offer-header">
      <div>
        <div class="offer-title">Roofing Lead Page</div>
        <p style="font-size:13px;color:var(--muted);margin-top:4px;">One-shot. Fixed price. Ready in days.</p>
      </div>
      <div style="text-align:right;">
        <div class="offer-price">£349 <span>one-off</span></div>
      </div>
    </div>
    <div class="offer-items">
      <div class="offer-item">
        <svg viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>
        <div><strong>Conversion-focused layout</strong><span>Designed to move visitors to action</span></div>
      </div>
      <div class="offer-item">
        <svg viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>
        <div><strong>Copywriting included</strong><span>You don't write a word</span></div>
      </div>
      <div class="offer-item">
        <svg viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>
        <div><strong>Mobile-first build</strong><span>Perfect on any phone</span></div>
      </div>
      <div class="offer-item">
        <svg viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>
        <div><strong>CTA: call / form / WhatsApp</strong><span>You pick what fits your workflow</span></div>
      </div>
      <div class="offer-item">
        <svg viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>
        <div><strong>Trust section</strong><span>Reviews, accreditations, photos</span></div>
      </div>
      <div class="offer-item">
        <svg viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>
        <div><strong>Delivered in 3–5 days</strong><span>Via file or hosted live URL</span></div>
      </div>
    </div>
    <div class="offer-footer">
      <div class="offer-note"><strong>1 roofing job won</strong> pays for this page 40× over.</div>
      <a href="#contact" class="btn-primary">Claim your page →</a>
    </div>
  </div>
</section>

<!-- HOW IT WORKS -->
<section id="how" style="padding-top:0;">
  <div class="section-label">The process</div>
  <h2>Up and running in under a week</h2>
  <p class="section-sub">No lengthy onboarding. No back-and-forth for months. Just a clear, fast process.</p>
  <div class="steps">
    <div class="step">
      <div class="step-num">01</div>
      <div class="step-content">
        <h4>You send me your basics</h4>
        <p>Company name, service area, contact details, any photos or reviews. A 10-minute job on your end.</p>
      </div>
    </div>
    <div class="step">
      <div class="step-num">02</div>
      <div class="step-content">
        <h4>I build your page</h4>
        <p>Copy, design, structure — all done. Optimised to convert local homeowners into quote requests.</p>
      </div>
    </div>
    <div class="step">
      <div class="step-num">03</div>
      <div class="step-content">
        <h4>Review & approve</h4>
        <p>You see the draft. One round of changes included. Most clients approve same day.</p>
      </div>
    </div>
    <div class="step">
      <div class="step-num">04</div>
      <div class="step-content">
        <h4>Go live — start getting leads</h4>
        <p>I deliver the page as a file or set it live on a URL you can point your domain or ads to.</p>
      </div>
    </div>
  </div>
</section>

<!-- SOCIAL PROOF -->
<section style="padding-top:0;">
  <div class="section-label">What they say</div>
  <h2>Roofers already winning more quotes</h2>
  <p class="section-sub" style="margin-bottom:2rem;">Real results from local roofing companies across the UK.</p>
  <div class="proof-grid">
    <div class="proof-card">
      <div class="stars">★★★★★</div>
      <p class="proof-text">"Had a basic website for years. Within two weeks of the new page going live, we had three quote requests in one weekend."</p>
      <div class="proof-author"><strong>Mike T.</strong>Flat Roofing Specialist — Manchester</div>
    </div>
    <div class="proof-card">
      <div class="stars">★★★★★</div>
      <p class="proof-text">"I was sceptical about spending money on a website but the maths is simple — one job more than covered it. Should've done this years ago."</p>
      <div class="proof-author"><strong>Steve R.</strong>Roofing & Guttering — Leeds</div>
    </div>
    <div class="proof-card">
      <div class="stars">★★★★★</div>
      <p class="proof-text">"The WhatsApp button alone changed things. People message straight away instead of disappearing. Great service, fast turnaround."</p>
      <div class="proof-author"><strong>D. Okafor</strong>Re-roofing & Repairs — Birmingham</div>
    </div>
  </div>
</section>

<!-- FINAL CTA -->
<div class="final-cta" id="contact">
  <div class="section-label" style="margin-bottom:1rem;">Ready to start?</div>
  <h2>Get more quote requests.<br>Starting this week.</h2>
  <p>Fixed price. Fast delivery. Built for roofers.</p>
  <a href="mailto:adam@markyz.fr" class="btn-primary">Get your page for £349 →</a>
  <p style="margin-top:1.5rem;font-size:13px;color:var(--muted);">Questions first? Email adam@markyz.fr — usually back within a few hours.</p>
</div>

<footer>
  © 2025 Convrt — High-converting landing pages for roofing companies in the UK
</footer>

</body>
</html>

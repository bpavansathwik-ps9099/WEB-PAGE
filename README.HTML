<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Build Your Quote — The Leaf Studio</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,500;1,400;1,500&family=Raleway:wght@200;300;400;500&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

:root {
  --black: #0a0a08;
  --dark: #111209;
  --dark2: #1a1a14;
  --gold: #c8a97e;
  --gold2: #e2c99a;
  --gold-dim: rgba(200,169,126,0.15);
  --gold-border: rgba(200,169,126,0.25);
  --cream: #f5f0e8;
  --text: #d4c9b5;
  --muted: #7a7265;
  --white: #faf8f4;
}

html { scroll-behavior: smooth; }

body {
  font-family: 'Raleway', sans-serif;
  background: var(--black);
  color: var(--text);
  min-height: 100vh;
  overflow-x: hidden;
  cursor: default;
}

/* ─── Noise texture overlay ─── */
body::before {
  content: '';
  position: fixed; inset: 0; z-index: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.04'/%3E%3C/svg%3E");
  pointer-events: none;
  opacity: 0.5;
}

/* ─── Ambient glow ─── */
.glow-top {
  position: fixed;
  top: -200px; left: 50%;
  transform: translateX(-50%);
  width: 700px; height: 400px;
  background: radial-gradient(ellipse, rgba(200,169,126,0.07) 0%, transparent 70%);
  pointer-events: none; z-index: 0;
}

/* ══════════════════════════════
   NAVIGATION
══════════════════════════════ */
nav {
  position: fixed; top: 0; left: 0; right: 0; z-index: 100;
  padding: 0 48px;
  height: 72px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: rgba(10,10,8,0.85);
  backdrop-filter: blur(16px);
  -webkit-backdrop-filter: blur(16px);
  border-bottom: 1px solid var(--gold-border);
}

.nav-logo {
  font-family: 'Playfair Display', serif;
  font-size: 18px;
  font-weight: 400;
  color: var(--gold2);
  letter-spacing: 2px;
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 10px;
}

.nav-logo-leaf {
  font-size: 22px;
  display: inline-block;
  animation: sway 4s ease-in-out infinite;
}

@keyframes sway {
  0%, 100% { transform: rotate(-5deg); }
  50% { transform: rotate(5deg); }
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 36px;
  list-style: none;
}

.nav-links a {
  font-size: 10px;
  font-weight: 400;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--muted);
  text-decoration: none;
  transition: color 0.3s;
  position: relative;
}

.nav-links a::after {
  content: '';
  position: absolute;
  bottom: -4px; left: 0; right: 0;
  height: 1px;
  background: var(--gold);
  transform: scaleX(0);
  transition: transform 0.3s ease;
  transform-origin: left;
}

.nav-links a:hover { color: var(--gold2); }
.nav-links a:hover::after { transform: scaleX(1); }

.nav-links a.active {
  color: var(--gold);
}

.nav-enquire {
  font-size: 10px !important;
  font-weight: 500 !important;
  letter-spacing: 3px;
  color: var(--black) !important;
  background: var(--gold);
  padding: 9px 20px;
  border-radius: 1px;
  transition: background 0.3s, transform 0.2s !important;
}

.nav-enquire::after { display: none !important; }
.nav-enquire:hover {
  background: var(--gold2) !important;
  color: var(--black) !important;
  transform: translateY(-1px);
}

/* hamburger */
.hamburger {
  display: none;
  flex-direction: column;
  gap: 5px;
  cursor: pointer;
  padding: 4px;
}
.hamburger span {
  display: block;
  width: 24px; height: 1px;
  background: var(--gold);
  transition: all 0.3s;
}

/* ══════════════════════════════
   HERO HEADER
══════════════════════════════ */
.page-header {
  position: relative; z-index: 10;
  padding: 148px 24px 72px;
  text-align: center;
  overflow: hidden;
}

.page-header::before {
  content: '';
  position: absolute;
  bottom: 0; left: 50%; transform: translateX(-50%);
  width: 60%; height: 1px;
  background: linear-gradient(90deg, transparent, var(--gold-border), transparent);
}

.header-tag {
  display: inline-block;
  font-size: 9px;
  font-weight: 400;
  letter-spacing: 5px;
  text-transform: uppercase;
  color: var(--gold);
  border: 1px solid var(--gold-border);
  padding: 7px 18px;
  margin-bottom: 28px;
  animation: fadeDown 0.8s ease both;
}

.page-header h1 {
  font-family: 'Playfair Display', serif;
  font-weight: 400;
  font-size: clamp(44px, 7vw, 86px);
  line-height: 1;
  color: var(--white);
  margin-bottom: 10px;
  animation: fadeDown 0.8s 0.1s ease both;
}

.page-header h1 em {
  font-style: italic;
  color: var(--gold);
}

.page-header p {
  font-weight: 200;
  font-size: 14px;
  letter-spacing: 1px;
  color: var(--muted);
  max-width: 440px;
  margin: 20px auto 0;
  line-height: 1.8;
  animation: fadeDown 0.8s 0.2s ease both;
}

@keyframes fadeDown {
  from { opacity: 0; transform: translateY(-16px); }
  to   { opacity: 1; transform: translateY(0); }
}

/* ══════════════════════════════
   PROGRESS
══════════════════════════════ */
.container {
  position: relative; z-index: 10;
  max-width: 860px;
  margin: 0 auto;
  padding: 0 24px 120px;
}

.progress-wrap {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 52px;
  gap: 0;
}

.pdot {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
}

.pdot-circle {
  width: 38px; height: 38px;
  border-radius: 50%;
  border: 1px solid var(--gold-border);
  display: flex; align-items: center; justify-content: center;
  font-size: 11px;
  font-weight: 300;
  letter-spacing: 1px;
  color: var(--muted);
  background: var(--dark);
  transition: all 0.4s ease;
  position: relative;
}

.pdot.active .pdot-circle {
  border-color: var(--gold);
  color: var(--black);
  background: var(--gold);
  box-shadow: 0 0 24px rgba(200,169,126,0.3);
}

.pdot.done .pdot-circle {
  border-color: var(--gold);
  background: transparent;
  color: var(--gold);
}

.pdot.done .pdot-circle::after {
  content: '✓';
  font-size: 14px;
}

.pdot.done .pdot-circle span { display: none; }

.pdot-label {
  font-size: 9px;
  letter-spacing: 2.5px;
  text-transform: uppercase;
  color: var(--muted);
  white-space: nowrap;
}

.pdot.active .pdot-label { color: var(--gold); }
.pdot.done .pdot-label { color: var(--gold); opacity: 0.6; }

.pline {
  flex: 1;
  height: 1px;
  max-width: 100px;
  background: var(--gold-border);
  margin-bottom: 26px;
  transition: background 0.5s;
}

.pline.done { background: var(--gold); opacity: 0.4; }

/* ══════════════════════════════
   CARD
══════════════════════════════ */
.card {
  background: var(--dark2);
  border: 1px solid var(--gold-border);
  padding: 56px;
  position: relative;
  overflow: hidden;
  animation: fadeUp 0.5s ease both;
}

.card::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0; height: 1px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
}

.card::after {
  content: '';
  position: absolute;
  top: -100px; right: -100px;
  width: 300px; height: 300px;
  border-radius: 50%;
  border: 1px solid rgba(200,169,126,0.04);
  pointer-events: none;
}

@keyframes fadeUp {
  from { opacity: 0; transform: translateY(20px); }
  to   { opacity: 1; transform: translateY(0); }
}

/* ─── Panel ─── */
.panel { display: none; }
.panel.active { display: block; animation: fadeUp 0.45s ease both; }

.panel-eyebrow {
  font-size: 9px;
  letter-spacing: 4px;
  text-transform: uppercase;
  color: var(--gold);
  opacity: 0.7;
  margin-bottom: 10px;
}

.panel-title {
  font-family: 'Playfair Display', serif;
  font-weight: 400;
  font-size: 30px;
  color: var(--white);
  margin-bottom: 6px;
}

.panel-sub {
  font-size: 12px;
  font-weight: 200;
  color: var(--muted);
  letter-spacing: 0.5px;
  margin-bottom: 40px;
  line-height: 1.7;
}

/* ─── Fields ─── */
.grid2 { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; }
.full  { grid-column: 1 / -1; }

.field { display: flex; flex-direction: column; gap: 7px; }

label.flabel {
  font-size: 9px;
  font-weight: 400;
  letter-spacing: 2.5px;
  text-transform: uppercase;
  color: var(--muted);
}

input[type="text"],
input[type="email"],
input[type="tel"],
input[type="date"],
select,
textarea {
  font-family: 'Raleway', sans-serif;
  font-weight: 300;
  font-size: 13px;
  color: var(--white);
  background: rgba(255,255,255,0.03);
  border: 1px solid var(--gold-border);
  padding: 13px 16px;
  outline: none;
  border-radius: 0;
  transition: border-color 0.25s, background 0.25s, box-shadow 0.25s;
  appearance: none;
  -webkit-appearance: none;
  width: 100%;
}

input::placeholder, textarea::placeholder { color: rgba(122,114,101,0.6); }

input:focus, select:focus, textarea:focus {
  border-color: var(--gold);
  background: rgba(200,169,126,0.04);
  box-shadow: 0 0 0 3px rgba(200,169,126,0.08);
}

select {
  cursor: pointer;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='10' height='6' viewBox='0 0 10 6'%3E%3Cpath d='M1 1l4 4 4-4' stroke='%23c8a97e' stroke-width='1.2' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");
  background-repeat: no-repeat;
  background-position: right 14px center;
  padding-right: 38px;
  color: var(--white);
}

select option { background: var(--dark2); color: var(--white); }

textarea { resize: vertical; min-height: 90px; }

.err-msg {
  font-size: 10px;
  color: #c0392b;
  letter-spacing: 0.5px;
  display: none;
}

.field.has-err input,
.field.has-err select,
.field.has-err textarea { border-color: #c0392b; }
.field.has-err .err-msg { display: block; }

/* ─── Services ─── */
.services-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
  margin-bottom: 6px;
}

.svc-card {
  border: 1px solid var(--gold-border);
  padding: 22px 14px 18px;
  text-align: center;
  cursor: pointer;
  transition: all 0.3s;
  background: rgba(255,255,255,0.02);
  user-select: none;
  position: relative;
}

.svc-card:hover {
  border-color: var(--gold);
  background: var(--gold-dim);
}

.svc-card.sel {
  border-color: var(--gold);
  background: var(--gold-dim);
}

.svc-card.sel::after {
  content: '✦';
  position: absolute;
  top: 8px; right: 10px;
  font-size: 9px;
  color: var(--gold);
}

.svc-icon { font-size: 26px; margin-bottom: 9px; display: block; }
.svc-name {
  font-size: 10px;
  font-weight: 400;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--text);
}

.svc-card.sel .svc-name { color: var(--gold2); }

/* ─── Guest Counter ─── */
.guest-wrap {
  border: 1px solid var(--gold-border);
  background: rgba(255,255,255,0.02);
  padding: 28px;
  text-align: center;
}

.counter-row {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 28px;
}

.cbtn {
  width: 42px; height: 42px;
  border-radius: 50%;
  border: 1px solid var(--gold-border);
  background: transparent;
  color: var(--gold);
  font-size: 22px;
  line-height: 1;
  cursor: pointer;
  display: flex; align-items: center; justify-content: center;
  transition: all 0.25s;
  font-family: 'Raleway', sans-serif;
  font-weight: 200;
}

.cbtn:hover { background: var(--gold); color: var(--black); border-color: var(--gold); }

.gnum {
  font-family: 'Playfair Display', serif;
  font-size: 56px;
  font-weight: 400;
  color: var(--white);
  min-width: 90px;
  line-height: 1;
}

.glabel {
  font-size: 9px;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--muted);
  margin-top: 8px;
}

/* ─── Nav Buttons ─── */
.nav-btns {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 44px;
  padding-top: 32px;
  border-top: 1px solid var(--gold-border);
}

.btn {
  font-family: 'Raleway', sans-serif;
  font-weight: 400;
  font-size: 10px;
  letter-spacing: 3px;
  text-transform: uppercase;
  padding: 13px 30px;
  border: none;
  cursor: pointer;
  transition: all 0.3s;
  border-radius: 0;
}

.btn-back {
  background: transparent;
  color: var(--muted);
  border: 1px solid var(--gold-border);
}

.btn-back:hover { border-color: var(--gold); color: var(--gold); }

.btn-next {
  background: var(--gold);
  color: var(--black);
  font-weight: 500;
  box-shadow: 0 4px 20px rgba(200,169,126,0.2);
}

.btn-next:hover {
  background: var(--gold2);
  transform: translateY(-2px);
  box-shadow: 0 8px 32px rgba(200,169,126,0.3);
}

.btn-submit {
  background: transparent;
  color: var(--gold);
  border: 1px solid var(--gold);
  font-size: 11px;
  letter-spacing: 4px;
  padding: 15px 40px;
  position: relative;
  overflow: hidden;
}

.btn-submit::before {
  content: '';
  position: absolute;
  inset: 0;
  background: var(--gold);
  transform: translateX(-100%);
  transition: transform 0.4s ease;
  z-index: 0;
}

.btn-submit:hover::before { transform: translateX(0); }
.btn-submit:hover { color: var(--black); }
.btn-submit span { position: relative; z-index: 1; }

/* ─── Thank You Screen ─── */
#thankyou {
  display: none;
  text-align: center;
  padding: 80px 40px;
  animation: fadeUp 0.7s ease both;
}

.ty-icon {
  font-size: 52px;
  margin-bottom: 24px;
  display: block;
  animation: pulse 2s ease-in-out infinite;
}

@keyframes pulse {
  0%, 100% { transform: scale(1); opacity: 1; }
  50% { transform: scale(1.08); opacity: 0.85; }
}

.ty-title {
  font-family: 'Playfair Display', serif;
  font-size: 40px;
  font-weight: 400;
  color: var(--white);
  margin-bottom: 14px;
}

.ty-title em { font-style: italic; color: var(--gold); }

.ty-line {
  width: 80px; height: 1px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
  margin: 20px auto;
}

.ty-msg {
  font-size: 14px;
  font-weight: 200;
  color: var(--muted);
  max-width: 420px;
  margin: 0 auto 10px;
  line-height: 1.9;
  letter-spacing: 0.3px;
}

.ty-name {
  font-family: 'Playfair Display', serif;
  font-style: italic;
  font-size: 22px;
  color: var(--gold2);
  margin-top: 18px;
}

.ty-whatsapp {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  margin-top: 36px;
  padding: 14px 28px;
  border: 1px solid rgba(37,211,102,0.3);
  color: #25d366;
  font-size: 10px;
  letter-spacing: 3px;
  text-transform: uppercase;
  text-decoration: none;
  transition: all 0.3s;
  font-family: 'Raleway', sans-serif;
  font-weight: 400;
}

.ty-whatsapp:hover {
  background: rgba(37,211,102,0.08);
  border-color: #25d366;
}

/* ─── Loading spinner ─── */
.spinner {
  display: inline-block;
  width: 12px; height: 12px;
  border: 1.5px solid rgba(0,0,0,0.3);
  border-top-color: var(--black);
  border-radius: 50%;
  animation: spin 0.6s linear infinite;
  margin-right: 8px;
  vertical-align: middle;
}

@keyframes spin { to { transform: rotate(360deg); } }

/* ─── Footer ─── */
footer {
  position: relative; z-index: 10;
  text-align: center;
  padding: 28px;
  border-top: 1px solid var(--gold-border);
  font-size: 10px;
  letter-spacing: 2px;
  color: var(--muted);
  font-weight: 200;
}

footer span { color: var(--gold); }

/* ─── Responsive ─── */
@media (max-width: 768px) {
  nav { padding: 0 20px; }
  .nav-links { display: none; }
  .hamburger { display: flex; }
  .card { padding: 28px 20px; }
  .grid2 { grid-template-columns: 1fr; }
  .services-grid { grid-template-columns: repeat(2, 1fr); }
  .page-header { padding: 120px 20px 56px; }
}

/* Mobile menu */
.mobile-menu {
  display: none;
  position: fixed;
  top: 72px; left: 0; right: 0;
  background: rgba(10,10,8,0.97);
  border-bottom: 1px solid var(--gold-border);
  padding: 24px;
  z-index: 99;
  flex-direction: column;
  gap: 20px;
}

.mobile-menu.open { display: flex; }

.mobile-menu a {
  font-size: 11px;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--muted);
  text-decoration: none;
  padding: 8px 0;
  border-bottom: 1px solid var(--gold-border);
  transition: color 0.3s;
}

.mobile-menu a:hover { color: var(--gold); }
</style>
</head>
<body>

<div class="glow-top"></div>

<!-- ══ NAV ══ -->
<nav>
  <a href="#" class="nav-logo">
    <span class="nav-logo-leaf">🌿</span>
    The Leaf Studio
  </a>
  <ul class="nav-links">
    <li><a href="#">Home</a></li>
    <li><a href="#">Services</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Films</a></li>
    <li><a href="#" class="nav-enquire active">Enquire</a></li>
  </ul>
  <div class="hamburger" onclick="toggleMenu()">
    <span></span><span></span><span></span>
  </div>
</nav>

<div class="mobile-menu" id="mobileMenu">
  <a href="#">Home</a>
  <a href="#">Services</a>
  <a href="#">About</a>
  <a href="#">Films</a>
  <a href="#">Enquire</a>
</div>

<!-- ══ HEADER ══ -->
<div class="page-header">
  <span class="header-tag">✦ The Leaf Studio ✦</span>
  <h1>Build Your <em>Quote</em></h1>
  <p>Share a few details about your vision and we'll craft something truly beautiful for you.</p>
</div>

<!-- ══ MAIN ══ -->
<div class="container">

  <!-- Progress -->
  <div class="progress-wrap" id="progressBar">
    <div class="pdot active" data-s="1">
      <div class="pdot-circle"><span>01</span></div>
      <span class="pdot-label">You</span>
    </div>
    <div class="pline" id="pl1"></div>
    <div class="pdot" data-s="2">
      <div class="pdot-circle"><span>02</span></div>
      <span class="pdot-label">Event</span>
    </div>
    <div class="pline" id="pl2"></div>
    <div class="pdot" data-s="3">
      <div class="pdot-circle"><span>03</span></div>
      <span class="pdot-label">Services</span>
    </div>
    <div class="pline" id="pl3"></div>
    <div class="pdot" data-s="4">
      <div class="pdot-circle"><span>04</span></div>
      <span class="pdot-label">Finish</span>
    </div>
  </div>

  <!-- Card -->
  <div class="card" id="mainCard">

    <!-- STEP 1 -->
    <div class="panel active" id="step-1">
      <p class="panel-eyebrow">Step 01 of 04</p>
      <p class="panel-title">Tell Us About Yourself</p>
      <p class="panel-sub">We'd love to know who we're speaking with. This helps us personalise everything just for you.</p>

      <div class="grid2">
        <div class="field">
          <label class="flabel" for="fName">First Name</label>
          <input type="text" id="fName" placeholder="Your first name">
          <span class="err-msg">Please enter your first name</span>
        </div>
        <div class="field">
          <label class="flabel" for="lName">Last Name</label>
          <input type="text" id="lName" placeholder="Your last name">
          <span class="err-msg">Please enter your last name</span>
        </div>
        <div class="field">
          <label class="flabel" for="email">Email Address</label>
          <input type="email" id="email" placeholder="hello@example.com">
          <span class="err-msg">Please enter a valid email</span>
        </div>
        <div class="field">
          <label class="flabel" for="phone">WhatsApp Number</label>
          <input type="tel" id="phone" placeholder="+91 98765 43210">
          <span class="err-msg">Please enter your phone number</span>
        </div>
        <div class="field full">
          <label class="flabel" for="heard">How Did You Discover Us?</label>
          <select id="heard">
            <option value="" disabled selected>— Select one —</option>
            <option>Instagram</option>
            <option>Google</option>
            <option>Friend or Family</option>
            <option>Pinterest</option>
            <option>Wedding Blog</option>
            <option>Word of Mouth</option>
            <option>Other</option>
          </select>
        </div>
      </div>

      <div class="nav-btns">
        <span></span>
        <button class="btn btn-next" onclick="goNext(1)">Continue →</button>
      </div>
    </div>

    <!-- STEP 2 -->
    <div class="panel" id="step-2">
      <p class="panel-eyebrow">Step 02 of 04</p>
      <p class="panel-title">Your Event Details</p>
      <p class="panel-sub">Tell us about the celebration you're planning. Every detail helps us create the perfect proposal.</p>

      <div class="grid2">
        <div class="field">
          <label class="flabel" for="eType">Type of Event</label>
          <select id="eType">
            <option value="" disabled selected>— Choose event —</option>
            <option>Wedding</option>
            <option>Engagement</option>
            <option>Birthday</option>
            <option>Anniversary</option>
            <option>Baby Shower</option>
            <option>Corporate Event</option>
            <option>Farewell</option>
            <option>Product Launch</option>
            <option>Other</option>
          </select>
          <span class="err-msg">Please select an event type</span>
        </div>
        <div class="field">
          <label class="flabel" for="eDate">Event Date</label>
          <input type="date" id="eDate">
          <span class="err-msg">Please select a date</span>
        </div>
        <div class="field full">
          <label class="flabel" for="venue">Venue / Location</label>
          <input type="text" id="venue" placeholder="Venue name, city, or area">
          <span class="err-msg">Please enter a venue or location</span>
        </div>
        <div class="field full">
          <label class="flabel">Approximate Guest Count</label>
          <div style="margin-top: 6px;">
            <div class="guest-wrap">
              <div class="counter-row">
                <button class="cbtn" onclick="changeG(-10)">−</button>
                <div class="gnum" id="gNum">50</div>
                <button class="cbtn" onclick="changeG(10)">+</button>
              </div>
              <p class="glabel">Guests Expected</p>
            </div>
          </div>
        </div>
        <div class="field full">
          <label class="flabel" for="notes">Any Special Notes or Vision</label>
          <textarea id="notes" placeholder="Themes, inspirations, specific requirements, or anything else on your mind…"></textarea>
        </div>
      </div>

      <div class="nav-btns">
        <button class="btn btn-back" onclick="goPrev(2)">← Back</button>
        <button class="btn btn-next" onclick="goNext(2)">Continue →</button>
      </div>
    </div>

    <!-- STEP 3 -->
    <div class="panel" id="step-3">
      <p class="panel-eyebrow">Step 03 of 04</p>
      <p class="panel-title">Services You Need</p>
      <p class="panel-sub">Select everything you'd like The Leaf Studio to take care of. You can pick as many as you like.</p>

      <div class="services-grid">
        <div class="svc-card" onclick="toggleSvc(this)" data-svc="Decor & Florals">
          <span class="svc-icon">🌸</span>
          <span class="svc-name">Decor & Florals</span>
        </div>
        <div class="svc-card" onclick="toggleSvc(this)" data-svc="Photography">
          <span class="svc-icon">📷</span>
          <span class="svc-name">Photography</span>
        </div>
        <div class="svc-card" onclick="toggleSvc(this)" data-svc="Videography">
          <span class="svc-icon">🎬</span>
          <span class="svc-name">Videography</span>
        </div>
        <div class="svc-card" onclick="toggleSvc(this)" data-svc="Catering">
          <span class="svc-icon">🍽️</span>
          <span class="svc-name">Catering</span>
        </div>
        <div class="svc-card" onclick="toggleSvc(this)" data-svc="Entertainment & DJ">
          <span class="svc-icon">🎵</span>
          <span class="svc-name">Entertainment & DJ</span>
        </div>
        <div class="svc-card" onclick="toggleSvc(this)" data-svc="Invitation Design">
          <span class="svc-icon">💌</span>
          <span class="svc-name">Invitation Design</span>
        </div>
        <div class="svc-card" onclick="toggleSvc(this)" data-svc="Lighting">
          <span class="svc-icon">✨</span>
          <span class="svc-name">Lighting</span>
        </div>
        <div class="svc-card" onclick="toggleSvc(this)" data-svc="Event Coordination">
          <span class="svc-icon">📋</span>
          <span class="svc-name">Coordination</span>
        </div>
        <div class="svc-card" onclick="toggleSvc(this)" data-svc="Makeup & Styling">
          <span class="svc-icon">💄</span>
          <span class="svc-name">Makeup & Styling</span>
        </div>
      </div>

      <p class="err-msg" id="svcErr" style="margin-top:12px; font-size:11px;">Please select at least one service</p>

      <div class="nav-btns">
        <button class="btn btn-back" onclick="goPrev(3)">← Back</button>
        <button class="btn btn-next" onclick="goNext(3)">Continue →</button>
      </div>
    </div>

    <!-- STEP 4 -->
    <div class="panel" id="step-4">
      <p class="panel-eyebrow">Step 04 of 04</p>
      <p class="panel-title">Almost There</p>
      <p class="panel-sub">Just a couple of final questions before we put your personalised proposal together.</p>

      <div class="grid2">
        <div class="field">
          <label class="flabel" for="timeline">When Are You Looking to Book?</label>
          <select id="timeline">
            <option value="" disabled selected>— Select timeline —</option>
            <option>Within 1 month</option>
            <option>1–3 months</option>
            <option>3–6 months</option>
            <option>6–12 months</option>
            <option>More than a year away</option>
            <option>Flexible / Not sure yet</option>
          </select>
        </div>
        <div class="field">
          <label class="flabel" for="eSetup">Event Setup Preference</label>
          <select id="eSetup">
            <option value="" disabled selected>— Select setup —</option>
            <option>Outdoor</option>
            <option>Indoor</option>
            <option>Both Indoor & Outdoor</option>
            <option>Destination</option>
            <option>Not decided yet</option>
          </select>
        </div>
        <div class="field full">
          <label class="flabel" for="inspiration">Style / Inspiration (Optional)</label>
          <input type="text" id="inspiration" placeholder="e.g. Rustic botanical, Modern luxury, Whimsical garden…">
        </div>
        <div class="field full">
          <label class="flabel" for="extra">Anything Else We Should Know?</label>
          <textarea id="extra" placeholder="Share anything extra — cultural preferences, accessibility needs, surprises planned…" style="min-height:80px;"></textarea>
        </div>
      </div>

      <div class="nav-btns">
        <button class="btn btn-back" onclick="goPrev(4)">← Back</button>
        <button class="btn btn-submit" id="submitBtn" onclick="submitForm()">
          <span id="submitLabel">✦ Submit My Enquiry</span>
        </button>
      </div>
    </div>

  </div><!-- /card -->

  <!-- THANK YOU -->
  <div id="thankyou">
    <div class="card" style="padding: 72px 48px;">
      <span class="ty-icon">🌿</span>
      <h2 class="ty-title">Thank You, <em id="ty-name">Friend</em></h2>
      <div class="ty-line"></div>
      <p class="ty-msg">Your enquiry has been received and is already in our hands. Our team will review your details and reach out to you very soon.</p>
      <p class="ty-msg" style="margin-top: 8px; font-size: 13px;">We're excited to start building something beautiful with you.</p>
      <br>
      <a class="ty-whatsapp" id="waLink" href="#" target="_blank">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
        Chat on WhatsApp
      </a>
    </div>
  </div>

</div>

<footer>
  <p>© 2025 <span>The Leaf Studio</span> &nbsp;·&nbsp; Crafting Unforgettable Moments &nbsp;·&nbsp; All Rights Reserved</p>
</footer>

<!-- ══ SCRIPTS ══ -->
<script>
// ─── EmailJS Config ───────────────────────────────────────────
// Replace these with your actual EmailJS credentials
// Sign up free at https://www.emailjs.com
const EJ_KEY      = 'i6T0olUyJpqyEBwaK';
const EJ_SERVICE  = 'service_w7a5moi';
const EJ_TEMPLATE = 'template_wj8mx5q';

emailjs.init(EJ_KEY);

// ─── State ────────────────────────────────────────────────────
let step = 1;
let guests = 50;
let services = [];

// ─── Nav ──────────────────────────────────────────────────────
function toggleMenu() {
  document.getElementById('mobileMenu').classList.toggle('open');
}

// ─── Step logic ───────────────────────────────────────────────
function goNext(s) {
  if (!validate(s)) return;
  setStep(s + 1);
}

function goPrev(s) {
  setStep(s - 1);
}

function setStep(n) {
  document.querySelectorAll('.panel').forEach(p => p.classList.remove('active'));
  document.getElementById('step-' + n).classList.add('active');

  document.querySelectorAll('.pdot').forEach(d => {
    const ds = parseInt(d.dataset.s);
    d.classList.remove('active', 'done');
    if (ds < n) d.classList.add('done');
    if (ds === n) d.classList.add('active');
  });

  for (let i = 1; i <= 3; i++) {
    document.getElementById('pl' + i).classList.toggle('done', i < n);
  }

  step = n;
  window.scrollTo({ top: 0, behavior: 'smooth' });
}

// ─── Validation ───────────────────────────────────────────────
function validate(s) {
  let ok = true;

  if (s === 1) {
    ok &= chk('fName', v => v.trim().length > 0);
    ok &= chk('lName', v => v.trim().length > 0);
    ok &= chk('email', v => /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(v));
    ok &= chk('phone', v => v.trim().length >= 7);
  }

  if (s === 2) {
    ok &= chk('eType', v => v !== '');
    ok &= chk('eDate', v => v !== '');
    ok &= chk('venue', v => v.trim().length > 0);
  }

  if (s === 3) {
    if (services.length === 0) {
      document.getElementById('svcErr').style.display = 'block';
      ok = false;
    } else {
      document.getElementById('svcErr').style.display = 'none';
    }
  }

  return !!ok;
}

function chk(id, fn) {
  const el = document.getElementById(id);
  const field = el.closest('.field');
  const valid = fn(el.value);
  field.classList.toggle('has-err', !valid);
  return valid;
}

// ─── Guest counter ────────────────────────────────────────────
function changeG(d) {
  guests = Math.max(10, Math.min(5000, guests + d));
  document.getElementById('gNum').textContent = guests;
}

// ─── Services toggle ──────────────────────────────────────────
function toggleSvc(card) {
  const svc = card.dataset.svc;
  if (card.classList.contains('sel')) {
    card.classList.remove('sel');
    services = services.filter(s => s !== svc);
  } else {
    card.classList.add('sel');
    services.push(svc);
  }
  if (services.length) document.getElementById('svcErr').style.display = 'none';
}

// ─── Submit ───────────────────────────────────────────────────
async function submitForm() {
  const btn = document.getElementById('submitBtn');
  const label = document.getElementById('submitLabel');

  const firstName   = document.getElementById('fName').value.trim();
  const lastName    = document.getElementById('lName').value.trim();
  const email       = document.getElementById('email').value.trim();
  const phone       = document.getElementById('phone').value.trim();
  const heard       = document.getElementById('heard').value || 'Not specified';
  const eType       = document.getElementById('eType').value;
  const eDate       = document.getElementById('eDate').value;
  const venue       = document.getElementById('venue').value.trim();
  const notes       = document.getElementById('notes').value.trim() || 'None';
  const timeline    = document.getElementById('timeline').value || 'Not specified';
  const setup       = document.getElementById('eSetup').value || 'Not specified';
  const inspiration = document.getElementById('inspiration').value.trim() || 'Not specified';
  const extra       = document.getElementById('extra').value.trim() || 'None';

  // Format date nicely
  const dateFormatted = eDate
    ? new Date(eDate).toLocaleDateString('en-IN', { day: 'numeric', month: 'long', year: 'numeric' })
    : 'Not specified';

  // Loading state
  btn.style.pointerEvents = 'none';
  label.innerHTML = '<span class="spinner"></span> Sending…';

  const params = {
    to_name:     'The Leaf Studio',
    to_email:    'b.pavansathwik@gmail.com',
    from_name:   `${firstName} ${lastName}`,
    from_email:  email,
    phone:       phone,
    heard:       heard,
    event_type:  eType,
    event_date:  dateFormatted,
    venue:       venue,
    guests:      guests,
    services:    services.join(', '),
    notes:       notes,
    timeline:    timeline,
    setup:       setup,
    inspiration: inspiration,
    extra:       extra,
  };

  try {
    await emailjs.send(EJ_SERVICE, EJ_TEMPLATE, params);
  } catch (e) {
    console.warn('EmailJS error (check credentials):', e);
  }

  // Build WhatsApp link
  const waNum = phone.replace(/\D/g, '');
  const waMsg = encodeURIComponent(
    `Hello ${firstName}! 🌿\n\nThank you for reaching out to *The Leaf Studio*. We've received your enquiry for your *${eType}* on *${dateFormatted}* at *${venue}*.\n\nOur team will be in touch with you very soon with a personalised proposal.\n\nWarm regards,\nThe Leaf Studio ✨`
  );
  document.getElementById('waLink').href = `https://wa.me/${waNum}?text=${waMsg}`;

  // Show thank you
  document.getElementById('mainCard').style.display = 'none';
  document.getElementById('progressBar').style.display = 'none';
  document.getElementById('thankyou').style.display = 'block';
  document.getElementById('ty-name').textContent = firstName;

  window.scrollTo({ top: 0, behavior: 'smooth' });
}
</script>

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>Stay Blessed Insurance — Dealer Portal V2</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,500;9..144,600;9..144,700;9..144,800&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="css/styles.css">
</head>
<body class="has-controls">

<div class="demo-controls">
  <span>📱 Prototype</span>
  <span class="demo-sep">·</span>
  <button class="demo-link" onclick="showScreen('home')">Home</button>
  <span class="demo-sep">·</span>
  <button class="demo-link" onclick="goToCapture()">Capture</button>
  <span class="demo-sep">·</span>
  <button class="demo-link" onclick="showScreen('verify')">Verify</button>
  <span class="demo-sep">·</span>
  <button class="demo-link" onclick="goToTracker(3)">Tracker</button>
  <span class="demo-sep">·</span>
  <button class="demo-link" onclick="showScreen('telegram')">Telegram</button>
  <span class="demo-sep">·</span>
  <button class="demo-link" onclick="openChat()">Evie</button>
</div>

<div class="app-frame">
  <div class="ambient"><div class="orb1"></div><div class="orb2"></div></div>

  <!-- ═══════════════ HOME ═══════════════ -->
  <div class="screen active" id="screen-home">
    <div class="header fade-in">
      <div>
        <div class="online-pill"><div class="online-dot pulse-dot"></div><span class="online-text">Online</span></div>
        <div class="greeting">Good morning,</div>
        <div class="font-display name">Lee Martinez</div>
        <div class="dealership">Premier Auto Group</div>
      </div>
      <button class="icon-btn">
        <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0"/></svg>
        <div class="badge"></div>
      </button>
    </div>

    <div class="brand fade-in" style="animation-delay:0.1s">
      <div class="brand-row">
        <h2 class="font-display brand-name">Stay <span class="shimmer-gold">Blessed</span></h2>
        <span class="brand-tag">Dealer</span>
      </div>
      <div class="brand-line"></div>
    </div>

    <button class="primary-action slide-up" style="animation-delay:0.15s" onclick="goToCapture()">
      <div class="primary-action-glow"></div>
      <div class="primary-action-inner">
        <div class="primary-action-icon">
          <svg class="icon-xl" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M6.827 6.175A2.31 2.31 0 015.186 7.23c-.38.054-.757.112-1.134.175C2.999 7.58 2.25 8.507 2.25 9.574V18a2.25 2.25 0 002.25 2.25h15A2.25 2.25 0 0021.75 18V9.574c0-1.067-.75-1.994-1.802-2.169a47.865 47.865 0 00-1.134-.175 2.31 2.31 0 01-1.64-1.055l-.822-1.316a2.192 2.192 0 00-1.736-1.039 48.774 48.774 0 00-5.232 0 2.192 2.192 0 00-1.736 1.039l-.821 1.316z"/><path stroke-linecap="round" stroke-linejoin="round" d="M16.5 12.75a4.5 4.5 0 11-9 0 4.5 4.5 0 019 0z"/></svg>
        </div>
        <div class="primary-action-text">
          <div class="font-display primary-action-title">New Submission</div>
          <div class="primary-action-sub">Snap the Bill of Sale → bound in minutes</div>
        </div>
        <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="color:rgba(255,255,255,0.8)"><path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5"/></svg>
      </div>
    </button>

    <div class="stats slide-up" style="animation-delay:0.2s">
      <div class="stat-card"><div class="stat-label">Today</div><div class="font-display stat-value">3</div><div class="stat-sub">submissions</div></div>
      <div class="stat-card"><div class="stat-label">Week</div><div class="font-display stat-value">14</div><div class="stat-sub">submissions</div></div>
      <div class="stat-card">
        <div class="stat-glow"></div>
        <div class="stat-label">Bind Rate</div>
        <div class="font-display stat-value gold-text">89<span class="stat-value-sm">%</span></div>
        <div class="stat-trend">
          <svg style="width:0.625rem;height:0.625rem" viewBox="0 0 24 24" fill="none" stroke="#34d399" stroke-width="2.5"><path stroke-linecap="round" stroke-linejoin="round" d="M2.25 18L9 11.25l4.306 4.306a11.95 11.95 0 015.814-5.518l2.74-1.22m0 0l-5.94-2.28m5.94 2.28l-2.28 5.941"/></svg>
          <span class="stat-trend-text">+2% mo</span>
        </div>
      </div>
    </div>

    <div class="slide-up" style="animation-delay:0.25s">
      <div class="section-head">
        <h3 class="font-display section-title">In Progress</h3>
        <button class="section-link">View All</button>
      </div>
      <div class="sub-list">
        <button class="sub-card" onclick="goToTracker(3)">
          <div class="sub-head">
            <div><div class="font-display sub-customer">Maria Rodriguez</div><div class="sub-meta">2022 Honda CR-V · SB-2401</div></div>
            <div class="live-pill"><div class="live-dot pulse-dot"></div><span class="live-text">Live</span></div>
          </div>
          <div class="stage-bar"><div class="stage-segment stage-active"></div><div class="stage-segment stage-active"></div><div class="stage-segment stage-active"></div><div class="stage-segment stage-inactive"></div><div class="stage-segment stage-inactive"></div></div>
          <div class="sub-foot"><span class="sub-status-active">Quoting<span class="sub-status-rep"> · Sara</span></span><span class="sub-eta">~3 min</span></div>
        </button>
        <button class="sub-card" onclick="goToTracker(2)">
          <div class="sub-head">
            <div><div class="font-display sub-customer">Aisha Patel</div><div class="sub-meta">2024 Tesla Model Y · SB-2395</div></div>
            <div class="live-pill"><div class="live-dot pulse-dot"></div><span class="live-text">Live</span></div>
          </div>
          <div class="stage-bar"><div class="stage-segment stage-active"></div><div class="stage-segment stage-active"></div><div class="stage-segment stage-inactive"></div><div class="stage-segment stage-inactive"></div><div class="stage-segment stage-inactive"></div></div>
          <div class="sub-foot"><span class="sub-status-active">Calling<span class="sub-status-rep"> · Fred</span></span><span class="sub-eta">~6 min</span></div>
        </button>
      </div>
    </div>
  </div>

  <!-- ═══════════════ CAPTURE ═══════════════ -->
  <div class="capture-screen" id="screen-capture">
    <div class="capture-header">
      <button class="icon-btn" onclick="goHome()">
        <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"/></svg>
      </button>
      <span class="capture-title">Bill of Sale · 1 of 1</span>
      <div style="width:2.75rem"></div>
    </div>

    <div class="capture-greeting" id="capture-greeting">Hey Lee, let's get your customer insured! 🚗</div>

    <div class="capture-body">
      <div class="viewfinder" id="viewfinder">
        <div class="doc-mock" id="doc-mock">
          <div class="scanner-line"></div>
          <div class="doc-title">BILL OF SALE</div>
          <div class="doc-sub">Motor Vehicle Purchase Agreement</div>
          <div class="doc-line h1"></div><div class="doc-line h2"></div>
          <div class="doc-line t1"></div><div class="doc-line t2"></div><div class="doc-line t3"></div>
          <div class="doc-line h3"></div>
          <div class="doc-line t4"></div><div class="doc-line t5"></div>
        </div>
        <div class="frame-corners">
          <div class="corner tl gold" id="c-tl"></div>
          <div class="corner tr gold" id="c-tr"></div>
          <div class="corner bl gold" id="c-bl"></div>
          <div class="corner br gold" id="c-br"></div>
        </div>
        <div class="status-label status-searching" id="vf-status">Searching for document…</div>
        <div class="processing-overlay" id="processing-overlay">
          <div class="processing-row">
            <svg style="width:1rem;height:1rem;animation:spin 1s linear infinite;color:#C9A961" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M16.023 9.348h4.992v-.001M2.985 19.644v-4.992m0 0h4.992m-4.993 0l3.181 3.183a8.25 8.25 0 0013.803-3.7M4.031 9.865a8.25 8.25 0 0113.803-3.7l3.181 3.182m0-4.991v4.99"/></svg>
            <span class="processing-text">Reading Bill of Sale…</span>
          </div>
          <div class="processing-sub" id="proc-sub">Extracting customer info…</div>
        </div>
        <div class="captured-overlay" id="captured-overlay">
          <div>
            <div class="check-circle"><svg class="icon-lg" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5"><path stroke-linecap="round" stroke-linejoin="round" d="M4.5 12.75l6 6 9-13.5"/></svg></div>
            <div style="color:white;font-size:1.125rem;font-weight:600">Captured!</div>
          </div>
        </div>
      </div>

      <!-- Controls -->
      <div class="capture-controls" id="capture-controls">
        <button class="gallery-btn">
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M2.25 15.75l5.159-5.159a2.25 2.25 0 013.182 0l5.159 5.159m-1.5-1.5l1.409-1.409a2.25 2.25 0 013.182 0l2.909 2.909m-18 3.75h16.5a1.5 1.5 0 001.5-1.5V6a1.5 1.5 0 00-1.5-1.5H3.75A1.5 1.5 0 002.25 6v12a1.5 1.5 0 001.5 1.5zm10.5-11.25h.008v.008h-.008V8.25zm.375 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z"/></svg>
        </button>
        <button class="shutter-btn" onclick="startCapture()">
          <div class="shutter-inner">
            <svg class="icon-lg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M6.827 6.175A2.31 2.31 0 015.186 7.23c-.38.054-.757.112-1.134.175C2.999 7.58 2.25 8.507 2.25 9.574V18a2.25 2.25 0 002.25 2.25h15A2.25 2.25 0 0021.75 18V9.574c0-1.067-.75-1.994-1.802-2.169a47.865 47.865 0 00-1.134-.175 2.31 2.31 0 01-1.64-1.055l-.822-1.316a2.192 2.192 0 00-1.736-1.039 48.774 48.774 0 00-5.232 0 2.192 2.192 0 00-1.736 1.039l-.821 1.316z"/><path stroke-linecap="round" stroke-linejoin="round" d="M16.5 12.75a4.5 4.5 0 11-9 0 4.5 4.5 0 019 0z"/></svg>
          </div>
        </button>
        <button class="flash-btn">
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M3.75 13.5l10.5-11.25L12 10.5h8.25L9.75 21.75 12 13.5H3.75z"/></svg>
        </button>
      </div>

      <!-- Blurry error state -->
      <div class="blurry-error" id="blurry-error">
        <div class="blurry-icon">
          <svg class="icon-lg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z"/><path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
        </div>
        <div style="color:white;font-size:0.875rem;font-weight:600">Photo too blurry</div>
        <div style="color:rgba(255,255,255,0.5);font-size:0.75rem;margin-top:0.375rem">Hold steady and try again</div>
        <button class="retake-btn" onclick="resetCapture()">Retake Photo</button>
      </div>
    </div>
  </div>

  <!-- ═══════════════ VERIFY ═══════════════ -->
  <div class="screen" id="screen-verify">
    <div class="back-row fade-in">
      <button class="icon-btn" onclick="goToCapture()">
        <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5L8.25 12l7.5-7.5"/></svg>
      </button>
      <div><div class="back-title">Verify Info</div><div class="back-sub">2 sources · confirm before submitting</div></div>
    </div>

    <div class="source-bar fade-in">
      <span class="source-pill source-bos">📄 Bill of Sale</span>
      <span class="source-pill source-dl">🪪 Driver's License</span>
    </div>

    <div class="confidence-card slide-up">
      <div class="confidence-icon-wrap"><svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12.75L11.25 15 15 9.75M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg></div>
      <div><div class="confidence-text">96% OCR confidence</div><div class="confidence-sub">Fields pre-filled · review before sending</div></div>
    </div>

    <!-- Address conflict -->
    <div class="conflict-box slide-up">
      <div class="conflict-label">Address conflict — two sources</div>
      <div class="conflict-row">
        <span class="conflict-source conflict-win">BOS</span>
        <span class="conflict-value">742 Collins Ave, Miami Beach FL 33139</span>
        <span class="conflict-check">✓ Used</span>
      </div>
      <div class="conflict-row">
        <span class="conflict-source conflict-lose">DL</span>
        <span class="conflict-value crossed">851 NW 7th St, Miami FL 33136</span>
      </div>
    </div>

    <!-- Customer -->
    <div class="field-group slide-up">
      <div class="field-group-label">Customer</div>
      <div class="field-list">
        <div class="field-row">
          <div class="field-content"><div class="field-label">Name</div><div class="field-value">Maria Rodriguez</div></div>
          <div class="field-badge bos"><span class="field-badge-text">BOS</span></div>
        </div>
        <div class="field-row">
          <div class="field-content"><div class="field-label">Date of Birth</div><div class="field-value">03 / 14 / 1989</div></div>
          <div class="field-badge dl"><span class="field-badge-text">DL</span></div>
        </div>
        <div class="field-row">
          <div class="field-content"><div class="field-label">Address</div><div class="field-value">742 Collins Ave, Miami Beach FL 33139</div><div class="field-note">Bill of Sale address overrides license — it's more current</div></div>
          <div class="field-badge bos"><span class="field-badge-text">BOS</span></div>
        </div>
        <div class="field-row">
          <div class="field-content"><div class="field-label">Phone <span style="color:#f87171;font-size:0.6rem">Required</span></div><div class="field-value">(305) 555-0142</div></div>
        </div>
        <div class="field-row">
          <div class="field-content"><div class="field-label">Email <span style="color:#f87171;font-size:0.6rem">Required</span></div><div class="field-value">m.rodriguez@email.com</div></div>
        </div>
      </div>
    </div>

    <!-- Vehicle -->
    <div class="field-group slide-up" style="animation-delay:0.08s">
      <div class="field-group-label">Vehicle</div>
      <div class="field-list">
        <div class="field-row">
          <div class="field-content"><div class="field-label">VIN</div><div class="field-value">5J6RW1H58NL023417</div></div>
          <div class="field-badge verified"><svg style="width:0.75rem;height:0.75rem" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12.75L11.25 15 15 9.75M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg><span class="field-badge-text">BOS</span></div>
        </div>
        <div class="field-row">
          <div class="field-content"><div class="field-label">Year / Make / Model</div><div class="field-value">2022 Honda CR-V EX-L</div></div>
          <div class="field-badge verified"><svg style="width:0.75rem;height:0.75rem" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12.75L11.25 15 15 9.75M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg><span class="field-badge-text">NHTSA</span></div>
        </div>
        <div class="field-row">
          <div class="field-content"><div class="field-label">Mileage <span style="color:rgba(255,255,255,0.3);font-size:0.6rem;font-style:italic">Optional</span></div><div class="field-value">12,847</div></div>
          <div class="field-badge warn"><span class="field-badge-text">Verify</span></div>
        </div>
      </div>
    </div>

    <!-- Lienholder -->
    <div class="field-group slide-up" style="animation-delay:0.12s">
      <div class="field-group-label" style="display:flex;align-items:center;justify-content:space-between">
        <span>Lienholder</span>
        <button class="owned-toggle" id="owned-toggle" onclick="toggleOwned()">Mark as Owned</button>
      </div>
      <div id="lienholder-fields">
        <div class="field-list">
          <div class="field-row"><div class="field-content"><div class="field-label">Name</div><div class="field-value">Honda Financial Services</div></div><div class="field-badge bos"><span class="field-badge-text">BOS</span></div></div>
          <div class="field-row"><div class="field-content"><div class="field-label">Address</div><div class="field-value">P.O. Box 1027, Alpharetta GA 30009</div></div><div class="field-badge bos"><span class="field-badge-text">BOS</span></div></div>
        </div>
      </div>
      <div id="owned-msg" style="display:none;padding:0.875rem;background:rgba(74,222,128,0.06);border:1px solid rgba(74,222,128,0.18);border-radius:0.75rem;font-size:0.8rem;color:#4ade80;text-align:center;">
        ✓ Vehicle owned outright — no lienholder required
      </div>
    </div>

    <!-- Language + Contact Preference -->
    <div class="field-group slide-up" style="animation-delay:0.16s">
      <div class="field-group-label">Customer Language</div>
      <div class="lang-toggle-row">
        <button class="lang-btn active" id="lang-en" onclick="setLang('en')">English</button>
        <button class="lang-btn" id="lang-es" onclick="setLang('es')">Spanish</button>
      </div>
    </div>

    <div class="field-group slide-up" style="animation-delay:0.19s">
      <div class="field-group-label">Contact Preference</div>
      <div class="lang-toggle-row">
        <button class="lang-btn active" id="contact-call" onclick="setContact('call')">📞 Call</button>
        <button class="lang-btn" id="contact-text" onclick="setContact('text')">💬 Text</button>
      </div>
    </div>

    <button class="submit-btn" onclick="submitToTracker()">
      <span>Submit to Stay Blessed</span>
      <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M6 12L3.269 3.125A59.769 59.769 0 0121.485 12 59.768 59.768 0 013.27 20.875L5.999 12zm0 0h7.5"/></svg>
    </button>
    <p class="submit-note">Submission fires instantly · Telegram alert sent to team</p>
  </div>

  <!-- ═══════════════ TRACKER ═══════════════ -->
  <div class="screen" id="screen-tracker">
    <div class="tracker-header">
      <button class="icon-btn" onclick="goHome()">
        <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5L8.25 12l7.5-7.5"/></svg>
      </button>
      <button class="toggle-pill" id="customer-toggle" onclick="toggleCustomerView()">Show Customer</button>
    </div>

    <div style="margin-bottom:1.75rem">
      <div class="tracker-id">SB-2401</div>
      <h2 class="font-display tracker-name">Maria Rodriguez</h2>
      <p class="tracker-vehicle">2022 Honda CR-V</p>
    </div>

    <div class="rep-card" id="rep-card" style="display:none">
      <div class="rep-avatar"><img src="assets/embedded-image-1.jpg" alt="Sara"></div>
      <div style="flex:1">
        <div class="rep-name">Sara Bedoya Castaño</div>
        <div class="rep-role">Operations & Production · Pereira</div>
      </div>
      <div class="active-pill" id="rep-active">
        <div class="active-dot pulse-dot"></div>
        <span class="active-text">Active</span>
      </div>
    </div>

    <div class="stages-list" id="stages-list"></div>

    <div class="bound-celebration" id="bound-celebration">
      <div class="bound-row">
        <div class="bound-icon-wrap"><svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M16.5 18.75h-9m9 0a3 3 0 013 3h-15a3 3 0 013-3m9 0v-3.375c0-.621-.503-1.125-1.125-1.125h-.871M7.5 18.75v-3.375c0-.621.504-1.125 1.125-1.125h.872m5.007 0H9.497m5.007 0a7.454 7.454 0 01-.982-3.172M9.497 14.25a7.454 7.454 0 00.981-3.172M5.25 4.236c-.982.143-1.954.317-2.916.52A6.003 6.003 0 007.73 9.728M5.25 4.236V4.5c0 2.108.966 3.99 2.48 5.228M5.25 4.236V2.721C7.456 2.41 9.71 2.25 12 2.25c2.291 0 4.545.16 6.75.47v1.516M7.73 9.728a6.726 6.726 0 002.748 1.35m8.272-6.842V4.5c0 2.108-.966 3.99-2.48 5.228m2.48-5.492a46.32 46.32 0 012.916.52 6.003 6.003 0 01-5.395 4.972m0 0a6.726 6.726 0 01-2.749 1.35m0 0a6.772 6.772 0 01-3.044 0"/></svg></div>
        <div><div class="font-display bound-title">Deal closed in 7 minutes 🎉</div><div class="bound-sub">Welcome packet emailed to Maria</div></div>
      </div>
      <div class="bound-msg">Sara will follow up for the welcome call within 24–48 hours.</div>
    </div>
  </div>

  <!-- ═══════════════ TELEGRAM ═══════════════ -->
  <div class="screen tg-screen" id="screen-telegram" style="padding:0;background:#1c1c1e;">
    <div class="tg-topbar">
      <button class="tg-back" onclick="goHome()">‹ Back</button>
      <div class="tg-bot-avatar">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="white"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm4.64 6.8l-1.68 7.93c-.12.58-.46.72-.94.45l-2.6-1.92-1.25 1.21c-.14.14-.26.26-.53.26l.19-2.69 4.87-4.4c.21-.19-.05-.29-.33-.1L7.28 14.4l-2.56-.8c-.56-.17-.57-.56.12-.83l10.01-3.86c.46-.17.87.11.79.89z"/></svg>
      </div>
      <div>
        <div class="tg-chat-name">Stay Blessed — Submissions</div>
        <div class="tg-chat-sub">3 members</div>
      </div>
    </div>

    <div class="tg-body">
      <div class="tg-demo-row">
        <button class="tg-demo-btn active" onclick="tgScenario('es',this)">Spanish</button>
        <button class="tg-demo-btn" onclick="tgScenario('en',this)">English</button>
        <button class="tg-demo-btn" onclick="tgScenario('claimed',this)">After claimed</button>
      </div>

      <div class="tg-ts">Today, 2:47 PM</div>

      <div class="tg-bubble">
        <div class="tg-sender">🤖 Stay Blessed Bot</div>
        <div class="tg-alert-head">
          <span style="font-size:1rem">🚗</span>
          <span class="tg-alert-title">New Submission</span>
          <span class="lang-badge" id="tg-lang-badge">SPANISH</span>
        </div>
        <div class="tg-info-row"><span class="tg-info-label">From</span><span class="tg-info-value">Lee Martinez · Premier Auto</span></div>
        <div class="tg-info-row"><span class="tg-info-label">Customer</span><span class="tg-info-value">Maria Rodriguez</span></div>
        <div class="tg-info-row"><span class="tg-info-label">Vehicle</span><span class="tg-info-value">2022 Honda CR-V</span></div>
        <div class="tg-info-row"><span class="tg-info-label">VIN</span><span class="tg-info-value" style="color:rgba(255,255,255,0.45)">···023417</span></div>
        <div class="tg-info-row"><span class="tg-info-label">Phone</span><span class="tg-info-value">(305) 555-0142</span></div>
        <div class="tg-divider"></div>
        <div class="tg-claim-label">Claim this lead</div>
        <div class="tg-buttons">
          <button class="tg-btn claim-btn" id="tg-claim-btn" onclick="tgClaim()">✋ I'm on it</button>
          <button class="tg-btn view-btn">👁 View in Portal</button>
        </div>
        <div class="tg-claimed-msg" id="tg-claimed-msg">
          <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="#4ade80" stroke-width="2.5"><path stroke-linecap="round" stroke-linejoin="round" d="M4.5 12.75l6 6 9-13.5"/></svg>
          <span>Locked in — you own this lead</span>
        </div>
      </div>

      <div class="tg-system-msg" id="tg-system-msg">
        ✅ <strong>Sara</strong> is on it — calling Maria now.
      </div>
    </div>
  </div>

  <!-- ═══════════════ EVIE CHAT ═══════════════ -->
  <button class="ai-fab" id="ai-fab" onclick="openChat()" style="right:1.5rem">
    <svg class="icon-lg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M9.813 15.904L9 18.75l-.813-2.846a4.5 4.5 0 00-3.09-3.09L2.25 12l2.846-.813a4.5 4.5 0 003.09-3.09L9 5.25l.813 2.846a4.5 4.5 0 003.09 3.09L15.75 12l-2.847.813a4.5 4.5 0 00-3.09 3.091zM18.259 8.715L18 9.75l-.259-1.035a3.375 3.375 0 00-2.455-2.456L14.25 6l1.036-.259a3.375 3.375 0 002.455-2.456L18 2.25l.259 1.035a3.375 3.375 0 002.456 2.456L21.75 6l-1.035.259a3.375 3.375 0 00-2.456 2.456z"/></svg>
    <div class="ai-fab-badge"></div>
  </button>

  <div class="chat-panel" id="chat-panel">
    <div class="chat-header-bar">
      <div class="evie-avatar">
        <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#0A1628" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M9.813 15.904L9 18.75l-.813-2.846a4.5 4.5 0 00-3.09-3.09L2.25 12l2.846-.813a4.5 4.5 0 003.09-3.09L9 5.25l.813 2.846a4.5 4.5 0 003.09 3.09L15.75 12l-2.847.813a4.5 4.5 0 00-3.09 3.091z"/></svg>
        <div class="evie-online"></div>
      </div>
      <div style="flex:1">
        <div class="chat-name">Evie</div>
        <div class="chat-status-line">Stay Blessed AI · Online</div>
      </div>
      <button class="icon-btn" onclick="closeChat()">
        <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"/></svg>
      </button>
    </div>

    <div class="context-pill">
      <div class="context-icon-wrap">
        <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="#C9A961" stroke-width="1.5"><path stroke-linecap="round" stroke-linejoin="round" d="M19.5 14.25v-2.625a3.375 3.375 0 00-3.375-3.375h-1.5A1.125 1.125 0 0113.5 7.125v-1.5a3.375 3.375 0 00-3.375-3.375H8.25m0 12.75h7.5m-7.5 3H12M10.5 2.25H5.625c-.621 0-1.125.504-1.125 1.125v17.25c0 .621.504 1.125 1.125 1.125h12.75c.621 0 1.125-.504 1.125-1.125V11.25a9 9 0 00-9-9z"/></svg>
      </div>
      <div>
        <div class="context-label">Active submission</div>
        <div class="context-value">SB-2401 · Maria Rodriguez · 2022 Honda CR-V</div>
      </div>
    </div>

    <div class="chat-messages" id="chat-messages">
      <div class="msg-row assistant">
        <div class="msg-bubble assistant">Hey Lee 👋 I'm Evie — here to help. Ask me about coverage, check a submission status, or get a script for a tough customer objection.</div>
      </div>
    </div>

    <div class="suggestions-row">
      <button class="suggestion-chip" onclick="quickAsk('Status of Maria?')">Status of Maria?</button>
      <button class="suggestion-chip" onclick="quickAsk('Customer says too expensive')">Too expensive</button>
      <button class="suggestion-chip" onclick="quickAsk('Do you cover rideshare?')">Rideshare?</button>
      <button class="suggestion-chip" onclick="quickAsk('Salvage title vehicle')">Salvage title?</button>
      <button class="suggestion-chip" onclick="quickAsk('What is the rate?')">Rate question</button>
    </div>

    <div class="chat-input-area">
      <div class="evie-thinking" id="evie-thinking">Evie is thinking…</div>
      <div class="chat-input-row">
        <input class="chat-input" id="chat-input" placeholder="Ask Evie anything…" onkeydown="if(event.key==='Enter')sendMessage()" oninput="updateSendBtn()">
        <button class="send-btn" id="send-btn" onclick="sendMessage()">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path stroke-linecap="round" stroke-linejoin="round" d="M6 12L3.269 3.125A59.769 59.769 0 0121.485 12 59.768 59.768 0 013.27 20.875L5.999 12zm0 0h7.5"/></svg>
        </button>
      </div>
    </div>
  </div>

  <div class="customer-banner" id="customer-banner">
    <span class="customer-banner-text">Customer view · Hand them the phone</span>
  </div>
</div>

<script src="js/app.js"></script>
</body>
</html>

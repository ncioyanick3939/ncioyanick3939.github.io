<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Login – Nico Rüttimann</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --gold: #b8912e;
    --gold-light: #d4aa52;
    --dark: #161614;
    --dark-2: #1e1d1a;
    --dark-3: #28261f;
    --mid: #5a5850;
    --muted: #9a9890;
    --light: #f5f3ee;
    --border: #e4e0d8;
    --white: #fefefe;
    --error: #c0392b;
    --ok: #2e7d4f;
    --serif: 'Cormorant Garamond', Georgia, serif;
    --sans: 'DM Sans', system-ui, sans-serif;
  }
  * { margin: 0; padding: 0; box-sizing: border-box; }
  html { scroll-behavior: smooth; }
  body { font-family: var(--sans); color: var(--dark); background: var(--light); line-height: 1.6; min-height: 100vh; }

  nav {
    position: fixed; top: 0; left: 0; right: 0; z-index: 200;
    display: flex; justify-content: space-between; align-items: center;
    padding: 0 3rem; height: 68px;
    background: rgba(22,22,20,0.96);
    backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px);
    border-bottom: 1px solid rgba(184,145,46,0.12);
  }
  nav .logo { text-decoration: none; display: flex; align-items: center; height: 100%; }
  nav .logo img { height: 42px; width: auto; object-fit: contain; display: block; }
  .nav-back { color: rgba(255,255,255,0.5); text-decoration: none; font-size: 0.72rem; font-weight: 500; letter-spacing: 1.8px; text-transform: uppercase; transition: color 0.2s; }
  .nav-back:hover { color: #fff; }

  .auth-wrap { min-height: 100vh; display: flex; align-items: center; justify-content: center; padding: 7rem 1.5rem 4rem; }
  .auth-card { width: 100%; max-width: 440px; background: var(--white); border: 1px solid var(--border); padding: 3rem 2.5rem; }
  .auth-label { font-size: 0.65rem; font-weight: 500; letter-spacing: 3px; text-transform: uppercase; color: var(--gold); margin-bottom: 0.8rem; }
  .auth-title { font-family: var(--serif); font-size: 2.2rem; font-weight: 300; line-height: 1.1; margin-bottom: 0.4rem; }
  .auth-title em { font-style: italic; color: var(--gold); }
  .auth-sub { font-size: 0.84rem; color: var(--muted); font-weight: 300; margin-bottom: 2rem; }

  .tabs { display: flex; border: 1px solid var(--border); margin-bottom: 2rem; }
  .tab { flex: 1; padding: 0.8rem; background: transparent; border: none; cursor: pointer; font-family: var(--sans); font-size: 0.7rem; font-weight: 500; letter-spacing: 1.5px; text-transform: uppercase; color: var(--muted); transition: all 0.2s; }
  .tab.active { background: var(--dark); color: var(--gold-light); }

  form { display: grid; gap: 1.1rem; }
  .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 1.1rem; }
  .form-group { display: flex; flex-direction: column; gap: 0.4rem; }
  label { font-size: 0.62rem; font-weight: 500; letter-spacing: 1.8px; text-transform: uppercase; color: var(--muted); }
  input {
    width: 100%; padding: 0.85rem 1rem; border: 1px solid var(--border); border-radius: 0;
    font-size: 0.9rem; font-family: var(--sans); background: var(--light); color: var(--dark);
    transition: border-color 0.2s, background 0.2s;
  }
  input:focus { outline: none; border-color: var(--gold); background: var(--white); }
  .btn-submit {
    display: flex; align-items: center; justify-content: center; gap: 0.6rem;
    width: 100%; padding: 1rem 2rem; background: var(--dark); color: #fff;
    border: none; cursor: pointer; font-family: var(--sans); font-size: 0.72rem;
    font-weight: 500; letter-spacing: 2px; text-transform: uppercase;
    transition: background 0.2s; margin-top: 0.5rem;
  }
  .btn-submit:hover { background: var(--gold); }
  .btn-submit:disabled { opacity: 0.5; cursor: not-allowed; }
  .hint { font-size: 0.72rem; color: var(--muted); font-weight: 300; line-height: 1.5; }
  .hint a { color: var(--gold); }

  .msg { font-size: 0.82rem; padding: 0.8rem 1rem; border-radius: 0; display: none; line-height: 1.5; }
  .msg.show { display: block; }
  .msg.error { background: rgba(192,57,43,0.08); color: var(--error); border: 1px solid rgba(192,57,43,0.2); }
  .msg.ok { background: rgba(46,125,79,0.08); color: var(--ok); border: 1px solid rgba(46,125,79,0.2); }

  .setup-warn { background: #fff8e6; border: 1px solid #e8d28a; color: #7a5d12; font-size: 0.78rem; padding: 0.9rem 1rem; margin-bottom: 1.5rem; line-height: 1.5; display: none; }
  .setup-warn.show { display: block; }

  @media (max-width: 600px) {
    nav { padding: 0 1.5rem; }
    .auth-card { padding: 2.5rem 1.5rem; }
    .form-row { grid-template-columns: 1fr; }
  }
</style>
</head>
<body>

<nav>
  <a href="index.html" class="logo">
    <img src="logo_nav_final.png" alt="Nico Rüttimann">
  </a>
  <a href="community.html" class="nav-back">← Zurück</a>
</nav>

<div class="auth-wrap">
  <div class="auth-card">
    <p class="auth-label">Community</p>
    <h1 class="auth-title" id="cardTitle">Willkommen<br><em>zurück.</em></h1>
    <p class="auth-sub" id="cardSub">Melde dich an, um auf die exklusiven Inhalte zuzugreifen.</p>

    <div class="setup-warn" id="setupWarn">
      ⚙️ <strong>Noch nicht eingerichtet:</strong> Trage deine Supabase-Zugangsdaten
      oben im Code ein (SUPABASE_URL und SUPABASE_ANON_KEY), dann funktioniert das Login.
    </div>

    <div class="tabs">
      <button class="tab active" id="tabLogin" onclick="switchTab('login')">Einloggen</button>
      <button class="tab" id="tabRegister" onclick="switchTab('register')">Registrieren</button>
    </div>

    <div class="msg" id="msg"></div>

    <!-- LOGIN -->
    <form id="loginForm">
      <div class="form-group">
        <label for="loginEmail">E-Mail</label>
        <input type="email" id="loginEmail" required placeholder="deine@email.ch" autocomplete="email">
      </div>
      <div class="form-group">
        <label for="loginPassword">Passwort</label>
        <input type="password" id="loginPassword" required placeholder="••••••••" autocomplete="current-password">
      </div>
      <button type="submit" class="btn-submit" id="loginBtn">
        Einloggen
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
      </button>
    </form>

    <!-- REGISTER -->
    <form id="registerForm" style="display:none;">
      <div class="form-row">
        <div class="form-group">
          <label for="regVorname">Vorname</label>
          <input type="text" id="regVorname" required placeholder="Max" autocomplete="given-name">
        </div>
        <div class="form-group">
          <label for="regName">Name</label>
          <input type="text" id="regName" required placeholder="Muster" autocomplete="family-name">
        </div>
      </div>
      <div class="form-group">
        <label for="regEmail">E-Mail</label>
        <input type="email" id="regEmail" required placeholder="deine@email.ch" autocomplete="email">
      </div>
      <div class="form-group">
        <label for="regPassword">Passwort</label>
        <input type="password" id="regPassword" required minlength="6" placeholder="Mind. 6 Zeichen" autocomplete="new-password">
      </div>
      <button type="submit" class="btn-submit" id="registerBtn">
        Konto erstellen
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
      </button>
      <p class="hint">Mit der Registrierung erhältst du kostenlosen Zugriff auf alle exklusiven Inhalte.</p>
    </form>
  </div>
</div>

<!-- Supabase Client -->
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>
<script>
  /* ============================================================
     SUPABASE EINRICHTEN — so geht's (einmalig):
     1. Auf supabase.com gratis registrieren → "New Project"
        → Region "Frankfurt (EU Central)" wählen (Datenschutz!)
     2. Im Projekt: Settings → API
        → "Project URL" und "anon public key" kopieren
     3. Unten einsetzen (die zwei Zeilen):
     ============================================================ */
  const SUPABASE_URL = "DEINE_SUPABASE_URL_HIER";
  const SUPABASE_ANON_KEY = "DEIN_ANON_KEY_HIER";
  /* ============================================================ */

  const configured = !SUPABASE_URL.includes("HIER") && !SUPABASE_ANON_KEY.includes("HIER");
  let sb = null;
  if (configured) {
    sb = window.supabase.createClient(SUPABASE_URL, SUPABASE_ANON_KEY);
  } else {
    document.getElementById("setupWarn").classList.add("show");
  }

  const msg = document.getElementById("msg");
  function showMsg(text, type) {
    msg.textContent = text;
    msg.className = "msg show " + type;
  }
  function clearMsg() { msg.className = "msg"; }

  // Schon eingeloggt? → direkt in den Mitgliederbereich
  if (sb) {
    sb.auth.getSession().then(({ data }) => {
      if (data.session) window.location.href = "mitglieder.html";
    });
  }

  // Tabs
  function switchTab(which) {
    clearMsg();
    const login = which === "login";
    document.getElementById("tabLogin").classList.toggle("active", login);
    document.getElementById("tabRegister").classList.toggle("active", !login);
    document.getElementById("loginForm").style.display = login ? "grid" : "none";
    document.getElementById("registerForm").style.display = login ? "none" : "grid";
    document.getElementById("cardTitle").innerHTML = login ? "Willkommen<br><em>zurück.</em>" : "Werde<br><em>Mitglied.</em>";
    document.getElementById("cardSub").textContent = login
      ? "Melde dich an, um auf die exklusiven Inhalte zuzugreifen."
      : "Kostenlos registrieren und sofort Zugriff erhalten.";
  }

  // LOGIN
  document.getElementById("loginForm").addEventListener("submit", async (e) => {
    e.preventDefault();
    clearMsg();
    if (!sb) { showMsg("Login ist noch nicht eingerichtet (Supabase-Daten fehlen).", "error"); return; }
    const btn = document.getElementById("loginBtn");
    btn.disabled = true;
    const email = document.getElementById("loginEmail").value.trim();
    const password = document.getElementById("loginPassword").value;
    const { error } = await sb.auth.signInWithPassword({ email, password });
    btn.disabled = false;
    if (error) {
      showMsg("Login fehlgeschlagen: E-Mail oder Passwort stimmt nicht.", "error");
    } else {
      window.location.href = "mitglieder.html";
    }
  });

  // REGISTER
  document.getElementById("registerForm").addEventListener("submit", async (e) => {
    e.preventDefault();
    clearMsg();
    if (!sb) { showMsg("Registrierung ist noch nicht eingerichtet (Supabase-Daten fehlen).", "error"); return; }
    const btn = document.getElementById("registerBtn");
    btn.disabled = true;
    const vorname = document.getElementById("regVorname").value.trim();
    const name = document.getElementById("regName").value.trim();
    const email = document.getElementById("regEmail").value.trim();
    const password = document.getElementById("regPassword").value;

    const { data, error } = await sb.auth.signUp({
      email,
      password,
      options: { data: { vorname: vorname, name: name } }
    });
    btn.disabled = false;

    if (error) {
      showMsg("Registrierung fehlgeschlagen: " + error.message, "error");
    } else if (data.session) {
      // E-Mail-Bestätigung ist AUS → direkt eingeloggt
      window.location.href = "mitglieder.html";
    } else {
      // E-Mail-Bestätigung ist AN → Hinweis zeigen
      showMsg("Fast geschafft! Bitte bestätige deine E-Mail-Adresse über den Link, den wir dir geschickt haben.", "ok");
    }
  });
</script>
</body>
</html>

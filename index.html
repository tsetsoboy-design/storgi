<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kitchen Manager — Supabase Test</title>
<style>
:root{
  --bg:#0f1117;--bg2:#161b27;--bg3:#1e2535;--bg4:#252d3d;
  --border:#2a3347;--border2:#334060;
  --text:#e8edf5;--text2:#8b95a8;--text3:#5a6478;
  --blue:#4a9eff;--blue-bg:#0d1f3c;--blue-border:#1a3a6e;
  --green:#34d399;--green-bg:#052e1a;--green-border:#0a5c34;
  --red:#f87171;--red-bg:#2d0f0f;--red-border:#5c1a1a;
  --amber:#fbbf24;--amber-bg:#2a1a00;--amber-border:#5c3a00;
}
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:system-ui,sans-serif;font-size:14px;background:var(--bg);color:var(--text);padding:1.25rem;min-height:100vh}
.card{background:var(--bg2);border:1px solid var(--border);border-radius:10px;padding:1.25rem;margin-bottom:.875rem;max-width:420px}
label{font-size:11px;color:var(--text3);display:block;margin-bottom:4px;text-transform:uppercase;letter-spacing:.05em}
input{width:100%;padding:9px 11px;border:1px solid var(--border2);border-radius:7px;font-size:13px;background:var(--bg3);color:var(--text);outline:none;margin-bottom:10px}
input:focus{border-color:var(--blue)}
.btn{padding:9px 16px;font-size:13px;font-weight:600;cursor:pointer;border-radius:7px;border:1px solid var(--border2);background:var(--bg3);color:var(--text);width:100%}
.btn-blue{background:var(--blue);color:#fff;border-color:var(--blue)}
.btn-blue:hover{background:#3a8eee}
.status{padding:10px 14px;border-radius:8px;font-size:13px;margin-bottom:10px;word-break:break-word}
.status-ok{background:var(--green-bg);color:var(--green);border:1px solid var(--green-border)}
.status-err{background:var(--red-bg);color:var(--red);border:1px solid var(--red-border)}
.status-info{background:var(--blue-bg);color:var(--blue);border:1px solid var(--blue-border)}
.hidden{display:none}
table{width:100%;border-collapse:collapse;font-size:13px;margin-top:10px}
th,td{padding:7px 8px;border-bottom:1px solid var(--border);text-align:left}
.icon-btn{background:none;border:none;cursor:pointer;color:var(--red);font-size:13px}
</style>
</head>
<body>

<h1 style="font-size:18px;margin-bottom:1rem">🧮 Kitchen Manager — Connection Test</h1>

<!-- LOGIN -->
<div class="card" id="login-card">
  <div style="font-size:11px;color:var(--text3);text-transform:uppercase;letter-spacing:.05em;margin-bottom:10px">Admin Login</div>
  <div id="login-status"></div>
  <label>Email</label>
  <input type="email" id="login-email" placeholder="you@example.com">
  <label>Password</label>
  <input type="password" id="login-password" placeholder="••••••••">
  <button class="btn btn-blue" onclick="signIn()">Sign in</button>
  <hr style="border:none;border-top:1px solid var(--border);margin:14px 0">
  <div style="font-size:12px;color:var(--text3);margin-bottom:8px">First time? Create the admin account:</div>
  <button class="btn" onclick="signUp()">Create account with email/password above</button>
</div>

<!-- APP -->
<div class="card hidden" id="app-card" style="max-width:600px">
  <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px">
    <div style="font-weight:700">Signed in as <span id="user-email" style="color:var(--blue)"></span></div>
    <button class="btn" style="width:auto;padding:6px 12px;font-size:12px" onclick="signOut()">Sign out</button>
  </div>
  <div id="db-status"></div>

  <div style="margin-top:14px">
    <label>Add a test supplier</label>
    <input type="text" id="sup-name" placeholder="e.g. Metro Cash & Carry">
    <button class="btn btn-blue" onclick="addSupplier()">＋ Add supplier (saves to Supabase)</button>
  </div>

  <table>
    <thead><tr><th>Supplier</th><th>Created</th><th></th></tr></thead>
    <tbody id="suppliers-tbody"></tbody>
  </table>
</div>

<script>
const SUPABASE_URL = 'https://bpejkfafsphgjhiwcytg.supabase.co';
const SUPABASE_KEY = 'sb_publishable_xNfpRZeC524iue4y91RgeA_er6d9qTp';

function showStatus(elId, msg, type) {
  document.getElementById(elId).innerHTML = `<div class="status status-${type}">${msg}</div>`;
}

// ── store session in localStorage so refresh keeps you logged in ──
function saveSession(session) {
  localStorage.setItem('km_session', JSON.stringify(session));
}
function getSession() {
  try { return JSON.parse(localStorage.getItem('km_session') || 'null'); } catch(e) { return null; }
}
function clearSession() {
  localStorage.removeItem('km_session');
}

// ── AUTH via raw fetch to Supabase Auth REST API ──
async function signUp() {
  const email = document.getElementById('login-email').value.trim();
  const password = document.getElementById('login-password').value;
  if (!email || !password) { showStatus('login-status','Enter email and password.','err'); return; }
  if (password.length < 6) { showStatus('login-status','Password must be at least 6 characters.','err'); return; }
  showStatus('login-status','Creating account...','info');
  try {
    const res = await fetch(`${SUPABASE_URL}/auth/v1/signup`, {
      method: 'POST',
      headers: { 'apikey': SUPABASE_KEY, 'Content-Type': 'application/json' },
      body: JSON.stringify({ email, password })
    });
    const data = await res.json();
    if (!res.ok) { showStatus('login-status','Error: ' + (data.msg || data.error_description || JSON.stringify(data)), 'err'); return; }
    if (data.access_token) {
      saveSession(data);
      showStatus('login-status','Account created and signed in!','ok');
      onSignedIn(data);
    } else {
      showStatus('login-status','Account created. If email confirmation is on, confirm via email then Sign in. Otherwise just click Sign in now.','ok');
    }
  } catch (e) {
    showStatus('login-status','Network error: ' + e.message, 'err');
  }
}

async function signIn() {
  const email = document.getElementById('login-email').value.trim();
  const password = document.getElementById('login-password').value;
  if (!email || !password) { showStatus('login-status','Enter email and password.','err'); return; }
  showStatus('login-status','Signing in...','info');
  try {
    const res = await fetch(`${SUPABASE_URL}/auth/v1/token?grant_type=password`, {
      method: 'POST',
      headers: { 'apikey': SUPABASE_KEY, 'Content-Type': 'application/json' },
      body: JSON.stringify({ email, password })
    });
    const data = await res.json();
    if (!res.ok) { showStatus('login-status','Error: ' + (data.msg || data.error_description || JSON.stringify(data)), 'err'); return; }
    saveSession(data);
    onSignedIn(data);
  } catch (e) {
    showStatus('login-status','Network error: ' + e.message, 'err');
  }
}

function signOut() {
  clearSession();
  document.getElementById('app-card').classList.add('hidden');
  document.getElementById('login-card').classList.remove('hidden');
  document.getElementById('login-status').innerHTML = '';
}

function onSignedIn(session) {
  document.getElementById('login-card').classList.add('hidden');
  document.getElementById('app-card').classList.remove('hidden');
  document.getElementById('user-email').textContent = session.user?.email || '(signed in)';
  loadSuppliers();
}

// ── DB calls via raw fetch to Supabase REST (PostgREST) ──
function authHeaders() {
  const session = getSession();
  return {
    'apikey': SUPABASE_KEY,
    'Authorization': 'Bearer ' + (session?.access_token || SUPABASE_KEY),
    'Content-Type': 'application/json'
  };
}

async function addSupplier() {
  const name = document.getElementById('sup-name').value.trim();
  if (!name) return;
  showStatus('db-status','Saving...','info');
  try {
    const res = await fetch(`${SUPABASE_URL}/rest/v1/suppliers`, {
      method: 'POST',
      headers: { ...authHeaders(), 'Prefer': 'return=representation' },
      body: JSON.stringify({ name, products: [] })
    });
    if (!res.ok) {
      const err = await res.json();
      showStatus('db-status','Error: ' + (err.message || JSON.stringify(err)), 'err');
      return;
    }
    document.getElementById('sup-name').value='';
    showStatus('db-status','Saved to Supabase ✓','ok');
    loadSuppliers();
  } catch (e) {
    showStatus('db-status','Network error: ' + e.message, 'err');
  }
}

async function deleteSupplier(id) {
  await fetch(`${SUPABASE_URL}/rest/v1/suppliers?id=eq.${id}`, {
    method: 'DELETE',
    headers: authHeaders()
  });
  loadSuppliers();
}

async function loadSuppliers() {
  try {
    const res = await fetch(`${SUPABASE_URL}/rest/v1/suppliers?select=*&order=created_at.desc`, {
      headers: authHeaders()
    });
    if (!res.ok) {
      const err = await res.json();
      showStatus('db-status','Error loading: ' + (err.message || JSON.stringify(err)), 'err');
      return;
    }
    const data = await res.json();
    const tbody = document.getElementById('suppliers-tbody');
    if (!data.length) { tbody.innerHTML = '<tr><td colspan="3" style="color:var(--text3)">No suppliers yet — add one above to test.</td></tr>'; return; }
    tbody.innerHTML = data.map(s => `
      <tr>
        <td style="font-weight:600">🏪 ${s.name}</td>
        <td style="color:var(--text3);font-size:12px">${new Date(s.created_at).toLocaleString()}</td>
        <td><button class="icon-btn" onclick="deleteSupplier(${s.id})">🗑 delete</button></td>
      </tr>`).join('');
  } catch (e) {
    showStatus('db-status','Network error: ' + e.message, 'err');
  }
}

// check for existing session on load
const existingSession = getSession();
if (existingSession?.access_token) onSignedIn(existingSession);
</script>
</body>
</html>

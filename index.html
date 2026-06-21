<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kitchen Manager</title>
<style>
:root{
  /* Benjamin Moore Color Trends 2026 palette */
  --silhouette:#5c5250;       /* warm charcoal brown */
  --raindance:#a3b3a8;        /* sage green */
  --swisscoffee:#ece8dc;      /* warm off-white */
  --firstcrush:#e3dac9;       /* warm beige */
  --batik:#cbb4b3;            /* dusty pink */
  --narragansett:#3f4f53;     /* deep teal */
  --southwestpottery:#9c5b54; /* terracotta red */
  --sherwoodtan:#b89a76;      /* tan */

  --bg:#1c1a19;               /* near-black warm */
  --bg2:#27231f;              /* card bg - warm dark brown */
  --bg3:#332e29;              /* input bg */
  --bg4:#3d3631;              /* hover bg */
  --border:#473f38;
  --border2:#5c5250;
  --text:#ece8dc;             /* swiss coffee as main text */
  --text2:#cbb4b3;            /* batik as secondary text */
  --text3:#8a7a72;            /* muted brown-grey */

  --blue:#a3b3a8;             /* raindance sage as accent */
  --blue-bg:#2e3530;
  --blue-border:#4a5950;

  --green:#a3b3a8;            /* sage for "good" */
  --green-bg:#2c332e;
  --green-border:#46554a;

  --red:#c17b73;              /* lighter southwest pottery for alerts */
  --red-bg:#3a2723;
  --red-border:#6b3f37;

  --amber:#cbb4ad;            /* batik-ish for warnings */
  --amber-bg:#3a302c;
  --amber-border:#6b5650;
}
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:system-ui,sans-serif;font-size:14px;background:var(--bg);color:var(--text);padding:1.25rem;min-height:100vh}
.tabs{display:flex;gap:0;border-bottom:1px solid var(--border);margin-bottom:1.25rem;flex-wrap:wrap}
.tab{padding:9px 13px;font-size:13px;font-weight:500;cursor:pointer;border:none;background:none;color:var(--text2);border-bottom:2px solid transparent;margin-bottom:-1px;transition:color .15s;white-space:nowrap}
.tab:hover{color:var(--text)}
.tab.active{color:var(--sherwoodtan);border-bottom-color:var(--sherwoodtan)}
.pane{display:none}.pane.active{display:block}
.card{background:var(--bg2);border:1px solid var(--border);border-radius:10px;padding:1rem 1.125rem;margin-bottom:.875rem}
.card-title{font-size:11px;font-weight:600;color:var(--text3);text-transform:uppercase;letter-spacing:.06em;margin-bottom:.875rem}
label{font-size:11px;color:var(--text3);display:block;margin-bottom:4px;text-transform:uppercase;letter-spacing:.05em}
input,select{width:100%;padding:8px 10px;border:1px solid var(--border2);border-radius:7px;font-size:13px;background:var(--bg3);color:var(--text);outline:none;transition:border-color .15s}
input:focus,select:focus{border-color:var(--sherwoodtan)}
input::placeholder{color:var(--text3)}
select option{background:var(--bg3)}
.g2{display:grid;grid-template-columns:1fr 1fr;gap:10px;align-items:end}
.g3{display:grid;grid-template-columns:1fr 1fr 1fr;gap:10px;align-items:end}
.g4{display:grid;grid-template-columns:1fr 1fr 1fr 1fr;gap:10px;align-items:end}
.btn{padding:8px 14px;font-size:13px;font-weight:500;cursor:pointer;border-radius:7px;border:1px solid var(--border2);background:var(--bg3);color:var(--text);display:inline-flex;align-items:center;gap:5px;transition:all .15s;white-space:nowrap}
.btn:hover{background:var(--bg4)}
.btn-blue{background:var(--narragansett);color:var(--swisscoffee);border-color:var(--narragansett)}
.btn-blue:hover{background:#324048}
.btn-green{background:var(--silhouette);color:var(--swisscoffee);border-color:var(--silhouette);font-weight:700}
.btn-green:hover{background:#6a605c}
.btn-sm{padding:5px 10px;font-size:12px}
.icon-btn{background:none;border:none;cursor:pointer;padding:4px 6px;border-radius:5px;font-size:14px;color:var(--text3);transition:all .15s;display:inline-flex;align-items:center}
.icon-btn:hover.del{color:var(--red);background:var(--red-bg)}
.icon-btn:hover.edit{color:var(--blue);background:var(--blue-bg)}
.icon-btn:hover.move{color:var(--blue);background:var(--blue-bg)}
table{width:100%;border-collapse:collapse;font-size:13px}
th{text-align:left;font-size:10px;color:var(--text3);font-weight:600;padding:5px 8px;border-bottom:1px solid var(--border);text-transform:uppercase;letter-spacing:.05em;white-space:nowrap}
td{padding:8px 8px;border-bottom:1px solid var(--border);vertical-align:middle}
tr:last-child td{border-bottom:none}
tr:hover td{background:rgba(255,255,255,.018)}
.badge{display:inline-flex;align-items:center;padding:2px 9px;border-radius:99px;font-size:11px;font-weight:600}
.b-blue{background:rgba(63,79,83,0.3);color:var(--raindance);border:1px solid var(--narragansett)}
.b-green{background:rgba(163,179,168,0.15);color:var(--raindance);border:1px solid var(--raindance)}
.b-amber{background:rgba(184,154,118,0.2);color:var(--sherwoodtan);border:1px solid var(--sherwoodtan)}
.b-red{background:rgba(156,91,84,0.2);color:var(--southwestpottery);border:1px solid var(--southwestpottery)}
.b-grey{background:var(--bg3);color:var(--text3);border:1px solid var(--border)}
.empty{text-align:center;color:var(--text3);padding:2rem;font-size:13px}
hr{border:none;border-top:1px solid var(--border);margin:12px 0}

/* delivery product row — 6 cols + remove btn */
.del-prod-row{display:grid;grid-template-columns:1fr 90px 80px 130px 90px 130px auto;gap:8px;align-items:end;background:var(--bg3);border:1px solid var(--border);border-radius:8px;padding:10px 12px;margin-bottom:8px}
.price-incl-display{font-size:14px;font-weight:700;color:var(--raindance);padding:8px 0;min-height:36px}

/* delivery log */
.del-log-card{background:var(--bg2);border:1px solid var(--border);border-radius:10px;margin-bottom:.875rem;overflow:hidden}
.del-log-head{padding:12px 16px;background:var(--bg3);border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;cursor:pointer}
.del-log-body{padding:12px 16px;display:none}
.del-log-body.open{display:block}

/* storage */
.storage-row{display:grid;grid-template-columns:1fr 100px 90px 90px 150px;gap:0;align-items:center;border-bottom:1px solid var(--border);background:var(--bg2);transition:background .15s}
.storage-row:hover{background:var(--bg3)}
.storage-row:last-child{border-bottom:none}
.storage-row.priority{border-left:3px solid var(--sherwoodtan)}
.sr-cell{padding:9px 10px;font-size:13px}
.sr-move{display:flex;flex-direction:column;gap:1px}
.min-inp{width:72px;padding:5px 7px;font-size:12px;text-align:center;background:var(--bg3);border:1px solid var(--border2);border-radius:6px;color:var(--text)}
.qty-inp-storage{width:80px;padding:5px 7px;font-size:12px;text-align:center;background:var(--bg3);border:1px solid var(--border2);border-radius:6px;color:var(--text)}
.sr-cell-avail,.sr-cell-min{text-align:center}
.sr-control{display:inline-flex;align-items:center;gap:6px}
.sr-unit{font-size:11px;color:var(--text3)}
.m-lbl{display:none}
.table-scroll{overflow-x:auto;-webkit-overflow-scrolling:touch}

/* recipe */
.ing-row{display:grid;grid-template-columns:1fr 1fr 90px 90px auto;gap:8px;align-items:end;background:var(--bg3);border:1px solid var(--border);border-radius:8px;padding:10px 12px;margin-bottom:8px}
.recipe-card{background:var(--bg2);border:1px solid var(--border);border-radius:10px;margin-bottom:1rem;overflow:hidden}
.recipe-head{padding:13px 16px;background:var(--bg3);border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between}
.recipe-title{font-size:15px;font-weight:700}
.recipe-sub{font-size:12px;color:var(--text2);margin-top:2px}
.recipe-body{padding:12px 16px}.recipe-body.collapsed{display:none}.scale-bar.collapsed{display:none}
.scale-bar{display:flex;align-items:center;gap:10px;padding:11px 16px;background:rgba(63,79,83,0.25);border-top:1px solid var(--narragansett);flex-wrap:wrap}
.scale-bar label{color:var(--raindance);font-size:11px;font-weight:600;white-space:nowrap;margin:0;text-transform:none;letter-spacing:0}
.scale-inp{width:72px;background:var(--bg3);border-color:var(--narragansett);color:var(--raindance);font-weight:700;text-align:center;padding:6px 8px}
.qty-orig{color:var(--text2);font-size:12px}
.qty-arrow{color:var(--text3);margin:0 5px;font-size:11px}
.qty-new{color:var(--blue);font-weight:700}

/* today used */
.day-group{margin-bottom:1.5rem}
.day-header{font-size:13px;font-weight:700;color:var(--text2);padding:8px 12px;background:var(--bg3);border:1px solid var(--border);border-radius:8px 8px 0 0;display:flex;align-items:center;justify-content:space-between}
.day-entries{border:1px solid var(--border);border-top:none;border-radius:0 0 8px 8px;overflow:hidden}
.entry-row{padding:12px 14px;border-bottom:1px solid var(--border);background:var(--bg2);cursor:pointer;transition:background .15s;display:flex;align-items:center;justify-content:space-between;gap:10px}
.entry-row:last-child{border-bottom:none}
.entry-row:hover{background:var(--bg3)}
.entry-name{font-weight:600;font-size:14px}
.entry-meta{font-size:12px;color:var(--text2);margin-top:2px}
.entry-detail{background:var(--bg3);border-bottom:1px solid var(--border);padding:12px 16px;display:none}
.entry-detail.open{display:block}
.detail-ing-row{display:flex;justify-content:space-between;padding:5px 0;border-bottom:1px solid var(--border);font-size:13px}
.detail-ing-row:last-child{border-bottom:none}


/* inline edit row for products in suppliers */
.prod-edit-row{background:var(--blue-bg);border:1px solid var(--blue-border);border-radius:7px;padding:8px 10px;margin-bottom:6px;display:grid;grid-template-columns:1fr 100px auto auto;gap:8px;align-items:center}

/* price calculator */
.pc-card{background:var(--bg2);border:1px solid var(--border);border-radius:10px;margin-bottom:1rem;overflow:hidden}
.pc-head{padding:13px 16px;background:var(--bg3);border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between}
.pc-title{font-size:15px;font-weight:700}
.pc-body.collapsed{display:none}.pc-total-bar.collapsed{display:none}.pc-portions-bar.collapsed{display:none}.pc-body{padding:14px 16px}
.pc-ing-row{display:flex;align-items:center;justify-content:space-between;padding:7px 0;border-bottom:1px solid var(--border);font-size:13px}
.pc-ing-row:last-child{border-bottom:none}
.pc-ing-left{display:flex;align-items:center;gap:8px}
.pc-price-inp{width:90px;padding:5px 8px;font-size:13px;text-align:right;background:var(--bg3);border:1px solid var(--border2);border-radius:6px;color:var(--text)}
.pc-price-inp:focus{border-color:var(--blue);outline:none}
.pc-total-bar{display:flex;justify-content:space-between;align-items:center;padding:12px 16px;background:var(--bg3);border-top:1px solid var(--border);flex-wrap:wrap;gap:8px}
.pc-portions-bar{display:flex;align-items:center;gap:10px;padding:10px 16px;background:rgba(63,79,83,0.25);border-top:1px solid var(--narragansett);flex-wrap:wrap}
.pc-portions-bar label{color:var(--raindance);font-size:11px;font-weight:600;margin:0;text-transform:none;letter-spacing:0}
.pc-scale-inp{width:72px;padding:6px 8px;font-size:13px;text-align:center;background:var(--bg3);border:1px solid var(--narragansett);border-radius:6px;color:var(--raindance);font-weight:700}

/* expiration */
.exp-card{background:var(--bg2);border:1px solid var(--border);border-radius:10px;margin-bottom:.875rem;overflow:hidden;border-left:4px solid var(--border)}
.exp-card.exp-good{border-left-color:var(--raindance)}
.exp-card.exp-soon{border-left-color:var(--sherwoodtan)}
.exp-card.exp-expired{border-left-color:var(--southwestpottery)}
.exp-row{padding:13px 16px;display:flex;align-items:center;justify-content:space-between;gap:12px;flex-wrap:wrap}
.exp-name{font-weight:700;font-size:15px}
.exp-meta{font-size:12px;color:var(--text2);margin-top:3px}
.exp-status{display:inline-flex;align-items:center;gap:5px;padding:4px 11px;border-radius:99px;font-size:12px;font-weight:700}
.exp-status.exp-good{background:rgba(163,179,168,0.18);color:var(--raindance);border:1px solid var(--raindance)}
.exp-status.exp-soon{background:rgba(184,154,118,0.2);color:var(--sherwoodtan);border:1px solid var(--sherwoodtan)}
.exp-status.exp-expired{background:rgba(156,91,84,0.2);color:var(--southwestpottery);border:1px solid var(--southwestpottery)}
.exp-dates{display:flex;gap:16px;font-size:12px;color:var(--text2)}
.exp-dates strong{color:var(--text)}


/* ════════════════════════════════════════
   MOBILE RESPONSIVE
   ════════════════════════════════════════ */
@media (max-width: 720px) {
  body{padding:.6rem .6rem 2.5rem;font-size:13px}
  h1{font-size:16px}
  .card{padding:.8rem .85rem;border-radius:12px}
  .card-title{font-size:10px}

  /* bigger inputs to avoid iOS auto-zoom + easier tapping */
  input,select{font-size:16px;padding:9px 10px}
  .btn{padding:9px 13px;font-size:13px}
  label{font-size:10px}

  /* tabs: horizontal scroll instead of wrapping */
  .tabs{flex-wrap:nowrap;overflow-x:auto;-webkit-overflow-scrolling:touch;scrollbar-width:none;-ms-overflow-style:none;gap:2px}
  .tabs::-webkit-scrollbar{display:none}
  .tab{padding:9px 12px;font-size:12px;flex-shrink:0}

  /* generic grids -> single column */
  .g2,.g3,.g4{grid-template-columns:1fr;gap:10px}
  .g2 [style*="grid-column"],.g3 [style*="grid-column"],.g4 [style*="grid-column"]{grid-column:1}

  /* ── delivery product rows ── */
  .del-header-row{display:none}
  .del-prod-row{grid-template-columns:1fr 1fr;gap:8px 10px;padding:12px}
  .del-prod-row > div:nth-child(1){grid-column:1/3}  /* product */
  .del-prod-row > div:nth-child(6){grid-column:1/3}  /* price after tax */
  .del-prod-row > button{grid-column:1/3;justify-self:end;width:auto}
  .m-lbl{display:block;font-size:10px;color:var(--text3);font-weight:600;text-transform:uppercase;letter-spacing:.04em;margin-bottom:3px}

  /* ── recipe ingredient rows ── */
  .ing-row{grid-template-columns:1fr 1fr;gap:8px 10px;padding:12px}
  .ing-row > div:nth-child(1){grid-column:1/3}  /* supplier */
  .ing-row > div:nth-child(2){grid-column:1/3}  /* product */
  .ing-row > button{grid-column:1/3;justify-self:end;width:auto}

  /* ── storage rows ── */
  .storage-header-row{display:none}
  .storage-row{grid-template-columns:1fr;gap:6px 0;padding:10px 8px}
  .sr-cell{padding:4px 0}
  .sr-cell-name{grid-column:1;grid-row:1}
  .sr-cell-avail,.sr-cell-min,.sr-cell-status,.sr-cell-supplier{
    grid-column:1/3;display:flex;align-items:center;justify-content:space-between;
    padding:6px 0;border-top:1px solid var(--border)
  }
  .qty-inp-storage,.min-inp{width:90px}

  /* ── recipe / price calc card headers ── */
  .recipe-head,.pc-head,.del-log-head{flex-wrap:wrap;row-gap:8px}
  .recipe-title,.pc-title{font-size:14px}

  /* ── scale bar (recipes: portions + made/expires + buttons) ── */
  .scale-bar{flex-direction:column;align-items:stretch;gap:10px;padding:12px}
  .scale-bar .scale-inp{width:100%}
  .scale-bar > div[style*="margin-left:12px"]{margin-left:0!important;width:100%;flex-wrap:wrap;gap:8px 12px}
  .scale-bar > div[style*="margin-left:12px"] input[type=date]{flex:1;width:auto;min-width:130px}
  .scale-bar > div[style*="margin-left:auto"]{margin-left:0!important;width:100%;flex-wrap:wrap}
  .scale-bar > div[style*="margin-left:auto"] .btn{flex:1;min-width:110px}

  /* ── price calculator ── */
  .pc-col-header{display:none}
  .pc-ing-row{flex-direction:column;align-items:stretch;gap:8px;padding:10px 0}
  .pc-ing-left{flex-wrap:wrap;gap:6px;width:100%}
  .pc-ing-row > div[style*="flex-shrink:0"]{width:100%;justify-content:space-between}
  .pc-ing-row > div[style*="flex-shrink:0"] > div[style*="align-items:flex-end"]{align-items:flex-start}
  .pc-price-inp{width:120px}
  .pc-total-bar{flex-wrap:wrap;gap:12px}
  .pc-portions-bar{flex-wrap:wrap}

  /* ── delivery totals + log footer ── */
  #del-totals{padding:12px}
  .del-totals-footer{flex-wrap:wrap;gap:10px!important;justify-content:space-between!important}

  /* ── expiration ── */
  .exp-row{flex-wrap:wrap;gap:10px}
  .exp-dates{flex-wrap:wrap;gap:8px 14px}
  .exp-name{font-size:14px}

  /* ── metrics / misc grids ── */
  .del-prod-row .price-incl-display{padding:9px 10px;background:var(--bg4);border-radius:7px;text-align:center}
}


/* ── geometric icon shapes (replacing emoji) ── */
.ic{display:inline-flex;align-items:center;justify-content:center;flex-shrink:0}
.ic svg{display:block}
.ic-square{width:14px;height:14px;border:2px solid currentColor;border-radius:3px}
.ic-circle{width:14px;height:14px;border:2px solid currentColor;border-radius:50%}
.ic-triangle{width:0;height:0;border-left:7px solid transparent;border-right:7px solid transparent;border-bottom:12px solid currentColor}
.ic-diamond{width:11px;height:11px;border:2px solid currentColor;transform:rotate(45deg)}
.ic-dot{width:8px;height:8px;border-radius:50%;background:currentColor}


/* companies */
.company-card{background:var(--bg2);border:1px solid var(--border);border-radius:10px;padding:1rem 1.125rem;margin-bottom:.875rem}
.company-head{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:10px}
.company-name{font-size:15px;font-weight:700}
.company-detail-row{display:flex;gap:8px;align-items:flex-start;padding:5px 0;font-size:13px;color:var(--text2)}
.company-detail-row strong{color:var(--text);min-width:80px;flex-shrink:0;font-weight:600}
.company-empty-field{color:var(--text3);font-style:italic}
</style>
</head>
<body>

<div style="display:flex;align-items:center;gap:10px;margin-bottom:1.25rem">
  <span style="font-size:22px"><span class="ic"><svg width="22" height="22" viewBox="0 0 22 22"><rect x="2" y="2" width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" rx="3"/><line x1="2" y1="8" x2="20" y2="8" stroke="currentColor" stroke-width="2"/><line x1="8" y1="8" x2="8" y2="20" stroke="currentColor" stroke-width="2"/><circle cx="14" cy="14" r="1.6" fill="currentColor"/><circle cx="14" cy="17" r="1.6" fill="currentColor"/></svg></span></span>
  <h1 style="font-size:18px;font-weight:700;letter-spacing:.01em;color:var(--swisscoffee)">Kitchen Manager</h1>
</div>

<div class="tabs">
  <button class="tab active" onclick="go('suppliers',this)"><span class="ic"><svg width="14" height="14" viewBox="0 0 14 14"><rect x="1" y="1" width="12" height="12" fill="none" stroke="currentColor" stroke-width="1.6" rx="2"/><line x1="1" y1="5" x2="13" y2="5" stroke="currentColor" stroke-width="1.6"/></svg></span> Suppliers</button>
  <button class="tab" onclick="go('delivery',this)"><span class="ic"><svg width="14" height="14" viewBox="0 0 14 14"><rect x="1" y="3" width="8" height="7" fill="none" stroke="currentColor" stroke-width="1.6" rx="1"/><polygon points="9,5 13,5 13,8 9,8" fill="none" stroke="currentColor" stroke-width="1.6"/><circle cx="4" cy="11.5" r="1.3" fill="currentColor"/><circle cx="10.5" cy="11.5" r="1.3" fill="currentColor"/></svg></span> Delivery</button>
  <button class="tab" onclick="go('storage',this)"><span class="ic"><svg width="14" height="14" viewBox="0 0 14 14"><polygon points="7,1 13,4.5 13,9.5 7,13 1,9.5 1,4.5" fill="none" stroke="currentColor" stroke-width="1.6"/><line x1="1" y1="4.5" x2="7" y2="8" stroke="currentColor" stroke-width="1.6"/><line x1="13" y1="4.5" x2="7" y2="8" stroke="currentColor" stroke-width="1.6"/><line x1="7" y1="8" x2="7" y2="13" stroke="currentColor" stroke-width="1.6"/></svg></span> Storage</button>
  <button class="tab" onclick="go('recipes',this)"><span class="ic"><svg width="14" height="14" viewBox="0 0 14 14"><rect x="2" y="1" width="10" height="12" fill="none" stroke="currentColor" stroke-width="1.6" rx="1"/><line x1="4.5" y1="4.5" x2="9.5" y2="4.5" stroke="currentColor" stroke-width="1.4"/><line x1="4.5" y1="7" x2="9.5" y2="7" stroke="currentColor" stroke-width="1.4"/><line x1="4.5" y1="9.5" x2="8" y2="9.5" stroke="currentColor" stroke-width="1.4"/></svg></span> Recipes</button>
  <button class="tab" onclick="go('today',this)"><span class="ic"><svg width="14" height="14" viewBox="0 0 14 14"><rect x="1" y="2" width="12" height="11" fill="none" stroke="currentColor" stroke-width="1.6" rx="1.5"/><line x1="1" y1="5.5" x2="13" y2="5.5" stroke="currentColor" stroke-width="1.6"/><line x1="4" y1="1" x2="4" y2="3" stroke="currentColor" stroke-width="1.6"/><line x1="10" y1="1" x2="10" y2="3" stroke="currentColor" stroke-width="1.6"/></svg></span> Today Used</button>
  <button class="tab" onclick="go('price',this)"><span class="ic"><svg width="14" height="14" viewBox="0 0 14 14"><rect x="1" y="1" width="12" height="12" fill="none" stroke="currentColor" stroke-width="1.6" rx="2"/><line x1="4" y1="4.5" x2="10" y2="4.5" stroke="currentColor" stroke-width="1.4"/><line x1="4" y1="7" x2="10" y2="7" stroke="currentColor" stroke-width="1.4"/><line x1="4" y1="9.5" x2="7" y2="9.5" stroke="currentColor" stroke-width="1.4"/></svg></span> Price Calculator</button>
  <button class="tab" onclick="go('expiration',this)"><span class="ic"><svg width="14" height="14" viewBox="0 0 14 14"><circle cx="7" cy="7.5" r="5.5" fill="none" stroke="currentColor" stroke-width="1.6"/><line x1="7" y1="4.5" x2="7" y2="7.5" stroke="currentColor" stroke-width="1.6"/><line x1="7" y1="7.5" x2="9" y2="8.5" stroke="currentColor" stroke-width="1.6"/><line x1="5" y1="1" x2="9" y2="1" stroke="currentColor" stroke-width="1.6"/></svg></span> Expiration</button>
  <button class="tab" onclick="go('companies',this)"><span class="ic"><svg width="14" height="14" viewBox="0 0 14 14"><rect x="1" y="2" width="12" height="11" fill="none" stroke="currentColor" stroke-width="1.6" rx="1"/><line x1="4" y1="5" x2="10" y2="5" stroke="currentColor" stroke-width="1.4"/><line x1="4" y1="7.5" x2="10" y2="7.5" stroke="currentColor" stroke-width="1.4"/><line x1="4" y1="10" x2="7.5" y2="10" stroke="currentColor" stroke-width="1.4"/></svg></span> Companies</button>
</div>

<!-- SUPPLIERS -->
<div class="pane active" id="pane-suppliers">
  <div class="card">
    <div class="card-title">Add supplier</div>
    <div class="g3">
      <div style="grid-column:1/3">
        <label>Company name</label>
        <input id="s-name" list="company-names-list" placeholder="Type or pick a saved company">
        <datalist id="company-names-list"></datalist>
      </div>
      <div style="padding-bottom:1px"><button class="btn btn-blue" onclick="addSupplier()" style="width:100%"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="6" y1="1" x2="6" y2="11" stroke="currentColor" stroke-width="2"/><line x1="1" y1="6" x2="11" y2="6" stroke="currentColor" stroke-width="2"/></svg></span> Add supplier</button></div>
    </div>
    <div style="font-size:11px;color:var(--text3);margin-top:8px">Start typing to see saved companies, or add a new name. Manage full company details (phone, address, notes) in the Companies tab.</div>
  </div>
  <div id="suppliers-list"></div>
</div>

<!-- COMPANIES -->
<div class="pane" id="pane-companies">
  <div class="card" id="company-form-card">
    <div class="card-title" id="company-form-label">Add company</div>
    <div class="g2" style="margin-bottom:10px">
      <div><label>Company name</label><input id="c-name" placeholder="e.g. Metro Cash & Carry"></div>
      <div><label>Phone number</label><input id="c-phone" placeholder="e.g. +359 888 000 000"></div>
    </div>
    <div style="margin-bottom:10px"><label>Address</label><input id="c-address" placeholder="e.g. 12 Market St, Sofia"></div>
    <div style="margin-bottom:10px"><label>Email</label><input id="c-email" type="email" placeholder="e.g. orders@metro.com"></div>
    <div style="margin-bottom:10px"><label>Notes</label><input id="c-notes" placeholder="e.g. delivers Mon/Thu, contact Maria for orders"></div>
    <div style="display:flex;gap:8px;justify-content:flex-end">
      <button class="btn btn-sm" id="company-cancel-btn" style="display:none" onclick="cancelEditCompany()"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="2" y1="2" x2="10" y2="10" stroke="currentColor" stroke-width="1.8"/><line x1="10" y1="2" x2="2" y2="10" stroke="currentColor" stroke-width="1.8"/></svg></span> Cancel</button>
      <button class="btn btn-blue btn-sm" onclick="saveCompany()"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><rect x="1" y="1" width="10" height="10" fill="none" stroke="currentColor" stroke-width="1.4" rx="1"/><rect x="3" y="1" width="4" height="3" fill="currentColor"/><rect x="3" y="7" width="6" height="3" fill="none" stroke="currentColor" stroke-width="1.2"/></svg></span> Save company</button>
    </div>
  </div>
  <div id="companies-list"></div>
</div>

<!-- DELIVERY -->
<div class="pane" id="pane-delivery">
  <div class="card">
    <div class="card-title">New delivery</div>
    <div class="g4" style="margin-bottom:12px">
      <div>
        <label>Supplier</label>
        <select id="del-supplier" onchange="onDelSupplierChange()">
          <option value="">— select supplier —</option>
        </select>
      </div>
      <div><label>Delivery date</label><input type="date" id="del-date"></div>
      <div><label>Document / invoice no.</label><input id="del-docno" placeholder="e.g. INV-2024-001"></div>
      <div>
        <label>Default VAT %</label>
        <select id="del-vat-default" onchange="applyDefaultVat()">
          <option value="0">0%</option><option value="9">9%</option>
          <option value="20" selected>20%</option><option value="23">23%</option><option value="25">25%</option>
        </select>
      </div>
    </div>
    <div class="card-title" style="margin-bottom:6px">Products in this delivery</div>
    <!-- column headers -->
    <div class="del-header-row" style="display:grid;grid-template-columns:1fr 90px 80px 130px 90px 130px auto;gap:8px;padding:0 14px;margin-bottom:4px">
      <span style="font-size:10px;color:var(--text3);font-weight:600;text-transform:uppercase;letter-spacing:.04em">Product</span>
      <span style="font-size:10px;color:var(--text3);font-weight:600;text-transform:uppercase;letter-spacing:.04em">Qty</span>
      <span style="font-size:10px;color:var(--text3);font-weight:600;text-transform:uppercase;letter-spacing:.04em">Unit</span>
      <span style="font-size:10px;color:var(--text3);font-weight:600;text-transform:uppercase;letter-spacing:.04em">Price/unit (fixed)</span>
      <span style="font-size:10px;color:var(--text3);font-weight:600;text-transform:uppercase;letter-spacing:.04em">VAT %</span>
      <span style="font-size:10px;color:var(--text3);font-weight:600;text-transform:uppercase;letter-spacing:.04em">Price/unit after tax</span>
      <span></span>
    </div>
    <div id="del-prod-rows"></div>
    <button class="btn btn-sm" id="del-add-prod-btn" onclick="addDelProdRow()" style="margin-bottom:14px;display:none"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="6" y1="1" x2="6" y2="11" stroke="currentColor" stroke-width="2"/><line x1="1" y1="6" x2="11" y2="6" stroke="currentColor" stroke-width="2"/></svg></span> Add product</button>
    <div id="del-no-supplier" style="font-size:13px;color:var(--text3);margin-bottom:14px"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="10" y1="6" x2="2" y2="6" stroke="currentColor" stroke-width="1.8"/><path d="M5 2L2 6l3 4" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Select a supplier first.</div>
    <!-- totals -->
    <div id="del-totals" style="display:none;background:var(--bg3);border:1px solid var(--border);border-radius:8px;padding:12px 16px;margin-bottom:14px">
      <div style="display:flex;justify-content:space-between;font-size:13px;margin-bottom:6px">
        <span style="color:var(--text2)">Total before tax</span><span id="tot-excl" style="font-weight:600">€0.00</span>
      </div>
      <div style="display:flex;justify-content:space-between;font-size:13px;margin-bottom:6px">
        <span style="color:var(--text2)">Tax amount</span><span id="tot-tax" style="font-weight:600;color:var(--sherwoodtan)">€0.00</span>
      </div>
      <hr style="margin:8px 0">
      <div style="display:flex;justify-content:space-between;font-size:15px">
        <span style="font-weight:600">Total after tax</span><span id="tot-incl" style="font-weight:700;color:var(--raindance)">€0.00</span>
      </div>
    </div>
    <hr>
    <div style="display:flex;gap:8px;justify-content:flex-end">
      <button class="btn btn-sm" onclick="clearDeliveryForm()">Clear</button>
      <button class="btn btn-green btn-sm" id="save-del-btn" onclick="saveDelivery()"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Save delivery & update storage</button>
    </div>
  </div>
  <div class="card-title" style="margin-top:.25rem">Delivery history</div>
  <div id="delivery-log"></div>
</div>

<!-- STORAGE -->
<div class="pane" id="pane-storage">
  <div class="card" style="padding:0;overflow:hidden">
    <div class="storage-header-row" style="display:grid;grid-template-columns:1fr 100px 90px 90px 150px;gap:0;border-bottom:1px solid var(--border);padding:8px 10px;background:var(--bg3)">
      <div class="card-title" style="margin:0;font-size:10px">Product (tap star for priority)</div>
      <div class="card-title" style="margin:0;font-size:10px;text-align:center">Available</div>
      <div class="card-title" style="margin:0;font-size:10px;text-align:center">Min qty</div>
      <div class="card-title" style="margin:0;font-size:10px">Status</div>
      <div class="card-title" style="margin:0;font-size:10px">Supplier</div>
    </div>
    <div id="storage-list"></div>
  </div>
  <div style="font-size:12px;color:var(--text3);margin-top:4px"><span class="ic"><svg width="13" height="13" viewBox="0 0 14 14"><circle cx="7" cy="6" r="4" fill="none" stroke="currentColor" stroke-width="1.4"/><line x1="5.5" y1="11" x2="8.5" y2="11" stroke="currentColor" stroke-width="1.4"/><line x1="6" y1="12.5" x2="8" y2="12.5" stroke="currentColor" stroke-width="1.4"/></svg></span> Set Min qty thresholds. Deliveries update Available automatically. Use the arrows to reorder.</div>
</div>

<!-- RECIPES -->
<div class="pane" id="pane-recipes">
  <div class="card" id="recipe-form-card">
    <div class="card-title" id="recipe-form-label">New recipe</div>
    <div class="g2" style="margin-bottom:14px">
      <div><label>Recipe name</label><input id="r-name" placeholder="e.g. Lemon tart"></div>
      <div><label>Base portions</label><input type="number" id="r-portions" value="1" min="1" step="1"></div>
    </div>
    <div class="card-title" style="margin-bottom:8px">Ingredients</div>
    <div id="ing-rows"></div>
    <button class="btn btn-sm" onclick="addIngRow(null)" style="margin-bottom:14px"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="6" y1="1" x2="6" y2="11" stroke="currentColor" stroke-width="2"/><line x1="1" y1="6" x2="11" y2="6" stroke="currentColor" stroke-width="2"/></svg></span> Add ingredient</button>
    <hr>
    <div style="display:flex;gap:8px;justify-content:flex-end">
      <button class="btn btn-sm" id="recipe-cancel" style="display:none" onclick="cancelRecipe()">Cancel</button>
      <button class="btn btn-blue btn-sm" onclick="saveRecipe()"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><rect x="1" y="1" width="10" height="10" fill="none" stroke="currentColor" stroke-width="1.4" rx="1"/><rect x="3" y="1" width="4" height="3" fill="currentColor"/><rect x="3" y="7" width="6" height="3" fill="none" stroke="currentColor" stroke-width="1.2"/></svg></span> Save recipe</button>
    </div>
  </div>
  <div id="recipes-list"></div>
</div>

<!-- TODAY USED -->
<div class="pane" id="pane-today">
  <div class="card">
    <div style="display:flex;align-items:center;gap:12px;flex-wrap:wrap">
      <div style="flex:1;min-width:160px"><label>View date</label><input type="date" id="view-date" oninput="onDateChange()"></div>
      <div style="font-size:13px;color:var(--text2)" id="day-summary"></div>
    </div>
  </div>

  <div id="today-entries"></div>
</div>

<!-- PRICE CALCULATOR -->
<div class="pane" id="pane-price">
  <div id="price-calc-list"></div>
</div>

<!-- EXPIRATION -->
<div class="pane" id="pane-expiration">
  <div id="expiration-list"></div>
</div>

<script>
let suppliers  = [];
let recipes    = [];
let usedLog    = [];
let storage    = [];
let deliveries = [];
let expirationLog = [];
let companies  = [];
let editingRecipe   = -1;
let editingDelivery = -1; // index of delivery being edited
let editingCompany  = -1;
let rowIdx    = 0;
let delRowIdx = 0;

try { suppliers  = JSON.parse(localStorage.getItem('km_sup') || '[]'); } catch(e){}
try { recipes    = JSON.parse(localStorage.getItem('km_rec') || '[]'); } catch(e){}
try { usedLog    = JSON.parse(localStorage.getItem('km_log') || '[]'); } catch(e){}
try { storage    = JSON.parse(localStorage.getItem('km_sto') || '[]'); } catch(e){}
try { deliveries = JSON.parse(localStorage.getItem('km_del') || '[]'); } catch(e){}
try { expirationLog = JSON.parse(localStorage.getItem('km_exp') || '[]'); } catch(e){}
try { companies  = JSON.parse(localStorage.getItem('km_com') || '[]'); } catch(e){}

function persist() {
  localStorage.setItem('km_sup',  JSON.stringify(suppliers));
  localStorage.setItem('km_rec',  JSON.stringify(recipes));
  localStorage.setItem('km_log',  JSON.stringify(usedLog));
  localStorage.setItem('km_sto',  JSON.stringify(storage));
  localStorage.setItem('km_del',  JSON.stringify(deliveries));
  localStorage.setItem('km_exp',  JSON.stringify(expirationLog));
  localStorage.setItem('km_com',  JSON.stringify(companies));
}
function todayStr() { return new Date().toISOString().split('T')[0]; }
function fmtDate(d) { return new Date(d+'T00:00:00').toLocaleDateString('en-GB',{weekday:'short',day:'numeric',month:'short',year:'numeric'}); }
function fmtMoney(n) { return '€'+parseFloat(n||0).toFixed(2); }

/* ── sync storage from suppliers ── */
function syncStorage() {
  suppliers.forEach(s => s.products.forEach(p => {
    const key = s.name+'::'+p.name;
    if (!storage.find(x => x.key===key))
      storage.push({key, supName:s.name, prodName:p.name, unit:p.unit, qty:0, minQty:0, priority:false});
  }));
  // remove products no longer in any supplier
  storage = storage.filter(x => {
    const s = suppliers.find(s => s.name===x.supName);
    return s && s.products.find(p => p.name===x.prodName);
  });
  // sync unit changes
  storage.forEach(x => {
    const s = suppliers.find(s => s.name===x.supName);
    if (!s) return;
    const p = s.products.find(p => p.name===x.prodName);
    if (p) x.unit = p.unit;
  });
  persist();
}

/* ── status ── */
function getStatus(item) {
  if (item.minQty<=0) return 'grey';
  if (item.qty<=0 || item.qty<item.minQty) return 'red';
  if (item.qty<item.minQty*1.5) return 'amber';
  return 'green';
}
function statusBadge(item) {
  const map = {green:['b-green','<span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Good'],amber:['b-amber','<span class="ic"><svg width="11" height="11" viewBox="0 0 14 14"><path d="M7 1.5l6 10.5H1z" fill="none" stroke="currentColor" stroke-width="1.4" stroke-linejoin="round"/><line x1="7" y1="5.5" x2="7" y2="8.5" stroke="currentColor" stroke-width="1.4"/><circle cx="7" cy="10.5" r="0.6" fill="currentColor"/></svg></span> Medium'],red:['b-red','<span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="2" y1="2" x2="10" y2="10" stroke="currentColor" stroke-width="1.8"/><line x1="10" y1="2" x2="2" y2="10" stroke="currentColor" stroke-width="1.8"/></svg></span> Low'],grey:['b-grey','— No min']};
  const [cls,lbl] = map[getStatus(item)];
  return `<span class="badge ${cls}">${lbl}</span>`;
}
function getStorageItem(supName,prodName) { return storage.find(x=>x.supName===supName&&x.prodName===prodName)||null; }
// Convert a quantity from one unit to another (used whenever recipe units and storage units differ)
function convertUnits(qty, fromUnit, toUnit) {
  if (fromUnit === toUnit) return qty;
  if (fromUnit === 'g'  && toUnit === 'kg')  return qty / 1000;
  if (fromUnit === 'kg' && toUnit === 'g')   return qty * 1000;
  if (fromUnit === 'ml' && toUnit === 'L')   return qty / 1000;
  if (fromUnit === 'L'  && toUnit === 'ml')  return qty * 1000;
  // same scale — pass through unchanged (pcs, box, bag)
  return qty;
}
function availBadge(supName,prodName,needed,recipeUnit) {
  const item = getStorageItem(supName,prodName);
  if (!item) return '<span class="badge b-grey">—</span>';
  if (needed!==undefined) {
    // convert the needed qty from recipe unit to storage unit for comparison
    const neededInStorageUnit = recipeUnit ? convertUnits(needed, recipeUnit, item.unit) : needed;
    const avail = item.qty;
    const availDisplay = avail.toFixed(2) + ' ' + item.unit;
    if (avail<=0||avail<neededInStorageUnit) return `<span class="badge b-red"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="2" y1="2" x2="10" y2="10" stroke="currentColor" stroke-width="1.8"/><line x1="10" y1="2" x2="2" y2="10" stroke="currentColor" stroke-width="1.8"/></svg></span> Low (${availDisplay})</span>`;
    if (avail<neededInStorageUnit*1.5) return `<span class="badge b-amber"><span class="ic"><svg width="11" height="11" viewBox="0 0 14 14"><path d="M7 1.5l6 10.5H1z" fill="none" stroke="currentColor" stroke-width="1.4" stroke-linejoin="round"/><line x1="7" y1="5.5" x2="7" y2="8.5" stroke="currentColor" stroke-width="1.4"/><circle cx="7" cy="10.5" r="0.6" fill="currentColor"/></svg></span> Medium (${availDisplay})</span>`;
    return `<span class="badge b-green"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Good (${availDisplay})</span>`;
  }
  return statusBadge(item);
}

/* ── tabs ── */
function go(tab,btn) {
  document.querySelectorAll('.tab').forEach(b=>b.classList.remove('active'));
  document.querySelectorAll('.pane').forEach(p=>p.classList.remove('active'));
  btn.classList.add('active');
  document.getElementById('pane-'+tab).classList.add('active');
  ({suppliers:renderSuppliers,delivery:initDeliveryTab,storage:()=>{syncStorage();renderStorage();},recipes:renderRecipes,today:initTodayTab,price:renderPriceCalc,expiration:renderExpiration,companies:renderCompanies})[tab]?.();
}

/* ══ SUPPLIERS ══ */
function addSupplier() {
  const name = document.getElementById('s-name').value.trim();
  if (!name) { alert('Enter a company name.'); return; }
  if (suppliers.find(s=>s.name.toLowerCase()===name.toLowerCase())) { alert('Already exists.'); return; }
  suppliers.push({name,products:[]});
  // auto-create a bare company record if this name doesn't exist yet in Companies
  if (!companies.find(c=>c.name.toLowerCase()===name.toLowerCase())) {
    companies.push({name, phone:'', address:'', email:'', notes:''});
  }
  persist();
  document.getElementById('s-name').value='';
  renderSuppliers();
}
function deleteSupplier(i) {
  if (!confirm('Delete "'+suppliers[i].name+'"?')) return;
  suppliers.splice(i,1); syncStorage(); renderSuppliers();
}
function addProduct(si) {
  const nameEl=document.getElementById('pname-'+si), unitEl=document.getElementById('punit-'+si);
  const name=nameEl.value.trim(), unit=unitEl.value;
  if (!name||!unit) { alert('Enter product name and unit.'); return; }
  if (suppliers[si].products.find(p=>p.name.toLowerCase()===name.toLowerCase())) { alert('Already exists.'); return; }
  suppliers[si].products.push({name,unit});
  syncStorage(); nameEl.value=''; unitEl.value='';
  renderSuppliers();
}
function deleteProduct(si,pi) {
  suppliers[si].products.splice(pi,1); syncStorage(); renderSuppliers();
}

/* ══ COMPANIES ══ */
function saveCompany() {
  const name    = document.getElementById('c-name').value.trim();
  const phone   = document.getElementById('c-phone').value.trim();
  const address = document.getElementById('c-address').value.trim();
  const email   = document.getElementById('c-email').value.trim();
  const notes   = document.getElementById('c-notes').value.trim();
  if (!name) { alert('Enter a company name.'); return; }

  if (editingCompany >= 0) {
    const oldName = companies[editingCompany].name;
    companies[editingCompany] = { name, phone, address, email, notes };
    // keep linked supplier name in sync if it changed
    if (oldName !== name) {
      const sup = suppliers.find(s => s.name === oldName);
      if (sup) sup.name = name;
      deliveries.forEach(d => { if (d.supName === oldName) d.supName = name; });
      storage.forEach(s => { if (s.supName === oldName) s.supName = name; });
      recipes.forEach(r => r.ingredients.forEach(ing => { if (ing.supplier === oldName) ing.supplier = name; }));
    }
    editingCompany = -1;
  } else {
    if (companies.find(c => c.name.toLowerCase() === name.toLowerCase())) { alert('A company with this name already exists.'); return; }
    companies.push({ name, phone, address, email, notes });
  }
  persist();
  cancelEditCompany();
  renderCompanies();
  renderCompanyDatalist();
}
function cancelEditCompany() {
  editingCompany = -1;
  document.getElementById('c-name').value = '';
  document.getElementById('c-phone').value = '';
  document.getElementById('c-address').value = '';
  document.getElementById('c-email').value = '';
  document.getElementById('c-notes').value = '';
  document.getElementById('company-form-label').textContent = 'Add company';
  document.getElementById('company-cancel-btn').style.display = 'none';
}
function editCompany(i) {
  const c = companies[i];
  editingCompany = i;
  document.getElementById('c-name').value = c.name;
  document.getElementById('c-phone').value = c.phone || '';
  document.getElementById('c-address').value = c.address || '';
  document.getElementById('c-email').value = c.email || '';
  document.getElementById('c-notes').value = c.notes || '';
  document.getElementById('company-form-label').innerHTML = '<span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M8.5 1.5l2 2L4 10l-2.5.5L2 8z" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/></svg></span> Editing: ' + c.name;
  document.getElementById('company-cancel-btn').style.display = '';
  document.getElementById('company-form-card').scrollIntoView({ behavior:'smooth', block:'start' });
}
function deleteCompany(i) {
  const c = companies[i];
  const linkedSupplier = suppliers.find(s => s.name === c.name);
  const msg = linkedSupplier
    ? `"${c.name}" is also an active supplier. Delete the company record only? (supplier + its products stay untouched)`
    : `Delete company "${c.name}"?`;
  if (!confirm(msg)) return;
  if (editingCompany === i) cancelEditCompany();
  companies.splice(i,1);
  persist();
  renderCompanies();
  renderCompanyDatalist();
}
function renderCompanies() {
  const list = document.getElementById('companies-list');
  if (!companies.length) { list.innerHTML = '<div class="empty">No companies yet. Add one above.</div>'; return; }
  list.innerHTML = companies.map((c,i) => {
    const isSupplier = suppliers.some(s => s.name === c.name);
    return `
    <div class="company-card">
      <div class="company-head">
        <div class="company-name">
          <span class="ic"><svg width="13" height="13" viewBox="0 0 14 14"><rect x="1" y="1" width="12" height="12" fill="none" stroke="currentColor" stroke-width="1.6" rx="2"/><line x1="1" y1="5" x2="13" y2="5" stroke="currentColor" stroke-width="1.6"/></svg></span>
          ${c.name}
          ${isSupplier ? '<span class="badge b-green" style="margin-left:8px">Active supplier</span>' : ''}
        </div>
        <div style="display:flex;gap:4px">
          <button class="icon-btn edit" onclick="editCompany(${i})" title="Edit"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M8.5 1.5l2 2L4 10l-2.5.5L2 8z" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/></svg></span></button>
          <button class="icon-btn del" onclick="deleteCompany(${i})" title="Delete"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 3h8M4.5 3V2a1 1 0 0 1 1-1h1a1 1 0 0 1 1 1v1M3 3l.5 8a1 1 0 0 0 1 .9h3a1 1 0 0 0 1-.9L9 3" fill="none" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg></span></button>
        </div>
      </div>
      <div class="company-detail-row"><strong>Phone</strong> ${c.phone ? c.phone : '<span class="company-empty-field">not set</span>'}</div>
      <div class="company-detail-row"><strong>Address</strong> ${c.address ? c.address : '<span class="company-empty-field">not set</span>'}</div>
      <div class="company-detail-row"><strong>Email</strong> ${c.email ? c.email : '<span class="company-empty-field">not set</span>'}</div>
      <div class="company-detail-row"><strong>Notes</strong> ${c.notes ? c.notes : '<span class="company-empty-field">not set</span>'}</div>
    </div>`;
  }).join('');
}

/* inline edit product */
function startEditProduct(si,pi) {
  const p = suppliers[si].products[pi];
  const rowId = `pedit-${si}-${pi}`;
  // replace the table row with an inline edit row
  const tr = document.getElementById(`ptr-${si}-${pi}`);
  if (!tr) return;
  const editDiv = document.createElement('tr');
  editDiv.id = rowId;
  editDiv.innerHTML = `
    <td colspan="3" style="padding:6px 8px">
      <div class="prod-edit-row">
        <input id="pe-name-${si}-${pi}" value="${p.name}" placeholder="Product name">
        <select id="pe-unit-${si}-${pi}">
          <option value="kg"${p.unit==='kg'?' selected':''}>kg</option>
          <option value="g"${p.unit==='g'?' selected':''}>g</option>
          <option value="L"${p.unit==='L'?' selected':''}>L</option>
          <option value="ml"${p.unit==='ml'?' selected':''}>ml</option>
          <option value="pcs"${p.unit==='pcs'?' selected':''}>pcs</option>
          <option value="box"${p.unit==='box'?' selected':''}>box</option>
          <option value="bag"${p.unit==='bag'?' selected':''}>bag</option>
        </select>
        <button class="btn btn-blue btn-sm" onclick="saveEditProduct(${si},${pi})"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Save</button>
        <button class="btn btn-sm" onclick="cancelEditProduct(${si},${pi})"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="2" y1="2" x2="10" y2="10" stroke="currentColor" stroke-width="1.8"/><line x1="10" y1="2" x2="2" y2="10" stroke="currentColor" stroke-width="1.8"/></svg></span></button>
      </div>
    </td>`;
  tr.replaceWith(editDiv);
}
function saveEditProduct(si,pi) {
  const newName = document.getElementById(`pe-name-${si}-${pi}`).value.trim();
  const newUnit = document.getElementById(`pe-unit-${si}-${pi}`).value;
  if (!newName||!newUnit) { alert('Fill both fields.'); return; }
  const oldName = suppliers[si].products[pi].name;
  const oldUnit = suppliers[si].products[pi].unit;
  suppliers[si].products[pi].name = newName;
  suppliers[si].products[pi].unit = newUnit;
  // update storage key + unit
  const oldKey = suppliers[si].name+'::'+oldName;
  const newKey = suppliers[si].name+'::'+newName;
  const stItem = storage.find(x=>x.key===oldKey);
  if (stItem) { stItem.key=newKey; stItem.prodName=newName; stItem.unit=newUnit; }
  // update deliveries unit references
  deliveries.forEach(d => {
    if (d.supName===suppliers[si].name) {
      d.items.forEach(it => { if (it.product===oldName) { it.product=newName; it.unit=newUnit; } });
    }
  });
  // update recipes ingredient references
  recipes.forEach(r => r.ingredients.forEach(ing => {
    if (ing.supplier===suppliers[si].name && ing.product===oldName) {
      ing.product=newName; ing.unit=newUnit;
    }
  }));
  // update usedLog
  usedLog.forEach(u => u.ingredients?.forEach(ing => {
    if (ing.supplier===suppliers[si].name && ing.product===oldName) { ing.product=newName; ing.unit=newUnit; }
  }));
  persist(); renderSuppliers();
}
function cancelEditProduct(si,pi) { renderSuppliers(); }

function renderCompanyDatalist() {
  const dl = document.getElementById('company-names-list');
  if (!dl) return;
  dl.innerHTML = companies.map(c => `<option value="${c.name}"></option>`).join('');
}
function renderSuppliers() {
  renderCompanyDatalist();
  const c = document.getElementById('suppliers-list');
  if (!suppliers.length) { c.innerHTML='<div class="empty">No suppliers yet.</div>'; return; }
  c.innerHTML = suppliers.map((s,si)=>`
    <div class="card">
      <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:12px">
        <div style="font-size:15px;font-weight:700;display:flex;align-items:center;gap:8px">
          <span class="ic"><svg width="11" height="11" viewBox="0 0 14 14"><rect x="1" y="1" width="12" height="12" fill="none" stroke="currentColor" stroke-width="1.6" rx="2"/><line x1="1" y1="5" x2="13" y2="5" stroke="currentColor" stroke-width="1.6"/></svg></span> ${s.name}
          <span class="badge b-blue">${s.products.length} product${s.products.length!==1?'s':''}</span>
        </div>
        <button class="icon-btn del" onclick="deleteSupplier(${si})"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 3h8M4.5 3V2a1 1 0 0 1 1-1h1a1 1 0 0 1 1 1v1M3 3l.5 8a1 1 0 0 0 1 .9h3a1 1 0 0 0 1-.9L9 3" fill="none" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg></span></button>
      </div>
      ${s.products.length?`
        <div class="table-scroll"><table style="margin-bottom:12px">
          <thead><tr><th>Product</th><th>Unit</th><th style="text-align:right">Actions</th></tr></thead>
          <tbody>
            ${s.products.map((p,pi)=>`
              <tr id="ptr-${si}-${pi}">
                <td style="font-weight:600">${p.name}</td>
                <td><span class="badge b-amber">${p.unit}</span></td>
                <td style="text-align:right;display:flex;gap:4px;justify-content:flex-end">
                  <button class="icon-btn edit" onclick="startEditProduct(${si},${pi})" title="Edit"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M8.5 1.5l2 2L4 10l-2.5.5L2 8z" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/></svg></span></button>
                  <button class="icon-btn del"  onclick="deleteProduct(${si},${pi})"    title="Delete"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="2" y1="2" x2="10" y2="10" stroke="currentColor" stroke-width="1.8"/><line x1="10" y1="2" x2="2" y2="10" stroke="currentColor" stroke-width="1.8"/></svg></span></button>
                </td>
              </tr>`).join('')}
          </tbody>
        </table></div>`:
        '<div style="font-size:12px;color:var(--text3);margin-bottom:12px">No products yet.</div>'}
      <div class="g4">
        <div style="grid-column:1/3"><label>Product name</label><input id="pname-${si}" placeholder="e.g. Sugar"></div>
        <div><label>Unit</label>
          <select id="punit-${si}">
            <option value="">— unit —</option>
            <option>kg</option><option>g</option><option>L</option><option>ml</option>
            <option>pcs</option><option>box</option><option>bag</option>
          </select>
        </div>
        <div style="padding-bottom:1px"><button class="btn btn-blue btn-sm" onclick="addProduct(${si})" style="width:100%"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="6" y1="1" x2="6" y2="11" stroke="currentColor" stroke-width="2"/><line x1="1" y1="6" x2="11" y2="6" stroke="currentColor" stroke-width="2"/></svg></span> Add</button></div>
      </div>
    </div>`).join('');
}

/* ══ DELIVERY ══ */
function initDeliveryTab() {
  const sel = document.getElementById('del-supplier');
  const cur = sel.value;
  sel.innerHTML='<option value="">— select supplier —</option>'+
    suppliers.map(s=>`<option value="${s.name}"${s.name===cur?' selected':''}>${s.name}</option>`).join('');
  if (!document.getElementById('del-date').value) document.getElementById('del-date').value=todayStr();
  const hasSup = sel.value!=='';
  document.getElementById('del-add-prod-btn').style.display = hasSup?'':'none';
  document.getElementById('del-no-supplier').style.display  = hasSup?'none':'';
  updateDeliveryTotals();
  renderDeliveryLog();
}

function onDelSupplierChange() {
  const supName = document.getElementById('del-supplier').value;
  document.getElementById('del-prod-rows').innerHTML='';
  delRowIdx=0;
  const hasSup = supName!=='';
  document.getElementById('del-add-prod-btn').style.display = hasSup?'':'none';
  document.getElementById('del-no-supplier').style.display  = hasSup?'none':'';
  document.getElementById('del-totals').style.display='none';
  if (hasSup) addDelProdRow();
}

function applyDefaultVat() {
  const vat=document.getElementById('del-vat-default').value;
  document.querySelectorAll('.dpr-vat').forEach(sel=>{sel.value=vat;calcDelRow(sel);});
}

function addDelProdRow(prefill) {
  const supName = document.getElementById('del-supplier').value;
  const s = suppliers.find(x=>x.name===supName);
  if (!s) return;
  const defaultVat = document.getElementById('del-vat-default').value;
  const id = 'dpr-'+(delRowIdx++);
  const div = document.createElement('div');
  div.className='del-prod-row'; div.id=id;
  const selProd = prefill?prefill.product:'';
  const prodOpts = s.products.map(p=>`<option value="${p.name}" data-unit="${p.unit}"${p.name===selProd?' selected':''}>${p.name}</option>`).join('');
  const firstUnit = prefill ? prefill.unit : (s.products[0]?s.products[0].unit:'');
  const qty       = prefill ? prefill.qty : '';
  const priceFixed = prefill && prefill.priceFixed!=null ? prefill.priceFixed : (prefill && prefill.priceExcl!=null ? prefill.priceExcl : '');
  const vat        = prefill ? prefill.vat : defaultVat;
  const priceAfter = (priceFixed!=='' && parseFloat(priceFixed)>0) ? '€'+(parseFloat(priceFixed)*(1+parseFloat(vat)/100)).toFixed(3) : '—';
  div.innerHTML=`
    <div><label class="m-lbl">Product</label><select class="dpr-prod" onchange="onDelProdChange('${id}',this)">${prodOpts}</select></div>
    <div><label class="m-lbl">Quantity</label><input type="number" class="dpr-qty" value="${qty}" placeholder="10" min="0.001" step="0.001" oninput="updateDeliveryTotals()"></div>
    <div><label class="m-lbl">Unit</label><input type="text" class="dpr-unit" value="${firstUnit}" style="text-align:center;background:var(--bg4);color:var(--text2)" readonly></div>
    <div><label class="m-lbl">Price (€)</label><input type="number" class="dpr-price-fixed" value="${priceFixed}" placeholder="0.000" min="0" step="0.001" oninput="calcDelRow(this)"></div>
    <div>
      <label class="m-lbl">VAT %</label>
      <select class="dpr-vat" onchange="calcDelRow(this)">
        <option value="0"${vat==='0'||vat===0?' selected':''}>0%</option>
        <option value="9"${vat==='9'||vat===9?' selected':''}>9%</option>
        <option value="20"${vat==='20'||vat===20?' selected':''}>20%</option>
        <option value="23"${vat==='23'||vat===23?' selected':''}>23%</option>
        <option value="25"${vat==='25'||vat===25?' selected':''}>25%</option>
      </select>
    </div>
    <div><label class="m-lbl">Price after tax</label><div class="price-incl-display dpr-price-after">${priceAfter}</div></div>
    <button class="icon-btn del" onclick="removeDelRow('${id}')" style="margin-bottom:1px"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="2" y1="2" x2="10" y2="10" stroke="currentColor" stroke-width="1.8"/><line x1="10" y1="2" x2="2" y2="10" stroke="currentColor" stroke-width="1.8"/></svg></span> Remove</button>`;
  document.getElementById('del-prod-rows').appendChild(div);
  updateDeliveryTotals();
}

function onDelProdChange(id,sel) {
  const row=document.getElementById(id);
  const opt=sel.options[sel.selectedIndex];
  row.querySelector('.dpr-unit').value=opt.dataset.unit||'';
  calcDelRow(sel);
}

function calcDelRow(el) {
  const row=el.closest('.del-prod-row');
  const price=parseFloat(row.querySelector('.dpr-price-fixed').value)||0;
  const vat  =parseFloat(row.querySelector('.dpr-vat').value)||0;
  const after=price>0?price*(1+vat/100):0;
  row.querySelector('.dpr-price-after').textContent=after>0?'€'+after.toFixed(3):'—';
  updateDeliveryTotals();
}

function removeDelRow(id) { document.getElementById(id)?.remove(); updateDeliveryTotals(); }

function updateDeliveryTotals() {
  let totalBefore=0,totalAfter=0;
  document.querySelectorAll('.del-prod-row').forEach(row=>{
    const price = parseFloat(row.querySelector('.dpr-price-fixed')?.value)||0;
    const vat   = parseFloat(row.querySelector('.dpr-vat')?.value)||0;
    totalBefore += price;
    totalAfter  += price*(1+vat/100);
  });
  const totEl=document.getElementById('del-totals');
  if (totalBefore>0||totalAfter>0) {
    totEl.style.display='';
    document.getElementById('tot-excl').textContent=fmtMoney(totalBefore);
    document.getElementById('tot-tax').textContent =fmtMoney(totalAfter-totalBefore);
    document.getElementById('tot-incl').textContent=fmtMoney(totalAfter);
  } else { totEl.style.display='none'; }
}

function collectDeliveryRows() {
  const items=[]; let valid=true;
  document.querySelectorAll('.del-prod-row').forEach(row=>{
    const product    = row.querySelector('.dpr-prod').value;
    const qty        = parseFloat(row.querySelector('.dpr-qty').value);
    const unit       = row.querySelector('.dpr-unit').value;
    const priceFixed = parseFloat(row.querySelector('.dpr-price-fixed').value);
    const vat        = parseFloat(row.querySelector('.dpr-vat').value)||0;
    const priceAfter = !isNaN(priceFixed)&&priceFixed>0 ? parseFloat((priceFixed*(1+vat/100)).toFixed(4)) : null;
    if (!product||isNaN(qty)||qty<=0) { valid=false; return; }
    // priceFixed = total price as entered, not multiplied by qty
    items.push({product,qty,unit,priceFixed:isNaN(priceFixed)?null:priceFixed,vat,priceAfter});
  });
  return {items,valid};
}

function saveDelivery() {
  const supName = document.getElementById('del-supplier').value;
  const date    = document.getElementById('del-date').value;
  const docNo   = document.getElementById('del-docno').value.trim();
  if (!supName) { alert('Select a supplier.'); return; }
  if (!date)    { alert('Select a date.'); return; }
  const rows = document.querySelectorAll('.del-prod-row');
  if (!rows.length) { alert('Add at least one product.'); return; }
  const {items,valid} = collectDeliveryRows();
  if (!valid) { alert('Check all rows — product and quantity are required.'); return; }
  let totalExcl=0,totalIncl=0;
  items.forEach(it=>{ if(it.priceFixed){totalExcl+=it.priceFixed;totalIncl+=(it.priceAfter||it.priceFixed);} });

  if (editingDelivery>=0) {
    // reverse old storage changes
    const old = deliveries[editingDelivery];
    old.items.forEach(it=>{
      const item=getStorageItem(old.supName,it.product);
      if (item) item.qty=Math.max(0,parseFloat((item.qty-it.qty).toFixed(4)));
    });
    deliveries[editingDelivery]={id:old.id,supName,date,docNo,items,totalExcl,totalIncl};
    editingDelivery=-1;
    document.getElementById('save-del-btn').innerHTML='<span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Save delivery & update storage';
  } else {
    deliveries.unshift({id:Date.now(),supName,date,docNo,items,totalExcl,totalIncl});
  }
  // apply new storage changes
  items.forEach(it=>{
    const item=getStorageItem(supName,it.product);
    if (!item) return;
    item.qty=parseFloat((item.qty+it.qty).toFixed(4));
    if (it.priceAfter) item.lastPriceIncl=it.priceAfter;
  });
  persist(); clearDeliveryForm(); renderDeliveryLog();
  const btn=document.getElementById('save-del-btn');
  const orig=btn.innerHTML;
  btn.innerHTML='<span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Saved!'; btn.disabled=true;
  setTimeout(()=>{btn.innerHTML=orig;btn.disabled=false;},2000);
}

function editDelivery(i) {
  const d=deliveries[i];
  editingDelivery=i;
  // populate header fields
  const sel=document.getElementById('del-supplier');
  sel.innerHTML='<option value="">— select supplier —</option>'+
    suppliers.map(s=>`<option value="${s.name}"${s.name===d.supName?' selected':''}>${s.name}</option>`).join('');
  document.getElementById('del-date').value=d.date;
  document.getElementById('del-docno').value=d.docNo||'';
  // clear and repopulate product rows
  document.getElementById('del-prod-rows').innerHTML='';
  delRowIdx=0;
  document.getElementById('del-add-prod-btn').style.display='';
  document.getElementById('del-no-supplier').style.display='none';
  d.items.forEach(it=>addDelProdRow(it));
  updateDeliveryTotals();
  document.getElementById('save-del-btn').innerHTML='<span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Update delivery';
  // scroll to form
  document.querySelector('#pane-delivery .card').scrollIntoView({behavior:'smooth',block:'start'});
}

function deleteDelivery(i) {
  if (!confirm('Delete this delivery? Storage quantities will NOT be reversed automatically.')) return;
  if (editingDelivery===i) { clearDeliveryForm(); editingDelivery=-1; }
  deliveries.splice(i,1); persist(); renderDeliveryLog();
}

function clearDeliveryForm() {
  editingDelivery=-1;
  document.getElementById('del-supplier').value='';
  document.getElementById('del-date').value=todayStr();
  document.getElementById('del-docno').value='';
  document.getElementById('del-prod-rows').innerHTML='';
  document.getElementById('del-totals').style.display='none';
  document.getElementById('del-add-prod-btn').style.display='none';
  document.getElementById('del-no-supplier').style.display='';
  document.getElementById('save-del-btn').innerHTML='<span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Save delivery & update storage';
}

function toggleDelLog(id) {
  const body=document.getElementById('dlb-'+id),chev=document.getElementById('dlc-'+id);
  if (!body) return;
  const open=body.classList.toggle('open');
  if (chev) chev.style.transform=open?'rotate(90deg)':'';
}

function renderDeliveryLog() {
  const container=document.getElementById('delivery-log');
  if (!deliveries.length){container.innerHTML='<div class="empty">No deliveries yet.</div>';return;}
  container.innerHTML=deliveries.map((d,i)=>`
    <div class="del-log-card">
      <div class="del-log-head" onclick="toggleDelLog(${d.id})">
        <div style="display:flex;align-items:center;gap:10px;flex-wrap:wrap">
          <span style="font-weight:700;font-size:14px"><span class="ic"><svg width="11" height="11" viewBox="0 0 14 14"><rect x="1" y="1" width="12" height="12" fill="none" stroke="currentColor" stroke-width="1.6" rx="2"/><line x1="1" y1="5" x2="13" y2="5" stroke="currentColor" stroke-width="1.6"/></svg></span> ${d.supName}</span>
          <span class="badge b-blue">${fmtDate(d.date)}</span>
          ${d.docNo?`<span class="badge b-grey"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><path d="M2 1h5l3 3v7H2z" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/><path d="M7 1v3h3" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/></svg></span> ${d.docNo}</span>`:''}
          <span class="badge b-green" style="color:var(--raindance)">Total: ${fmtMoney(d.totalIncl)}</span>
          <span style="font-size:12px;color:var(--text3)">${d.items.length} product${d.items.length!==1?'s':''}</span>
        </div>
        <div style="display:flex;align-items:center;gap:6px">
          <button class="icon-btn edit" onclick="event.stopPropagation();editDelivery(${i})" title="Edit"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M8.5 1.5l2 2L4 10l-2.5.5L2 8z" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/></svg></span></button>
          <button class="icon-btn del"  onclick="event.stopPropagation();deleteDelivery(${i})" title="Delete"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 3h8M4.5 3V2a1 1 0 0 1 1-1h1a1 1 0 0 1 1 1v1M3 3l.5 8a1 1 0 0 0 1 .9h3a1 1 0 0 0 1-.9L9 3" fill="none" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg></span></button>
          <span style="color:var(--text3);transition:transform .2s;display:inline-flex" id="dlc-${d.id}"><span class="ic"><svg width="10" height="10" viewBox="0 0 10 10"><polygon points="2,1 8,5 2,9" fill="currentColor"/></svg></span></span>
        </div>
      </div>
      <div class="del-log-body" id="dlb-${d.id}">
        <div class="table-scroll"><table>
          <thead><tr><th>Product</th><th>Qty</th><th>Unit</th><th>Price/unit</th><th>VAT</th><th>Price/unit after tax</th><th>Price after tax</th></tr></thead>
          <tbody>
            ${d.items.map(it=>`
              <tr>
                <td style="font-weight:600">${it.product}</td>
                <td>${it.qty}</td>
                <td><span class="badge b-amber" style="font-size:11px">${it.unit}</span></td>
                <td style="color:var(--text2)">${(it.priceFixed??it.priceExcl)!=null?fmtMoney(it.priceFixed??it.priceExcl):'—'}</td>
                <td><span class="badge b-grey">${it.vat}%</span></td>
                <td style="color:var(--green);font-weight:600">${(it.priceAfter??it.priceIncl)!=null?'€'+(it.priceAfter??it.priceIncl).toFixed(3):'—'}</td>
                <td style="font-weight:600">${(it.priceAfter??it.priceIncl)!=null?fmtMoney(it.priceAfter??it.priceIncl):'—'}</td>
              </tr>`).join('')}
          </tbody>
        </table></div>
        <div class="del-totals-footer" style="display:flex;justify-content:flex-end;gap:24px;margin-top:12px;padding-top:12px;border-top:1px solid var(--border);font-size:13px">
          <span style="color:var(--text2)">Before tax: <strong>${fmtMoney(d.totalExcl)}</strong></span>
          <span style="color:var(--text2)">Tax: <strong style="color:var(--amber)">${fmtMoney(d.totalIncl-d.totalExcl)}</strong></span>
          <span style="color:var(--text2)">After tax: <strong style="color:var(--green);font-size:15px">${fmtMoney(d.totalIncl)}</strong></span>
        </div>
      </div>
    </div>`).join('');
}

/* ══ STORAGE ══ */
function togglePriority(idx){storage[idx].priority=!storage[idx].priority;persist();renderStorage();}

// Live-update just the qty/min value in memory (no persist, no re-render) so typing stays smooth.
function updateStorageQtyLive(idx,val){ storage[idx].qty = parseFloat(val) || 0; refreshStorageRowStatus(idx); }
function updateStorageMinLive(idx,val){ storage[idx].minQty = parseFloat(val) || 0; refreshStorageRowStatus(idx); }

// Update only this row's status badge + row priority class in place, without touching the input the user is typing in.
function refreshStorageRowStatus(idx){
  const item = storage[idx];
  const badgeEl = document.querySelector(`.sr-status-badge[data-idx="${idx}"]`);
  if (badgeEl) badgeEl.innerHTML = statusBadge(item);
}

// Persist + full re-sort/re-render only happens once the user leaves the field.
function commitStorageChange(){ persist(); renderStorage(); }

function renderStorage(){
  const list=document.getElementById('storage-list');
  if(!storage.length){list.innerHTML='<div class="empty">No products yet — add them in Suppliers.</div>';return;}

  // Auto-sort: lowest stock first (red), then medium (amber), then no-min-set (grey), then good (green) last.
  // Within each status group, priority items come first, and original relative order is preserved otherwise.
  const order = { red: 0, amber: 1, grey: 2, green: 3 };
  const indexed = storage.map((item, originalIdx) => ({ item, originalIdx, status: getStatus(item) }));
  indexed.sort((a, b) => {
    if (order[a.status] !== order[b.status]) return order[a.status] - order[b.status];
    if (a.item.priority !== b.item.priority) return a.item.priority ? -1 : 1;
    return a.originalIdx - b.originalIdx;
  });

  list.innerHTML=indexed.map(({item, originalIdx: i})=>`
    <div class="${item.priority?'storage-row priority':'storage-row'}">
      <div class="sr-cell sr-cell-name" style="display:flex;align-items:center;gap:8px">
        <button class="icon-btn" onclick="togglePriority(${i})" style="font-size:18px;padding:0 2px" title="Mark as priority">
          ${item.priority?'<span class="ic" style="color:var(--sherwoodtan)"><svg width="13" height="13" viewBox="0 0 14 14"><polygon points="7,1 13,7 7,13 1,7" fill="currentColor"/></svg></span>':'<span class="ic" style="color:var(--text3)"><svg width="13" height="13" viewBox="0 0 14 14"><polygon points="7,1 13,7 7,13 1,7" fill="none" stroke="currentColor" stroke-width="1.4"/></svg></span>'}
        </button>
        <div>
          <div style="font-weight:600">${item.prodName}</div>
          <div style="font-size:11px;color:var(--text3)">${item.supName}</div>
        </div>
      </div>
      <div class="sr-cell sr-cell-avail">
        <span class="m-lbl">Available</span>
        <span class="sr-control">
          <input type="number" class="qty-inp-storage" value="${item.qty}" min="0" step="0.01"
            oninput="updateStorageQtyLive(${i},this.value)" onblur="commitStorageChange()">
          <span class="sr-unit">${item.unit}</span>
        </span>
      </div>
      <div class="sr-cell sr-cell-min">
        <span class="m-lbl">Min qty</span>
        <span class="sr-control">
          <input type="number" class="min-inp" value="${item.minQty}" min="0" step="0.01"
            oninput="updateStorageMinLive(${i},this.value)" onblur="commitStorageChange()">
          <span class="sr-unit">${item.unit}</span>
        </span>
      </div>
      <div class="sr-cell sr-cell-status">
        <span class="m-lbl">Status</span>
        <span class="sr-status-badge" data-idx="${i}">${statusBadge(item)}</span>
      </div>
      <div class="sr-cell sr-cell-supplier">
        <span class="m-lbl">Supplier</span>
        <span class="badge b-blue" style="font-size:11px">${item.supName}</span>
      </div>
    </div>`).join('');
}

/* ══ RECIPES ══ */
function supOpts(sel){return suppliers.map(s=>`<option value="${s.name}"${s.name===sel?' selected':''}>${s.name}</option>`).join('');}
function prodOpts(supName,sel){
  const s=suppliers.find(x=>x.name===supName);
  if(!s||!s.products.length)return'<option value="">— no products —</option>';
  return s.products.map(p=>`<option value="${p.name}"${p.name===sel?' selected':''}>${p.name}</option>`).join('');
}
function unitOf(sn,pn){const s=suppliers.find(x=>x.name===sn);if(!s)return'';const p=s.products.find(x=>x.name===pn);return p?p.unit:'';}
function addIngRow(ing){
  const id='ir-'+(rowIdx++);
  const sn=ing?ing.supplier:(suppliers[0]?suppliers[0].name:'');
  const pn=ing?ing.product:'';
  const qty=ing?ing.qty:'';
  const unit=ing?ing.unit:unitOf(sn,pn);
  const div=document.createElement('div');div.className='ing-row';div.id=id;
  div.innerHTML=`
    <div><label>Supplier</label><select onchange="onSupChange('${id}',this)">${supOpts(sn)}</select></div>
    <div><label>Product</label><select class="prod-sel" onchange="onProdChange('${id}',this)">${prodOpts(sn,pn)}</select></div>
    <div><label>Quantity</label><input type="number" class="qty-inp" value="${qty}" placeholder="200" min="0.001" step="0.001"></div>
    <div><label>Unit</label><select class="unit-inp">
      <option value="g"${unit==='g'?' selected':''}>g</option>
      <option value="kg"${unit==='kg'?' selected':''}>kg</option>
      <option value="ml"${unit==='ml'?' selected':''}>ml</option>
      <option value="L"${unit==='L'?' selected':''}>L</option>
      <option value="pcs"${unit==='pcs'?' selected':''}>pcs</option>
      <option value="box"${unit==='box'?' selected':''}>box</option>
      <option value="bag"${unit==='bag'?' selected':''}>bag</option>
    </select></div>
    <button class="icon-btn del" style="margin-bottom:1px" onclick="document.getElementById('${id}').remove()"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="2" y1="2" x2="10" y2="10" stroke="currentColor" stroke-width="1.8"/><line x1="10" y1="2" x2="2" y2="10" stroke="currentColor" stroke-width="1.8"/></svg></span></button>`;
  document.getElementById('ing-rows').appendChild(div);
}
function onSupChange(id,sel){
  const row=document.getElementById(id);row.querySelector('.prod-sel').innerHTML=prodOpts(sel.value,'');
  const s=suppliers.find(x=>x.name===sel.value);const uInp=row.querySelector('.unit-inp');if(uInp){uInp.value=s&&s.products[0]?s.products[0].unit:'g';}
}
function onProdChange(id,sel){
  const row=document.getElementById(id);row.querySelector('.unit-inp').value=unitOf(row.querySelectorAll('select')[0].value,sel.value);
}
function saveRecipe(){
  const name=document.getElementById('r-name').value.trim();
  const portions=parseInt(document.getElementById('r-portions').value)||1;
  if(!name){alert('Enter a recipe name.');return;}
  const rows=document.querySelectorAll('.ing-row');
  if(!rows.length){alert('Add at least one ingredient.');return;}
  const ingredients=[];let valid=true;
  rows.forEach(row=>{
    const supplier=row.querySelectorAll('select')[0].value;
    const product=row.querySelector('.prod-sel').value;
    const qty=parseFloat(row.querySelector('.qty-inp').value);
    const unit=row.querySelector('.unit-inp').value.trim();
    if(!product||isNaN(qty)||qty<=0){valid=false;return;}
    ingredients.push({supplier,product,qty,unit});
  });
  if(!valid){alert('Check all ingredient rows.');return;}
  const recipe={name,portions,ingredients};
  if(editingRecipe>=0){recipes[editingRecipe]=recipe;editingRecipe=-1;}
  else recipes.push(recipe);
  persist();clearRecipeForm();renderRecipes();
}
function clearRecipeForm(){
  document.getElementById('r-name').value='';document.getElementById('r-portions').value='1';
  document.getElementById('ing-rows').innerHTML='';
  document.getElementById('recipe-form-label').textContent='New recipe';
  document.getElementById('recipe-cancel').style.display='none';editingRecipe=-1;
}
function cancelRecipe(){clearRecipeForm();}
function editRecipe(i){
  const r=recipes[i];editingRecipe=i;
  document.getElementById('r-name').value=r.name;document.getElementById('r-portions').value=r.portions;
  document.getElementById('ing-rows').innerHTML='';r.ingredients.forEach(ing=>addIngRow(ing));
  document.getElementById('recipe-form-label').innerHTML='<span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M8.5 1.5l2 2L4 10l-2.5.5L2 8z" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/></svg></span> Editing: '+r.name;
  document.getElementById('recipe-cancel').style.display='';
  document.getElementById('recipe-form-card').scrollIntoView({behavior:'smooth',block:'start'});
}
function deleteRecipe(i){
  if(!confirm('Delete "'+recipes[i].name+'"?'))return;
  if(editingRecipe===i)clearRecipeForm();recipes.splice(i,1);persist();renderRecipes();
}
function getTarget(i){return parseFloat(document.getElementById('scale-'+i)?.value)||recipes[i].portions;}
function scaledIngredients(recipe,target){
  return recipe.ingredients.map(ing=>({...ing,scaledQty:parseFloat((ing.qty/recipe.portions*target).toFixed(4))}));
}
function updateScale(i){
  const r=recipes[i],target=getTarget(i);
  const tbody=document.getElementById('tbody-'+i);if(!tbody)return;
  tbody.querySelectorAll('tr').forEach((tr,j)=>{
    const ing=r.ingredients[j];if(!ing)return;
    const scaled=parseFloat((ing.qty/r.portions*target).toFixed(4));
    const same=scaled===ing.qty;
    tr.querySelector('.qty-cell').innerHTML=same
      ?`<span class="qty-orig">${ing.qty} ${ing.unit}</span>`
      :`<span class="qty-orig">${ing.qty} ${ing.unit}</span><span class="qty-arrow">&rarr;</span><span class="qty-new">${scaled} ${ing.unit}</span>`;
    const ac=tr.querySelector('.avail-cell');if(ac)ac.innerHTML=availBadge(ing.supplier,ing.product,scaled,ing.unit);
  });
  const lbl=document.getElementById('plabel-'+i);
  if(lbl)lbl.innerHTML=target===r.portions?`${r.portions} portion${r.portions!==1?'s':''} (base)`:`Scaled: ${r.portions} &rarr; ${target} portions`;
}
function resetScale(i){document.getElementById('scale-'+i).value=recipes[i].portions;updateScale(i);}

function sendToToday(i){
  const r=recipes[i],target=getTarget(i),date=todayStr();
  const scaled=scaledIngredients(r,target);
  scaled.forEach(ing=>{
    const item=getStorageItem(ing.supplier,ing.product);if(!item)return;
    const deduct = convertUnits(ing.scaledQty, ing.unit, item.unit);
    item.qty=Math.max(0,parseFloat((item.qty-deduct).toFixed(6)));
  });
  usedLog.push({id:Date.now(),date,recipeName:r.name,basePortions:r.portions,portions:target,ingredients:scaled});

  // ── expiration tracking ──
  const madeDate = document.getElementById('made-'+i)?.value || date;
  const expiresDate = document.getElementById('expires-'+i)?.value || '';
  if (expiresDate) {
    expirationLog.push({
      id: Date.now() + 1,
      recipeName: r.name,
      portions: target,
      madeDate,
      expiresDate
    });
  }

  persist();
  const btn=document.getElementById('send-btn-'+i);
  if(btn){btn.innerHTML='<span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Sent!';btn.disabled=true;setTimeout(()=>{btn.innerHTML='<span class="ic"><svg width="13" height="13" viewBox="0 0 14 14"><path d="M2 12l10-10M6 2h6v6" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Send to Today Used';btn.disabled=false;updateScale(i);},1800);}
  updateScale(i);
}
function moveRecipe(i, dir) {
  const ni = i + dir;
  if (ni < 0 || ni >= recipes.length) return;
  [recipes[i], recipes[ni]] = [recipes[ni], recipes[i]];
  persist(); renderRecipes();
}
function toggleRecipeBody(i) {
  const body  = document.getElementById('rbody-' + i);
  const sbar  = document.getElementById('rscale-' + i);
  const chev  = document.getElementById('rchev-' + i);
  if (!body) return;
  const closing = !body.classList.contains('collapsed');
  body.classList.toggle('collapsed', closing);
  sbar.classList.toggle('collapsed', closing);
  if (chev) chev.style.transform = closing ? '' : 'rotate(90deg)';
}
function renderRecipes(){
  const list=document.getElementById('recipes-list');
  if(!recipes.length){list.innerHTML='<div class="empty">No recipes yet.</div>';return;}
  list.innerHTML=recipes.map((r,i)=>{
    const rows=r.ingredients.map(ing=>`
      <tr>
        <td style="font-weight:600">${ing.product}</td>
        <td><span class="badge b-blue" style="font-size:10px">${ing.supplier}</span></td>
        <td class="qty-cell"><span class="qty-orig">${ing.qty} ${ing.unit}</span></td>
        <td class="avail-cell">${availBadge(ing.supplier,ing.product,ing.qty,ing.unit)}</td>
      </tr>`).join('');
    return `
    <div class="recipe-card">
      <div class="recipe-head" style="cursor:pointer" onclick="toggleRecipeBody(${i})">
        <div style="display:flex;align-items:center;gap:8px">
          <div style="display:flex;flex-direction:column;gap:1px" onclick="event.stopPropagation()">
            <button class="icon-btn move" onclick="moveRecipe(${i},-1)" style="padding:1px 5px;font-size:11px"><span class="ic"><svg width="9" height="9" viewBox="0 0 10 10"><polygon points="5,1 9,8 1,8" fill="currentColor"/></svg></span></button>
            <button class="icon-btn move" onclick="moveRecipe(${i},1)"  style="padding:1px 5px;font-size:11px"><span class="ic"><svg width="9" height="9" viewBox="0 0 10 10"><polygon points="1,2 9,2 5,9" fill="currentColor"/></svg></span></button>
          </div>
          <div>
            <div class="recipe-title">${r.name}</div>
            <div class="recipe-sub" id="plabel-${i}">${r.portions} portion${r.portions!==1?'s':''} (base)</div>
          </div>
        </div>
        <div style="display:flex;gap:4px;align-items:center">
          <button class="icon-btn edit" onclick="event.stopPropagation();editRecipe(${i})"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M8.5 1.5l2 2L4 10l-2.5.5L2 8z" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/></svg></span></button>
          <button class="icon-btn del"  onclick="event.stopPropagation();deleteRecipe(${i})"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 3h8M4.5 3V2a1 1 0 0 1 1-1h1a1 1 0 0 1 1 1v1M3 3l.5 8a1 1 0 0 0 1 .9h3a1 1 0 0 0 1-.9L9 3" fill="none" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg></span></button>
          <span style="color:var(--text3);transition:transform .2s;margin-left:4px;display:inline-flex;transform:rotate(90deg)" id="rchev-${i}"><span class="ic"><svg width="10" height="10" viewBox="0 0 10 10"><polygon points="2,1 8,5 2,9" fill="currentColor"/></svg></span></span>
        </div>
      </div>
      <div class="recipe-body collapsed" id="rbody-${i}">
        <div class="table-scroll"><table>
          <thead><tr><th>Ingredient</th><th>Supplier</th><th>Qty needed</th><th>Available</th></tr></thead>
          <tbody id="tbody-${i}">${rows}</tbody>
        </table></div>
      </div>
      <div class="scale-bar collapsed" id="rscale-${i}">
        <label>Calculate for</label>
        <input type="number" id="scale-${i}" class="scale-inp" value="${r.portions}" min="0.5" step="0.5" oninput="updateScale(${i})">
        <span style="font-size:12px;color:var(--text2)">portions</span>
        <div style="display:flex;align-items:center;gap:8px;margin-left:12px">
          <label style="margin:0;text-transform:none;letter-spacing:0;font-size:11px;color:var(--raindance)">Made on</label>
          <input type="date" id="made-${i}" value="${todayStr()}" style="width:130px;background:var(--bg3);border-color:var(--narragansett);color:var(--raindance);font-weight:600;padding:6px 8px;font-size:12px">
          <label style="margin:0;text-transform:none;letter-spacing:0;font-size:11px;color:var(--raindance)">Expires on</label>
          <input type="date" id="expires-${i}" style="width:130px;background:var(--bg3);border-color:var(--narragansett);color:var(--raindance);font-weight:600;padding:6px 8px;font-size:12px">
        </div>
        <div style="display:flex;gap:6px;margin-left:auto;flex-wrap:wrap">
          <button class="btn btn-sm" onclick="updateScale(${i})"><span class="ic"><svg width="12" height="12" viewBox="0 0 14 14"><path d="M12 7A5 5 0 1 1 10.3 3.3M12 1v3h-3" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Calculate</button>
          <button class="btn btn-sm" onclick="resetScale(${i})">Reset</button>
          <button class="btn btn-green btn-sm" id="send-btn-${i}" onclick="sendToToday(${i})"><span class="ic"><svg width="13" height="13" viewBox="0 0 14 14"><path d="M2 12l10-10M6 2h6v6" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Send to Today Used</button>
        </div>
      </div>
    </div>`;
  }).join('');
}

/* ══ TODAY USED ══ */
function initTodayTab(){
  const vd=document.getElementById('view-date');if(!vd.value)vd.value=todayStr();
  renderTodayUsed();
}
function onDateChange(){renderTodayUsed();}
function renderTodayUsed(){
  const date=document.getElementById('view-date').value||todayStr();
  const entries=usedLog.filter(e=>e.date===date);
  document.getElementById('day-summary').textContent=entries.length
    ?`${fmtDate(date)} — ${entries.length} recipe${entries.length!==1?'s':''} made`
    :`${fmtDate(date)} — nothing logged`;
  const container=document.getElementById('today-entries');
  if(!entries.length){container.innerHTML='<div class="empty">No entries for this day.<br>Go to Recipes, set portions and hit <span class="ic"><svg width="13" height="13" viewBox="0 0 14 14"><path d="M2 12l10-10M6 2h6v6" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Send to Today Used.</div>';return;}
  container.innerHTML=`
    <div class="day-group">
      <div class="day-header">
        <span>${fmtDate(date)}</span>
        <span class="badge b-green">${entries.length} recipe${entries.length!==1?'s':''}</span>
      </div>
      <div class="day-entries">
        ${entries.map(e=>{
          const logIdx=usedLog.findIndex(x=>x.id===e.id);
          const portionLabel=e.portions===e.basePortions?`${e.portions} portion${e.portions!==1?'s':''}`:`${e.portions} portions (base: ${e.basePortions})`;
          const detailRows=e.ingredients.map(ing=>`
            <div class="detail-ing-row">
              <span style="font-weight:600">${ing.product} <span style="font-size:11px;color:var(--text3)">· ${ing.supplier}</span></span>
              <span style="color:var(--blue);font-weight:600">${ing.scaledQty} ${ing.unit}</span>
            </div>`).join('');
          return `
            <div>
              <div class="entry-row" onclick="toggleDetail('detail-${e.id}','chev-${e.id}')">
                <div>
                  <div class="entry-name">${e.recipeName}</div>
                  <div class="entry-meta">${portionLabel} · tap to expand</div>
                </div>
                <div style="display:flex;align-items:center;gap:8px;flex-shrink:0">
                  <span class="badge b-green">${e.portions} portions</span>
                  <button class="icon-btn del" onclick="event.stopPropagation();deleteUsed(${logIdx})" title="Delete"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 3h8M4.5 3V2a1 1 0 0 1 1-1h1a1 1 0 0 1 1 1v1M3 3l.5 8a1 1 0 0 0 1 .9h3a1 1 0 0 0 1-.9L9 3" fill="none" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg></span></button>
                  <span style="color:var(--text3);transition:transform .2s;display:inline-flex" id="chev-${e.id}"><span class="ic"><svg width="10" height="10" viewBox="0 0 10 10"><polygon points="2,1 8,5 2,9" fill="currentColor"/></svg></span></span>
                </div>
              </div>
              <div class="entry-detail" id="detail-${e.id}">
                <div style="font-size:11px;color:var(--text3);font-weight:600;text-transform:uppercase;letter-spacing:.05em;margin-bottom:8px">Ingredients used</div>
                ${detailRows}
              </div>
            </div>`;
        }).join('')}
      </div>
    </div>`;
}
function toggleDetail(detailId,chevId){
  const el=document.getElementById(detailId),ch=document.getElementById(chevId);if(!el)return;
  el.classList.toggle('open');if(ch)ch.style.transform=el.classList.contains('open')?'rotate(90deg)':'';
}
function deleteUsed(i){
  const entry = usedLog[i];
  if (!entry) return;
  const isToday = entry.date === todayStr();
  const confirmMsg = isToday
    ? 'Remove this entry? Storage quantities will be restored since it was logged today.'
    : 'Remove this entry? Storage will NOT be changed (entry is from a previous day).';
  if (!confirm(confirmMsg)) return;

  // Only restore storage if the entry was logged today
  if (isToday && entry.ingredients) {
    entry.ingredients.forEach(ing => {
      const item = getStorageItem(ing.supplier, ing.product);
      if (!item) return;
      const restore = convertUnits(ing.scaledQty, ing.unit, item.unit);
      item.qty = parseFloat((item.qty + restore).toFixed(6));
    });
  }

  usedLog.splice(i, 1);
  persist();
  renderTodayUsed();
}


/* ══ PRICE CALCULATOR ══ */
function movePc(i, dir) {
  const ni = i + dir;
  if (ni < 0 || ni >= recipes.length) return;
  [recipes[i], recipes[ni]] = [recipes[ni], recipes[i]];
  persist(); renderPriceCalc();
}
function togglePcBody(i) {
  const body  = document.getElementById('pcbody-'  + i);
  const tot   = document.getElementById('pctot-'   + i);
  const port  = document.getElementById('pcport-'  + i);
  const chev  = document.getElementById('pcchev-'  + i);
  if (!body) return;
  const closing = !body.classList.contains('collapsed');
  body.classList.toggle('collapsed',  closing);
  tot.classList.toggle('collapsed',   closing);
  port.classList.toggle('collapsed',  closing);
  if (chev) chev.style.transform = closing ? '' : 'rotate(90deg)';
}

// Get price-per-base-unit from most recent delivery.
// delivery stores: priceFixed (total price for the delivery), qty (amount delivered), unit (e.g. kg, g, L, ml)
// Returns: { pricePerUnit, unit, priceFixed, deliveredQty } or null
function getDeliveryPrice(supName, prodName) {
  for (const d of deliveries) {
    if (d.supName !== supName) continue;
    const item = d.items.find(it => it.product === prodName);
    if (item) {
      const price = item.priceFixed ?? item.priceExcl ?? null;
      if (price === null || !item.qty) return null;
      // price / qty = price per delivery unit
      const pricePerUnit = price / item.qty;
      return { pricePerUnit, unit: item.unit, priceFixed: price, deliveredQty: item.qty };
    }
  }
  return null;
}

// (Price Calculator unit conversion now reuses the shared convertUnits() function above.)
function renderPriceCalc() {
  const list = document.getElementById('price-calc-list');
  if (!recipes.length) {
    list.innerHTML = '<div class="empty">No recipes yet — add them in the Recipes tab first.</div>';
    return;
  }
  list.innerHTML = recipes.map((r, ri) => {
    const ings = r.ingredients.map((ing, ii) => {
      const delPrice = getDeliveryPrice(ing.supplier, ing.product);
      // calculate price per recipe unit
      let pricePerRecipeUnit = null;
      let deliveryNote = '<span style="font-size:10px;color:var(--text3)">no delivery price</span>';
      if (delPrice) {
        // convert recipe unit to delivery unit to get correct ratio
        const recipeQtyInDelUnit = convertUnits(1, ing.unit, delPrice.unit);
        pricePerRecipeUnit = delPrice.pricePerUnit * recipeQtyInDelUnit;
        const unitLabel = delPrice.unit;
        const ppu = (delPrice.priceFixed / delPrice.deliveredQty).toFixed(4);
        deliveryNote = `<span style="font-size:10px;color:var(--green)"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="6" y1="1" x2="6" y2="10" stroke="currentColor" stroke-width="1.8"/><path d="M3 7l3 3 3-3" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg></span> €${delPrice.priceFixed} / ${delPrice.deliveredQty}${unitLabel} = €${ppu}/${unitLabel}</span>`;
      }
      const inputVal = pricePerRecipeUnit !== null ? pricePerRecipeUnit.toFixed(6) : '';
      return `
        <div class="pc-ing-row">
          <div class="pc-ing-left" style="flex:1;min-width:0">
            <span style="font-weight:600">${ing.product}</span>
            <span class="badge b-blue" style="font-size:10px">${ing.supplier}</span>
            <span style="color:var(--text3);font-size:12px" id="pc-qty-${ri}-${ii}">${ing.qty} ${ing.unit}</span>
          </div>
          <div style="display:flex;align-items:center;gap:6px;flex-shrink:0">
            <div style="display:flex;flex-direction:column;align-items:flex-end;gap:2px">
              ${deliveryNote}
              <div style="display:flex;align-items:center;gap:4px">
                <span style="font-size:11px;color:var(--text3)">€ per ${ing.unit}</span>
                <input type="number" class="pc-price-inp" id="pc-price-${ri}-${ii}"
                  value="${inputVal}" placeholder="0.000000" min="0" step="0.000001"
                  oninput="recalcPc(${ri})">
              </div>
            </div>
            <span style="font-size:13px;color:var(--text2);min-width:80px;text-align:right;font-weight:600" id="pc-line-${ri}-${ii}">—</span>
          </div>
        </div>`;
    }).join('');

    return `
    <div class="pc-card" id="pcc-${ri}">
      <div class="pc-head" style="cursor:pointer" onclick="togglePcBody(${ri})">
        <div style="display:flex;align-items:center;gap:8px">
          <div style="display:flex;flex-direction:column;gap:1px" onclick="event.stopPropagation()">
            <button class="icon-btn move" onclick="movePc(${ri},-1)" style="padding:1px 5px;font-size:11px"><span class="ic"><svg width="9" height="9" viewBox="0 0 10 10"><polygon points="5,1 9,8 1,8" fill="currentColor"/></svg></span></button>
            <button class="icon-btn move" onclick="movePc(${ri},1)"  style="padding:1px 5px;font-size:11px"><span class="ic"><svg width="9" height="9" viewBox="0 0 10 10"><polygon points="1,2 9,2 5,9" fill="currentColor"/></svg></span></button>
          </div>
          <div>
            <div class="pc-title">${r.name}</div>
            <div style="font-size:12px;color:var(--text2);margin-top:2px" id="pc-sub-${ri}">${r.portions} portion${r.portions!==1?'s':''} (base)</div>
          </div>
        </div>
        <div style="display:flex;gap:6px;align-items:center" onclick="event.stopPropagation()">
          <button class="btn btn-sm" onclick="importDeliveryPrices(${ri})" style="font-size:11px;color:var(--green);border-color:var(--green-border)"><span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="6" y1="1" x2="6" y2="10" stroke="currentColor" stroke-width="1.8"/><path d="M3 7l3 3 3-3" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Re-import prices</button>
          <button class="btn btn-sm" onclick="resetPc(${ri})"><span class="ic"><svg width="12" height="12" viewBox="0 0 14 14"><path d="M2 7a5 5 0 1 0 1.7-3.7M2 1v3h3" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Clear</button>
          <span style="color:var(--text3);transition:transform .2s;margin-left:4px;display:inline-flex" id="pcchev-${ri}"><span class="ic"><svg width="10" height="10" viewBox="0 0 10 10"><polygon points="2,1 8,5 2,9" fill="currentColor"/></svg></span></span>
        </div>
      </div>
      <div class="pc-body collapsed" id="pcbody-${ri}">
        <div class="pc-col-header" style="display:grid;grid-template-columns:1fr auto auto;font-size:10px;color:var(--text3);font-weight:600;text-transform:uppercase;letter-spacing:.05em;padding:0 0 6px;border-bottom:1px solid var(--border);margin-bottom:2px">
          <span>Ingredient</span>
          <span style="text-align:right;padding-right:8px;min-width:140px">Price (€)</span>
          <span style="min-width:80px;text-align:right">Line cost</span>
        </div>
        ${ings}
      </div>
      <div class="pc-total-bar collapsed" id="pctot-${ri}">
        <div>
          <div style="font-size:11px;color:var(--text2);margin-bottom:2px">Recipe cost</div>
          <div style="font-size:20px;font-weight:700;color:var(--raindance)" id="pc-total-${ri}">—</div>
        </div>
        <div style="text-align:right">
          <div style="font-size:11px;color:var(--text2);margin-bottom:2px">Cost per portion</div>
          <div style="font-size:20px;font-weight:700;color:var(--sherwoodtan)" id="pc-per-${ri}">—</div>
        </div>
      </div>
      <div class="pc-portions-bar collapsed" id="pcport-${ri}">
        <label>Calculate for</label>
        <input type="number" class="pc-scale-inp" id="pc-scale-${ri}" value="${r.portions}" min="0.5" step="0.5" oninput="recalcPc(${ri})">
        <span style="font-size:12px;color:var(--text2)">portions</span>
      </div>
    </div>`;
  }).join('');

  // auto-calculate on load
  recipes.forEach((r, ri) => recalcPc(ri));
}

function importDeliveryPrices(ri) {
  const r = recipes[ri];
  if (!r) return;
  r.ingredients.forEach((ing, ii) => {
    const delPrice = getDeliveryPrice(ing.supplier, ing.product);
    if (!delPrice) return;
    const recipeQtyInDelUnit = convertUnits(1, ing.unit, delPrice.unit);
    const pricePerRecipeUnit = delPrice.pricePerUnit * recipeQtyInDelUnit;
    const inp = document.getElementById(`pc-price-${ri}-${ii}`);
    if (inp) inp.value = pricePerRecipeUnit.toFixed(6);
  });
  recalcPc(ri);
}

function recalcPc(ri) {
  const r = recipes[ri];
  if (!r) return;
  const targetPortions = parseFloat(document.getElementById(`pc-scale-${ri}`)?.value) || r.portions;
  const scale = targetPortions / r.portions;
  let total = 0;
  let anyFilled = false;

  r.ingredients.forEach((ing, ii) => {
    const scaledQty = parseFloat((ing.qty * scale).toFixed(4));
    const qtyLbl = document.getElementById(`pc-qty-${ri}-${ii}`);
    if (qtyLbl) qtyLbl.textContent = scaledQty + ' ' + ing.unit;

    const priceVal = parseFloat(document.getElementById(`pc-price-${ri}-${ii}`)?.value);
    const lineCostEl = document.getElementById(`pc-line-${ri}-${ii}`);
    if (!isNaN(priceVal) && priceVal >= 0) {
      const lineCost = priceVal * scaledQty;
      total += lineCost;
      anyFilled = true;
      if (lineCostEl) lineCostEl.innerHTML = `<span style="color:var(--amber);font-weight:600">€${lineCost.toFixed(3)}</span>`;
    } else {
      if (lineCostEl) lineCostEl.textContent = '—';
    }
  });

  const totalEl = document.getElementById(`pc-total-${ri}`);
  const perEl   = document.getElementById(`pc-per-${ri}`);
  const subEl   = document.getElementById(`pc-sub-${ri}`);

  if (totalEl) totalEl.textContent = anyFilled ? '€' + total.toFixed(2) : '—';
  if (perEl)   perEl.textContent   = anyFilled && targetPortions > 0 ? '€' + (total / targetPortions).toFixed(3) : '—';
  if (subEl)   subEl.innerHTML     = targetPortions === r.portions
    ? `${r.portions} portion${r.portions!==1?'s':''} (base)`
    : `Scaled: ${r.portions} &rarr; ${targetPortions} portions`;
}

function resetPc(ri) {
  const r = recipes[ri];
  if (!r) return;
  r.ingredients.forEach((ing, ii) => {
    const inp = document.getElementById(`pc-price-${ri}-${ii}`);
    if (inp) inp.value = '';
    const lbl = document.getElementById(`pc-line-${ri}-${ii}`);
    if (lbl) lbl.textContent = '—';
    const qty = document.getElementById(`pc-qty-${ri}-${ii}`);
    if (qty) qty.textContent = ing.qty + ' ' + ing.unit;
  });
  const scaleInp = document.getElementById(`pc-scale-${ri}`);
  if (scaleInp) scaleInp.value = r.portions;
  const tot = document.getElementById(`pc-total-${ri}`);
  if (tot) tot.textContent = '—';
  const per = document.getElementById(`pc-per-${ri}`);
  if (per) per.textContent = '—';
  const sub = document.getElementById(`pc-sub-${ri}`);
  if (sub) sub.textContent = `${r.portions} portion${r.portions!==1?'s':''} (base)`;
}



/* ══ EXPIRATION ══ */
function getExpStatus(madeDate, expiresDate) {
  const now = new Date(); now.setHours(0,0,0,0);
  const made = new Date(madeDate + 'T00:00:00');
  const expires = new Date(expiresDate + 'T00:00:00');
  const totalSpan = expires - made;          // total shelf life in ms
  const elapsed = now - made;                // time passed since made
  const remaining = expires - now;           // time left until expiry

  if (remaining <= 0) return 'exp-expired';
  if (totalSpan > 0 && elapsed / totalSpan >= 0.5) return 'exp-soon';
  return 'exp-good';
}
function getExpDaysLeft(expiresDate) {
  const now = new Date(); now.setHours(0,0,0,0);
  const expires = new Date(expiresDate + 'T00:00:00');
  return Math.ceil((expires - now) / (1000*60*60*24));
}
function deleteExpiration(i) {
  if (!confirm('Remove this expiration entry?')) return;
  expirationLog.splice(i,1); persist(); renderExpiration();
}
function startEditExpiration(i) {
  document.getElementById('exp-view-'+i).style.display = 'none';
  document.getElementById('exp-edit-'+i).style.display = 'flex';
}
function cancelEditExpiration(i) {
  document.getElementById('exp-view-'+i).style.display = '';
  document.getElementById('exp-edit-'+i).style.display = 'none';
}
function saveExpirationDate(i) {
  const newDate = document.getElementById('exp-date-input-'+i).value;
  if (!newDate) { alert('Pick a date.'); return; }
  expirationLog[i].expiresDate = newDate;
  persist();
  renderExpiration();
}
function renderExpiration() {
  const list = document.getElementById('expiration-list');
  if (!expirationLog.length) {
    list.innerHTML = '<div class="empty">No expiration entries yet.<br>In Recipes, set "Made on" / "Expires on" dates and hit <span class="ic"><svg width="13" height="13" viewBox="0 0 14 14"><path d="M2 12l10-10M6 2h6v6" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Send to Today Used.</div>';
    return;
  }
  // compute status + sort: expired first, then soonest expiring, then good (soonest first too)
  const enriched = expirationLog.map((e, idx) => ({
    ...e,
    _idx: idx,
    _status: getExpStatus(e.madeDate, e.expiresDate),
    _daysLeft: getExpDaysLeft(e.expiresDate)
  }));
  const order = { 'exp-expired': 0, 'exp-soon': 1, 'exp-good': 2 };
  enriched.sort((a,b) => {
    if (order[a._status] !== order[b._status]) return order[a._status] - order[b._status];
    return a._daysLeft - b._daysLeft; // soonest expiry first within same group
  });

  const statusLabel = { 'exp-good': '<span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Good', 'exp-soon': '<span class="ic"><svg width="11" height="11" viewBox="0 0 14 14"><path d="M7 1.5l6 10.5H1z" fill="none" stroke="currentColor" stroke-width="1.4" stroke-linejoin="round"/><line x1="7" y1="5.5" x2="7" y2="8.5" stroke="currentColor" stroke-width="1.4"/><circle cx="7" cy="10.5" r="0.6" fill="currentColor"/></svg></span> Close to date', 'exp-expired': '<span class="ic"><svg width="11" height="11" viewBox="0 0 12 12"><line x1="2" y1="2" x2="10" y2="10" stroke="currentColor" stroke-width="1.8"/><line x1="10" y1="2" x2="2" y2="10" stroke="currentColor" stroke-width="1.8"/></svg></span> Expired' };

  list.innerHTML = enriched.map(e => {
    const daysTxt = e._status === 'exp-expired'
      ? `${Math.abs(e._daysLeft)} day${Math.abs(e._daysLeft)!==1?'s':''} overdue`
      : `${e._daysLeft} day${e._daysLeft!==1?'s':''} left`;
    return `
    <div class="exp-card ${e._status}">
      <div class="exp-row">
        <div>
          <div class="exp-name">${e.recipeName}</div>
          <div class="exp-meta">${e.portions} portion${e.portions!==1?'s':''}</div>
          <div class="exp-dates" style="margin-top:6px" id="exp-view-${e._idx}">
            <span>Made: <strong>${fmtDate(e.madeDate)}</strong></span>
            <span>Expires: <strong>${fmtDate(e.expiresDate)}</strong></span>
            <span>${daysTxt}</span>
          </div>
          <div class="exp-dates" style="margin-top:6px;display:none;align-items:center;gap:10px" id="exp-edit-${e._idx}">
            <label style="margin:0;text-transform:none;letter-spacing:0;font-size:12px;color:var(--text2)">New expiry date:</label>
            <input type="date" id="exp-date-input-${e._idx}" value="${e.expiresDate}" style="width:150px;padding:5px 8px;font-size:12px">
            <button class="btn btn-blue btn-sm" onclick="saveExpirationDate(${e._idx})"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 6.5l3 3 5-6" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg></span> Save</button>
            <button class="btn btn-sm" onclick="cancelEditExpiration(${e._idx})">Cancel</button>
          </div>
        </div>
        <div style="display:flex;align-items:center;gap:10px">
          <span class="exp-status ${e._status}">${statusLabel[e._status]}</span>
          <button class="icon-btn edit" onclick="startEditExpiration(${e._idx})" title="Extend / edit expiry date"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M8.5 1.5l2 2L4 10l-2.5.5L2 8z" fill="none" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/></svg></span></button>
          <button class="icon-btn del" onclick="deleteExpiration(${e._idx})" title="Remove"><span class="ic"><svg width="12" height="12" viewBox="0 0 12 12"><path d="M2 3h8M4.5 3V2a1 1 0 0 1 1-1h1a1 1 0 0 1 1 1v1M3 3l.5 8a1 1 0 0 0 1 .9h3a1 1 0 0 0 1-.9L9 3" fill="none" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg></span></button>
        </div>
      </div>
    </div>`;
  }).join('');
}
/* init */
syncStorage();renderSuppliers();renderRecipes();
document.getElementById('view-date').value=todayStr();
document.getElementById('del-date').value=todayStr();
</script>
</body>
</html>

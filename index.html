<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>DayLog</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,500;9..144,600;9..144,700&family=Inter:wght@400;500;600;700&family=IBM+Plex+Mono:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#211B29;
    --surface:#2A2333;
    --surface-2:#342C40;
    --paper:#F5EFE4;
    --paper-line:#E1D5BC;
    --ink:#2B2333;
    --ink-dim:#6B6478;
    --text:#EFE8DD;
    --text-dim:#B0A6BE;
    --gold:#D3A15D;
    --gold-dim:#8A7454;
    --red:#C1503D;
    --border: rgba(239,232,221,0.09);
    --radius: 16px;
  }
  *{box-sizing:border-box; margin:0; padding:0;}
  html,body{height:100%;}
  body{
    background: var(--bg);
    color: var(--text);
    font-family:'Inter', sans-serif;
    min-height:100vh;
    -webkit-font-smoothing: antialiased;
  }
  #root{min-height:100vh;}
  h1,h2,h3,.display{ font-family:'Fraunces', serif; font-weight:600; letter-spacing:-0.01em;}
  .mono{font-family:'IBM Plex Mono', monospace;}
  ::selection{ background: var(--gold); color:var(--ink);}
  button{font-family:inherit; cursor:pointer; border:none;}
  input,textarea{font-family:inherit;}
  a{color:inherit;}

  /* ---------- AUTH ---------- */
  .auth-wrap{
    min-height:100vh; display:flex; align-items:center; justify-content:center;
    padding:24px;
    background:
      radial-gradient(circle at 20% 15%, rgba(211,161,93,0.10), transparent 45%),
      radial-gradient(circle at 85% 80%, rgba(193,80,61,0.10), transparent 40%),
      var(--bg);
  }
  .auth-card{
    width:100%; max-width:400px;
    background: var(--paper);
    color: var(--ink);
    border-radius: var(--radius);
    padding:44px 36px 36px;
    position:relative;
    box-shadow: 0 30px 60px -20px rgba(0,0,0,0.55);
    background-image: repeating-linear-gradient(var(--paper) 0px, var(--paper) 31px, var(--paper-line) 32px);
  }
  .auth-card::before{
    content:"";
    position:absolute; left:44px; top:0; bottom:0; width:1px;
    background: rgba(193,80,61,0.35);
  }
  .auth-mark{ width:9px; height:9px; border-radius:50%; background:var(--red); display:inline-block; margin-right:8px; position:relative; top:-2px;}
  .auth-brand{ font-size:28px; margin-bottom:4px; padding-left:20px;}
  .auth-tag{ font-size:13px; color: var(--ink-dim); margin-bottom:30px; padding-left:20px; }
  .field{ margin-bottom:16px; padding-left:20px;}
  .field label{ display:block; font-size:11px; text-transform:uppercase; letter-spacing:0.08em; color:var(--ink-dim); margin-bottom:6px;}
  .field input{
    width:100%; background:transparent; border:none; border-bottom:1px solid rgba(43,35,51,0.25);
    padding:6px 2px; font-size:16px; color:var(--ink); outline:none;
  }
  .field input:focus{ border-bottom-color: var(--red); }
  .auth-btn{
    margin-left:20px; margin-top:22px;
    background: var(--ink); color:var(--paper);
    padding:12px 22px; border-radius:999px; font-size:14px; font-weight:600;
    display:inline-flex; align-items:center; gap:8px;
    transition: transform .15s ease, background .15s ease;
  }
  .auth-btn:hover{ background:var(--red); }
  .auth-btn:active{ transform: scale(0.97); }
  .auth-note{ padding-left:20px; margin-top:18px; font-size:11.5px; color:var(--ink-dim); line-height:1.5; max-width:300px;}

  /* ---------- APP SHELL ---------- */
  .shell{ display:flex; min-height:100vh; }
  .sidebar{
    width:232px; flex-shrink:0; background:var(--surface);
    border-right:1px solid var(--border);
    display:flex; flex-direction:column;
    padding:26px 18px;
    position:sticky; top:0; height:100vh;
  }
  .brand{ display:flex; align-items:center; gap:8px; padding:0 6px 26px; }
  .brand .dot{ width:8px; height:8px; border-radius:50%; background:var(--red); }
  .brand span{ font-family:'Fraunces',serif; font-size:19px; font-weight:600; }
  .nav-label{ font-size:10.5px; text-transform:uppercase; letter-spacing:0.1em; color:var(--text-dim); padding:0 10px 8px;}
  .nav{ display:flex; flex-direction:column; gap:2px; margin-bottom:22px;}
  .nav-item{
    display:flex; align-items:center; gap:10px;
    padding:9px 10px; border-radius:10px; background:transparent; color:var(--text-dim);
    font-size:14px; text-align:left; width:100%; transition: background .15s, color .15s;
  }
  .nav-item svg{ width:16px; height:16px; opacity:0.8; flex-shrink:0;}
  .nav-item:hover{ background:var(--surface-2); color:var(--text); }
  .nav-item.active{ background:var(--surface-2); color:var(--gold); }
  .nav-item.active svg{ opacity:1;}
  .sidebar hr{ border:none; border-top:1px solid var(--border); margin:10px 0 18px; }
  .jump{ padding:0 10px; }
  .jump label{ font-size:10.5px; text-transform:uppercase; letter-spacing:0.1em; color:var(--text-dim); display:block; margin-bottom:8px;}
  .jump-row{ display:flex; gap:6px; }
  .jump input[type=date]{
    flex:1; background:var(--surface-2); border:1px solid var(--border); color:var(--text);
    border-radius:8px; padding:7px 8px; font-size:12.5px; outline:none; color-scheme: dark;
  }
  .jump button{
    background:var(--gold); color:var(--ink); border-radius:8px; padding:0 12px; font-size:13px; font-weight:600;
  }
  .sidebar-foot{ margin-top:auto; padding:0 10px; display:flex; align-items:center; justify-content:space-between;}
  .sidebar-foot .who{ display:flex; align-items:center; gap:8px; font-size:13px; color:var(--text-dim);}
  .avatar{ width:26px; height:26px; border-radius:50%; background:var(--gold); color:var(--ink); display:flex; align-items:center; justify-content:center; font-size:12px; font-weight:700; font-family:'Fraunces',serif;}
  .signout{ background:none; color:var(--text-dim); font-size:11.5px; text-decoration:underline; text-underline-offset:2px;}
  .signout:hover{ color:var(--red); }

  .main{ flex:1; padding:34px 42px 70px; max-width:1080px; }
  .header{ display:flex; align-items:flex-end; justify-content:space-between; margin-bottom:26px; flex-wrap:wrap; gap:10px;}
  .header h1{ font-size:26px; }
  .header .date{ font-size:13px; color:var(--text-dim); }
  .header .datebox{ text-align:right; }

  /* ledger paper input */
  .ledger{
    background: var(--paper); color:var(--ink); border-radius: var(--radius);
    padding:22px 24px 20px; position:relative; margin-bottom:24px;
    background-image: repeating-linear-gradient(var(--paper) 0px, var(--paper) 33px, var(--paper-line) 34px);
    box-shadow: 0 20px 40px -24px rgba(0,0,0,0.5);
  }
  .ledger::before{ content:""; position:absolute; left:46px; top:0; bottom:0; width:1px; background:rgba(193,80,61,0.3); }
  .ledger-label{ font-size:11px; text-transform:uppercase; letter-spacing:0.08em; color:var(--ink-dim); margin-bottom:10px; padding-left:22px;}
  .ledger textarea{
    width:100%; background:transparent; border:none; outline:none; resize:none;
    padding-left:22px; font-size:15.5px; color:var(--ink); line-height:34px; min-height:102px;
  }
  .ledger textarea::placeholder{ color: rgba(43,35,51,0.38); }
  .ledger-actions{ display:flex; justify-content:space-between; align-items:center; padding-left:22px; margin-top:6px; flex-wrap:wrap; gap:10px;}
  .ledger-hint{ font-size:11.5px; color:var(--ink-dim); }
  .log-btn{
    background:var(--ink); color:var(--paper); padding:10px 18px; border-radius:999px; font-size:13.5px; font-weight:600;
    display:flex; align-items:center; gap:6px; transition: background .15s;
  }
  .log-btn:hover{ background:var(--red); }
  .log-btn:disabled{ opacity:0.4; cursor:default; }

  /* today's thread of logs */
  .thread{ display:flex; flex-direction:column; gap:10px; margin-bottom:26px; }
  .bubble{
    background:var(--surface); border:1px solid var(--border); border-radius:12px;
    padding:12px 16px; font-size:13.5px; line-height:1.5;
  }
  .bubble .t{ font-size:10.5px; color:var(--gold); margin-bottom:4px; }
  .chips{ display:flex; flex-wrap:wrap; gap:6px; margin-top:8px;}
  .chip{ font-size:11px; padding:3px 9px; border-radius:999px; color:var(--ink); font-weight:600; }

  /* stat cards */
  .stats{ display:grid; grid-template-columns:repeat(3,1fr); gap:14px; margin-bottom:26px; }
  .stat{ background:var(--surface); border:1px solid var(--border); border-radius:14px; padding:18px 18px; }
  .stat .label{ font-size:11px; text-transform:uppercase; letter-spacing:0.07em; color:var(--text-dim); margin-bottom:8px;}
  .stat .value{ font-family:'IBM Plex Mono', monospace; font-size:26px; font-weight:600; }
  .stat .sub{ font-size:12px; color:var(--text-dim); margin-top:4px; }

  /* charts row */
  .viz-row{ display:grid; grid-template-columns: 1fr 1.3fr; gap:16px; margin-bottom:26px; }
  .panel{ background:var(--surface); border:1px solid var(--border); border-radius:14px; padding:20px; }
  .panel h3{ font-size:14.5px; margin-bottom:14px; font-weight:600; font-family:'Inter',sans-serif; color:var(--text); }
  .panel h3 .sm{ font-family:'IBM Plex Mono',monospace; font-size:11px; color:var(--text-dim); font-weight:400; margin-left:6px;}

  .timeline{ display:flex; height:40px; border-radius:8px; overflow:hidden; margin-bottom:10px; background:var(--surface-2); }
  .timeline .seg{ height:100%; position:relative; min-width:2px; }
  .timeline-axis{ display:flex; justify-content:space-between; font-family:'IBM Plex Mono',monospace; font-size:10px; color:var(--text-dim); }
  .legend{ display:flex; flex-wrap:wrap; gap:10px; margin-top:14px; }
  .legend-item{ display:flex; align-items:center; gap:6px; font-size:12px; color:var(--text-dim); }
  .legend-dot{ width:8px; height:8px; border-radius:50%; }

  .empty{ text-align:center; padding:40px 10px; color:var(--text-dim); }
  .empty .big{ font-family:'Fraunces',serif; font-size:16px; color:var(--text); margin-bottom:6px; }

  /* history */
  .hist-row{
    display:flex; align-items:center; justify-content:space-between; gap:12px;
    padding:13px 16px; border-radius:12px; background:var(--surface); border:1px solid var(--border);
    margin-bottom:8px; cursor:pointer; transition: border-color .15s;
  }
  .hist-row:hover{ border-color: var(--gold-dim); }
  .hist-left{ display:flex; align-items:center; gap:12px; }
  .hist-date{ font-family:'IBM Plex Mono',monospace; font-size:12.5px; color:var(--text); width:104px; flex-shrink:0;}
  .hist-bar{ display:flex; height:8px; width:150px; border-radius:5px; overflow:hidden; background:var(--surface-2);}
  .hist-right{ display:flex; align-items:center; gap:14px; }
  .hist-hours{ font-family:'IBM Plex Mono',monospace; font-size:12.5px; color:var(--text-dim); }
  .del-btn{ background:none; color:var(--text-dim); font-size:15px; line-height:1; padding:4px; }
  .del-btn:hover{ color:var(--red); }

  .day-detail{ margin-top:6px; padding:14px 16px 4px; }
  .act-row{ display:flex; align-items:center; gap:10px; padding:7px 0; border-bottom:1px dashed var(--border); font-size:13px; }
  .act-row:last-child{ border-bottom:none; }
  .act-time{ font-family:'IBM Plex Mono',monospace; color:var(--text-dim); width:64px; flex-shrink:0; font-size:12px;}
  .act-dot{ width:8px; height:8px; border-radius:50%; flex-shrink:0; }
  .act-dur{ margin-left:auto; font-family:'IBM Plex Mono',monospace; font-size:11.5px; color:var(--text-dim); }

  .section-title{ font-size:13px; text-transform:uppercase; letter-spacing:0.08em; color:var(--text-dim); margin:6px 0 12px; }

  @media (max-width: 860px){
    .shell{ flex-direction:column; }
    .sidebar{ width:100%; height:auto; position:relative; flex-direction:row; flex-wrap:wrap; padding:16px; }
    .sidebar-foot{ display:none; }
    .nav{ flex-direction:row; flex-wrap:wrap; }
    .jump{ width:100%; margin-top:10px; }
    .main{ padding:22px 18px 60px; }
    .stats{ grid-template-columns:1fr 1fr; }
    .viz-row{ grid-template-columns:1fr; }
  }
</style>
</head>
<body>
<div id="root"></div>

<script>
/* ============================= DATA / CATEGORIES ============================= */
const CATEGORIES = {
  rest:          { label:'Sleep & Rest',  color:'#9585B8', keywords:['sleep','nap','wake','rest','woke up','wake up','bed'] },
  study:         { label:'Study & Work',  color:'#6F91A8', keywords:['study','work','class','office','meeting','code','coding','homework','assignment','exam','project','lecture','read','reading','write','writing','client','deploy','debug'] },
  food:          { label:'Food',          color:'#DD8468', keywords:['lunch','dinner','breakfast','eat','food','snack','meal','brunch','cook'] },
  exercise:      { label:'Exercise',      color:'#7FA07C', keywords:['gym','workout','exercise','walk','run','yoga','sport','jog','cricket','football','swim','stretch'] },
  entertainment: { label:'Entertainment', color:'#C97B94', keywords:['reel','scroll','instagram','tiktok','youtube','movie','tv','netflix','game','gaming','social media','phone','music','drama','chill','relax'] },
  commute:       { label:'Commute',       color:'#B5824F', keywords:['travel','commute','drive','driving','bus','ride','uber','transport'] },
  social:        { label:'Social',        color:'#5E9C93', keywords:['friend','family','hangout','party','call','chat','meet','visit'] },
  other:         { label:'Other',         color:'#7D7689', keywords:[] }
};
const CAT_ORDER = ['rest','study','food','exercise','entertainment','commute','social','other'];

function categorize(desc){
  const d = (desc||'').toLowerCase();
  for(const key of CAT_ORDER){
    if(key==='other') continue;
    if(CATEGORIES[key].keywords.some(k=>d.includes(k))) return key;
  }
  return 'other';
}

function parseAndBuildActivities(text){
  const segments = text.split(/,|\band\b/i).map(s=>s.trim()).filter(Boolean);
  const timeRe = /(\d{1,2})(?::(\d{2}))?\s*(am|pm)?/i;
  const items = segments.map(seg=>{
    const m = seg.match(timeRe);
    let timeMinutes = null, desc = seg;
    if(m){
      let hour = parseInt(m[1],10);
      const minute = m[2] ? parseInt(m[2],10) : 0;
      const mer = m[3] ? m[3].toLowerCase() : null;
      if(mer==='pm' && hour<12) hour += 12;
      if(mer==='am' && hour===12) hour = 0;
      if(!mer && hour>=1 && hour<=6) hour += 12; // bare small numbers -> assume afternoon/evening
      if(hour>=24) hour = 23;
      timeMinutes = hour*60+minute;
      desc = (seg.slice(0,m.index)+seg.slice(m.index+m[0].length)).trim();
      desc = desc.replace(/^(am|pm)\b/i,'').replace(/^[-:]+/,'').trim();
    }
    return { raw:seg, timeMinutes, desc: desc || seg, category: categorize(desc||seg) };
  });
  const timed = items.filter(i=>i.timeMinutes!==null).sort((a,b)=>a.timeMinutes-b.timeMinutes);
  const untimed = items.filter(i=>i.timeMinutes===null);
  const activities = [];
  for(let i=0;i<timed.length;i++){
    const cur = timed[i], next = timed[i+1];
    let duration = next ? Math.max(15, next.timeMinutes - cur.timeMinutes)
                         : Math.min(120, Math.max(30, 24*60 - cur.timeMinutes));
    activities.push({...cur, durationMin: duration});
  }
  untimed.forEach(u => activities.push({...u, durationMin:60}));
  return activities;
}

function addLogToDay(data, dateStr, text){
  const activities = parseAndBuildActivities(text);
  const entry = data.entries[dateStr] || { logs:[], activities:[] };
  entry.logs.push({ text, loggedAt: new Date().toISOString() });
  entry.activities = entry.activities.concat(activities);
  entry.categoryTotals = {};
  entry.totalMin = 0;
  entry.activities.forEach(a=>{
    entry.categoryTotals[a.category] = (entry.categoryTotals[a.category]||0) + a.durationMin;
    entry.totalMin += a.durationMin;
  });
  data.entries[dateStr] = entry;
  return activities;
}

/* ============================= DATE HELPERS ============================= */
function fmtDate(d){
  const y=d.getFullYear(), m=String(d.getMonth()+1).padStart(2,'0'), day=String(d.getDate()).padStart(2,'0');
  return `${y}-${m}-${day}`;
}
function parseDateStr(s){ const [y,m,d]=s.split('-').map(Number); return new Date(y,m-1,d); }
function todayStr(){ return fmtDate(new Date()); }
function niceDate(s){ return parseDateStr(s).toLocaleDateString(undefined,{weekday:'short',month:'short',day:'numeric'}); }
function niceDateLong(s){ return parseDateStr(s).toLocaleDateString(undefined,{weekday:'long',month:'long',day:'numeric',year:'numeric'}); }
function minToHrs(min){ return (min/60); }
function fmtHrs(min){ return (min/60).toFixed(1)+'h'; }
function fmtTime(mins){
  if(mins==null) return '--:--';
  let h = Math.floor(mins/60), m = mins%60;
  const mer = h>=12 ? 'PM':'AM';
  let hh = h%12; if(hh===0) hh=12;
  return `${hh}:${String(m).padStart(2,'0')} ${mer}`;
}
function weekRange(anchor){
  const d = parseDateStr(anchor);
  const day = (d.getDay()+6)%7; // Monday=0
  const start = new Date(d); start.setDate(d.getDate()-day);
  const dates = []; for(let i=0;i<7;i++){ const x=new Date(start); x.setDate(start.getDate()+i); dates.push(fmtDate(x)); }
  return dates;
}
function monthRange(anchor){
  const d = parseDateStr(anchor);
  const first = new Date(d.getFullYear(), d.getMonth(), 1);
  const daysIn = new Date(d.getFullYear(), d.getMonth()+1, 0).getDate();
  const dates = []; for(let i=0;i<daysIn;i++){ const x=new Date(first); x.setDate(1+i); dates.push(fmtDate(x)); }
  return dates;
}
function monthLabel(anchor){ return parseDateStr(anchor).toLocaleDateString(undefined,{month:'long',year:'numeric'}); }
function yearMonths(anchor){
  const y = parseDateStr(anchor).getFullYear();
  const buckets = [];
  for(let m=0;m<12;m++){
    const daysIn = new Date(y, m+1, 0).getDate();
    const dates = []; for(let i=1;i<=daysIn;i++) dates.push(fmtDate(new Date(y,m,i)));
    buckets.push({ label: new Date(y,m,1).toLocaleDateString(undefined,{month:'short'}), dates });
  }
  return buckets;
}

/* ============================= STORAGE ============================= */
const STORE_KEY = 'daylog-data';
let DATA = { profile:null, entries:{} };
let STORAGE_READY = false;

async function loadData(){
  try{
    const res = await window.storage.get(STORE_KEY);
    if(res && res.value) DATA = JSON.parse(res.value);
  }catch(e){ /* no existing data yet */ }
  STORAGE_READY = true;
}
async function persist(){
  try{ await window.storage.set(STORE_KEY, JSON.stringify(DATA)); }
  catch(e){ console.error('Storage error', e); }
}

/* ============================= APP STATE ============================= */
let STATE = { view:'today', anchor: todayStr(), draft:'', expandedDate:null, loading:true };

function setState(patch){ STATE = {...STATE, ...patch}; render(); }

/* ============================= RENDER HELPERS ============================= */
function iconFor(view){
  const icons = {
    today:  '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><rect x="3" y="5" width="18" height="16" rx="3"/><path d="M3 10h18M8 3v4M16 3v4"/></svg>',
    week:   '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><rect x="3" y="5" width="18" height="16" rx="3"/><path d="M3 10h18M8 3v4M16 3v4M7 14h2M11 14h2M15 14h2M7 17h2M11 17h2"/></svg>',
    month:  '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><rect x="3" y="5" width="18" height="16" rx="3"/><path d="M3 10h18M8 3v4M16 3v4"/><circle cx="8" cy="14" r="1" fill="currentColor" stroke="none"/><circle cx="12" cy="14" r="1" fill="currentColor" stroke="none"/><circle cx="16" cy="14" r="1" fill="currentColor" stroke="none"/><circle cx="8" cy="17" r="1" fill="currentColor" stroke="none"/></svg>',
    year:   '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M4 19V9l8-6 8 6v10"/><path d="M9 19v-6h6v6"/></svg>'
  };
  return icons[view]||icons.today;
}

function statsFor(dates){
  const totals = {}; let totalMin=0; let daysLogged=0;
  const daily = [];
  dates.forEach(dt=>{
    const e = DATA.entries[dt];
    let dayMin = 0;
    if(e){
      daysLogged++;
      Object.entries(e.categoryTotals||{}).forEach(([k,v])=>{ totals[k]=(totals[k]||0)+v; dayMin+=v; });
      totalMin += e.totalMin||0;
    }
    daily.push({ date:dt, min:dayMin });
  });
  let topCat=null, topVal=-1;
  Object.entries(totals).forEach(([k,v])=>{ if(v>topVal){ topVal=v; topCat=k; } });
  return { totals, totalMin, daysLogged, daily, topCat };
}

function catChip(cat, extra){
  const c = CATEGORIES[cat];
  return `<span class="chip" style="background:${c.color}">${c.label}${extra?` · ${extra}`:''}</span>`;
}

/* ============================= CHARTS (dependency-free SVG/CSS) ============================= */
function doughnutSvg(totals, size, strokeWidth){
  const entries = CAT_ORDER.filter(k=>totals[k]).map(k=>({ k, v:totals[k], color:CATEGORIES[k].color }));
  const total = entries.reduce((s,e)=>s+e.v,0);
  if(total<=0) return '';
  const r = (size - strokeWidth)/2;
  const c = 2*Math.PI*r;
  let offsetFrac = 0;
  const circles = entries.map(e=>{
    const frac = e.v/total;
    const dash = Math.max(0, frac*c - (entries.length>1?1.5:0)); // tiny gap between segments
    const gap = c - dash;
    const rotate = offsetFrac*360 - 90;
    offsetFrac += frac;
    return `<circle cx="${size/2}" cy="${size/2}" r="${r}" fill="none" stroke="${e.color}" stroke-width="${strokeWidth}" stroke-dasharray="${dash} ${gap}" stroke-linecap="round" transform="rotate(${rotate} ${size/2} ${size/2})"/>`;
  }).join('');
  return `<svg width="${size}" height="${size}" viewBox="0 0 ${size} ${size}">
      ${circles}
      <text x="${size/2}" y="${size/2-2}" text-anchor="middle" fill="#EFE8DD" font-family="IBM Plex Mono, monospace" font-size="19" font-weight="600">${(total/60).toFixed(1)}h</text>
      <text x="${size/2}" y="${size/2+17}" text-anchor="middle" fill="#B0A6BE" font-family="Inter, sans-serif" font-size="10">logged</text>
    </svg>`;
}

function barChartHtml(daily, labelFmt, height){
  height = height || 170;
  const max = Math.max(1, ...daily.map(d=>d.min));
  return `<div style="display:flex;align-items:flex-end;gap:${daily.length>20?3:7}px;height:${height}px;">
    ${daily.map(d=>{
      const h = d.min>0 ? Math.max(4,(d.min/max)*(height-22)) : 2;
      return `<div style="flex:1;display:flex;flex-direction:column;align-items:center;justify-content:flex-end;height:100%;min-width:0;">
        <div title="${fmtHrs(d.min)}" style="width:100%;max-width:28px;height:${h}px;background:${d.min>0?'var(--gold)':'var(--surface-2)'};border-radius:5px 5px 2px 2px;"></div>
        <div class="mono" style="font-size:${daily.length>20?'8px':'9.5px'};color:var(--text-dim);margin-top:6px;white-space:nowrap;">${labelFmt(d)}</div>
      </div>`;
    }).join('')}
  </div>`;
}

/* ============================= SCREENS ============================= */
function renderAuth(){
  const root = document.getElementById('root');
  root.innerHTML = `
    <div class="auth-wrap">
      <div class="auth-card">
        <div class="auth-brand"><span class="auth-mark"></span>DayLog</div>
        <div class="auth-tag">Turn your day into data. Talk to it like a notebook.</div>
        <div class="field">
          <label>Your name</label>
          <input id="nameInput" type="text" placeholder="e.g. Zobi" autocomplete="off" />
        </div>
        <button class="auth-btn" id="beginBtn">Begin logging →</button>
        <div class="auth-note">Saved privately to your account here in Claude. For a shareable, multi-device version, this screen would sit in front of a real login backed by Supabase — happy to help scaffold that separately.</div>
      </div>
    </div>
  `;
  const nameInput = document.getElementById('nameInput');
  const begin = async ()=>{
    const name = nameInput.value.trim();
    if(!name) { nameInput.style.borderBottomColor='#C1503D'; nameInput.focus(); return; }
    DATA.profile = { name };
    await persist();
    render();
  };
  document.getElementById('beginBtn').addEventListener('click', begin);
  nameInput.addEventListener('keydown', e=>{ if(e.key==='Enter') begin(); });
  nameInput.focus();
}

function navItems(){
  return [
    {k:'today', label:'Today'},
    {k:'week', label:'This Week'},
    {k:'month', label:'This Month'},
    {k:'year', label:'This Year'},
  ];
}

function renderShellFrame(bodyHtml){
  const root = document.getElementById('root');
  const initials = DATA.profile.name.trim().slice(0,1).toUpperCase();
  root.innerHTML = `
    <div class="shell">
      <div class="sidebar">
        <div class="brand"><span class="dot"></span><span>DayLog</span></div>
        <div class="nav-label">Overview</div>
        <div class="nav">
          ${navItems().map(n=>`
            <button class="nav-item ${STATE.view===n.k?'active':''}" data-view="${n.k}">
              ${iconFor(n.k)}<span>${n.label}</span>
            </button>`).join('')}
        </div>
        <hr/>
        <div class="jump">
          <label>Jump to a date</label>
          <div class="jump-row">
            <input type="date" id="jumpDate" value="${STATE.expandedDate||todayStr()}" max="${todayStr()}" />
            <button id="jumpGo">Go</button>
          </div>
        </div>
        <div class="sidebar-foot">
          <div class="who"><span class="avatar">${initials}</span><span>${DATA.profile.name}</span></div>
          <button class="signout" id="signoutBtn">Sign out</button>
        </div>
      </div>
      <div class="main">${bodyHtml}</div>
    </div>
  `;
  navItems().forEach(n=>{
    document.querySelector(`.nav-item[data-view="${n.k}"]`).addEventListener('click', ()=>{
      setState({ view:n.k, anchor: todayStr() });
    });
  });
  document.getElementById('jumpGo').addEventListener('click', ()=>{
    const v = document.getElementById('jumpDate').value;
    if(v) setState({ view:'today', anchor:v });
  });
  document.getElementById('signoutBtn').addEventListener('click', ()=>{
    DATA.profile = null; persist(); render();
  });
}

function renderTodayView(){
  const dt = STATE.anchor;
  const entry = DATA.entries[dt];
  const isToday = dt===todayStr();
  const dayLabel = isToday ? "Today" : niceDateLong(dt);
  const greetHour = new Date().getHours();
  const greet = greetHour<12?'Good morning':greetHour<18?'Good afternoon':'Good evening';

  let body = `
    <div class="header">
      <div><h1>${isToday? `${greet}, ${DATA.profile.name.split(' ')[0]}` : dayLabel}</h1></div>
      <div class="datebox"><div class="date mono">${niceDateLong(dt)}</div></div>
    </div>
    <div class="ledger">
      <div class="ledger-label">${isToday? "Tell the bot how your day's going" : "Add to this day's log"}</div>
      <textarea id="draftInput" placeholder="e.g. 7am woke up, 9 study, 1pm lunch, 4 gym, 8pm reel scrolling...">${STATE.draft||''}</textarea>
      <div class="ledger-actions">
        <div class="ledger-hint">Separate activities with commas — a rough time helps it split your hours accurately.</div>
        <button class="log-btn" id="logBtn">Log it ↵</button>
      </div>
    </div>
  `;

  if(entry && entry.logs.length){
    body += `<div class="thread">` + entry.logs.map(l=>{
      const time = new Date(l.loggedAt).toLocaleTimeString(undefined,{hour:'numeric',minute:'2-digit'});
      const acts = parseAndBuildActivities(l.text);
      return `<div class="bubble">
        <div class="t mono">logged at ${time}</div>
        <div>${l.text}</div>
        <div class="chips">${acts.map(a=>catChip(a.category, fmtTime(a.timeMinutes))).join('')}</div>
      </div>`;
    }).join('') + `</div>`;
  }

  const stats = statsFor([dt]);
  body += `
    <div class="stats">
      <div class="stat"><div class="label">Hours logged</div><div class="value mono">${fmtHrs(stats.totalMin)}</div><div class="sub">${entry?entry.activities.length:0} activities</div></div>
      <div class="stat"><div class="label">Top category</div><div class="value" style="font-size:18px; font-family:'Fraunces',serif;">${stats.topCat?CATEGORIES[stats.topCat].label:'—'}</div><div class="sub">${stats.topCat?fmtHrs(stats.totals[stats.topCat]):''}</div></div>
      <div class="stat"><div class="label">Entries today</div><div class="value mono">${entry?entry.logs.length:0}</div><div class="sub">times you checked in</div></div>
    </div>
  `;

  if(entry && entry.activities.length){
    body += `
      <div class="viz-row">
        <div class="panel">
          <h3>Category breakdown</h3>
          <div style="display:flex;justify-content:center;align-items:center;height:190px;">${doughnutSvg(stats.totals, 168, 22)}</div>
          <div class="legend">${CAT_ORDER.filter(k=>stats.totals[k]).map(k=>`<div class="legend-item"><span class="legend-dot" style="background:${CATEGORIES[k].color}"></span>${CATEGORIES[k].label} · ${fmtHrs(stats.totals[k])}</div>`).join('')}</div>
        </div>
        <div class="panel">
          <h3>Day timeline<span class="sm">${entry.activities.length} logged</span></h3>
          <div class="timeline">
            ${entry.activities.filter(a=>a.timeMinutes!=null).sort((a,b)=>a.timeMinutes-b.timeMinutes).map(a=>
              `<div class="seg" title="${a.desc} (${fmtTime(a.timeMinutes)}, ${fmtHrs(a.durationMin)})" style="width:${(a.durationMin/(24*60)*100).toFixed(2)}%; background:${CATEGORIES[a.category].color}"></div>`
            ).join('')}
          </div>
          <div class="timeline-axis"><span>12 AM</span><span>6 AM</span><span>12 PM</span><span>6 PM</span><span>12 AM</span></div>
          <div class="day-detail">
            ${entry.activities.slice().sort((a,b)=>(a.timeMinutes??9999)-(b.timeMinutes??9999)).map(a=>`
              <div class="act-row">
                <span class="act-time">${fmtTime(a.timeMinutes)}</span>
                <span class="act-dot" style="background:${CATEGORIES[a.category].color}"></span>
                <span>${a.desc}</span>
                <span class="act-dur">${fmtHrs(a.durationMin)}</span>
              </div>`).join('')}
          </div>
        </div>
      </div>
    `;
  } else {
    body += `<div class="panel empty"><div class="big">Nothing logged for this day yet</div>Tell the bot above what you got up to and it'll build the breakdown.</div>`;
  }

  body += renderHistory();
  renderShellFrame(body);

  const draftEl = document.getElementById('draftInput');
  draftEl.addEventListener('input', e=>{ STATE.draft = e.target.value; });
  const submit = async ()=>{
    const text = draftEl.value.trim();
    if(!text) return;
    addLogToDay(DATA, dt, text);
    STATE.draft='';
    await persist();
    render();
  };
  document.getElementById('logBtn').addEventListener('click', submit);
  draftEl.addEventListener('keydown', e=>{ if(e.key==='Enter' && (e.metaKey||e.ctrlKey)) submit(); });

  wireHistory();
}

function renderPeriodView(kind){
  let dates, title, labelFmt, anchorLabel;
  if(kind==='week'){
    dates = weekRange(STATE.anchor);
    anchorLabel = `${niceDate(dates[0])} – ${niceDate(dates[6])}`;
    title = 'This Week';
    labelFmt = d=>parseDateStr(d.date).toLocaleDateString(undefined,{weekday:'short'});
  } else if(kind==='month'){
    dates = monthRange(STATE.anchor);
    anchorLabel = monthLabel(STATE.anchor);
    title = 'This Month';
    labelFmt = d=>parseDateStr(d.date).getDate();
  } else {
    const buckets = yearMonths(STATE.anchor);
    dates = buckets.flatMap(b=>b.dates);
    anchorLabel = parseDateStr(STATE.anchor).getFullYear();
    title = 'This Year';
  }

  let daily, statsAll;
  if(kind==='year'){
    const buckets = yearMonths(STATE.anchor);
    daily = buckets.map(b=>{
      const s = statsFor(b.dates);
      return { date:b.label, min:s.totalMin };
    });
    statsAll = statsFor(dates);
    labelFmt = d=>d.date;
  } else {
    statsAll = statsFor(dates);
    daily = statsAll.daily;
  }

  let body = `
    <div class="header">
      <div><h1>${title}</h1></div>
      <div class="datebox"><div class="date mono">${anchorLabel}</div></div>
    </div>
    <div class="stats">
      <div class="stat"><div class="label">Hours logged</div><div class="value mono">${fmtHrs(statsAll.totalMin)}</div><div class="sub">across ${statsAll.daysLogged} of ${dates.length} days</div></div>
      <div class="stat"><div class="label">Top category</div><div class="value" style="font-size:18px; font-family:'Fraunces',serif;">${statsAll.topCat?CATEGORIES[statsAll.topCat].label:'—'}</div><div class="sub">${statsAll.topCat?fmtHrs(statsAll.totals[statsAll.topCat]):''}</div></div>
      <div class="stat"><div class="label">Daily average</div><div class="value mono">${statsAll.daysLogged? fmtHrs(statsAll.totalMin/statsAll.daysLogged) : '0.0h'}</div><div class="sub">on days you logged</div></div>
    </div>
  `;

  if(statsAll.totalMin>0){
    body += `
      <div class="viz-row">
        <div class="panel">
          <h3>Category breakdown</h3>
          <div style="display:flex;justify-content:center;align-items:center;height:190px;">${doughnutSvg(statsAll.totals, 168, 22)}</div>
          <div class="legend">${CAT_ORDER.filter(k=>statsAll.totals[k]).map(k=>`<div class="legend-item"><span class="legend-dot" style="background:${CATEGORIES[k].color}"></span>${CATEGORIES[k].label} · ${fmtHrs(statsAll.totals[k])}</div>`).join('')}</div>
        </div>
        <div class="panel">
          <h3>${kind==='year' ? 'Hours per month' : 'Hours per day'}</h3>
          <div style="height:190px;">${barChartHtml(daily, kind==='year' ? d=>d.date : labelFmt, 168)}</div>
        </div>
      </div>
    `;
  } else {
    body += `<div class="panel empty"><div class="big">No logs in this period yet</div>Head to Today to start your ledger.</div>`;
  }

  body += `<div class="section-title">Days in this period</div>`;
  const relevantDates = kind==='year' ? [] : dates;
  if(kind==='year'){
    const buckets = yearMonths(STATE.anchor);
    body += buckets.map(b=>{
      const s = statsFor(b.dates);
      if(s.totalMin===0) return '';
      return historyRowHtml(b.dates[0].slice(0,7)+'-01', s, true, b.label);
    }).join('') || `<div class="panel empty" style="padding:24px;">Nothing logged yet.</div>`;
  } else {
    const rows = relevantDates.filter(d=>DATA.entries[d]).slice().reverse();
    body += rows.length ? rows.map(d=>historyRowHtml(d, statsFor([d]))).join('') : `<div class="panel empty" style="padding:24px;">Nothing logged yet.</div>`;
  }

  renderShellFrame(body);
  wireHistory();
}

function historyRowHtml(dt, stats, isMonthAgg, monthLabelText){
  const segs = CAT_ORDER.filter(k=>stats.totals[k]).map(k=>
    `<span style="display:inline-block;height:100%;width:${(stats.totals[k]/stats.totalMin*100).toFixed(1)}%;background:${CATEGORIES[k].color}"></span>`
  ).join('');
  const label = isMonthAgg ? monthLabelText : niceDate(dt);
  return `
    <div class="hist-row" data-date="${dt}" data-agg="${isMonthAgg?'1':'0'}">
      <div class="hist-left">
        <div class="hist-date">${label}</div>
        <div class="hist-bar">${segs}</div>
      </div>
      <div class="hist-right">
        <div class="hist-hours">${fmtHrs(stats.totalMin)}</div>
        ${isMonthAgg ? '' : `<button class="del-btn" data-del="${dt}" title="Delete this day's log">×</button>`}
      </div>
    </div>
  `;
}

function renderHistory(){
  const dates = Object.keys(DATA.entries).sort().reverse().filter(d=>d!==STATE.anchor);
  if(!dates.length) return '';
  return `<div class="section-title">Previous days</div>` +
    dates.slice(0,14).map(d=>historyRowHtml(d, statsFor([d]))).join('');
}

function wireHistory(){
  document.querySelectorAll('.hist-row').forEach(row=>{
    row.addEventListener('click', (e)=>{
      if(e.target.dataset.del) return;
      const dt = row.dataset.date;
      const isAgg = row.dataset.agg==='1';
      if(isAgg){ setState({ view:'month', anchor: dt }); }
      else{ setState({ view:'today', anchor: dt }); }
    });
  });
  document.querySelectorAll('.del-btn').forEach(btn=>{
    btn.addEventListener('click', async (e)=>{
      e.stopPropagation();
      const dt = btn.dataset.del;
      if(confirm(`Delete the log for ${niceDate(dt)}? This can't be undone.`)){
        delete DATA.entries[dt];
        await persist();
        render();
      }
    });
  });
}

/* ============================= ROOT RENDER ============================= */
function render(){
  if(!STORAGE_READY){
    document.getElementById('root').innerHTML = `<div class="auth-wrap"><div style="color:#B0A6BE; font-family:'IBM Plex Mono',monospace; font-size:13px;">loading your ledger…</div></div>`;
    return;
  }
  if(!DATA.profile){ renderAuth(); return; }
  if(STATE.view==='today') renderTodayView();
  else renderPeriodView(STATE.view);
}

/* ============================= BOOT ============================= */
(async function boot(){
  await loadData();
  render();
})();
</script>
</body>
</html>

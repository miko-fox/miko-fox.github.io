<!DOCTYPE html>

<html lang="ru">
<head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1" name="viewport"/>
<title>Лисий культ — Досье № засекречено</title>
<style>
:root {
  --site-primary: #a51f1f;
  --site-secondary: #222222;
  --site-background: #080909;
  --site-on-primary: #ffffff;
  --site-on-secondary: #f1eee8;
  --site-on-background: #f1eee8;
  --site-font-body: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  --site-font-heading: "Arial Narrow", Impact, Haettenschweiler, sans-serif;
  --site-heading-scale: 1;
  --site-spacing-scale: 1;
  --site-radius-scale: 1;
  --site-decoration-opacity: 1;
  --ink: #f1eee8;
  --muted: #9c9b95;
  --red: #e33a30;
  --paper: #e9e1cf;
  --paper-ink: #1b1b18;
}
* { box-sizing: border-box; }
html, body { margin: 0; min-height: 100%; background: var(--site-background); color: var(--ink); font-family: var(--site-font-body); }
body { overflow: hidden; }
button { font: inherit; }
#app { background-color: light-dark(var(--site-background), var(--site-background)); color: var(--site-on-background); width: 100%; height: 100dvh; min-height: 540px; position: relative; overflow: hidden; border-radius: 0; isolation: isolate; }
#app::before { content:""; position:absolute; inset:0; pointer-events:none; opacity:calc(.16 * var(--site-decoration-opacity)); z-index:10; background-image: repeating-linear-gradient(0deg, transparent 0px, transparent 3px, rgba(255,255,255,.05) 4px); mix-blend-mode:screen; }
#app::after { content:""; position:absolute; inset:0; pointer-events:none; opacity:calc(.18 * var(--site-decoration-opacity)); z-index:10; background:radial-gradient(ellipse at center, transparent 35%, #000 100%); }
.deck { height:100%; position:relative; }
.slide { position:absolute; inset:0; padding:clamp(24px,5vw,72px) clamp(24px,7vw,100px) 90px; display:flex; flex-direction:column; justify-content:center; opacity:0; transform:translateX(22px) scale(.99); pointer-events:none; transition:opacity .45s ease, transform .45s ease; overflow:auto; scrollbar-width:thin; scrollbar-color:#555 transparent; }
.slide.active { opacity:1; transform:none; pointer-events:auto; z-index:2; }
.slide::before { content:attr(data-index); position:absolute; top:24px; right:clamp(24px,4vw,60px); font:700 12px/1 monospace; letter-spacing:.18em; color:#7a7a73; }
.eyebrow { display:flex; align-items:center; gap:12px; text-transform:uppercase; font:700 11px/1.4 monospace; letter-spacing:.2em; color:var(--red); margin-bottom:20px; }
.eyebrow::before { content:""; width:28px; height:2px; background:var(--red); }
h1,h2,h3,p { margin-top:0; }
h1,h2,h3 { font-family:var(--site-font-heading); text-transform:uppercase; letter-spacing:.015em; }
h1 { font-size:clamp(54px,10vw,140px); line-height:.86; margin-bottom:24px; font-weight:900; }
h2 { font-size:clamp(38px,6vw,76px); line-height:.95; margin-bottom:22px; }
h3 { font-size:clamp(22px,3vw,34px); line-height:1; margin-bottom:14px; }
p { color:#d0cec7; font-size:clamp(14px,1.45vw,18px); line-height:1.62; max-width:880px; }
.lead { font-size:clamp(17px,2vw,24px); line-height:1.5; max-width:780px; }
.muted { color:var(--muted); }
.red { color:var(--red); }
.mono { font-family:ui-monospace,SFMono-Regular,Menlo,monospace; }
.stamp { display:inline-block; border:2px solid var(--red); color:var(--red); padding:9px 13px; font:900 13px/1 monospace; letter-spacing:.14em; transform:rotate(-4deg); }
.cover { background:radial-gradient(ellipse at 50% 45%,#151515 0%,#050505 60%); align-items:center; text-align:center; }
.cover h1 { text-shadow:3px 0 rgba(227,58,48,.28),-3px 0 rgba(60,140,180,.18); }
.cover .tiny { color:#73736e; font:11px monospace; letter-spacing:.2em; }
.glitch { animation:glitch 7s infinite steps(1); }
@keyframes glitch { 0%,94%,97%,100% {transform:translate(0); text-shadow:none} 95% {transform:translate(1.5px,-0.5px);text-shadow:-1.5px 0 #e33a30} 96% {transform:translate(-1px,0.5px);text-shadow:1.5px 0 #65b9d4} }
.noise-screen { position:absolute; inset:0; opacity:.07; pointer-events:none; background-image:url("data:image/svg+xml,%3Csvg viewBox='0 0 180 180' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='.75' numOctaves='2' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='.7'/%3E%3C/svg%3E"); animation:noise 1.8s steps(3) infinite; }
@keyframes noise { 0%{transform:translate(0)} 33%{transform:translate(-0.6%,0.3%)} 66%{transform:translate(0.4%,-0.4%)} 100%{transform:translate(0)} }
.scanline { position:absolute; top:-20%; left:0; right:0; height:60px; background:linear-gradient(transparent,rgba(255,255,255,.035),transparent); animation:scan 14s linear infinite; pointer-events:none; }
@keyframes scan { to { top:120%; } }
.case-title { display:flex; align-items:flex-start; gap:clamp(20px,4vw,58px); }
.case-number { font:900 clamp(55px,9vw,120px)/.8 monospace; color:transparent; -webkit-text-stroke:1px #5d5b56; }
.case-meta { border-top:1px solid #343431; border-bottom:1px solid #343431; display:flex; gap:24px; flex-wrap:wrap; padding:14px 0; margin-top:22px; font:11px monospace; color:#96958e; letter-spacing:.08em; }
.grid2 { display:grid; grid-template-columns:1fr 1fr; gap:clamp(18px,3vw,38px); align-items:center; }
.evidence-grid { display:grid; grid-template-columns:repeat(2,minmax(0,1fr)); gap:12px; margin-top:16px; }
.evidence-card { border:1px solid #353531; background:linear-gradient(135deg,rgba(255,255,255,.045),rgba(255,255,255,.012)); padding:clamp(14px,2vw,23px); position:relative; min-height:160px; }
.evidence-card::after { content:"EVIDENCE"; position:absolute; top:12px; right:12px; font:9px monospace; letter-spacing:.15em; color:#686862; }

.evidence-card h3 { font-size:clamp(19px,2.3vw,28px); padding-right:38px; }
.evidence-card p { font-size:clamp(12px,1.1vw,14px); line-height:1.5; margin-bottom:0; }
.evidence-card .interpret { color:#e4b3ad; margin-top:9px; }
.evidence-card.wide { grid-column:1 / -1; min-height:130px; }
.redline { display:inline; background:var(--red); color:white; padding:2px 6px; font:900 12px monospace; letter-spacing:.08em; }
.fake-art { min-height:250px; height:100%; position:relative; overflow:hidden; border:1px solid #383833; background:radial-gradient(circle at 50% 48%,#4a2417,#111 55%,#080808); display:flex; align-items:center; justify-content:center; }
.fox-svg { width:min(100%,350px); max-height:360px; filter:drop-shadow(0 15px 28px rgba(0,0,0,.7)); }
.art-label { position:absolute; left:14px; bottom:12px; color:#a8a59b; font:10px monospace; letter-spacing:.12em; }
.red-circle { position:absolute; border:2px solid var(--red); border-radius:50%; width:92px; height:92px; right:27%; top:26%; box-shadow:0 0 0 5px rgba(227,58,48,.08); }
.city-art { background:linear-gradient(#10151b,#161717); }
.city-art svg { width:100%; height:100%; position:absolute; inset:0; }
.chart-box { border:1px solid #3a3934; background:#101110; padding:18px; }
.chart-title { display:flex; justify-content:space-between; gap:12px; font:11px monospace; color:#a6a49c; margin-bottom:12px; }
.chart-box svg { width:100%; height:auto; display:block; }
.graph-line { stroke-dasharray:800; stroke-dashoffset:800; animation:draw 2.2s .4s ease forwards; }
@keyframes draw { to {stroke-dashoffset:0;} }
.paper-wrap { background:#151513; padding:clamp(12px,2.5vw,30px); border:1px solid #353530; box-shadow:0 18px 60px #0009; max-width:980px; margin:auto; width:100%; }
.paper { background:var(--paper); color:var(--paper-ink); padding:clamp(22px,4vw,48px); position:relative; font-family:Georgia,"Times New Roman",serif; transform:rotate(-.25deg); box-shadow:inset 0 0 45px #6f62451a; }
.paper::before { content:""; position:absolute; inset:9px; border:1px solid #4c483b; pointer-events:none; }
.paper-top { display:flex; justify-content:space-between; gap:18px; align-items:flex-start; border-bottom:2px solid #282720; padding-bottom:13px; margin-bottom:18px; }
.paper-kicker { font:700 10px/1.5 monospace; letter-spacing:.08em; max-width:62%; }
.paper h2 { font-family:Georgia,serif; font-size:clamp(24px,4vw,43px); letter-spacing:0; line-height:1; margin:10px 0; }
.paper p { color:#282720; font:clamp(12px,1.3vw,15px)/1.5 Georgia,serif; margin-bottom:10px; }
.paper .section-label { font:bold 11px monospace; text-transform:uppercase; border-bottom:1px solid #77705d; padding-bottom:5px; margin:18px 0 10px; }
.paper .seal { border:3px double #a52822; color:#a52822; padding:9px 12px; font:900 11px monospace; transform:rotate(8deg); white-space:nowrap; }
.paper .recommend { border:2px solid #a52822; padding:9px 12px; font-weight:bold; }
.paper-foot { display:flex; justify-content:space-between; gap:12px; margin-top:18px; padding-top:10px; border-top:1px solid #77705d; color:#5a5548; font:9px monospace; }
.versions { display:grid; grid-template-columns:repeat(3,1fr); gap:14px; margin-top:12px; }
.version { padding:22px 20px; border:1px solid #383833; background:#111210; position:relative; min-height:245px; }
.version .letter { font:900 56px/.9 monospace; color:#5b2824; margin-bottom:20px; }
.version h3 { font-size:clamp(18px,2vw,25px); }
.version p { font-size:14px; }
.version .tag { font:10px monospace; letter-spacing:.1em; color:var(--red); border-top:1px solid #383833; padding-top:12px; margin-top:12px; }
.poll-layout { display:grid; grid-template-columns:1.05fr .95fr; gap:clamp(22px,4vw,60px); align-items:center; }
.poll-list { display:grid; gap:16px; }
.poll-row { display:grid; grid-template-columns:1fr auto; gap:8px 14px; align-items:end; }
.poll-row .label { font-size:14px; line-height:1.35; color:#d8d6cf; }
.poll-row strong { font:900 24px monospace; color:var(--red); }
.bar { grid-column:1/-1; height:8px; background:#292925; overflow:hidden; }
.bar span { display:block; height:100%; width:var(--w); background:linear-gradient(90deg,#76201c,#e33a30); animation:barin 1s ease both; transform-origin:left; }
@keyframes barin { from {width:0} to {width:var(--w)} }
.disclaimer { font:10px/1.5 monospace; color:#77766e; margin-top:20px; }
.final-slide { text-align:center; align-items:center; background:radial-gradient(ellipse at center,#111 0%,#030303 75%); }
.final-slide h2 { font-size:clamp(38px,7vw,92px); }
.final-image { width:min(44vw,340px); min-width:200px; aspect-ratio:1; border:1px solid #3b3b35; margin:8px auto 18px; background:radial-gradient(circle at 50% 40%,#502b1d,#12110f 68%); display:grid; place-items:center; position:relative; }
.final-image .fox-svg { width:92%; }
.final-caption { color:#fff; font:900 clamp(13px,2vw,21px)/1.4 monospace; letter-spacing:.08em; background:#a51f1f; padding:12px 16px; transform:rotate(-1deg); box-shadow:5px 5px 0 #000; }
.controls { position:absolute; z-index:30; left:0; right:0; bottom:0; height:68px; display:flex; align-items:center; justify-content:space-between; padding:0 clamp(18px,4vw,52px); background:linear-gradient(transparent,rgba(0,0,0,.9)); }
.control-group { display:flex; gap:8px; align-items:center; }
.ctrl { color:#ddd; background:#161715; border:1px solid #42423c; padding:10px 13px; cursor:pointer; font:11px monospace; letter-spacing:.06em; transition:background .2s,border-color .2s; }
.ctrl:hover,.ctrl:focus-visible { background:#2a2a26; border-color:var(--red); outline:none; }
.ctrl:disabled { opacity:.25; cursor:not-allowed; }
.counter { min-width:76px; text-align:center; color:#b5b3aa; font:12px monospace; }
.progress { position:absolute; bottom:67px; left:0; right:0; height:2px; background:#2b2b27; z-index:31; }
.progress span { display:block; height:100%; width:14.285%; background:var(--red); transition:width .3s; }
.hint { color:#74736c; font:10px monospace; }
@media(max-width:760px) {
  #app { min-height:560px; }
  .slide { padding:52px 22px 86px; justify-content:flex-start; }
  .cover,.final-slide { justify-content:center; }
  .grid2,.poll-layout { grid-template-columns:1fr; }
  .fake-art { min-height:190px; max-height:250px; }
  .evidence-grid { grid-template-columns:1fr; }
  .evidence-card.wide { grid-column:auto; }
  .versions { grid-template-columns:1fr; }
  .version { min-height:auto; }
  .paper-wrap { margin-top:0; }
  .paper { padding:22px 18px; }
  .paper .seal { font-size:9px; }
  .case-title { gap:16px; }
  .case-meta { gap:12px; }
  .controls { height:64px; padding:0 12px; }
  .ctrl { padding:9px 10px; }
  .hint { display:none; }
  .progress { bottom:63px; }
}
@media(prefers-reduced-motion:reduce) { *,*::before,*::after { animation:none!important; transition:none!important; } }


.evidence-card.wide 








/* === Improved evidence photos & layout === */
.evidence-grid {
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 10px;
  margin-top: 10px;
}
.evidence-card {
  min-height: 0 !important;
  padding: 12px 14px 14px !important;
  display: flex;
  flex-direction: column;
}
.evidence-card.wide {
  grid-column: 1 / -1;
  min-height: 0 !important;
}
.evidence-photo {
  width: 100%;
  height: 110px;
  object-fit: cover;
  object-position: center 30%;
  display: block;
  margin-bottom: 8px;
  border: 1px solid #2a2a28;
  border-radius: 2px;
}
.evidence-card.wide .evidence-photo {
  height: 100px;
  object-position: center 40%;
}
.evidence-card h3 {
  font-size: clamp(16px, 1.8vw, 22px) !important;
  margin-bottom: 6px !important;
  line-height: 1.15 !important;
}
.evidence-card p {
  font-size: clamp(11px, 1.05vw, 13px) !important;
  line-height: 1.4 !important;
  margin-bottom: 0 !important;
}
.evidence-card .num {
  margin-bottom: 4px !important;
  font-size: 11px !important;
}
.evidence-card .interpret {
  margin-top: 4px !important;
  font-size: 11.5px !important;
}

/* Specific better crops for each photo */
.evidence-card:nth-child(1) .evidence-photo { object-position: center 25%; } /* math fox face */
.evidence-card:nth-child(2) .evidence-photo { object-position: center 35%; } /* urban fox */
.evidence-card:nth-child(3) .evidence-photo { object-position: center 40%; } /* sleeping */
.evidence-card:nth-child(4) .evidence-photo { object-position: center 20%; } /* white fox face close */
.evidence-card:nth-child(5) .evidence-photo { object-position: center 50%; } /* medieval full scene */

/* Make the whole evidence slide more compact */
.slide[data-index="03 / 07"] {
  padding-top: 36px !important;
  padding-bottom: 70px !important;
  justify-content: flex-start !important;
}
.slide[data-index="03 / 07"] .eyebrow {
  margin-bottom: 10px !important;
}
.slide[data-index="03 / 07"] h2 {
  margin-bottom: 6px !important;
  font-size: clamp(28px, 4.5vw, 48px) !important;
}

/* Final image better */
.final-image {
  width: min(38vw, 280px) !important;
  aspect-ratio: 1;
  overflow: hidden;
}
.final-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center 30%;
  display: block;
}

@media (max-height: 800px) {
  .evidence-photo { height: 90px !important; }
  .evidence-card.wide .evidence-photo { height: 80px !important; }
  .evidence-card { padding: 10px 12px !important; }
}
@media (max-height: 700px) {
  .evidence-photo { height: 75px !important; }
  .evidence-grid { gap: 8px; }
}

/* === 5 cards in one row === */
.evidence-grid {
  display: grid !important;
  grid-template-columns: repeat(5, minmax(0, 1fr)) !important;
  gap: 8px !important;
  margin-top: 12px !important;
}
.evidence-card {
  min-height: 0 !important;
  padding: 8px 10px 10px !important;
  display: flex !important;
  flex-direction: column !important;
}
.evidence-card.wide {
  grid-column: auto !important;   /* no longer spans full width */
  min-height: 0 !important;
}
.evidence-photo {
  width: 100% !important;
  height: 90px !important;
  object-fit: cover !important;
  object-position: center 30% !important;
  display: block !important;
  margin-bottom: 6px !important;
  border: 1px solid #2a2a28 !important;
  border-radius: 2px !important;
}
.evidence-card.wide .evidence-photo {
  height: 90px !important;
}
.evidence-card h3 {
  font-size: clamp(13px, 1.3vw, 16px) !important;
  margin-bottom: 4px !important;
  line-height: 1.15 !important;
  padding-right: 0 !important;
}
.evidence-card p {
  font-size: clamp(10px, 0.95vw, 12px) !important;
  line-height: 1.35 !important;
  margin-bottom: 0 !important;
}
.evidence-card .num {
  margin-bottom: 3px !important;
  font-size: 10px !important;
}
.evidence-card .interpret {
  margin-top: 3px !important;
  font-size: 10.5px !important;
}
.evidence-card::after {
  font-size: 8px !important;
  top: 6px !important;
  right: 6px !important;
}

/* Better crops for row layout */
.evidence-card:nth-child(1) .evidence-photo { object-position: center 20% !important; }
.evidence-card:nth-child(2) .evidence-photo { object-position: center 30% !important; }
.evidence-card:nth-child(3) .evidence-photo { object-position: center 45% !important; }
.evidence-card:nth-child(4) .evidence-photo { object-position: center 15% !important; }
.evidence-card:nth-child(5) .evidence-photo { object-position: center 45% !important; }

/* Compact the whole slide a bit more */
.slide[data-index="03 / 07"] {
  padding-top: 32px !important;
  padding-bottom: 70px !important;
  justify-content: flex-start !important;
}
.slide[data-index="03 / 07"] h2 {
  margin-bottom: 4px !important;
  font-size: clamp(26px, 4vw, 42px) !important;
}

@media (max-width: 1100px) {
  .evidence-grid {
    grid-template-columns: repeat(3, minmax(0, 1fr)) !important;
  }
  .evidence-card:nth-child(4),
  .evidence-card:nth-child(5) {
    /* still ok */
  }
}
@media (max-width: 700px) {
  .evidence-grid {
    grid-template-columns: 1fr 1fr !important;
  }
}


/* Stretch cards to fill vertical space */
.slide[data-index="03 / 07"] {
  justify-content: flex-start !important;
  padding-top: 28px !important;
  padding-bottom: 80px !important;
}
.slide[data-index="03 / 07"] .evidence-grid {
  flex: 1;
  align-content: stretch;
  height: auto;
  min-height: 55vh;
}
.evidence-grid {
  display: grid !important;
  grid-template-columns: repeat(5, minmax(0, 1fr)) !important;
  gap: 10px !important;
  margin-top: 14px !important;
  align-items: stretch !important;
}
.evidence-card {
  min-height: 0 !important;
  height: 100% !important;
  padding: 10px 11px 12px !important;
  display: flex !important;
  flex-direction: column !important;
}
.evidence-card.wide {
  grid-column: auto !important;
}
.evidence-photo {
  width: 100% !important;
  height: 140px !important;
  min-height: 120px !important;
  object-fit: cover !important;
  display: block !important;
  margin-bottom: 8px !important;
  border: 1px solid #2a2a28 !important;
  flex-shrink: 0 !important;
}
.evidence-card h3 {
  font-size: clamp(13px, 1.25vw, 15.5px) !important;
  margin-bottom: 5px !important;
  line-height: 1.2 !important;
}
.evidence-card p {
  font-size: clamp(10.5px, 0.95vw, 12px) !important;
  line-height: 1.4 !important;
  margin-bottom: 0 !important;
  flex-grow: 1;
}
.evidence-card .interpret {
  margin-top: 6px !important;
  font-size: 11px !important;
  color: #e4b3ad !important;
  border-top: 1px solid #333;
  padding-top: 6px;
}
.evidence-card .num {
  margin-bottom: 4px !important;
  font-size: 10px !important;
}

@media (max-height: 850px) {
  .evidence-photo { height: 115px !important; min-height: 100px !important; }
}
@media (max-height: 750px) {
  .evidence-photo { height: 95px !important; min-height: 85px !important; }
}

/* Final compact layout for evidence slide - no empty space */
.slide[data-index="03 / 07"] {
  justify-content: flex-start !important;
  padding-top: 24px !important;
  padding-bottom: 70px !important;
}
.slide[data-index="03 / 07"] .eyebrow {
  margin-bottom: 8px !important;
}
.slide[data-index="03 / 07"] h2 {
  margin-bottom: 8px !important;
  font-size: clamp(26px, 4vw, 40px) !important;
}
.evidence-grid {
  display: grid !important;
  grid-template-columns: repeat(5, minmax(0, 1fr)) !important;
  gap: 10px !important;
  margin-top: 10px !important;
  margin-bottom: 0 !important;
  align-items: start !important;
}
.evidence-card {
  min-height: 0 !important;
  height: auto !important;
  padding: 8px 10px 10px !important;
  display: flex !important;
  flex-direction: column !important;
}
.evidence-card.wide {
  grid-column: auto !important;
}
.evidence-photo {
  width: 100% !important;
  height: 150px !important;
  object-fit: cover !important;
  display: block !important;
  margin-bottom: 8px !important;
  border: 1px solid #2a2a28 !important;
  flex-shrink: 0 !important;
}
.evidence-card h3 {
  font-size: clamp(13px, 1.3vw, 16px) !important;
  margin-bottom: 5px !important;
  line-height: 1.2 !important;
}
.evidence-card p {
  font-size: clamp(11px, 1vw, 12.5px) !important;
  line-height: 1.4 !important;
  margin-bottom: 0 !important;
}
.evidence-card .num {
  margin-bottom: 3px !important;
  font-size: 10px !important;
}
.evidence-card .interpret {
  display: none !important;
}

@media (max-height: 800px) {
  .evidence-photo { height: 120px !important; }
}
@media (max-height: 700px) {
  .evidence-photo { height: 100px !important; }
}

/* Kill empty space on evidence slide */
.slide[data-index="03 / 07"] {
  justify-content: flex-start !important;
  padding: 20px clamp(20px, 5vw, 60px) 60px !important;
  height: 100% !important;
}
.slide[data-index="03 / 07"] > * {
  flex-shrink: 0;
}
.slide[data-index="03 / 07"] .eyebrow {
  margin-bottom: 6px !important;
}
.slide[data-index="03 / 07"] h2 {
  margin-bottom: 10px !important;
  font-size: clamp(24px, 3.8vw, 38px) !important;
}
.evidence-grid {
  display: grid !important;
  grid-template-columns: repeat(5, minmax(0, 1fr)) !important;
  gap: 8px !important;
  margin: 0 !important;
  width: 100% !important;
}
.evidence-card {
  padding: 8px !important;
  margin: 0 !important;
}
.evidence-photo {
  height: clamp(130px, 22vh, 180px) !important;
  margin-bottom: 6px !important;
}
.evidence-card h3 {
  font-size: clamp(12px, 1.2vw, 15px) !important;
  margin-bottom: 4px !important;
}
.evidence-card p {
  font-size: clamp(10.5px, 0.95vw, 12px) !important;
  line-height: 1.35 !important;
}

.slide[data-index="03 / 07"] {
  padding-bottom: 55px !important;
}
.evidence-grid {
  margin-bottom: 0 !important;
}

/* Cooler evidence cards */
.evidence-grid {
  display: grid !important;
  grid-template-columns: repeat(5, minmax(0, 1fr)) !important;
  gap: 12px !important;
  margin-top: 12px !important;
}
.evidence-card {
  background: linear-gradient(160deg, #141413 0%, #0c0c0b 100%) !important;
  border: 1px solid #2e2e2a !important;
  border-top: 2px solid #e33a30 !important;
  border-radius: 3px !important;
  padding: 0 !important;
  overflow: hidden !important;
  display: flex !important;
  flex-direction: column !important;
  transition: border-color .25s, transform .2s, box-shadow .25s !important;
  position: relative !important;
  box-shadow: 0 4px 20px rgba(0,0,0,.35);
}
.evidence-card:hover {
  border-color: #e33a30 !important;
  transform: translateY(-3px);
  box-shadow: 0 8px 28px rgba(227,58,48,.15);
}
.evidence-card::after {
  content: "EVIDENCE" !important;
  position: absolute !important;
  top: 8px !important;
  right: 8px !important;
  font: 8px monospace !important;
  letter-spacing: .12em !important;
  color: rgba(255,255,255,.25) !important;
  z-index: 2;
  background: rgba(0,0,0,.4);
  padding: 2px 5px;
}
.evidence-photo {
  width: 100% !important;
  height: 135px !important;
  object-fit: cover !important;
  display: block !important;
  margin: 0 !important;
  border: none !important;
  border-bottom: 1px solid #2a2a28 !important;
}
.evidence-card .num {
  color: #e33a30 !important;
  font: 700 10px/1 monospace !important;
  letter-spacing: .12em !important;
  margin: 10px 11px 4px !important;
}
.evidence-card h3 {
  font-size: clamp(13px, 1.25vw, 15.5px) !important;
  margin: 0 11px 6px !important;
  line-height: 1.2 !important;
  color: #f1eee8 !important;
  text-transform: uppercase;
  letter-spacing: .02em;
}
.evidence-card p {
  font-size: clamp(10.5px, 0.95vw, 12px) !important;
  line-height: 1.4 !important;
  margin: 0 11px 6px !important;
  color: #b0aea6 !important;
}
.evidence-card .card-extra {
  font-size: clamp(10px, 0.9vw, 11.5px) !important;
  line-height: 1.4 !important;
  margin: 0 11px 12px !important;
  padding-top: 7px !important;
  border-top: 1px solid #2a2a28 !important;
  color: #d4a39c !important;
  flex-grow: 1;
}

.slide[data-index="03 / 07"] {
  padding: 22px clamp(18px, 4vw, 50px) 58px !important;
}
.slide[data-index="03 / 07"] h2 {
  margin-bottom: 8px !important;
  font-size: clamp(24px, 3.6vw, 36px) !important;
}

/* Stretch cards + bigger images */
.slide[data-index="03 / 07"] {
  display: flex !important;
  flex-direction: column !important;
  justify-content: flex-start !important;
  padding: 18px clamp(16px, 3.5vw, 40px) 52px !important;
  height: 100% !important;
}
.slide[data-index="03 / 07"] .eyebrow {
  margin-bottom: 4px !important;
  flex-shrink: 0;
}
.slide[data-index="03 / 07"] h2 {
  margin-bottom: 10px !important;
  font-size: clamp(22px, 3.2vw, 34px) !important;
  flex-shrink: 0;
}
.evidence-grid {
  display: grid !important;
  grid-template-columns: repeat(5, minmax(0, 1fr)) !important;
  gap: 10px !important;
  margin: 0 !important;
  flex: 1 1 auto !important;
  align-items: stretch !important;
  min-height: 0 !important;
}
.evidence-card {
  height: 100% !important;
  min-height: 0 !important;
  display: flex !important;
  flex-direction: column !important;
  padding: 0 !important;
}
.evidence-photo {
  width: 100% !important;
  height: auto !important;
  flex: 1 1 55% !important;
  min-height: 160px !important;
  max-height: none !important;
  object-fit: cover !important;
  object-position: center 25% !important;
  margin: 0 !important;
  border: none !important;
  border-bottom: 1px solid #2a2a28 !important;
}
.evidence-card .num {
  margin: 8px 10px 3px !important;
  flex-shrink: 0;
}
.evidence-card h3 {
  margin: 0 10px 4px !important;
  font-size: clamp(12px, 1.15vw, 14.5px) !important;
  flex-shrink: 0;
}
.evidence-card p {
  margin: 0 10px 4px !important;
  font-size: clamp(10px, 0.9vw, 11.5px) !important;
  flex-shrink: 0;
}
.evidence-card .card-extra {
  margin: 0 10px 10px !important;
  padding-top: 5px !important;
  font-size: clamp(9.5px, 0.85vw, 11px) !important;
  flex-shrink: 0;
}

/* Better face crops */
.evidence-card:nth-child(1) .evidence-photo { object-position: center 18% !important; }
.evidence-card:nth-child(2) .evidence-photo { object-position: center 30% !important; }
.evidence-card:nth-child(3) .evidence-photo { object-position: center 40% !important; }
.evidence-card:nth-child(4) .evidence-photo { object-position: center 12% !important; }
.evidence-card:nth-child(5) .evidence-photo { object-position: center 40% !important; }

/* Fixed equal image sizes */
.evidence-photo {
  width: 100% !important;
  height: 180px !important;
  min-height: 180px !important;
  max-height: 180px !important;
  flex: 0 0 180px !important;
  object-fit: cover !important;
  object-position: center 25% !important;
}
.evidence-card {
  height: auto !important;
}
.evidence-grid {
  align-items: start !important;
  flex: 0 0 auto !important;
}

@media (max-height: 850px) {
  .evidence-photo {
    height: 150px !important;
    min-height: 150px !important;
    max-height: 150px !important;
    flex-basis: 150px !important;
  }
}
@media (max-height: 750px) {
  .evidence-photo {
    height: 130px !important;
    min-height: 130px !important;
    max-height: 130px !important;
    flex-basis: 130px !important;
  }
}

/* Final slide sequence */
.final-slide {
  background: #000 !important;
  justify-content: center !important;
  align-items: center !important;
  text-align: center !important;
}
.final-reveal {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 18px;
}
.final-notif {
  display: flex;
  align-items: center;
  gap: 10px;
  background: #141413;
  border: 1px solid #333;
  padding: 10px 16px;
  font: 13px monospace;
  color: #ccc;
  letter-spacing: 0.04em;
  margin-bottom: 8px;
}
.notif-dot {
  width: 8px;
  height: 8px;
  background: #e33a30;
  border-radius: 50%;
  display: inline-block;
  animation: blink 1.1s infinite;
}
@keyframes blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.25; }
}
.final-image {
  width: min(42vw, 300px);
  aspect-ratio: 1;
  border: 2px solid #e33a30;
  overflow: hidden;
  box-shadow: 0 0 40px rgba(227,58,48,0.35);
}
.final-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center 25%;
  display: block;
}
.final-caption {
  font: 700 clamp(16px, 2.4vw, 26px) monospace;
  letter-spacing: 0.12em;
  color: #f1eee8;
  text-transform: uppercase;
  margin-top: 6px;
}
.final-sub {
  font-size: 12px !important;
  letter-spacing: 0.18em !important;
  color: #e33a30 !important;
  margin: 0 !important;
}
.final-reveal.visible {
  opacity: 1 !important;
  transform: scale(1) !important;
}
.final-notif.visible {
  opacity: 1 !important;
  transform: translateY(0) !important;
}
</style>
</head>
<body>
<div data-sites-preview-theme="custom" id="app">
<main aria-label="Презентация Лисий культ" class="deck">
<section aria-label="Слайд 1" class="slide cover active" data-index="01 / 07">
<div class="noise-screen"></div><div class="scanline"></div>
<div class="tiny">ВХОДЯЩИЙ СИГНАЛ // КАНАЛ НЕ ОПРЕДЕЛЁН</div>
<div style="font:12px monospace;color:#666;margin:22px 0 12px">[ VHS PLAYBACK ERROR ]</div>
<h1 class="glitch" style="font-size:clamp(42px,8vw,100px)">СИГНАЛ<br/>ПЕРЕХВАЧЕН</h1>
<p style="color:#777;font:12px monospace;letter-spacing:.12em">НЕ ВЫКЛЮЧАЙТЕ ЭКРАН</p>
<div style="position:absolute;bottom:105px;left:8%;right:8%;height:1px;background:#333"></div>
<div style="position:absolute;bottom:78px;left:8%;font:10px monospace;color:#65655f">REC ● 00:00:00:07</div>
</section>
<section aria-label="Слайд 2" class="slide" data-index="02 / 07">
<div class="eyebrow">Архив необъяснимых явлений / файл восстановлен</div>
<div class="case-title"><div class="case-number">FOX<br/>001</div><div>
<div class="stamp">СОВЕРШЕННО СЕКРЕТНО</div>
<h1 style="font-size:clamp(48px,8.7vw,116px);margin-top:25px">ЛИСИЙ<br/><span class="red">КУЛЬТ</span></h1>
<p class="lead">Досье о возможной скрытой структуре влияния, которая уже слишком глубоко проникла в человеческую культуру.</p>
</div></div>
<div class="case-meta"><span>ДОСЬЕ № ЗАСЕКРЕЧЕНО</span><span>СТАТУС: АКТИВНО</span><span>ОБЪЕКТ: <i>VULPES</i></span><span>ДОСТУП: УРОВЕНЬ 7</span></div>
<p class="muted mono" style="font-size:11px;margin-top:16px">ПРЕДУПРЕЖДЕНИЕ: дальнейший просмотр может вызвать необоснованное подозрение к рыжим хвостам.</p>
</section>
<section aria-label="Слайд 3" class="slide" data-index="03 / 07">
<div class="eyebrow">Материалы дела / пять независимых улик</div>
<h2>Пять главных <span class="red">улик</span></h2>
<div class="evidence-grid">
<article class="evidence-card"><img alt="Лиса-манипулятор с формулами" class="evidence-photo" src="fox-math.jpg"/><div class="num">УЛИКА № 01</div><h3>Лиса — профессиональный манипулятор</h3><p>Во многих сказках лиса — хитрый персонаж, способный обвести вокруг пальца других.</p><p class="card-extra">Многовековая информационная кампания. Репутация «хитрой, но безобидной» — идеальное прикрытие.</p></article>
<article class="evidence-card"><img alt="Городская лиса в ночном переулке" class="evidence-photo" src="fox-urban.jpg"/><div class="num">УЛИКА № 02</div><h3>Они уже внутри</h3><p>Лисы приспосабливаются к жизни рядом с людьми и встречаются в крупных городах.</p><p class="card-extra">Дороги, парки, тоннели и мусорные контейнеры — готовая сеть снабжения. Они здесь давно.</p></article>
<article class="evidence-card"><img alt="Мемная лиса в наушниках" class="evidence-photo" src="fox-sleep.jpg"/><div class="num">УЛИКА № 03</div><h3>Информационная экспансия</h3><p>Видео с лисами регулярно появляются в соцсетях и превращаются в мемы.</p><p class="card-extra">Каждый лайк — добровольный взнос в развитие лисьего влияния. Мы сами их продвигаем.</p></article>
<article class="evidence-card"><img alt="Лиса с прямым взглядом" class="evidence-photo" src="fox-gamer.jpg"/><div class="num">УЛИКА № 04</div><h3>Прямой зрительный контакт</h3><p>Лисы наблюдают за окружающей средой и быстро реагируют на происходящее.</p><p class="card-extra">Взгляд аудитора, который знает, что вы опять не выполнили квартальный план.</p></article>
<article class="evidence-card wide"><img alt="Средневековое изображение лис" class="evidence-photo" src="fox-medieval.jpg"/><div class="num">УЛИКА № 05</div><h3>Древний культ</h3><p>Образ лисы встречается в мифологии разных народов. В японском синтоизме лисы связаны с культом Инари.</p><p class="card-extra">Что, если древние люди договаривались не с символом, а с теми, кто за ним стоял?</p></article>
</div>
</section>
<section aria-label="Слайд 4" class="slide" data-index="04 / 07">
<div class="eyebrow">Утечка из закрытого архива</div>
<div class="paper-wrap"><div class="paper">
<div class="paper-top"><div class="paper-kicker">УПРАВЛЕНИЕ ПО ИЗУЧЕНИЮ<br/>НЕОБЪЯСНИМЫХ ЯВЛЕНИЙ<br/><span style="font-weight:400">Отдел межвидовых угроз / Сектор V</span></div><div class="seal">СОВЕРШЕННО<br/>СЕКРЕТНО</div></div>
<div style="font:10px monospace;color:#5a5548">ДОКУМЕНТ № FOX-001   |   ДАТА СОЗДАНИЯ: ЗАСЕКРЕЧЕНА</div>
<h2>Операция<br/>«Рыжий рассвет»</h2>
<div class="section-label">Цель операции</div>
<p>Установить природу устойчивого положительного отношения граждан к представителям рода <i>Vulpes</i>.</p>
<div class="section-label">Выдержки из протокола</div>
<p>— Объект вызывает у наблюдателей непропорционально высокий уровень умиления.</p>
<p>— Попытки объяснить поведение объекта словами «просто животное» признаны недостаточными.</p>
<p>— Установлено: после просмотра изображения лисы субъект склонен показывать его другим субъектам.</p>
<p>— Особую опасность представляет хвост. Его назначение официально объясняется вопросами баланса и коммуникации, однако данная версия требует дальнейшей проверки.</p>
<div class="recommend">РЕКОМЕНДАЦИЯ КОМИССИИ: не устанавливать зрительный контакт с объектом дольше 7 секунд.</div>
<div class="paper-foot"><span>КОПИРОВАНИЕ ЗАПРЕЩЕНО</span><span>ЛИСТ 1 ИЗ 1</span><span>FOX / INTERNAL</span></div>
</div></div>
<p class="disclaimer">* Документ, ведомство и выводы вымышлены. Секретность распространяется даже на автора.</p>
</section>
<section aria-label="Слайд 5" class="slide" data-index="05 / 07">
<div class="eyebrow">Рабочие гипотезы / уровень угрозы повышен</div>
<h2>Кто стоит за <span class="red">заговором?</span></h2>
<div class="versions">
<article class="version"><div class="letter">A</div><h3>Древняя цивилизация лис</h3><p>Скрытое общество существует параллельно человеческому. Их коммуникация настолько сложна, что мы принимаем её за обычное поведение животных.</p><div class="tag">ГИПОТЕЗА: «ПАРАЛЛЕЛЬНОЕ ОБЩЕСТВО»</div></article>
<article class="version"><div class="letter">B</div><h3>Правительство всё знает</h3><p>Почему нет ежедневных экстренных заявлений? Возможно, существует секретное соглашение: люди пользуются планетой, пока не мешают лисам.</p><div class="tag">ГИПОТЕЗА: «МОЛЧАЛИВЫЙ ДОГОВОР»</div></article>
<article class="version"><div class="letter">C</div><h3>Лисы управляют алгоритмами</h3><p>В этой вымышленной версии рекомендации соцсетей — инструмент распространения влияния, а каждое видео захватывает ещё немного нашего внимания.</p><div class="tag">ГИПОТЕЗА: «ЦИФРОВОЙ ХВОСТ»</div></article>
</div>
<div style="display:flex;align-items:center;gap:14px;margin-top:22px"><span class="stamp">ВСЕ СВЯЗИ СЛУЧАЙНЫ?</span><p class="muted" style="font:11px/1.5 monospace;margin:0">СОВПАДЕНИЙ СЛИШКОМ МНОГО. ИЛИ НАМ ТАК КАЖЕТСЯ?</p></div>
</section>
<section aria-label="Слайд 6" class="slide" data-index="06 / 07">
<div class="eyebrow">Полевое исследование / результаты засекречены</div>
<div class="poll-layout">
<div><h2>А вы уже <span class="red">завербованы?</span></h2><p class="lead">Мы провели абсолютно подозрительный опрос. Ответы заставляют задуматься. Методология — засекречена.</p>
<div class="poll-list">
<div class="poll-row"><span class="label">Признали лис милыми</span><strong>92%</strong><div class="bar"><span style="--w:92%"></span></div></div>
<div class="poll-row"><span class="label">Пересылали изображения лис</span><strong>76%</strong><div class="bar"><span style="--w:76%"></span></div></div>
<div class="poll-row"><span class="label">Не могут объяснить свою симпатию</span><strong>64%</strong><div class="bar"><span style="--w:64%"></span></div></div>
<div class="poll-row"><span class="label">Начнут подозрительно смотреть на лис</span><strong>100%</strong><div class="bar"><span style="--w:100%"></span></div></div>
</div>
<p class="disclaimer">* Шуточные, выдуманные показатели для презентации. Это не результаты реального опроса.</p>
</div>
<div class="chart-box"><div class="chart-title"><span>ИНДЕКС ЛИСЬЕГО ВЛИЯНИЯ</span><span>НЕЗАВИСИМЫЕ ДАННЫЕ*</span></div>
<svg aria-label="Шуточный график роста лисьего влияния" role="img" viewbox="0 0 500 340"><g stroke="#30302b" stroke-width="1"><path d="M50 30V285H475" fill="none"></path><path d="M50 80H475M50 130H475M50 180H475M50 230H475" stroke-dasharray="3 6"></path></g><g fill="#77766f" font-family="monospace" font-size="11"><text x="10" y="34">100</text><text x="20" y="84">80</text><text x="20" y="134">60</text><text x="20" y="184">40</text><text x="20" y="234">20</text><text x="48" y="310">1990</text><text x="155" y="310">2000</text><text x="260" y="310">2010</text><text x="365" y="310">2020</text><text x="442" y="310">2026</text></g><path class="graph-line" d="M52 263 C85 260 100 250 126 252 S175 238 200 244 S245 212 270 222 S305 175 330 188 S360 150 385 155 S425 75 470 42" fill="none" stroke="#e33a30" stroke-linecap="round" stroke-width="4"></path><path d="M52 263 C85 260 100 250 126 252 S175 238 200 244 S245 212 270 222 S305 175 330 188 S360 150 385 155 S425 75 470 42 L470 285 L52 285Z" fill="#e33a30" opacity=".1"></path><circle cx="470" cy="42" fill="#e33a30" r="6"></circle><text fill="#e33a30" font-family="monospace" font-size="12" font-weight="bold" x="300" y="30">КРИТИЧЕСКИЙ УРОВЕНЬ</text></svg>
<p class="disclaimer">* График нарисован для драматического эффекта. Научная ценность: отсутствует.</p>
</div>
</div>
</section>
<section aria-label="Слайд 7" class="slide final-slide" data-index="07 / 07"><div class="noise-screen" id="finalNoise"></div><div class="final-reveal" id="finalReveal" style="opacity:0; transform:scale(0.96); transition: opacity 1.2s ease, transform 1.2s ease;"><div class="final-notif" id="finalNotif" style="opacity:0; transform:translateY(-12px); transition: all 0.5s ease;"><span class="notif-dot"></span> Новое уведомление</div><div class="final-image"><img alt="Они уже здесь" src="fox-urban.jpg"/></div><div class="final-caption">ВЫ ПОДПИСАНЫ НА НАС С 2012 ГОДА</div><p class="muted mono final-sub">ОНИ УЖЕ ПОБЕДИЛИ</p></div></section>
</main>
<div class="progress"><span id="progress"></span></div>
<nav aria-label="Управление презентацией" class="controls">
<div class="control-group"><button aria-label="Предыдущий слайд" class="ctrl" id="prev">← НАЗАД</button><button aria-pressed="false" class="ctrl" id="sound">♫ ЗВУК: ВЫКЛ</button></div>
<div class="control-group"><span class="hint">← → ПРОБЕЛ</span><span class="counter" id="counter">01 / 07</span><button aria-label="Следующий слайд" class="ctrl" id="next">ДАЛЕЕ →</button><button aria-label="Полноэкранный режим" class="ctrl" id="full">⛶</button></div>
</nav>
</div>
<script>
(() => {
  const slides = [...document.querySelectorAll('.slide')];
  const prev = document.getElementById('prev');
  const next = document.getElementById('next');
  const counter = document.getElementById('counter');
  const progress = document.getElementById('progress');
  const soundBtn = document.getElementById('sound');
  let index = 0;
  let audioCtx = null;
  let soundOn = false;
  let noiseNode = null;
  let master = null;
  
  // Final slide sequence
  let finalPlayed = false;
  function runFinalSequence() {
    if (finalPlayed) return;
    finalPlayed = true;
    const reveal = document.getElementById('finalReveal');
    const notif = document.getElementById('finalNotif');
    if (!reveal) return;

    // 1. Stay black for 1.1s
    setTimeout(() => {
      // 2. Play notification sound
      playNotificationBeep();
      // 3. Show content
      reveal.classList.add('visible');
      setTimeout(() => {
        if (notif) notif.classList.add('visible');
      }, 200);
    }, 1100);
  }
  function playNotificationBeep() {
    try {
      if (!audioCtx) audioCtx = new (window.AudioContext || window.webkitAudioContext)();
      if (audioCtx.state === 'suspended') audioCtx.resume();
      const osc = audioCtx.createOscillator();
      const gain = audioCtx.createGain();
      osc.connect(gain);
      gain.connect(audioCtx.destination);
      osc.type = 'sine';
      osc.frequency.value = 880;
      gain.gain.setValueAtTime(0.0001, audioCtx.currentTime);
      gain.gain.exponentialRampToValueAtTime(0.12, audioCtx.currentTime + 0.02);
      gain.gain.exponentialRampToValueAtTime(0.0001, audioCtx.currentTime + 0.35);
      osc.start();
      osc.stop(audioCtx.currentTime + 0.4);
      setTimeout(() => {
        const osc2 = audioCtx.createOscillator();
        const g2 = audioCtx.createGain();
        osc2.connect(g2);
        g2.connect(audioCtx.destination);
        osc2.type = 'sine';
        osc2.frequency.value = 1175;
        g2.gain.setValueAtTime(0.0001, audioCtx.currentTime);
        g2.gain.exponentialRampToValueAtTime(0.09, audioCtx.currentTime + 0.02);
        g2.gain.exponentialRampToValueAtTime(0.0001, audioCtx.currentTime + 0.28);
        osc2.start();
        osc2.stop(audioCtx.currentTime + 0.3);
      }, 160);
    } catch(e) {}
  }

  function show(n) {

    index = Math.max(0, Math.min(slides.length - 1, n));
    slides.forEach((s, i) => { s.classList.toggle('active', i === index); s.setAttribute('aria-hidden', i === index ? 'false' : 'true'); });
    counter.textContent = `${String(index + 1).padStart(2,'0')} / ${String(slides.length).padStart(2,'0')}`;
    progress.style.width = `${((index + 1) / slides.length) * 100}%`;
    if (index === slides.length - 1) runFinalSequence();
    else { finalPlayed = false; const r = document.getElementById('finalReveal'); if(r){ r.classList.remove('visible'); const n=document.getElementById('finalNotif'); if(n) n.classList.remove('visible'); } }
    prev.disabled = index === 0;
    next.disabled = index === slides.length - 1;
    if (soundOn) playCue(index);
  }
  function tone(freq, duration, type='sine', volume=.04) {
    if (!audioCtx || !master) return;
    const osc = audioCtx.createOscillator();
    const gain = audioCtx.createGain();
    osc.type = type; osc.frequency.value = freq;
    gain.gain.setValueAtTime(.0001, audioCtx.currentTime);
    gain.gain.exponentialRampToValueAtTime(volume, audioCtx.currentTime + .03);
    gain.gain.exponentialRampToValueAtTime(.0001, audioCtx.currentTime + duration);
    osc.connect(gain); gain.connect(master); osc.start(); osc.stop(audioCtx.currentTime + duration + .05);
  }
  function playCue(i) {
    if (!audioCtx || !soundOn) return;
    if (i === 0) { tone(55,.45,'sawtooth',.035); setTimeout(()=>tone(90,.18,'square',.02),150); }
    else if (i === 6) { tone(880,.12,'sine',.06); setTimeout(()=>tone(660,.2,'sine',.045),120); }
    else { tone(110,.09,'square',.018); }
  }
  function startNoise() {
    if (!audioCtx) audioCtx = new (window.AudioContext || window.webkitAudioContext)();
    if (audioCtx.state === 'suspended') audioCtx.resume();
    master = audioCtx.createGain(); master.gain.value = .22; master.connect(audioCtx.destination);
    const buffer = audioCtx.createBuffer(1, audioCtx.sampleRate * 2, audioCtx.sampleRate);
    const data = buffer.getChannelData(0);
    for (let i=0; i<data.length; i++) data[i] = (Math.random()*2-1) * .18;
    noiseNode = audioCtx.createBufferSource(); noiseNode.buffer = buffer; noiseNode.loop = true;
    const filter = audioCtx.createBiquadFilter(); filter.type = 'bandpass'; filter.frequency.value = 900; filter.Q.value = .7;
    const gain = audioCtx.createGain(); gain.gain.value = .11;
    noiseNode.connect(filter); filter.connect(gain); gain.connect(master); noiseNode.start();
  }
  prev.addEventListener('click', () => show(index - 1));
  next.addEventListener('click', () => show(index + 1));
  document.getElementById('full').addEventListener('click', async () => {
    try { if (!document.fullscreenElement) await document.getElementById('app').requestFullscreen(); else await document.exitFullscreen(); } catch(e) {}
  });
  soundBtn.addEventListener('click', () => {
    soundOn = !soundOn;
    if (soundOn) { startNoise(); soundBtn.textContent = '♫ ЗВУК: ВКЛ'; soundBtn.setAttribute('aria-pressed','true'); playCue(index); }
    else { if (noiseNode) { try { noiseNode.stop(); } catch(e) {} noiseNode = null; } if (master) master.gain.setTargetAtTime(.0001, audioCtx.currentTime, .04); soundBtn.textContent = '♫ ЗВУК: ВЫКЛ'; soundBtn.setAttribute('aria-pressed','false'); }
  });
  document.addEventListener('keydown', e => {
    if (['ArrowRight',' ','PageDown','Enter'].includes(e.key)) { e.preventDefault(); show(index + 1); }
    else if (['ArrowLeft','PageUp','Backspace'].includes(e.key)) { e.preventDefault(); show(index - 1); }
    else if (e.key === 'Home') show(0);
    else if (e.key === 'End') show(slides.length - 1);
  });
  let touchX = null;
  document.getElementById('app').addEventListener('touchstart', e => { touchX = e.changedTouches[0].screenX; }, {passive:true});
  document.getElementById('app').addEventListener('touchend', e => { if (touchX === null) return; const dx=e.changedTouches[0].screenX-touchX; if (Math.abs(dx)>70) show(index+(dx<0?1:-1)); touchX=null; }, {passive:true});
  show(0);
})();
</script>
  
</body>
</html>

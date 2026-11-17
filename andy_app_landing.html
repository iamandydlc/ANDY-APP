<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#050505">
<title>ANDY APP — Cuenta Regresiva</title>
<style>
:root{
  --gold:#d8b35d;--gold2:#f3d58b;--bg:#030305;
  --muted:#9d9da5;--line:rgba(216,179,93,.22)
}
*{box-sizing:border-box;margin:0;padding:0}
html,body{width:100%;min-height:100%;font-family:Inter,system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;background:var(--bg);color:#fff}
body{overflow-x:hidden}
canvas{position:fixed;inset:0;width:100%;height:100%;z-index:0}
body:after{content:"";position:fixed;inset:0;z-index:1;pointer-events:none;background:radial-gradient(circle at 50% 38%,rgba(216,179,93,.09),transparent 28%),linear-gradient(180deg,rgba(0,0,0,.05),rgba(0,0,0,.72))}
.wrap{position:relative;z-index:2;min-height:100vh;display:flex;justify-content:center;padding:28px 18px 60px}
.container{width:min(1080px,100%);text-align:center}
.brand{display:inline-flex;align-items:center;gap:10px;margin-top:8px;color:var(--gold2);font-weight:900;letter-spacing:5px;font-size:clamp(18px,3vw,28px)}
.brand:before,.brand:after{content:"";height:1px;width:55px;background:linear-gradient(90deg,transparent,var(--gold))}
.brand:after{transform:rotate(180deg)}
.kicker{margin-top:45px;color:var(--gold);font-size:12px;font-weight:800;letter-spacing:4px;text-transform:uppercase}
h1{font-size:clamp(42px,10vw,92px);line-height:.9;margin:14px auto 12px;font-weight:950;letter-spacing:-4px;text-shadow:0 0 35px rgba(216,179,93,.18)}
h1 span{color:var(--gold);text-shadow:0 0 30px rgba(216,179,93,.35)}
.subtitle{color:#c5c5c9;font-size:clamp(14px,2vw,18px);letter-spacing:.3px}
.countdown{margin:34px auto 18px;display:grid;grid-template-columns:repeat(4,1fr);gap:12px;max-width:760px}
.box{padding:22px 10px;border:1px solid var(--line);border-radius:20px;background:linear-gradient(145deg,rgba(15,15,18,.86),rgba(5,5,7,.76));box-shadow:inset 0 0 35px rgba(216,179,93,.025),0 15px 60px rgba(0,0,0,.35)}
.num{font-size:clamp(34px,8vw,62px);font-weight:900;color:#fff;font-variant-numeric:tabular-nums}
.label{font-size:10px;color:var(--gold);letter-spacing:3px;font-weight:800;margin-top:5px}
.status{display:inline-flex;align-items:center;gap:8px;padding:10px 16px;border-radius:999px;border:1px solid var(--line);background:rgba(0,0,0,.42);color:#c9c9cd;font-size:12px}
.dot{width:7px;height:7px;background:#d8b35d;border-radius:50%;box-shadow:0 0 14px #d8b35d}
.glass{margin:45px auto 0;max-width:980px;padding:25px;border:1px solid var(--line);border-radius:26px;background:rgba(7,7,9,.68);backdrop-filter:blur(12px);box-shadow:0 30px 100px rgba(0,0,0,.45)}
.glass h2{font-size:18px;letter-spacing:2px;margin-bottom:18px;color:var(--gold2)}
.grid{display:grid;grid-template-columns:repeat(4,1fr);gap:10px}
.timecard{text-align:left;padding:15px;border:1px solid rgba(255,255,255,.08);border-radius:16px;background:rgba(255,255,255,.025)}
.country{font-weight:800;font-size:13px}
.zone{font-size:10px;color:var(--gold);margin-top:3px;letter-spacing:1px}
.local{margin-top:12px;font-size:18px;font-weight:900;color:#fff}
.date{font-size:10px;color:#8f8f96;margin-top:3px}
footer{margin-top:28px;color:#707077;font-size:11px;letter-spacing:.7px}
.download-launch{display:none;max-width:580px;margin:28px auto 0;animation:launchIn .65s cubic-bezier(.2,.8,.2,1) both}
.download-launch.visible{display:block}
@keyframes launchIn{from{opacity:0;transform:translateY(18px) scale(.98)}to{opacity:1;transform:translateY(0) scale(1)}}
.download-toggle{width:min(420px,100%);min-height:62px;padding:16px 24px;border:1px solid #f3d58b;border-radius:14px;background:linear-gradient(135deg,#f3d58b,#bd9140);color:#17130a;font:900 13px/1.2 Inter,system-ui,sans-serif;letter-spacing:2px;cursor:pointer;box-shadow:0 12px 42px #d8b35d35;transition:transform .2s,box-shadow .2s}
.download-toggle:hover{transform:translateY(-2px);box-shadow:0 16px 48px #d8b35d55}
.download-options{display:none;grid-template-columns:repeat(3,1fr);gap:10px;margin-top:14px;text-align:left}
.download-options.open{display:grid}
.download-card{display:flex;flex-direction:column;align-items:flex-start;gap:9px;min-height:145px;padding:16px 14px;border:1px solid var(--line);border-radius:16px;background:linear-gradient(145deg,rgba(20,19,17,.96),rgba(5,5,7,.92));color:#fff;text-decoration:none;transition:transform .2s,border-color .2s}
.download-card:hover{transform:translateY(-3px);border-color:var(--gold2)}
.download-icon{font-size:22px}
.download-card strong{font-size:13px;color:var(--gold2)}
.download-card small{font-size:11px;line-height:1.45;color:#aaaab0}
.download-note{margin:12px auto 0;max-width:490px;color:#aaaab0;font-size:11px;line-height:1.55}
@media(max-width:720px){.grid{grid-template-columns:repeat(2,1fr)}}
@media(max-width:520px){
  .countdown{grid-template-columns:repeat(2,1fr)}
  .glass{padding:18px}
  .brand:before,.brand:after{width:28px}
  h1{letter-spacing:-2px}
  .download-options{grid-template-columns:1fr}
  .download-card{min-height:0;display:grid;grid-template-columns:30px 1fr;align-items:center}
  .download-card small{grid-column:2}
}
</style>
</head>
<body>
<canvas id="stars"></canvas>
<div class="wrap">
<main class="container">
  <div class="brand">ANDY APP</div>
  <div class="kicker">Lanzamiento oficial</div>
  <h1>La espera<br><span>termina pronto.</span></h1>
  <p class="subtitle">Cuenta regresiva para el lanzamiento de ANDY APP</p>

  <div class="countdown" aria-label="Cuenta regresiva">
    <div class="box"><div class="num" id="days">00</div><div class="label">DÍAS</div></div>
    <div class="box"><div class="num" id="hours">00</div><div class="label">HORAS</div></div>
    <div class="box"><div class="num" id="minutes">00</div><div class="label">MINUTOS</div></div>
    <div class="box"><div class="num" id="seconds">00</div><div class="label">SEGUNDOS</div></div>
  </div>

  <div class="status"><span class="dot"></span><span id="statusText">17 NOV · 12:00 AM · HORA DE PERÚ</span></div>

  <section class="download-launch" id="downloadLaunch" aria-live="polite">
    <button class="download-toggle" id="downloadToggle" type="button" aria-expanded="false" aria-controls="downloadOptions">✦ &nbsp; DESCARGAR ANDY APP &nbsp; ✦</button>
    <div class="download-options" id="downloadOptions">
      <a class="download-card" href="https://pub-f94148bfb21f45bc8f23d4baf93b2c5f.r2.dev/Andy-App-1.6.apk" download>
        <span class="download-icon" aria-hidden="true">🤖</span><strong>Android</strong><small>Descargar APK · versión 1.6</small>
      </a>
      <a class="download-card" href="https://pub-f94148bfb21f45bc8f23d4baf93b2c5f.r2.dev/Andy-App-Desktop.zip" download>
        <span class="download-icon" aria-hidden="true">▣</span><strong>Windows</strong><small>Paquete web · ZIP para instalar desde el navegador</small>
      </a>
      <a class="download-card" href="https://pub-f94148bfb21f45bc8f23d4baf93b2c5f.r2.dev/Andy-App-Desktop.zip" download>
        <span class="download-icon" aria-hidden="true">⌘</span><strong>macOS</strong><small>Paquete web · ZIP para instalar desde el navegador</small>
      </a>
    </div>
    <p class="download-note">En Windows y Mac se descarga el paquete web ZIP; no es un instalador .exe o .dmg. Para instalarla como app de escritorio, publica Andy App y usa “Instalar aplicación” en Edge o Chrome.</p>
  </section>

  <section class="glass">
    <h2>🌎 HORARIOS DEL LANZAMIENTO</h2>
    <div class="grid" id="zones"></div>
  </section>

  <footer>ANDY APP · LLEGANDO A TU MUNDO · 17 NOVIEMBRE</footer>
</main>
</div>

<script>
// Lanzamiento: 17 de noviembre de 2026 a las 00:00 en Perú.
const launchUTC = Date.UTC(2026,10,17,5,0,0);

const zones = [
  ["🇵🇪","Perú","America/Lima","PET"],
  ["🇰🇷","Corea del Sur","Asia/Seoul","KST"],
  ["🇯🇵","Japón","Asia/Tokyo","JST"],
  ["🇪🇸","España","Europe/Madrid","CET/CEST"],
  ["🇬🇧","Reino Unido","Europe/London","GMT/BST"],
  ["🇺🇸","Nueva York","America/New_York","ET"],
  ["🇺🇸","Los Ángeles","America/Los_Angeles","PT"],
  ["🇲🇽","México CDMX","America/Mexico_City","CST"],
  ["🇦🇷","Argentina","America/Argentina/Buenos_Aires","ART"],
  ["🇧🇷","Brasil SP","America/Sao_Paulo","BRT"],
  ["🇨🇱","Chile Santiago","America/Santiago","CLT/CLST"],
  ["🇨🇴","Colombia","America/Bogota","COT"]
];

function fmtTime(date,tz){
  return new Intl.DateTimeFormat("es-ES",{timeZone:tz,hour:"2-digit",minute:"2-digit",hour12:false}).format(date);
}
function fmtDate(date,tz){
  return new Intl.DateTimeFormat("es-ES",{timeZone:tz,day:"2-digit",month:"short"}).format(date).replace(".","");
}
function renderZones(){
  const el=document.getElementById("zones");
  el.innerHTML=zones.map(([flag,name,tz,abbr])=>`
    <div class="timecard">
      <div class="country">${flag} ${name}</div>
      <div class="zone">${abbr}</div>
      <div class="local">${fmtTime(new Date(launchUTC),tz)}</div>
      <div class="date">${fmtDate(new Date(launchUTC),tz)}</div>
    </div>`).join("");
}
function pad(n){return String(n).padStart(2,"0")}

const previewMode = new URLSearchParams(location.search).has("preview");
function revealDownloads(){
  document.getElementById("downloadLaunch").classList.add("visible");
}
document.getElementById("downloadToggle").addEventListener("click",()=>{
  const options=document.getElementById("downloadOptions");
  const open=options.classList.toggle("open");
  document.getElementById("downloadToggle").setAttribute("aria-expanded",String(open));
});

function update(){
  let diff=launchUTC-Date.now();
  if(previewMode) diff=0;
  if(diff<=0){
    document.getElementById("days").textContent="00";
    document.getElementById("hours").textContent="00";
    document.getElementById("minutes").textContent="00";
    document.getElementById("seconds").textContent="00";
    document.getElementById("statusText").textContent="🚀 ANDY APP YA ESTÁ AQUÍ";
    revealDownloads();
    return;
  }
  const d=Math.floor(diff/86400000); diff-=d*86400000;
  const h=Math.floor(diff/3600000); diff-=h*3600000;
  const m=Math.floor(diff/60000); diff-=m*60000;
  const s=Math.floor(diff/1000);
  document.getElementById("days").textContent=pad(d);
  document.getElementById("hours").textContent=pad(h);
  document.getElementById("minutes").textContent=pad(m);
  document.getElementById("seconds").textContent=pad(s);
}

renderZones();
update();
setInterval(update,1000);

// Fondo de estrellas animado, ligero y sin dependencias.
const c=document.getElementById("stars"),ctx=c.getContext("2d");
let stars=[];
function resize(){
  const dpr=Math.min(devicePixelRatio||1,2);
  c.width=innerWidth*dpr;c.height=innerHeight*dpr;ctx.setTransform(dpr,0,0,dpr,0,0);
  stars=Array.from({length:Math.min(180,Math.floor(innerWidth/5))},()=>({
    x:Math.random()*innerWidth,y:Math.random()*innerHeight,r:Math.random()*1.4+.2,
    a:Math.random()*.7+.2,s:Math.random()*.018+.003
  }));
}
function draw(){
  ctx.clearRect(0,0,innerWidth,innerHeight);
  for(const st of stars){
    st.a+=Math.sin(Date.now()*st.s)*.002;
    ctx.globalAlpha=Math.max(.08,Math.min(.85,st.a));
    ctx.fillStyle="#fff";ctx.beginPath();ctx.arc(st.x,st.y,st.r,0,Math.PI*2);ctx.fill();
  }
  requestAnimationFrame(draw);
}
addEventListener("resize",resize);
resize();
draw();
</script>
</body>
</html>

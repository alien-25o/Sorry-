
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sorry Meri Kajukatli 🧸💗</title>

<style>
*{box-sizing:border-box}
body{
 margin:0;min-height:100vh;padding:18px;
 display:grid;place-items:center;overflow-x:hidden;
 font-family:"Trebuchet MS",sans-serif;color:#87445e;
 background:linear-gradient(135deg,#ffe0ec,#fff8f2,#f9e3ef);
}
.card{
 width:min(100%,560px);padding:26px 20px;text-align:center;
 background:#ffffffdc;border:2px solid #ffb8cd;
 border-radius:28px;box-shadow:0 15px 45px #c0447620;
 position:relative;z-index:1;
}
.page{display:none;animation:appear .45s ease}
.page.active{display:block}
@keyframes appear{
 from{opacity:0;transform:translateY(12px)}
 to{opacity:1;transform:translateY(0)}
}
h1{color:#bd4776;font-size:clamp(27px,7vw,38px)}
p{line-height:1.7}
.teddy{font-size:85px;animation:bob 2s infinite ease-in-out}
@keyframes bob{
 0%,100%{transform:translateY(0) rotate(-4deg)}
 50%{transform:translateY(-9px) rotate(4deg)}
}
.letter{
 background:#fff8fb;border:1px dashed #f3a1bb;
 border-radius:18px;padding:17px;margin:20px 0;line-height:1.8
}
.pill{
 display:inline-block;background:#ffe1eb;color:#bd4776;
 border-radius:30px;padding:8px 14px;font-size:12px;font-weight:bold
}
button{
 border:0;border-radius:30px;padding:13px 21px;
 font-size:16px;font-weight:bold;cursor:pointer;
 transition:transform .2s;touch-action:manipulation
}
button:active{transform:scale(.96)}
.primary,.yes{background:#ff8fb1;color:white}
.secondary{background:#ffe1eb;color:#bd4776}
.no{background:#b9eac5;color:#386d48}
.warning{
 display:inline-block;background:#fff0f5;border-radius:12px;
 padding:9px 12px;font-size:14px
}
.options{
 display:flex;justify-content:center;align-items:center;
 flex-wrap:wrap;gap:18px;min-height:70px;margin:18px 0
}
#reply{color:#bd4776;font-weight:bold;min-height:50px;line-height:1.6}
.nav{display:flex;justify-content:center;gap:9px;flex-wrap:wrap;margin-top:18px}
.nav button{font-size:14px}
.dots{margin-top:18px;color:#e78baa;letter-spacing:6px}
.bg-heart{
 position:fixed;bottom:-40px;pointer-events:none;
 animation:floatUp 8s linear infinite;opacity:.7;z-index:0
}
@keyframes floatUp{
 to{transform:translateY(-115vh) rotate(40deg);opacity:0}
}
.pop{
 position:fixed;z-index:10;pointer-events:none;font-size:24px;
 animation:pop 1.7s ease-out forwards
}
@keyframes pop{
 to{transform:translateY(-150px) scale(1.4);opacity:0}
}
.small{font-size:12px;color:#b47b91;margin-top:20px}
</style>
</head>

<body>
<div id="backgroundHearts"></div>

<main class="card">

<!-- PAGE 1: SWEET SHORT LETTER -->
<section class="page active" id="page1">
 <span class="pill">EK CHHOTI SI LETTER 💌</span>
 <div class="teddy">🧸💗</div>
 <h1>Meri Pyaari Kajukatli 🥹</h1>

 <div class="letter">
  I'm really sorry 🥺💗
 </b>
Mujhe maaf kar do na, please. 🥹🧸
Tumhe hurt karna mera intention nahi tha. ❤️‍🩹 and ab se nhi boluga aisa kuch 🥺
  <br><br>
 </b>
  sorry ab gussa mat kro plzz 🤗🧸</b>
 </div>

 <button class="primary" onclick="showPage(2)">
  Aage dekho 🙈 💗
 </button>
 <div class="dots">● ○ ○</div>
</section>

<!-- PAGE 2: PLEASE FORGIVE ME -->
<section class="page" id="page2">
 <span class="pill">PLEASE PLEASE 🥺</span>
 <div class="teddy">🧸🥺💐</div>
 <h1>Plzz maaf kr do na 🥹💗</h1>

 <p>
  Ab se aisa kuch nahi karunga, pakka promise! 🤞🏻💗
 </p>

 <div class="warning">
  (Dhyaan se choose karna option… 🙈)
 </div>

 <div class="options">
  <button id="yesBtn" class="yes">YES 💗</button>
  <button id="noBtn" class="no">NO 🥹</button>
 </div>

 <p id="reply" aria-live="polite"></p>

 <div class="nav">
  <button class="secondary" onclick="showPage(1)">← Back</button>
  <button class="secondary" onclick="showPage(3)">Surprise 🧸</button>
 </div>
 <div class="dots">○ ● ○</div>
</section>

<!-- PAGE 3: TEDDY HUG -->
<section class="page" id="page3">
 <span class="pill">EK LAST BAAT 💗</span>
 <div class="teddy">🐻💌</div>
 <h1> 🤗🤗🤗</h1>

 <div class="letter">
  tum bhi thoda wait kr liya kro . kabhi nhi aauga to phle hi bta duga  🥺💗
  <br><br>
  Yayyy 🥹💗 Mujhe pta tha tum mujhe maaf kr dogi! 🧸💕 Ab gussa chhodo aur ek cute si smile de do na 🙈❤️ Love you, meri kajukatli! 🫶🏻
  <br><br>
  <b>Tumhari smile = meri happiness! 🌷</b>
 </div>

 <button class="primary" onclick="hug()"> 🤗</button>
 <p id="hugReply"></p>

 <div class="nav">
  <button class="secondary" onclick="showPage(1)">Letter 💌</button>
  <button class="secondary" onclick="showPage(2)">Maaf kar do? 🥹</button>
 </div>
 <div class="dots">○ ○ ●</div>
</section>

<div class="small">Made with pyaar 🧸💗</div>
</main>

<script>
// Floating hearts in the background
const bg=document.getElementById("backgroundHearts");
["💗","♡","💕","♥","✨"].forEach((heart,i)=>{
 const el=document.createElement("span");
 el.className="bg-heart";
 el.textContent=heart;
 el.style.left=(8+i*20)+"%";
 el.style.animationDelay=(i*1.2)+"s";
 el.style.fontSize=(20+i*3)+"px";
 bg.appendChild(el);
});

// Switch between the 3 pages
function showPage(n){
 document.querySelectorAll(".page").forEach((p,i)=>{
  p.classList.toggle("active",i===n-1);
 });
 window.scrollTo({top:0,behavior:"smooth"});
 burst(n===2?5:3);
}

// Cute floating emoji animation
function burst(count){
 const emojis=["💗","💕","🧸","💌","✨","🌷"];
 for(let i=0;i<count;i++){
  const el=document.createElement("span");
  el.className="pop";
  el.textContent=emojis[Math.floor(Math.random()*emojis.length)];
  el.style.left=(5+Math.random()*90)+"vw";
  el.style.top=(55+Math.random()*35)+"vh";
  document.body.appendChild(el);
  setTimeout(()=>el.remove(),1800);
 }
}

// NO button runs away when touched or approached
const noBtn=document.getElementById("noBtn");
const yesBtn=document.getElementById("yesBtn");
const reply=document.getElementById("reply");
let noMoves=0;

function runAway(e){
 e.preventDefault();
 noMoves++;

 const margin=12;
 const maxX=Math.max(margin,window.innerWidth-noBtn.offsetWidth-margin);
 const maxY=Math.max(margin,window.innerHeight-noBtn.offsetHeight-margin);

 noBtn.style.position="fixed";
 noBtn.style.left=(margin+Math.random()*(maxX-margin))+"px";
 noBtn.style.top=(margin+Math.random()*(maxY-margin))+"px";
 noBtn.style.zIndex="20";

 if(noMoves===1){
  reply.textContent="Pakad ke dikhao 😜🙈";
 }else if(noMoves===2){
  reply.textContent="Hehe! Itni jaldi nahi pakad paoge 😂💨";
 }else{
  reply.textContent="YES pe click kar do na, please 🥹💗";
 }
}

noBtn.addEventListener("pointerenter",runAway);
noBtn.addEventListener("click",runAway);

// YES button reveals the sweet message
yesBtn.addEventListener("click",()=>{
 noBtn.style.position="relative";
 noBtn.style.left="";
 noBtn.style.top="";
 noBtn.style.zIndex="";

 reply.textContent=
 "Mujhe pta tha tum mujhe maaf kr dogi 🥹💗 Thank you meri kajukatli! 🤗🧸💕";

 yesBtn.textContent="YAYYY! LOVE YOU 💗";
 burst(28);
});

// Teddy hug on page 3
function hug(){
 document.getElementById("hugReply").textContent=
 "Awww! How sweet you are 🤗🧸💗";
 burst(18);
}
</script>
</body>
</html>

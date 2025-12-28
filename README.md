<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>For My Vaishnavi ❤️</title>

<link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600&family=Playfair+Display:wght@600&family=Poppins:wght@300;400;500&display=swap" rel="stylesheet">

<style>
:root{
 --primary:#c2185b;
 --secondary:#ffc1e3;
 --glass:rgba(255,255,255,.9);
}

*{box-sizing:border-box}

body{
 margin:0;
 font-family:Poppins,sans-serif;
 background:linear-gradient(135deg,#fff0f3,#ffe6e9);
 color:#444;
 overflow-x:hidden;
}

/* PASSWORD */
#lockScreen{
 position:fixed;inset:0;
 background:#000;
 display:flex;
 flex-direction:column;
 justify-content:center;
 align-items:center;
 z-index:99999;
 color:white;
}
#lockScreen input{
 padding:12px 20px;
 border-radius:30px;
 border:none;
 margin:15px;
 font-size:1rem;
}

/* START */
#start-overlay{
 position:fixed;inset:0;
 background:#000;
 display:flex;
 flex-direction:column;
 justify-content:center;
 align-items:center;
 color:white;
 z-index:9999;
 transition:.8s;
}

/* BACKGROUND HEARTS */
.bg-hearts{position:fixed;inset:0;z-index:-1;overflow:hidden}
.heart-bg{
 position:absolute;
 bottom:-50px;
 opacity:.3;
 animation:floatUp linear infinite;
}
@keyframes floatUp{
 to{transform:translateY(-110vh) rotate(360deg)}
}

/* SECTIONS */
section{
 max-width:650px;
 margin:40px auto;
 padding:35px 25px;
 background:var(--glass);
 border-radius:20px;
 box-shadow:0 10px 30px rgba(0,0,0,.08);
 text-align:center;
 opacity:0;
 transform:translateY(30px);
 transition:.8s;
}
section.visible{opacity:1;transform:none}

h1,h2{
 font-family:Playfair Display,serif;
 color:var(--primary);
}

/* TEXT BOX */
.text-content{
 text-align:left;
 background:#fff;
 padding:25px;
 border-radius:15px;
 border-left:5px solid var(--primary);
}

/* DIVIDER */
.divider{
 display:flex;
 justify-content:center;
 margin:40px 0;
}
.divider span{
 font-size:2rem;
 opacity:.6;
 animation:floatHeart 3s infinite;
}
@keyframes floatHeart{
 50%{transform:translateY(-10px)}
}

/* MOOD */
#moodText{font-weight:bold}

/* TIMER */
.timer-container{
 display:flex;
 justify-content:space-around;
 background:#fff;
 padding:15px;
 border-radius:15px;
}
.time-val{
 font-size:1.8rem;
 font-weight:700;
 color:var(--primary)
}

/* CHAT */
.chat-box{
 background:#efe7dd;
 height:320px;
 overflow-y:auto;
 padding:15px;
 border-radius:15px;
 display:flex;
 flex-direction:column;
}
.msg{
 max-width:80%;
 padding:10px 15px;
 margin:8px 0;
 border-radius:15px;
 background:#dcf8c6;
 align-self:flex-end;
}

/* POETRY */
.poetry-box{
 font-family:Dancing Script,cursive;
 font-size:1.6rem;
 color:#880e4f;
 background:#fff;
 padding:30px;
 border-radius:15px;
}
.signature{
 display:inline-block;
 font-size:1.8rem;
 color:#c2185b;
 opacity:0;
 transform:translateY(10px);
 animation:fadeSig 2s ease forwards;
 animation-delay:1.5s;
}
@keyframes fadeSig{to{opacity:1;transform:none}}

/* HEARTBEAT */
.heartbeat{
 font-size:2.2rem;
 animation:beat 1.4s infinite;
}
@keyframes beat{
 0%,100%{transform:scale(1)}
 50%{transform:scale(1.2)}
}

/* PROMISE */
.jar{font-size:90px;cursor:pointer}
#promise-modal{
 position:fixed;inset:0;
 background:rgba(0,0,0,.7);
 display:none;
 justify-content:center;
 align-items:center;
}
.modal-content{
 background:#fff;
 padding:30px;
 border-radius:20px;
 text-align:center;
}
.promise-text{
 font-family:Dancing Script,cursive;
 font-size:2rem;
 color:var(--primary);
}

/* COUPON */
.coupon-card{
 display:none;
 background:#fff;
 border:2px dashed var(--primary);
 padding:20px;
 border-radius:15px;
 margin-top:15px;
}

/* GALLERY */
.gallery{
 display:flex;
 gap:12px;
 flex-wrap:wrap;
 justify-content:center;
}
.gallery img{
 width:45%;
 border-radius:10px;
}

/* CHOICE */
.choice-box{
 display:flex;
 gap:10px;
 justify-content:center;
 flex-wrap:wrap;
 margin-top:20px;
}
.choice-box button{
 border:none;
 padding:10px 18px;
 border-radius:25px;
 background:#f3f3f3;
 cursor:pointer;
}

/* WHATSAPP */
.wa-btn{
 position:fixed;
 bottom:20px;
 right:20px;
 background:#25d366;
 color:#fff;
 padding:12px 22px;
 border-radius:40px;
 text-decoration:none;
 font-weight:600;
 display:none;
}

/* NIGHT MODE */
body.night{
 background:linear-gradient(135deg,#0f0f1a,#1a1a2e);
 color:#eee;
}
body.night section{background:rgba(30,30,50,.9)}

/* CONFETTI */
.confetti{
 position:fixed;
 width:10px;height:10px;
 top:-10px;
 animation:fall linear forwards;
}
@keyframes fall{
 to{top:110vh;transform:rotate(720deg)}
}
</style>
</head>

<body>

<!-- PASSWORD -->
<div id="lockScreen">
 <h2>Only for Vaishnavi 💖</h2>
 <input id="passInput" type="password" placeholder="Enter password">
 <button onclick="unlockSite()">Enter</button>
 <p id="err" style="color:#ff6b6b"></p>
</div>

<div class="bg-hearts" id="bg-hearts"></div>

<div id="start-overlay">
 <h1>For My Vaishnavi ❤️</h1>
 <button onclick="startExperience()">Open My Heart</button>
</div>

<div id="main-content" style="display:none">

<!-- APOLOGY -->
<section>
<h1>I am Sorry.</h1>
<p>How angry are you?</p>
<input type="range" min="0" max="100" value="100" id="moodRange" oninput="checkMood()">
<p id="moodText">😡 Furious!</p>

<div class="text-content" style="margin-top:25px">
<p>Vaishnavi,</p>
<p>Main bina kisi excuse ke apni har galti accept karta hoon.</p>
<p>Gussa, ego aur misunderstanding meri wajah se hui.</p>
<p>Agar tumhe meri kisi baat se dard hua ho, toh main dil se sorry hoon.</p>
<p><b>Please mujhe maaf kar do.</b></p>
<p style="font-style:italic;color:#777">
I take full responsibility for my actions — without excuses.
</p>
</div>
</section>

<div class="divider"><span>🤍</span></div>

<!-- TIMER -->
<section>
<h2>⏳ Countdown</h2>
<div class="timer-container">
<div><span id="days" class="time-val">00</span> Days</div>
<div><span id="hours" class="time-val">00</span> Hrs</div>
<div><span id="minutes" class="time-val">00</span> Min</div>
<div><span id="seconds" class="time-val">00</span> Sec</div>
</div>
</section>

<!-- CHAT -->
<section>
<h2>💬 One Conversation</h2>
<div class="chat-box" id="chatBox"></div>
</section>

<!-- CONFESSION -->
<section>
<h2>💌 My Confession</h2>
<div class="text-content">
<p><b>My Dear Vaishnavi,</b></p>
<p>Tum sirf meri girlfriend nahi thi, tum meri safe place thi.</p>
<p>Main perfect nahi hoon, par mera pyaar kabhi fake nahi tha.</p>
<p>Future ka har scene mujhe tumhare saath hi dikhta hai.</p>
<p><b>Agar ek chhota sa bhi chance bacha ho, toh please mujhe de do.</b></p>
</div>

<p class="heartbeat">💗</p>

<div class="choice-box">
<button onclick="choice('yes')">🤍 I’m open to talk</button>
<button onclick="choice('maybe')">💭 I need time</button>
<button onclick="choice('no')">🕊️ I understand</button>
</div>
<p id="choiceText"></p>
</section>

<!-- POETRY -->
<section>
<h2>🌹 For You</h2>
<div class="poetry-box">
Only you can make me whole ❤️<br><br>
<span class="signature">— urs Devulla 💌</span>
</div>
</section>

<!-- PROMISE -->
<section>
<h2>🏺 Promise Jar</h2>
<div class="jar" onclick="openJar()">🏺</div>
</section>

<!-- COUPON -->
<section>
<h2>🎁 Love Coupon</h2>
<button onclick="revealGift()">Reveal</button>
<div class="coupon-card" id="myCoupon">
🫂 Unlimited Hugs<br>
🥟 Unlimited Momos<br>
💬 Lifetime Communication
</div>
</section>

<!-- GALLERY -->
<section>
<h2>📸 Memories</h2>
<div class="gallery">
<img src="https://i.ibb.co/WvZCqXrJ/f050c675-8b43-4e06-be87-a6d71669c771-d146cfb7-252f-48cb-ba3c-9da826f0f173-2.jpg">
<img src="https://i.ibb.co/xbLT1BP/Screenshot-20251227-063846-Photos.jpg">
</div>
</section>

<!-- FINAL MESSAGE -->
<section id="finalMsg" style="display:none">
<h2>💖 One Last Thing</h2>
<p style="font-family:Dancing Script,cursive;font-size:1.8rem">
Agar tum yahan tak aayi ho…<br>
toh shayad dil maanta hai ❤️<br><br>
— urs Devulla 💌
</p>
</section>

<a class="wa-btn" id="waBtn" href="https://wa.me/919369068575">Reply 💬</a>
<button onclick="toggleNight()" style="position:fixed;bottom:80px;right:20px">🌙</button>

</div>

<div id="promise-modal" onclick="closeJar()">
<div class="modal-content" onclick="event.stopPropagation()">
<div class="promise-text" id="modalText"></div>
<button onclick="closeJar()">Keep ❤️</button>
</div>
</div>

<audio id="bgMusic" loop>
<source src="https://cdn.pixabay.com/download/audio/2022/03/23/audio_07b2a04654.mp3">
</audio>

<script>
function unlockSite(){
 if(passInput.value==="vaishnavi") lockScreen.style.display="none";
 else err.innerText="Wrong password 💔";
}

function startExperience(){
 bgMusic.volume=.5;
 bgMusic.play().catch(()=>{});
 start-overlay.style.opacity=0;
 setTimeout(()=>{
  start-overlay.style.display="none";
  main-content.style.display="block";
  revealSections();startChat();
 },800);
}

function revealSections(){
 const o=new IntersectionObserver(e=>e.forEach(x=>x.isIntersecting&&x.target.classList.add("visible")));
 document.querySelectorAll("section").forEach(s=>o.observe(s));
}

for(let i=0;i<20;i++){
 let h=document.createElement("div");
 h.innerText="❤️";
 h.className="heart-bg";
 h.style.left=Math.random()*100+"vw";
 h.style.fontSize=(10+Math.random()*20)+"px";
 h.style.animationDuration=(8+Math.random()*6)+"s";
 bg-hearts.appendChild(h);
}

function checkMood(){
 let v=moodRange.value;
 moodText.textContent=v>80?"😡 Furious!":v>40?"😠 Still Upset":"💖 Maybe forgiving…";
}

const target=new Date(2025,7,2).getTime();
setInterval(()=>{
 let d=target-Date.now();if(d<0)d=0;
 days.textContent=Math.floor(d/86400000);
 hours.textContent=Math.floor(d/3600000)%24;
 minutes.textContent=Math.floor(d/60000)%60;
 seconds.textContent=Math.floor(d/1000)%60;
},1000);

const msgs=["Vaishnavi...","I know you are upset.","Please read this once.","I made this for you ❤️"];
let i=0;
function startChat(){
 function add(){
  if(i<msgs.length){
   let m=document.createElement("div");
   m.className="msg";
   m.innerText=msgs[i++];
   chatBox.appendChild(m);
   setTimeout(add,2000);
  }else waBtn.style.display="block";
 }
 add();
}

const promises=[
"I promise to listen more.",
"I promise to respect your feelings.",
"I promise to control my anger.",
"I promise to never take you for granted.",
"I promise to love you always."
];
let sp=[],pi=0;
function shuffle(){sp=[...promises].sort(()=>Math.random()-.5);pi=0}
shuffle();
function openJar(){
 if(pi>=sp.length)shuffle();
 modalText.innerText="✨ "+sp[pi++];
 promise-modal.style.display="flex";
 confetti();
}
function closeJar(){promise-modal.style.display="none"}

function revealGift(){myCoupon.style.display="block";confetti()}

function confetti(){
 for(let i=0;i<25;i++){
  let c=document.createElement("div");
  c.className="confetti";
  c.style.left=Math.random()*100+"vw";
  c.style.background=["#ffeb3b","#ff4081","#00e676","#2979ff"][Math.floor(Math.random()*4)];
  c.style.animationDuration=(2+Math.random()*2)+"s";
  document.body.appendChild(c);
  setTimeout(()=>c.remove(),3000);
 }
}

function toggleNight(){document.body.classList.toggle("night")}

function choice(type){
 if(type==="yes") choiceText.innerText="Thank you for giving us a chance 🤍";
 if(type==="maybe") choiceText.innerText="I respect your space. I’ll wait 💭";
 if(type==="no") choiceText.innerText="I respect your decision. Always wishing you happiness 🕊️";
}

addEventListener("scroll",()=>{
 if(innerHeight+scrollY>=document.body.offsetHeight-50)
  finalMsg.style.display="block";
});
</script>

</body>
</html>

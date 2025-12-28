<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>For My Vaishnavi ❤️</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600&family=Playfair+Display:ital,wght@0,600;1,600&family=Poppins:wght@300;400;500&display=swap" rel="stylesheet">

<style>
    :root {
        --primary: #c2185b; /* Deep Rose */
        --secondary: #ffc1e3; /* Soft Pink */
        --gold: #d4af37;
        --text: #4a4a4a;
        --glass: rgba(255, 255, 255, 0.9);
        --bg-gradient: linear-gradient(135deg, #fff0f3 0%, #ffe6e9 100%);
    }

    * { box-sizing: border-box; }

    body {
        margin: 0;
        font-family: 'Poppins', sans-serif;
        background: var(--bg-gradient);
        color: var(--text);
        overflow-x: hidden;
        /* Custom Cursor */
        cursor: url('https://cur.cursors-4u.net/nature/nat-10/nat984.cur'), auto;
    }

    /* Force cursor on interactive elements */
    a, button, .jar-container, .gift-box, input, .close-btn {
        cursor: url('https://cur.cursors-4u.net/nature/nat-10/nat984.cur'), pointer;
    }

    /* --- BACKGROUND ANIMATION --- */
    .bg-hearts {
        position: fixed; top: 0; left: 0; width: 100%; height: 100%;
        overflow: hidden; z-index: -1; pointer-events: none;
    }
    .heart-bg {
        position: absolute; bottom: -50px;
        color: var(--primary); opacity: 0.3;
        animation: floatUp linear infinite;
    }
    @keyframes floatUp {
        to { transform: translateY(-110vh) rotate(360deg); }
    }

    /* --- START SCREEN (Music Fix) --- */
    #start-overlay {
        position: fixed; top: 0; left: 0; width: 100%; height: 100%;
        background: #000; display: flex; flex-direction: column;
        justify-content: center; align-items: center; z-index: 10000;
        color: white; text-align: center;
        transition: opacity 0.8s ease;
    }
    #start-overlay h1 {
        font-family: 'Playfair Display', serif; font-size: 3rem; color: var(--secondary);
        margin-bottom: 20px;
    }
    .enter-btn {
        padding: 15px 40px; background: var(--primary); color: white;
        border: 2px solid var(--secondary); border-radius: 50px;
        font-size: 1.2rem; font-family: 'Poppins', sans-serif;
        box-shadow: 0 0 20px rgba(194, 24, 91, 0.5);
        animation: pulse 2s infinite;
    }

    /* --- SECTIONS --- */
    section {
        max-width: 650px; margin: 40px auto; padding: 40px 25px;
        background: var(--glass); border-radius: 20px;
        box-shadow: 0 10px 30px rgba(0,0,0,0.08);
        text-align: center;
        border: 1px solid white;
        opacity: 0; transform: translateY(30px); transition: all 0.8s ease;
    }
    section.visible { opacity: 1; transform: translateY(0); }

    h1, h2 { font-family: 'Playfair Display', serif; color: var(--primary); margin-top: 0; }
    h1 { font-size: 2.5rem; }
    h2 { font-size: 1.8rem; border-bottom: 2px solid var(--secondary); display: inline-block; padding-bottom: 10px; margin-bottom: 25px; }
    p { font-size: 1rem; line-height: 1.7; color: #555; }

    /* --- SPECIAL SECTIONS --- */
    .text-content {
        text-align: left; background: #fff; padding: 25px;
        border-radius: 15px; border-left: 5px solid var(--primary);
        box-shadow: inset 0 0 10px rgba(0,0,0,0.03);
    }
    .highlight { background: #fff3cd; padding: 2px 6px; border-radius: 4px; font-weight: 600; color: #333; }

    .poetry-box {
        font-family: 'Dancing Script', cursive; font-size: 1.6rem;
        line-height: 1.5; color: #880e4f;
        background: radial-gradient(circle, #fff0f3, #fff);
        padding: 30px; border: 1px dashed var(--primary); border-radius: 15px;
    }

    /* --- TIMER --- */
    .timer-container {
        display: flex; justify-content: space-around;
        background: #fff; padding: 15px; border-radius: 15px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.05);
    }
    .time-unit { display: flex; flex-direction: column; }
    .time-val { font-size: 1.8rem; font-weight: 700; color: var(--primary); font-family: 'Poppins', sans-serif;}
    .time-label { font-size: 0.8rem; color: #888; text-transform: uppercase; letter-spacing: 1px;}

    /* --- CHAT --- */
    .chat-box {
        background: #efe7dd; height: 320px; overflow-y: auto;
        padding: 20px; border-radius: 15px; display: flex; flex-direction: column;
        border: 4px solid #fff;
    }
    .msg {
        max-width: 80%; padding: 10px 15px; margin: 8px 0; border-radius: 15px;
        font-size: 0.95rem; position: relative; opacity: 0; transform: translateY(10px);
        transition: 0.5s; box-shadow: 0 2px 5px rgba(0,0,0,0.05);
    }
    .msg.show { opacity: 1; transform: translateY(0); }
    .sent { align-self: flex-end; background: #dcf8c6; border-bottom-right-radius: 2px; }
    .received { align-self: flex-start; background: #fff; border-bottom-left-radius: 2px; }

    /* --- PROMISE JAR (FIXED) --- */
    .jar-wrapper { position: relative; display: inline-block; transition: transform 0.2s; }
    .jar-wrapper:active { transform: scale(0.95) rotate(5deg); }
    .jar-icon { font-size: 90px; filter: drop-shadow(0 5px 5px rgba(0,0,0,0.1)); }
    
    /* Promise Modal */
    #promise-modal {
        position: fixed; top: 0; left: 0; width: 100%; height: 100%;
        background: rgba(0,0,0,0.8); z-index: 5000;
        display: none; justify-content: center; align-items: center;
        backdrop-filter: blur(5px);
    }
    .modal-content {
        background: white; padding: 40px; border-radius: 20px;
        max-width: 85%; width: 400px; text-align: center;
        position: relative; animation: popIn 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        border: 4px solid var(--gold);
    }
    .promise-text { font-family: 'Dancing Script', cursive; font-size: 2rem; color: var(--primary); margin-bottom: 20px; }
    .close-btn {
        background: var(--text); color: white; border: none;
        padding: 10px 25px; border-radius: 30px; font-weight: bold;
    }
    
    /* --- GALLERY (Polaroid) --- */
    .gallery { display: flex; flex-wrap: wrap; justify-content: center; gap: 15px; }
    .polaroid {
        background: white; padding: 10px 10px 35px 10px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.15); width: 45%; max-width: 180px;
        transform: rotate(-3deg); transition: transform 0.3s;
    }
    .polaroid:nth-child(even) { transform: rotate(3deg); }
    .polaroid:hover { transform: scale(1.1) rotate(0deg); z-index: 10; }
    .polaroid img { width: 100%; height: 180px; object-fit: cover; }

    /* --- COUPON --- */
    .coupon-container { margin-top: 20px; }
    .gift-btn { font-size: 70px; animation: bounce 2s infinite; }
    .coupon-card {
        display: none; background: #fff; border: 2px dashed var(--primary);
        padding: 20px; margin-top: 20px; border-radius: 10px;
    }

    /* --- EXTRAS --- */
    .wa-btn {
        position: fixed; bottom: 25px; right: 25px;
        background: #25d366; color: white; padding: 15px 25px;
        border-radius: 50px; text-decoration: none; font-weight: 600;
        box-shadow: 0 5px 15px rgba(0,0,0,0.2); z-index: 2000;
        display: none;
    }

    @keyframes pulse { 0% { transform: scale(1); } 50% { transform: scale(1.05); } 100% { transform: scale(1); } }
    @keyframes popIn { from { opacity: 0; transform: scale(0.5); } to { opacity: 1; transform: scale(1); } }
    @keyframes bounce { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-15px); } }

    .confetti { position: fixed; width: 10px; height: 10px; top: -10px; z-index: 9999; animation: fall linear forwards; }
    @keyframes fall { to { top: 110vh; transform: rotate(720deg); } }

</style>
</head>
<body>

    <div class="bg-hearts" id="bg-hearts"></div>

    <div id="start-overlay">
        <h1>For My Vaishnavi ❤️</h1>
        <p>Headphones Recommended 🎧</p>
        <button class="enter-btn" onclick="startExperience()">Open My Heart</button>
    </div>

    <div id="main-content" style="display:none;">

        <section>
            <h1>I am Sorry.</h1>
            <p>I know I messed up. Just hear me out?</p>
            <div style="margin-top: 30px;">
                <p style="margin-bottom:10px;">How angry are you?</p>
                <input type="range" min="0" max="100" value="100" id="moodRange" style="width:100%; accent-color: var(--primary);" oninput="checkMood()">
                <p id="moodText" style="font-weight:bold; color:var(--primary); margin-top:10px;">😡 Furious!</p>
            </div>
        </section>

        <section>
            <h2>⏳ The Countdown</h2>
            <p>Time remaining until our fresh start (Aug 2, 2025)</p>
            <div class="timer-container">
                <div class="time-unit"><span class="time-val" id="days">00</span><span class="time-label">Days</span></div>
                <div class="time-unit"><span class="time-val" id="hours">00</span><span class="time-label">Hrs</span></div>
                <div class="time-unit"><span class="time-val" id="minutes">00</span><span class="time-label">Mins</span></div>
                <div class="time-unit"><span class="time-val" id="seconds">00</span><span class="time-label">Secs</span></div>
            </div>
        </section>

        <section>
            <h2>💬 Just One Conversation</h2>
            <div class="chat-box" id="chatBox"></div>
        </section>

        <section>
            <h2>😔 My Confession</h2>
            <div class="text-content">
                <p>My Dear Vaishnavi,</p>
                <p>I know maine galti ki hai aur main apni saari galti accept karta hoon. Please Vaishnavi mujhe maaf kar do.</p>
                <p>Main tere rude behaviour se gusse mein aa gaya tha. <span class="highlight">Teri story pe Anush ka comment dekh ke main sach mein toot gaya tha.</span></p>
                <p>Maine <span class="highlight">Antrika</span> ke saath koi chugli nahi ki thi. Main sirf itna kehne gaya tha ki wo apne bf ko control kare.</p>
                <p>Meri wajah se agar teri friendship toot gayi ho, toh main dil se maafi maangta hoon.</p>
                <p><b>Please Vaishnavi, ek last chance de do. I swear, I will treat you like a queen. 👑</b></p>
            </div>
        </section>

        <section>
            <h2>💌 A Letter From My Heart</h2>
            <div class="text-content">
                <p><b>My Dearest Vaishnavi,</b></p>
                <p>Before you, I was just existing, but with you, I started living. You are not just my girlfriend; you are my best friend, my safe place, and the only person who truly understands me.</p>
                <p>I know I am not perfect. I make mistakes. But never for a second doubt my love for you.</p>
                <p>I cannot imagine a future that doesn't have you in it.</p>
                <p>I love you more than words can say, and I will keep loving you until my very last breath. You are my forever. 💐🛐</p>
            </div>
        </section>

        <section>
            <h2>🌹 For You</h2>
            <div class="poetry-box">
                "I miss the smile upon your face,<br>
                I miss your warm and loving embrace.<br>
                Please forget the fights we had,<br>
                Being apart makes me so sad.<br><br>
                Vaishnavi, you are my heart and soul,<br>
                Only you can make me whole." ❤️
            </div>
        </section>

        <section>
            <h2>🏺 The Promise Jar</h2>
            <p>Tap the jar to pull out a promise.</p>
            <div class="jar-wrapper" onclick="openJar()">
                <div class="jar-icon">🏺</div>
            </div>
        </section>

        <section>
            <h2>📸 Our Memories</h2>
            <div class="gallery">
                <div class="polaroid"><img src="https://i.ibb.co/WvZCqXrJ/f050c675-8b43-4e06-be87-a6d71669c771-d146cfb7-252f-48cb-ba3c-9da826f0f173-2.jpg"></div>
                <div class="polaroid"><img src="https://i.ibb.co/xbLT1BP/Screenshot-20251227-063846-Photos.jpg"></div>
                <div class="polaroid"><img src="https://i.ibb.co/Txmdv3Kr/Screenshot-20251227-145012-Gallery.jpg"></div>
                <div class="polaroid"><img src="https://i.ibb.co/RkN4dd2P/Screenshot-20251227-145038-Gallery.jpg"></div>
            </div>
        </section>

        <section>
            <h2>🎁 Peace Offering</h2>
            <div class="coupon-container">
                <div class="gift-btn" onclick="revealGift()">🎁</div>
                <div class="coupon-card" id="myCoupon">
                    <h3>Coupon Code: LOVE2025</h3>
                    <p>Valid for: <b>One Long Hug 🫂 & Unlimited Momos 🥟</b></p>
                    <p><small>Redeemable anytime. Lifetime validity.</small></p>
                </div>
            </div>
        </section>

        <a href="https://wa.me/919369068575" class="wa-btn" id="waBtn">Reply? 💬</a>

    </div>

    <div id="promise-modal" onclick="closeJar()">
        <div class="modal-content" onclick="event.stopPropagation()">
            <div class="promise-text" id="modalText">...</div>
            <button class="close-btn" onclick="closeJar()">Keep This Promise ❤️</button>
        </div>
    </div>

    <audio id="bgMusic" loop>
        <source src="https://cdn.pixabay.com/download/audio/2022/03/23/audio_07b2a04654.mp3?filename=emotional-piano-113572.mp3" type="audio/mp3">
    </audio>

<script>
    // --- 1. START EXPERIENCE (Fixes Audio) ---
    function startExperience() {
        // Play Audio
        const music = document.getElementById('bgMusic');
        music.volume = 0.5;
        music.play().catch(e => console.log("Audio Error:", e));

        // Fade out overlay
        const overlay = document.getElementById('start-overlay');
        overlay.style.opacity = '0';
        setTimeout(() => {
            overlay.style.display = 'none';
            document.getElementById('main-content').style.display = 'block';
            revealSections(); // Start Scroll Animation
            startChat(); // Start Chat
        }, 800);
    }

    // --- 2. SCROLL ANIMATION ---
    function revealSections() {
        const sections = document.querySelectorAll('section');
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) entry.target.classList.add('visible');
            });
        }, { threshold: 0.1 });
        sections.forEach(sec => observer.observe(sec));
    }

    // --- 3. BACKGROUND HEARTS ---
    function createHearts() {
        const container = document.getElementById('bg-hearts');
        for (let i = 0; i < 20; i++) {
            const heart = document.createElement('div');
            heart.innerHTML = '❤️';
            heart.className = 'heart-bg';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = (Math.random() * 5 + 8) + 's';
            heart.style.fontSize = (Math.random() * 20 + 10) + 'px';
            container.appendChild(heart);
        }
    }
    createHearts();

    // --- 4. TIMER (Countdown to Aug 2, 2025) ---
    const targetDate = new Date("August 2, 2025 00:00:00").getTime();
    
    setInterval(() => {
        const now = new Date().getTime();
        const diff = targetDate - now;

        if (diff < 0) {
            document.getElementById("days").innerText = "00";
            return;
        }

        const d = Math.floor(diff / (1000 * 60 * 60 * 24));
        const h = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        const m = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
        const s = Math.floor((diff % (1000 * 60)) / 1000);

        document.getElementById("days").innerText = d;
        document.getElementById("hours").innerText = h;
        document.getElementById("minutes").innerText = m;
        document.getElementById("seconds").innerText = s;
    }, 1000);

    // --- 5. CHAT ANIMATION ---
    const messages = [
        { text: "Vaishnavi...", type: "sent", delay: 1000 },
        { text: "I know you are upset.", type: "sent", delay: 3000 },
        { text: "Please just read this once.", type: "sent", delay: 5000 },
        { text: "I made this for you. ❤️", type: "sent", delay: 7000 }
    ];

    function startChat() {
        const box = document.getElementById('chatBox');
        let i = 0;
        function addMsg() {
            if (i < messages.length) {
                const div = document.createElement('div');
                div.className = `msg ${messages[i].type}`;
                div.innerText = messages[i].text;
                box.appendChild(div);
                setTimeout(() => div.classList.add('show'), 50);
                box.scrollTop = box.scrollHeight;
                i++;
                if (i < messages.length) setTimeout(addMsg, messages[i-1].delay);
                else setTimeout(() => document.getElementById('waBtn').style.display = 'block', 2000);
            }
        }
        addMsg();
    }

    // --- 6. PROMISE JAR LOGIC (FIXED) ---
    const promises = [
        "I promise to listen more and argue less.",
        "I promise to always bring you Momos.",
        "I promise to never take you for granted.",
        "I promise to support your dreams.",
        "I promise to communicate better.",
        "I promise to love you, even on bad days.",
        "I promise to make you feel like a Queen."
    ];

    function openJar() {
        const modal = document.getElementById('promise-modal');
        const text = document.getElementById('modalText');
        
        // Pick random promise
        const random = promises[Math.floor(Math.random() * promises.length)];
        text.innerText = "✨ " + random;
        
        modal.style.display = 'flex';
        triggerConfetti();
    }

    function closeJar() {
        document.getElementById('promise-modal').style.display = 'none';
    }

    // --- 7. MOOD SLIDER ---
    function checkMood() {
        const val = document.getElementById('moodRange').value;
        const txt = document.getElementById('moodText');
        if (val > 80) txt.innerText = "😡 Furious!";
        else if (val > 40) { txt.innerText = "😠 Still Upset"; txt.style.color = "orange"; }
        else { txt.innerText = "💖 Maybe forgiving..."; txt.style.color = "green"; }
    }

    // --- 8. COUPON ---
    function revealGift() {
        document.getElementById('myCoupon').style.display = 'block';
        triggerConfetti();
    }

    // --- 9. CONFETTI ---
    function triggerConfetti() {
        for (let i = 0; i < 50; i++) {
            const c = document.createElement('div');
            c.className = 'confetti';
            c.style.left = Math.random() * 100 + 'vw';
            c.style.backgroundColor = ['#ffeb3b', '#ff4081', '#00e676', '#2979ff'][Math.floor(Math.random() * 4)];
            c.style.animationDuration = (Math.random() * 2 + 2) + 's';
            document.body.appendChild(c);
            setTimeout(() => c.remove(), 4000);
        }
    }
</script>
</body>
</html>

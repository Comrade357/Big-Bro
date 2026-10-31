
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080706">
<title>For My Nana | Bimal ❤️</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Great+Vibes&family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
:root {
  --bg:#080706;
  --gold:#d7b46a;
  --light:#f6e5bd;
  --muted:#b9ad98;
  --border:rgba(215,180,106,.3);
  --panel:rgba(255,255,255,.035);
}

* {
  box-sizing:border-box;
  margin:0;
  padding:0;
}

html {scroll-behavior:smooth;}

body {
  background:
    radial-gradient(ellipse at 50% 0%,rgba(166,120,45,.13),transparent 45%),
    var(--bg);
  color:#f8f1e5;
  font-family:Montserrat,sans-serif;
  overflow-x:hidden;
}

button {font:inherit;}

#particles {
  position:fixed;
  inset:0;
  overflow:hidden;
  pointer-events:none;
  z-index:100;
}

.particle {
  position:absolute;
  bottom:-30px;
  animation:floatUp linear forwards;
  opacity:0;
  text-shadow:0 0 12px rgba(255,205,115,.6);
}

@keyframes floatUp {
  0% {transform:translateY(0) rotate(0);opacity:0;}
  15% {opacity:.85;}
  100% {transform:translateY(-110vh) rotate(360deg);opacity:0;}
}

@keyframes glow {
  0%,100% {text-shadow:0 0 15px rgba(215,180,106,.15);}
  50% {text-shadow:0 0 35px rgba(215,180,106,.55);}
}

@keyframes fadeIn {
  from {opacity:0;transform:translateY(25px);}
  to {opacity:1;transform:translateY(0);}
}

.gold {color:var(--gold);}
.script {font-family:"Great Vibes",cursive;}
.serif {font-family:"Cormorant Garamond",serif;}

.eyebrow {
  font-size:.7rem;
  letter-spacing:.3em;
  text-transform:uppercase;
  color:var(--gold);
  margin-bottom:18px;
}

.section {
  padding:100px 20px;
  position:relative;
  z-index:1;
}

.center {text-align:center;}

.section-title {
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(2.5rem,7vw,5rem);
  font-weight:500;
  line-height:1.05;
  margin-bottom:20px;
}

.subtitle {
  max-width:650px;
  margin:auto;
  color:var(--muted);
  line-height:1.9;
  font-size:.9rem;
}

.line {
  width:75px;
  height:1px;
  margin:25px auto;
  background:linear-gradient(90deg,transparent,var(--gold),transparent);
}

.btn {
  display:inline-block;
  padding:14px 28px;
  border:1px solid var(--gold);
  border-radius:50px;
  background:rgba(215,180,106,.08);
  color:var(--light);
  font-size:.72rem;
  letter-spacing:.15em;
  text-transform:uppercase;
  cursor:pointer;
  transition:.3s;
  text-decoration:none;
}

.btn:hover {
  background:var(--gold);
  color:#080706;
  transform:translateY(-3px);
  box-shadow:0 10px 30px rgba(215,180,106,.2);
}

/* Music */

.music-box {
  position:fixed;
  top:15px;
  right:15px;
  z-index:200;
  display:flex;
  align-items:center;
  gap:10px;
  padding:10px 14px;
  border:1px solid var(--border);
  border-radius:50px;
  background:rgba(8,7,6,.9);
  backdrop-filter:blur(15px);
}

.music-box span {
  font-size:.65rem;
  color:var(--gold);
}

.music-box button {
  width:32px;
  height:32px;
  border-radius:50%;
  border:1px solid var(--gold);
  color:var(--gold);
  background:transparent;
  cursor:pointer;
}

/* Locked screen */

#lockScreen {
  min-height:100vh;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  padding:100px 20px 60px;
  position:relative;
  z-index:2;
  overflow:hidden;
}

.lock-content {
  max-width:800px;
  animation:fadeIn 1.2s ease;
}

.lock-ring {
  width:210px;
  height:210px;
  border:1px solid rgba(215,180,106,.35);
  border-radius:50%;
  margin:0 auto 35px;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:5rem;
  box-shadow:0 0 0 18px rgba(215,180,106,.025),
             0 0 0 38px rgba(215,180,106,.015),
             inset 0 0 50px rgba(215,180,106,.05);
  animation:glow 4s infinite;
}

.lock-title {
  font-family:"Great Vibes",cursive;
  font-size:clamp(4rem,12vw,8rem);
  color:var(--light);
  font-weight:400;
  line-height:1;
}

.lock-name {
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(1.5rem,5vw,2.8rem);
  letter-spacing:.2em;
  margin-top:20px;
  text-transform:uppercase;
}

.lock-description {
  max-width:570px;
  margin:25px auto;
  color:var(--muted);
  line-height:1.9;
  font-size:.9rem;
}

.lock-date {
  color:var(--gold);
  letter-spacing:.35em;
  font-size:.8rem;
  margin:30px 0;
}

.countdown {
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
  gap:12px;
  margin:35px auto;
}

.time {
  width:105px;
  padding:20px 10px;
  border:1px solid var(--border);
  background:var(--panel);
  border-radius:8px;
}

.time strong {
  display:block;
  font-family:"Cormorant Garamond",serif;
  font-size:2.6rem;
  color:var(--light);
  font-weight:500;
}

.time span {
  display:block;
  color:var(--muted);
  font-size:.6rem;
  letter-spacing:.15em;
  margin-top:5px;
}

.lock-quote {
  margin:35px auto;
  color:var(--gold);
  font-family:"Cormorant Garamond",serif;
  font-size:1.45rem;
  font-style:italic;
  min-height:55px;
  max-width:600px;
  line-height:1.5;
}

.lock-small {
  font-size:.65rem;
  color:#817765;
  letter-spacing:.12em;
}

/* Main website */

#birthdaySite {display:none;}

.hero {
  min-height:100vh;
  padding:130px 20px 80px;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
}

.hero-content {
  max-width:900px;
  animation:fadeIn 1.4s ease;
}

.hero h1 {
  font-family:"Great Vibes",cursive;
  font-size:clamp(5rem,15vw,11rem);
  color:var(--light);
  font-weight:400;
  line-height:1;
  animation:glow 4s infinite;
}

.hero h2 {
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(1.5rem,5vw,3rem);
  letter-spacing:.2em;
  margin-top:25px;
  text-transform:uppercase;
}

.hero p {
  max-width:600px;
  color:var(--muted);
  line-height:1.9;
  margin:25px auto;
}

.hero-date {
  color:var(--gold);
  letter-spacing:.3em;
  font-size:.8rem;
  margin:30px 0;
}

.scroll {
  position:absolute;
  bottom:25px;
  color:var(--gold);
  font-size:.65rem;
  letter-spacing:.2em;
}

/* Countdown */

.countdown-section {
  border-top:1px solid var(--border);
  border-bottom:1px solid var(--border);
  background:rgba(255,255,255,.015);
}

/* Cards */

.cards {
  max-width:1100px;
  margin:50px auto 0;
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(230px,1fr));
  gap:18px;
}

.card {
  border:1px solid var(--border);
  background:var(--panel);
  padding:30px 23px;
  border-radius:8px;
  transition:.3s;
}

.card:hover {
  transform:translateY(-5px);
  border-color:var(--gold);
}

.card .symbol {
  font-size:2.5rem;
  margin-bottom:15px;
}

.card h3 {
  font-family:"Cormorant Garamond",serif;
  font-size:1.6rem;
  color:var(--light);
  margin-bottom:12px;
}

.card p {
  color:var(--muted);
  line-height:1.8;
  font-size:.82rem;
}

/* Quotes */

.quote-card {
  max-width:850px;
  margin:20px auto;
  padding:35px;
  border-left:2px solid var(--gold);
  background:var(--panel);
  text-align:left;
}

.quote-card p {
  font-family:"Cormorant Garamond",serif;
  color:var(--light);
  font-size:1.5rem;
  line-height:1.7;
}

.quote-card span {
  display:block;
  color:var(--gold);
  font-size:.7rem;
  margin-top:15px;
  letter-spacing:.15em;
  text-transform:uppercase;
}

/* Gallery */

.gallery {
  max-width:1100px;
  margin:50px auto 0;
  display:grid;
  grid-template-columns:repeat(12,1fr);
  gap:15px;
}

.photo {
  grid-column:span 4;
  min-height:300px;
  overflow:hidden;
  border:1px solid var(--border);
  border-radius:8px;
  position:relative;
}

.photo:first-child,.photo:nth-child(2) {
  grid-column:span 6;
  min-height:400px;
}

.photo img {
  width:100%;
  height:100%;
  min-height:inherit;
  object-fit:cover;
  transition:.6s;
}

.photo:hover img {transform:scale(1.06);}

/* Letter */

.letter {
  max-width:850px;
  margin:45px auto 0;
  padding:clamp(25px,6vw,60px);
  border:1px solid var(--border);
  border-radius:10px;
  background:var(--panel);
  text-align:left;
}

.letter p {
  font-family:"Cormorant Garamond",serif;
  font-size:1.35rem;
  line-height:1.9;
  color:#ded2bf;
  margin-bottom:20px;
}

.signature {
  text-align:right;
  font-family:"Great Vibes",cursive;
  font-size:2.8rem;
  color:var(--gold);
}

/* Timeline */

.timeline {
  max-width:800px;
  margin:50px auto;
  position:relative;
}

.timeline:before {
  content:"";
  position:absolute;
  left:50%;
  top:0;
  bottom:0;
  width:1px;
  background:var(--gold-dark);
}

.event {
  width:50%;
  padding:20px 35px;
  position:relative;
}

.event:nth-child(odd) {
  text-align:right;
}

.event:nth-child(even) {
  margin-left:50%;
}

.event h3 {
  font-family:"Cormorant Garamond",serif;
  color:var(--gold);
  font-size:1.6rem;
  margin-bottom:8px;
}

.event p {
  color:var(--muted);
  line-height:1.8;
  font-size:.85rem;
}

/* Gifts */

.progress {
  max-width:500px;
  margin:35px auto;
}

.progress-label {
  display:flex;
  justify-content:space-between;
  font-size:.75rem;
  color:var(--muted);
  margin-bottom:10px;
}

.track {
  height:5px;
  background:#27231c;
  border-radius:10px;
  overflow:hidden;
}

.fill {
  height:100%;
  width:0;
  background:var(--gold);
  transition:.5s;
}

.gift-grid {
  max-width:1100px;
  margin:40px auto;
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:15px;
}

.gift {
  min-height:190px;
  padding:22px 12px;
  border:1px solid var(--border);
  background:var(--panel);
  border-radius:8px;
  color:var(--light);
  cursor:pointer;
  transition:.3s;
}

.gift:hover {
  transform:translateY(-5px);
  border-color:var(--gold);
}

.gift.opened {background:rgba(215,180,106,.1);}

.gift .symbol {font-size:2.5rem;}
.gift h3 {
  font-family:"Cormorant Garamond",serif;
  font-size:1.4rem;
  margin:10px 0;
}
.gift small {
  color:var(--gold);
  font-size:.65rem;
}

/* Modal */

.modal {
  display:none;
  position:fixed;
  inset:0;
  z-index:300;
  background:rgba(0,0,0,.85);
  backdrop-filter:blur(12px);
  align-items:center;
  justify-content:center;
  padding:20px;
}

.modal.active {display:flex;}

.modal-box {
  max-width:600px;
  width:100%;
  padding:45px 30px;
  text-align:center;
  border:1px solid var(--gold);
  background:#100e0a;
  border-radius:10px;
  animation:fadeIn .4s ease;
}

.modal-box .symbol {font-size:3rem;}
.modal-box h2 {
  font-family:"Cormorant Garamond",serif;
  color:var(--gold);
  font-size:2.4rem;
  margin:15px;
}
.modal-box p {
  color:var(--muted);
  line-height:1.9;
}

/* Cake */

.cake {
  width:210px;
  height:170px;
  margin:60px auto 30px;
  position:relative;
  cursor:pointer;
}

.cake-base {
  position:absolute;
  bottom:0;
  left:5px;
  width:200px;
  height:100px;
  background:linear-gradient(135deg,#916a2c,#f0d394,#916a2c);
  border-radius:10px 10px 15px 15px;
}

.cake-top {
  position:absolute;
  bottom:85px;
  left:20px;
  width:170px;
  height:45px;
  border-radius:50%;
  background:#f3dfb0;
}

.candle {
  position:absolute;
  bottom:125px;
  left:100px;
  height:40px;
  width:10px;
  background:repeating-linear-gradient(45deg,#fff 0 5px,#b58b42 5px 10px);
}

.flame {
  position:absolute;
  bottom:162px;
  left:96px;
  width:18px;
  height:25px;
  border-radius:50%;
  background:radial-gradient(#fff7bd,#f7a23b 65%,transparent);
  filter:drop-shadow(0 0 12px orange);
  animation:glow .7s infinite;
}

.cake.blown .flame {display:none;}

#cakeMessage {
  font-family:"Cormorant Garamond",serif;
  font-size:1.5rem;
  color:var(--gold);
}

/* Final */

.final-box {
  max-width:750px;
  margin:40px auto;
  padding:45px 25px;
  border:1px solid var(--border);
  background:var(--panel);
  border-radius:10px;
}

.final-box h2 {
  font-family:"Great Vibes",cursive;
  font-size:4rem;
  color:var(--gold);
  margin:20px;
}

.final-box p {
  color:var(--muted);
  line-height:1.9;
}

#finalMessage {display:none;}
#finalMessage.show {display:block;animation:fadeIn 1s;}

footer {
  text-align:center;
  padding:35px 15px;
  color:var(--muted);
  border-top:1px solid var(--border);
  font-size:.7rem;
  letter-spacing:.1em;
}

footer span {color:var(--gold);}

@media(max-width:800px) {
  .gift-grid {grid-template-columns:repeat(2,1fr);}
  .photo,.photo:first-child,.photo:nth-child(2) {
    grid-column:span 6;
    min-height:260px;
  }
  .timeline:before {left:10px;}
  .event,.event:nth-child(odd),.event:nth-child(even) {
    width:100%;
    margin-left:0;
    text-align:left;
    padding:20px 20px 20px 35px;
  }
}

@media(max-width:500px) {
  .music-box {top:8px;right:8px;}
  .lock-ring {width:160px;height:160px;font-size:4rem;}
  .time {width:calc(50% - 8px);max-width:130px;}
  .gift-grid {gap:10px;}
  .gift {min-height:175px;}
  .photo,.photo:first-child,.photo:nth-child(2) {
    grid-column:span 6;
    min-height:200px;
  }
  .section {padding:75px 15px;}
}
</style>
</head>

<body>

<div id="particles"></div>

<!-- Song player appears on the locked screen too -->
<div class="music-box">
  <span>♫ SONG22</span>
  <button id="musicButton" aria-label="Play or pause song">▶</button>
</div>

<audio id="song" src="Song22.mp3" loop preload="auto"></audio>

<!-- LOCK SCREEN -->
<section id="lockScreen">
  <div class="lock-content">

    <p class="eyebrow">A private little surprise for someone special</p>

    <div class="lock-ring">🔒</div>

    <h1 class="lock-title">Something Special</h1>

    <h2 class="lock-name">For My <span class="gold">Nana</span></h2>

    <div class="line"></div>

    <p class="lock-description">
      Dear Nana, this little world has been created with love,
      memories, wishes and countless surprises.
      But some beautiful things are worth waiting for.
      Your surprise will open on your special day.
    </p>

    <p class="lock-date">05 NOVEMBER 2026</p>

    <div class="countdown">
      <div class="time"><strong id="d">00</strong><span>Days</span></div>
      <div class="time"><strong id="h">00</strong><span>Hours</span></div>
      <div class="time"><strong id="m">00</strong><span>Minutes</span></div>
      <div class="time"><strong id="s">00</strong><span>Seconds</span></div>
    </div>

    <p class="lock-quote" id="rotatingQuote">
      "A brother is a forever friend written into your story."
    </p>

    <p class="lock-small">
      YOUR SURPRISE IS WAITING · PLEASE COME BACK ON YOUR DAY
    </p>

  </div>
</section>

<!-- UNLOCKED WEBSITE -->
<div id="birthdaySite">

  <header class="hero">
    <div class="hero-content">
      <p class="eyebrow">A celebration of someone extraordinary</p>
      <h1>Happy Birthday</h1>
      <h2>My <span class="gold">Nana</span> · Bimal</h2>
      <div class="line"></div>
      <p>
        Today is not just another date.
        It is a celebration of the person who makes the word
        brother mean so much more.
      </p>
      <div class="hero-date">05 · 11 · 2026</div>
      <a class="btn" href="#letter">Enter Your Surprise ✦</a>
    </div>
    <div class="scroll">SCROLL TO DISCOVER ↓</div>
  </header>

  <!-- WISHES -->
  <section class="section center">
    <p class="eyebrow">A few words for you</p>
    <h2 class="section-title">To My <span class="gold">Big Brother</span></h2>
    <p class="subtitle">
      Some relationships don't need perfect words.
      They simply need to be celebrated.
    </p>

    <div class="cards">
      <div class="card">
        <div class="symbol">❤️</div>
        <h3>My Forever Support</h3>
        <p>Thank you for being someone I can always look up to. Your presence means more than you know.</p>
      </div>
      <div class="card">
        <div class="symbol">🌟</div>
        <h3>My Inspiration</h3>
        <p>May you continue to grow, achieve great things and shine in every chapter of your life.</p>
      </div>
      <div class="card">
        <div class="symbol">🤝</div>
        <h3>My Forever Friend</h3>
        <p>Life is better with a brother like you. Here's to many more memories and laughs together.</p>
      </div>
      <div class="card">
        <div class="symbol">🕊️</div>
        <h3>My Best Wishes</h3>
        <p>May peace stay in your heart, happiness find your home and success follow your efforts.</p>
      </div>
    </div>
  </section>

  <!-- QUOTES -->
  <section class="section center">
    <p class="eyebrow">Words that come from the heart</p>
    <h2 class="section-title">Nana, <span class="gold">Remember This</span></h2>

    <div class="quote-card">
      <p>"A brother is not just family. He is a lifetime of memories, protection, laughter and love."</p>
      <span>A little reminder</span>
    </div>

    <div class="quote-card">
      <p>"No matter how old we grow, a part of us will always be the little ones who share the same beautiful bond."</p>
      <span>For my Nana</span>
    </div>

    <div class="quote-card">
      <p>"May your dreams be bigger than your fears, your courage stronger than your doubts, and your future brighter than your past."</p>
      <span>Your future</span>
    </div>

    <div class="quote-card">
      <p>"Some people make life beautiful simply by being in it. You are one of those people."</p>
      <span>With love</span>
    </div>

    <div class="quote-card">
      <p>"Wherever life takes us, you will always have a special place in my heart."</p>
      <span>Always</span>
    </div>
  </section>

  <!-- PHOTO GALLERY -->
  <section class="section center">
    <p class="eyebrow">Our moments, our memories</p>
    <h2 class="section-title">A Little <span class="gold">Memory Gallery</span></h2>
    <p class="subtitle">A few photographs, a thousand feelings.</p>

    <div class="gallery">
      <div class="photo"><img src="Nana.jpg" alt="Nana memory"></div>
      <div class="photo"><img src="Nana2.jpg" alt="Nana memory"></div>
      <div class="photo"><img src="Nana3.jpg" alt="Nana memory"></div>
      <div class="photo"><img src="Nana4.jpg" alt="Nana memory"></div>
      <div class="photo"><img src="Nana5.jpg" alt="Nana memory"></div>
    </div>
  </section>

  <!-- LETTER -->
  <section class="section center" id="letter">
    <p class="eyebrow">A letter from my heart</p>
    <h2 class="section-title">Dear <span class="gold">Nana</span></h2>

    <div class="letter">
      <p>Dear Nana,</p>
      <p>
        Happy Birthday to the most special big brother.
        I honestly don't know how to put every feeling into words,
        but I want you to know how important you are to me.
      </p>
      <p>
        You are not just my brother. You are someone I admire,
        someone I learn from, and someone whose presence makes
        life feel a little more complete.
      </p>
      <p>
        Thank you for all the memories, the laughter, the support,
        the guidance and all those little moments that may seem ordinary
        but mean a lot to me.
      </p>
      <p>
        I wish you a life full of good health, peace, confidence,
        success and endless reasons to smile.
        May every hard-working step take you closer to your dreams.
      </p>
      <p>
        Never stop believing in yourself. Never settle for less than
        the happiness you deserve. And never forget that someone
        will always be cheering for you.
      </p>
      <p>
        No matter how many birthdays pass, my wish will remain the same:
        may life always be kind to you.
      </p>
      <div class="signature">Your little one ❤️</div>
    </div>
  </section>

  <!-- MEMORY TIMELINE -->
  <section class="section center">
    <p class="eyebrow">Every chapter matters</p>
    <h2 class="section-title">Our <span class="gold">Story</span></h2>

    <div class="timeline">
      <div class="event">
        <h3>The Beginning</h3>
        <p>A bond that became one of the most beautiful parts of life.</p>
      </div>
      <div class="event">
        <h3>Growing Together</h3>
        <p>Little moments, countless memories and a relationship that keeps growing.</p>
      </div>
      <div class="event">
        <h3>Through Everything</h3>
        <p>Every season teaches something, and every memory becomes part of our story.</p>
      </div>
      <div class="event">
        <h3>Forever Ahead</h3>
        <p>More birthdays, more achievements, more happiness and many more memories.</p>
      </div>
    </div>
  </section>

  <!-- 12 GIFTS -->
  <section class="section center" id="gifts">
    <p class="eyebrow">Twelve little surprises</p>
    <h2 class="section-title">12 Gifts for <span class="gold">My Nana</span></h2>
    <p class="subtitle">Tap every gift. Each one carries a special message for you.</p>

    <div class="progress">
      <div class="progress-label">
        <span>Gifts opened</span>
        <span id="giftCounter">0 / 12</span>
      </div>
      <div class="track"><div class="fill" id="giftProgress"></div></div>
    </div>

    <div class="gift-grid" id="giftGrid"></div>
  </section>

  <!-- SURPRISE CARDS -->
  <section class="section center">
    <p class="eyebrow">A few more things for you</p>
    <h2 class="section-title">Little <span class="gold">Surprises</span></h2>

    <div class="cards">
      <div class="card">
        <div class="symbol">🌹</div>
        <h3>A Rose for You</h3>
        <p>For all the kindness and warmth you bring into the lives around you.</p>
      </div>
      <div class="card">
        <div class="symbol">🏆</div>
        <h3>Your Future Award</h3>
        <p>For the achievements waiting ahead. Keep working, keep believing.</p>
      </div>
      <div class="card">
        <div class="symbol">✨</div>
        <h3>One More Wish</h3>
        <p>May every new beginning bring something wonderful into your life.</p>
      </div>
    </div>
  </section>

  <!-- CAKE -->
  <section class="section center">
    <p class="eyebrow">Your birthday moment</p>
    <h2 class="section-title">Make a <span class="gold">Wish</span></h2>
    <p class="subtitle">Tap the cake to blow out your candle.</p>

    <div class="cake" id="cake">
      <div class="cake-base"></div>
      <div class="cake-top"></div>
      <div class="candle"></div>
      <div class="flame"></div>
    </div>

    <p id="cakeMessage">A special wish for a special person.</p>
    <br><br>
    <button class="btn" id="wishButton">Blow the Candle</button>
  </section>

  <!-- FINAL SURPRISE -->
  <section class="section center">
    <p class="eyebrow">The last little surprise</p>
    <h2 class="section-title">One Last <span class="gold">Gift</span></h2>

    <div class="final-box">
      <div style="font-size:3rem" id="finalLock">🔒</div>
      <h3 class="serif gold" style="font-size:2rem;margin:20px">
        A Message Just for You
      </h3>
      <p id="finalDescription">
        Open all twelve gifts to reveal your final birthday surprise.
      </p>

      <br>
      <button class="btn" id="finalButton" disabled style="opacity:.4">
        Unlock Final Surprise
      </button>

      <div id="finalMessage">
        <h2>Happy Birthday, Nana!</h2>
        <p>
          If there is one thing I hope you always remember,
          it is how much you mean to me.
          <br><br>
          You are my big brother, my inspiration and one of the
          most precious people in my life.
          <br><br>
          May your days be peaceful, your dreams come true,
          your hard work be rewarded and your smile never fade.
          <br><br>
          I hope the coming years give you more reasons to feel proud,
          more opportunities to grow and more beautiful moments to cherish.
          <br><br>
          <strong class="gold">I am lucky to have you as my Nana. ❤️</strong>
        </p>
      </div>
    </div>
  </section>

  <footer>
    MADE WITH <span>♥</span> FOR MY NANA · BIMAl · 05 NOVEMBER 2026
  </footer>

</div>

<!-- GIFT POPUP -->
<div class="modal" id="giftModal">
  <div class="modal-box">
    <div class="symbol" id="modalIcon">🎁</div>
    <h2 id="modalTitle">A Gift for You</h2>
    <p id="modalText"></p>
    <br><br>
    <button class="btn" id="closeModal">Close Gift</button>
  </div>
</div>

<script>
/* --------------------------------
   FLOATING HEARTS AND SPARKLES
-------------------------------- */

const particles = document.getElementById("particles");
const symbols = ["♡","♥","✦","✧","✨","⋆","✶","❋"];
const colors = ["#d7b46a","#f6e5bd","#fff2ce","#c69b4c"];

function createParticle() {
  const p = document.createElement("span");
  p.className = "particle";
  p.textContent = symbols[Math.floor(Math.random()*symbols.length)];
  p.style.left = Math.random()*100 + "%";
  p.style.color = colors[Math.floor(Math.random()*colors.length)];
  p.style.fontSize = (Math.random()*17+9) + "px";

  const duration = Math.random()*9+8;
  p.style.animationDuration = duration+"s";

  particles.appendChild(p);
  setTimeout(()=>p.remove(),duration*1000);
}

for(let i=0;i<30;i++) {
  setTimeout(createParticle,i*180);
}

setInterval(createParticle,350);

/* --------------------------------
   MUSIC PLAYER
-------------------------------- */

const song = document.getElementById("song");
const musicButton = document.getElementById("musicButton");

musicButton.addEventListener("click",async()=>{
  if(song.paused) {
    try {
      await song.play();
      musicButton.textContent="Ⅱ";
    } catch(e) {
      alert("Please check that Song22.mp3 is in the same folder as index.html.");
    }
  } else {
    song.pause();
    musicButton.textContent="▶";
  }
});

song.addEventListener("play",()=>musicButton.textContent="Ⅱ");
song.addEventListener("pause",()=>musicButton.textContent="▶");

/* --------------------------------
   DATE LOCK AND COUNTDOWN
   Indian Standard Time
-------------------------------- */

const unlockDate = new Date("2026-11-05T00:00:00+05:30").getTime();

const lockScreen = document.getElementById("lockScreen");
const birthdaySite = document.getElementById("birthdaySite");

const quoteList = [
  "A brother is a forever friend written into your story.",
  "Some bonds become stronger with every passing year.",
  "A great brother is one of life's greatest blessings.",
  "May your future be as beautiful as the memories we share.",
  "Your dreams deserve every chance to become reality.",
  "A brother's place in the heart can never be replaced.",
  "Keep growing, keep smiling, and keep shining, Nana.",
  "The best chapters of your life are still waiting to be written."
];

let quoteIndex=0;

const rotatingQuote=document.getElementById("rotatingQuote");

setInterval(()=>{
  if(rotatingQuote) {
    quoteIndex=(quoteIndex+1)%quoteList.length;
    rotatingQuote.style.opacity=0;
    setTimeout(()=>{
      rotatingQuote.textContent='"'+quoteList[quoteIndex]+'"';
      rotatingQuote.style.opacity=1;
    },350);
  }
},4500);

function updateLock() {
  const remaining=unlockDate-Date.now();

  if(remaining<=0) {
    lockScreen.style.display="none";
    birthdaySite.style.display="block";
    document.body.style.overflowX="hidden";
    return;
  }

  document.getElementById("d").textContent=
    String(Math.floor(remaining/86400000)).padStart(2,"0");

  document.getElementById("h").textContent=
    String(Math.floor(remaining/3600000)%24).padStart(2,"0");

  document.getElementById("m").textContent=
    String(Math.floor(remaining/60000)%60).padStart(2,"0");

  document.getElementById("s").textContent=
    String(Math.floor(remaining/1000)%60).padStart(2,"0");

  lockScreen.style.display="flex";
  birthdaySite.style.display="none";
}

updateLock();
setInterval(updateLock,1000);

/* --------------------------------
   TWELVE GIFTS
-------------------------------- */

const gifts=[
  ["💛","A Wish","May your life always be filled with happiness, good health, peace and success. May every day bring you a reason to smile."],
  ["🌟","A Star","You deserve to shine. Never stop believing in your abilities, and never stop reaching for the dreams that matter to you."],
  ["🤝","A Promise","Whatever happens in life, you will always have someone who cares for you and wishes the very best for you."],
  ["📸","A Memory","Every memory we create is a little treasure. I hope we make thousands more together."],
  ["🛡️","Strength","May you always have courage in difficult times and confidence in every new beginning."],
  ["🌹","A Thank You","Thank you for being my brother, my guide and someone I can always admire."],
  ["☀️","A Smile","May your smile never fade and may happiness find you even on the simplest days."],
  ["🎯","Your Dreams","May all the dreams you work so hard for slowly become your beautiful reality."],
  ["🕊️","Peace","May your mind stay peaceful, your heart stay kind and your journey stay meaningful."],
  ["💎","A Reminder","Never underestimate your worth. You are more special than you sometimes realise."],
  ["🎂","Celebration","Today is your day. Celebrate every little achievement and every wonderful thing about yourself."],
  ["❤️","My Love","I am grateful to have you as my Nana. I will always wish for your happiness and success."]
];

const giftGrid=document.getElementById("giftGrid");
const giftModal=document.getElementById("giftModal");
const opened=new Set();

function renderGifts() {
  giftGrid.innerHTML="";

  gifts.forEach((g,i)=>{
    const button=document.createElement("button");
    button.className="gift"+(opened.has(i)?" opened":"");
    button.innerHTML=`
      <div class="symbol">${g[0]}</div>
      <h3>${g[1]}</h3>
      <small>${opened.has(i)?"✦ OPENED":"TAP TO OPEN"}</small>
    `;

    button.addEventListener("click",()=>openGift(i));
    giftGrid.appendChild(button);
  });
}

function openGift(i) {
  const g=gifts[i];
  opened.add(i);

  document.getElementById("modalIcon").textContent=g[0];
  document.getElementById("modalTitle").textContent=g[1];
  document.getElementById("modalText").textContent=g[2];

  giftModal.classList.add("active");

  updateProgress();
  renderGifts();
}

function updateProgress() {
  const count=opened.size;
  document.getElementById("giftCounter").textContent=count+" / 12";
  document.getElementById("giftProgress").style.width=(count/12*100)+"%";

  const button=document.getElementById("finalButton");

  if(count===12) {
    button.disabled=false;
    button.style.opacity="1";
    document.getElementById("finalLock").textContent="🔓";
    document.getElementById("finalDescription").textContent=
      "All twelve gifts have been opened. Your final surprise is ready.";
  }
}

document.getElementById("closeModal").addEventListener("click",()=>{
  giftModal.classList.remove("active");
});

giftModal.addEventListener("click",(e)=>{
  if(e.target===giftModal) giftModal.classList.remove("active");
});

document.addEventListener("keydown",(e)=>{
  if(e.key==="Escape") giftModal.classList.remove("active");
});

renderGifts();

/* --------------------------------
   CAKE AND WISH
-------------------------------- */

let cakeBlown=false;

function blowCandle() {
  if(cakeBlown) return;
  cakeBlown=true;

  document.getElementById("cake").classList.add("blown");
  document.getElementById("cakeMessage").textContent=
    "May every beautiful wish come true, Nana! ❤️";

  document.getElementById("wishButton").textContent="Wish Made ✦";

  for(let i=0;i<30;i++) {
    setTimeout(createParticle,i*60);
  }
}

document.getElementById("cake").addEventListener("click",blowCandle);
document.getElementById("wishButton").addEventListener("click",blowCandle);

/* --------------------------------
   FINAL SURPRISE
-------------------------------- */

document.getElementById("finalButton").addEventListener("click",()=>{
  if(opened.size!==12) return;

  document.getElementById("finalMessage").classList.add("show");
  document.getElementById("finalButton").textContent="SURPRISE UNLOCKED ❤️";
  document.getElementById("finalButton").disabled=true;

  document.getElementById("finalMessage").scrollIntoView({
    behavior:"smooth",
    block:"center"
  });

  for(let i=0;i<45;i++) {
    setTimeout(createParticle,i*60);
  }
});
</script>

</body>
</html>

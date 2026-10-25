
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080808">

<title>For My Big Brother | 05.11.2026</title>

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>
:root {
  --gold: #d8b56a;
  --light-gold: #f8e7b0;
  --dark-gold: #8b682b;
  --black: #080808;
  --white: #f7f1e7;
  --muted: #a8a29a;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  background: var(--black);
  color: var(--white);
  font-family: "DM Sans", sans-serif;
  overflow-x: hidden;
}

body::before {
  content: "";
  position: fixed;
  inset: 0;
  background:
    radial-gradient(ellipse at 50% 0%, #5b41151c, transparent 55%),
    radial-gradient(ellipse at 100% 100%, #8b682b10, transparent 40%);
  pointer-events: none;
  z-index: -1;
}

button {
  font-family: inherit;
  cursor: pointer;
}

section {
  padding: 85px 20px;
}

.container {
  width: 100%;
  max-width: 1050px;
  margin: auto;
}

.serif {
  font-family: "Cormorant Garamond", serif;
}

.gold {
  color: var(--gold);
}

.eyebrow {
  color: var(--gold);
  font-size: 10px;
  letter-spacing: 5px;
  text-transform: uppercase;
  margin-bottom: 17px;
}

.heading {
  text-align: center;
  margin-bottom: 45px;
}

.heading h2 {
  font-family: "Cormorant Garamond", serif;
  font-size: clamp(38px, 8vw, 65px);
  font-weight: 500;
  line-height: 1.1;
}

.heading p {
  color: var(--muted);
  font-size: 13px;
  line-height: 1.9;
  margin-top: 16px;
}

.gold-line {
  width: 65px;
  height: 1px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
  margin: 22px auto;
}

/* INTRO */

#intro {
  min-height: 100svh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  position: relative;
  padding: 50px 20px;
  overflow: hidden;
}

.intro-content {
  position: relative;
  z-index: 2;
  max-width: 800px;
}

.intro-label {
  color: var(--gold);
  font-size: 10px;
  letter-spacing: 7px;
  margin-bottom: 30px;
}

.intro-title {
  font-family: "Cormorant Garamond", serif;
  font-size: clamp(60px, 13vw, 120px);
  font-weight: 400;
  line-height: .9;
}

.intro-title span {
  display: block;
  color: var(--gold);
  font-style: italic;
}

.intro-subtitle {
  color: #c9c0b1;
  font-size: 11px;
  letter-spacing: 3px;
  margin-top: 30px;
}

.intro-date {
  color: var(--gold);
  font-size: 11px;
  letter-spacing: 5px;
  margin-top: 40px;
}

.enter-btn {
  margin-top: 40px;
  padding: 16px 32px;
  color: var(--light-gold);
  background: transparent;
  border: 1px solid var(--dark-gold);
  font-size: 10px;
  letter-spacing: 3px;
  transition: .4s;
}

.enter-btn:hover {
  background: var(--gold);
  color: #000;
  box-shadow: 0 0 35px #d8b56a35;
}

.corner {
  position: absolute;
  width: 75px;
  height: 75px;
  border-color: #8d6c37;
  border-style: solid;
  opacity: .5;
}

.top-left {
  top: 25px;
  left: 25px;
  border-width: 1px 0 0 1px;
}

.top-right {
  top: 25px;
  right: 25px;
  border-width: 1px 1px 0 0;
}

.bottom-left {
  bottom: 25px;
  left: 25px;
  border-width: 0 0 1px 1px;
}

.bottom-right {
  bottom: 25px;
  right: 25px;
  border-width: 0 1px 1px 0;
}

/* PARTICLES */

#particles {
  position: fixed;
  inset: 0;
  overflow: hidden;
  pointer-events: none;
  z-index: 5;
}

.particle {
  position: absolute;
  bottom: -20px;
  width: 3px;
  height: 3px;
  background: var(--gold);
  border-radius: 50%;
  box-shadow: 0 0 10px var(--gold);
  animation: floatUp linear infinite;
}

@keyframes floatUp {
  0% {
    transform: translateY(0);
    opacity: 0;
  }
  20% {
    opacity: .8;
  }
  100% {
    transform: translateY(-110vh);
    opacity: 0;
  }
}

/* COUNTDOWN */

.countdown-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 12px;
  max-width: 600px;
  margin: 35px auto;
}

.time-box {
  border: 1px solid #4d3c20;
  background: linear-gradient(145deg, #17130c, #090909);
  padding: 25px 10px;
}

.time-box strong {
  display: block;
  font-family: "Cormorant Garamond", serif;
  font-size: clamp(32px, 7vw, 55px);
  font-weight: 400;
  color: var(--light-gold);
}

.time-box span {
  color: #9c8a68;
  font-size: 9px;
  letter-spacing: 3px;
}

#countdown-message {
  color: var(--gold);
  font-family: "Cormorant Garamond", serif;
  font-size: 25px;
  text-align: center;
}

/* MUSIC */

.music-card {
  max-width: 650px;
  margin: auto;
  border: 1px solid #42341d;
  background: linear-gradient(135deg, #17130c, #0a0a0a);
  padding: 25px;
  display: flex;
  align-items: center;
  gap: 18px;
}

.music-disc {
  width: 58px;
  height: 58px;
  border: 1px solid var(--gold);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--gold);
  font-size: 24px;
  flex-shrink: 0;
}

.music-disc.playing {
  animation: rotateDisc 5s linear infinite;
}

@keyframes rotateDisc {
  to {
    transform: rotate(360deg);
  }
}

.music-info {
  flex: 1;
  min-width: 0;
}

.music-info h3 {
  font-family: "Cormorant Garamond", serif;
  font-size: 25px;
  font-weight: 500;
}

.music-info p {
  color: var(--muted);
  font-size: 11px;
  margin-top: 5px;
}

.music-button {
  border: 1px solid var(--dark-gold);
  color: var(--gold);
  background: transparent;
  padding: 12px 18px;
  font-size: 10px;
  letter-spacing: 2px;
}

.music-button:hover {
  background: var(--gold);
  color: #000;
}

/* GIFTS */

.gifts-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 16px;
}

.gift-card {
  min-height: 185px;
  padding: 20px 10px;
  border: 1px solid #40321d;
  background: linear-gradient(150deg, #17130c, #0b0b0b);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 12px;
  text-align: center;
  transition: .35s;
}

.gift-card:hover {
  transform: translateY(-6px);
  border-color: var(--gold);
  box-shadow: 0 10px 35px #d8b56a12;
}

.gift-card.opened {
  background: linear-gradient(150deg, #241d10, #100e09);
  border-color: var(--gold);
}

.gift-number {
  color: var(--dark-gold);
  font-size: 9px;
  letter-spacing: 3px;
}

.gift-icon {
  font-size: 39px;
  transition: .4s;
}

.gift-card:hover .gift-icon {
  transform: scale(1.12);
}

.gift-card h3 {
  font-family: "Cormorant Garamond", serif;
  font-size: 20px;
  font-weight: 500;
}

.gift-card p {
  color: var(--muted);
  font-size: 10px;
  line-height: 1.6;
}

.gift-progress {
  text-align: center;
  margin-top: 35px;
  color: var(--gold);
  font-size: 11px;
  letter-spacing: 3px;
}

.progress-track {
  height: 2px;
  max-width: 300px;
  margin: 15px auto;
  background: #292319;
}

.progress-fill {
  width: 0%;
  height: 100%;
  background: var(--gold);
  transition: width .5s;
}

/* MODAL */

.modal {
  position: fixed;
  inset: 0;
  background: #000000e8;
  backdrop-filter: blur(12px);
  display: none;
  align-items: center;
  justify-content: center;
  padding: 20px;
  z-index: 100;
}

.modal.show {
  display: flex;
  animation: fadeIn .3s;
}

.modal-content {
  max-width: 550px;
  width: 100%;
  border: 1px solid var(--dark-gold);
  background: linear-gradient(145deg, #19140c, #080808);
  padding: 45px 30px;
  text-align: center;
  position: relative;
  animation: modalUp .4s;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes modalUp {
  from {
    transform: translateY(25px) scale(.96);
  }
  to {
    transform: translateY(0) scale(1);
  }
}

.modal-icon {
  font-size: 55px;
  margin-bottom: 20px;
}

.modal-content h2 {
  font-family: "Cormorant Garamond", serif;
  font-size: 42px;
  font-weight: 500;
  color: var(--light-gold);
}

.modal-content p {
  color: #c5bcae;
  line-height: 1.9;
  font-size: 14px;
  margin-top: 20px;
  white-space: pre-line;
}

.modal-close {
  position: absolute;
  top: 15px;
  right: 18px;
  color: var(--gold);
  background: none;
  border: none;
  font-size: 25px;
}

/* MEMORIES */

.photo-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 15px;
}

.photo-frame {
  border: 1px solid #4d3c20;
  background: #111;
  padding: 8px;
  overflow: hidden;
}

.photo-frame img {
  width: 100%;
  aspect-ratio: 1 / 1.15;
  object-fit: cover;
  display: block;
  filter: grayscale(20%);
  transition: .5s;
}

.photo-frame:hover img {
  filter: grayscale(0%);
  transform: scale(1.04);
}

.photo-frame p {
  text-align: center;
  font-family: "Cormorant Garamond", serif;
  color: var(--gold);
  font-size: 18px;
  padding: 12px 4px 5px;
}

/* LETTER */

.letter {
  max-width: 750px;
  margin: auto;
  padding: 45px;
  border: 1px solid #4b3a20;
  background: radial-gradient(ellipse at top, #4a351318, transparent 60%), #0c0b09;
}

.letter h3 {
  font-family: "Cormorant Garamond", serif;
  color: var(--gold);
  font-size: 32px;
  font-weight: 500;
  margin-bottom: 25px;
}

.letter p {
  color: #c8c0b4;
  font-size: 14px;
  line-height: 2;
  margin-bottom: 20px;
}

.signature {
  font-family: "Cormorant Garamond", serif;
  font-size: 28px;
  font-style: italic;
  color: var(--gold);
  margin-top: 30px;
}

/* CAKE */

.cake-area {
  text-align: center;
}

.cake {
  position: relative;
  width: 180px;
  height: 160px;
  margin: 60px auto 35px;
}

.cake-base {
  position: absolute;
  bottom: 0;
  width: 180px;
  height: 90px;
  background: linear-gradient(90deg, #79502b, #c89553, #80502a);
  border-radius: 8px 8px 15px 15px;
  box-shadow: 0 15px 30px #000;
}

.cake-base::before {
  content: "";
  position: absolute;
  top: 0;
  width: 100%;
  height: 25px;
  border-radius: 50%;
  background: #f0d5a3;
}

.cake-top {
  position: absolute;
  bottom: 85px;
  left: 15px;
  width: 150px;
  height: 45px;
  background: linear-gradient(90deg, #8d592f, #e4bb78, #956033);
  border-radius: 50%;
}

.candle {
  position: absolute;
  width: 9px;
  height: 38px;
  bottom: 125px;
  left: 85px;
  background: linear-gradient(90deg, #f4dfab, #a77d35);
  z-index: 3;
}

.flame {
  position: absolute;
  width: 15px;
  height: 24px;
  background: radial-gradient(ellipse at bottom, #fff8bc, #ffc34c 45%, #ff6c16);
  border-radius: 50% 50% 50% 0;
  transform: rotate(-45deg);
  bottom: 158px;
  left: 82px;
  filter: drop-shadow(0 0 12px #ff9b25);
  animation: flame 1s ease-in-out infinite alternate;
}

@keyframes flame {
  from { transform: rotate(-45deg) scale(.9); }
  to { transform: rotate(-40deg) scale(1.1); }
}

.cake-button,
.final-button {
  background: transparent;
  border: 1px solid var(--gold);
  color: var(--gold);
  padding: 15px 25px;
  font-size: 10px;
  letter-spacing: 3px;
}

.cake-button:hover {
  background: var(--gold);
  color: #000;
}

#wish-message {
  color: var(--gold);
  margin-top: 25px;
  font-family: "Cormorant Garamond", serif;
  font-size: 24px;
}

/* FINAL */

.final-gift {
  max-width: 700px;
  margin: auto;
  padding: 55px 25px;
  border: 1px solid #68502a;
  background: radial-gradient(ellipse at center, #33220f40, transparent 70%);
  text-align: center;
}

.big-icon {
  font-size: 70px;
  margin-bottom: 25px;
}

.final-gift h2 {
  font-family: "Cormorant Garamond", serif;
  font-size: clamp(40px, 8vw, 75px);
  color: var(--light-gold);
  font-weight: 400;
}

.final-gift p {
  color: #c4b9a6;
  font-size: 13px;
  line-height: 2;
  margin-top: 20px;
}

.final-button {
  margin-top: 35px;
  background: var(--gold);
  color: #090909;
  border: none;
}

.final-button:disabled {
  opacity: .3;
  cursor: not-allowed;
}

#final-message {
  display: none;
  margin-top: 30px;
  font-family: "Cormorant Garamond", serif;
  color: var(--light-gold);
  font-size: 28px;
  line-height: 1.7;
}

footer {
  border-top: 1px solid #302719;
  text-align: center;
  padding: 35px 20px;
  color: #82786a;
  font-size: 10px;
  letter-spacing: 3px;
}

footer span {
  color: var(--gold);
}

@media(max-width: 750px) {
  .gifts-grid {
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
  }

  .gift-card {
    min-height: 160px;
    padding: 18px 8px;
  }

  .gift-icon {
    font-size: 34px;
  }

  .gift-card h3 {
    font-size: 17px;
  }

  .photo-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .letter {
    padding: 35px 25px;
  }
}

@media(max-width: 420px) {
  .gifts-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .countdown-grid {
    gap: 7px;
  }

  .time-box {
    padding: 20px 5px;
  }

  .time-box span {
    letter-spacing: 1px;
    font-size: 8px;
  }

  .music-card {
    padding: 16px;
    gap: 12px;
  }

  .music-disc {
    width: 45px;
    height: 45px;
    font-size: 18px;
  }

  .music-button {
    padding: 10px;
  }

  .music-info h3 {
    font-size: 20px;
  }

  .modal-content {
    padding: 40px 20px;
  }

  .modal-content h2 {
    font-size: 34px;
  }
}

@media(prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: .01ms !important;
    transition-duration: .01ms !important;
  }
}
</style>
</head>

<body>

<div id="particles"></div>

<!-- INTRO -->

<section id="intro">

  <div class="corner top-left"></div>
  <div class="corner top-right"></div>
  <div class="corner bottom-left"></div>
  <div class="corner bottom-right"></div>

  <div class="intro-content">

    <div class="intro-label">A Special Celebration</div>

    <h1 class="intro-title">
      For My
      <span>Big Brother</span>
    </h1>

    <div class="intro-subtitle">
      A LITTLE SURPRISE FROM YOUR LITTLE BROTHER
    </div>

    <div class="intro-date">
      NOVEMBER 05 · 2026
    </div>

    <button class="enter-btn" onclick="enterWebsite()">
      ENTER YOUR SURPRISE ✦
    </button>

  </div>
</section>

<!-- COUNTDOWN -->

<section id="countdown-section">

  <div class="container">

    <div class="heading">
      <div class="eyebrow">The Moment Is Coming</div>

      <h2>Counting Down To <span class="gold">Your Day</span></h2>

      <div class="gold-line"></div>

      <p>
        Every second brings us closer to celebrating someone truly special.
      </p>
    </div>

    <div class="countdown-grid">

      <div class="time-box">
        <strong id="days">00</strong>
        <span>Days</span>
      </div>

      <div class="time-box">
        <strong id="hours">00</strong>
        <span>Hours</span>
      </div>

      <div class="time-box">
        <strong id="minutes">00</strong>
        <span>Minutes</span>
      </div>

      <div class="time-box">
        <strong id="seconds">00</strong>
        <span>Seconds</span>
      </div>

    </div>

    <div id="countdown-message"></div>

  </div>
</section>

<!-- TWO SONGS -->

<section id="music-section">

  <div class="container">

    <div class="heading">
      <div class="eyebrow">A Song For Every Moment</div>

      <h2>Music For <span class="gold">Your Day</span></h2>

      <div class="gold-line"></div>

      <p id="music-description">
        A special melody while we wait for your birthday.
      </p>
    </div>

    <div class="music-card">

      <div class="music-disc" id="music-disc">♫</div>

      <div class="music-info">
        <h3 id="music-title">The Countdown Song</h3>
        <p id="music-status">A special melody while we wait.</p>
      </div>

      <button class="music-button"
              id="music-button"
              onclick="toggleMusic()">
        PLAY
      </button>

    </div>

    <!-- SONG BEFORE BIRTHDAY -->
    <audio id="song-before" loop preload="metadata">
      <source src="Song11.mp3" type="audio/mpeg">
    </audio>

    <!-- SONG ON BIRTHDAY -->
    <audio id="song-after" loop preload="metadata">
      <source src="Song22.mp3" type="audio/mpeg">
    </audio>

  </div>
</section>

<!-- 12 GIFTS -->

<section id="gifts-section">

  <div class="container">

    <div class="heading">
      <div class="eyebrow">12 Little Surprises</div>

      <h2>Open Your <span class="gold">Gifts</span></h2>

      <div class="gold-line"></div>

      <p>
        Each gift holds a little piece of love, gratitude, and memories.
        <br>Tap every gift to discover what's inside.
      </p>
    </div>

    <div class="gifts-grid" id="gifts-grid"></div>

    <div class="gift-progress">

      <span id="opened-count">0</span> / 12 GIFTS OPENED

      <div class="progress-track">
        <div class="progress-fill" id="progress-fill"></div>
      </div>

      <p style="color:#84745b;font-size:10px;letter-spacing:1px">
        Open every gift to unlock the final surprise.
      </p>

    </div>

  </div>
</section>

<!-- PHOTO MEMORIES -->

<section id="memories-section">

  <div class="container">

    <div class="heading">
      <div class="eyebrow">Moments That Matter</div>

      <h2>Our Little <span class="gold">Memories</span></h2>

      <div class="gold-line"></div>

      <p>
        Different moments, one beautiful bond.
      </p>
    </div>

    <div class="photo-grid">

      <div class="photo-frame">
        <img src="Nana.jpg" alt="A special memory together">
        <p>Our Beginning</p>
      </div>

      <div class="photo-frame">
        <img src="Nana1.jpg" alt="A happy memory together">
        <p>Good Times</p>
      </div>

      <div class="photo-frame">
        <img src="Nana2.jpg" alt="A memorable moment">
        <p>Unforgettable</p>
      </div>

      <div class="photo-frame">
        <img src="Nana3.jpg" alt="A memory with my brother">
        <p>My Favourite</p>
      </div>

      <div class="photo-frame">
        <img src="Nana4.jpg" alt="A special day">
        <p>Always Together</p>
      </div>

      <div class="photo-frame">
        <img src="Nana5.jpg" alt="A brotherhood memory">
        <p>Forever Us</p>
      </div>

    </div>

  </div>
</section>

<!-- LETTER -->

<section id="letter-section">

  <div class="container">

    <div class="heading">
      <div class="eyebrow">From My Heart</div>

      <h2>A Letter To <span class="gold">My Brother</span></h2>

      <div class="gold-line"></div>
    </div>

    <div class="letter">

      <h3>Dear Bhai,</h3>

      <p>
        There are some people in life who make everything feel a little
        easier, a little safer, and a lot more meaningful.
        For me, you are one of those people.
      </p>

      <p>
        Having you as my big brother is one of the greatest blessings
        of my life. You have been more than just a brother.
        You have been a friend, a guide, a source of strength,
        and someone I can always look up to.
      </p>

      <p>
        I may not always say it, and sometimes I may not even show it,
        but I genuinely appreciate everything you do.
        Your presence means more to me than words can explain.
      </p>

      <p>
        On your birthday, I wish you endless happiness, good health,
        peace of mind, success in everything you do, and all the
        beautiful things this world has to offer.
      </p>

      <p>
        No matter how much we grow, where life takes us,
        or how busy our days become, one thing will never change:
        I will always be your little brother, and you will
        always be my big brother.
      </p>

      <p>
        Thank you for being you.
        Thank you for being my brother.
        And thank you for being a part of my life.
      </p>

      <div class="signature">
        With all my love,<br>
        Your Little Brother ❤️
      </div>

    </div>

  </div>
</section>

<!-- CAKE -->

<section id="cake-section">

  <div class="container">

    <div class="heading">
      <div class="eyebrow">Make A Wish</div>

      <h2>A Cake Just <span class="gold">For You</span></h2>

      <div class="gold-line"></div>

      <p>
        One candle. One wish. A thousand beautiful possibilities.
      </p>
    </div>

    <div class="cake-area">

      <div class="cake">

        <div class="cake-base"></div>
        <div class="cake-top"></div>
        <div class="candle"></div>
  

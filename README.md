
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080706">

<title>For Bimal Bhai | The Golden Celebration</title>

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>
:root {
  --black: #080706;
  --black2: #100e0b;
  --gold: #d8b56a;
  --gold2: #f8e7b0;
  --gold3: #92703a;
  --white: #f8f1e5;
  --muted: #aaa092;
  --line: #4b3a20;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
  scroll-padding-top: 80px;
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
  z-index: -1;
  pointer-events: none;
  background:
    radial-gradient(ellipse at 50% 0%, #8a621c18, transparent 55%),
    radial-gradient(ellipse at 100% 50%, #d8b56a08, transparent 40%),
    radial-gradient(ellipse at 0% 100%, #8a621c10, transparent 40%);
}

button, input, textarea {
  font: inherit;
}

button {
  cursor: pointer;
}

button:focus-visible,
a:focus-visible {
  outline: 2px solid var(--gold);
  outline-offset: 4px;
}

a {
  color: inherit;
  text-decoration: none;
}

img {
  max-width: 100%;
}

.serif {
  font-family: "Cormorant Garamond", serif;
}

.gold {
  color: var(--gold);
}

.gold-text {
  background: linear-gradient(110deg, #b58b42, #fff0be, #d8b56a, #fff0be);
  background-size: 200% auto;
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: goldShine 6s linear infinite;
}

@keyframes goldShine {
  to {
    background-position: 200% center;
  }
}

.container {
  width: 100%;
  max-width: 1100px;
  margin: auto;
}

section {
  padding: 100px 22px;
  position: relative;
}

.section-heading {
  text-align: center;
  margin-bottom: 50px;
}

.eyebrow {
  color: var(--gold);
  font-size: 10px;
  letter-spacing: 5px;
  text-transform: uppercase;
  margin-bottom: 18px;
}

.section-heading h2 {
  font-family: "Cormorant Garamond", serif;
  font-size: clamp(38px, 8vw, 72px);
  font-weight: 400;
  line-height: 1.05;
}

.section-heading p {
  color: var(--muted);
  font-size: 13px;
  line-height: 1.9;
  max-width: 650px;
  margin: 15px auto 0;
}

.gold-line {
  height: 1px;
  width: 80px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
  margin: 25px auto;
}

.gold-button {
  display: inline-block;
  padding: 15px 25px;
  border: 1px solid var(--gold);
  color: var(--gold);
  background: transparent;
  font-size: 10px;
  letter-spacing: 3px;
  transition: .4s;
}

.gold-button:hover {
  color: #080706;
  background: var(--gold);
  box-shadow: 0 0 30px #d8b56a30;
}

.gold-button.filled {
  background: var(--gold);
  color: #080706;
}

.gold-button:disabled {
  opacity: .35;
  cursor: not-allowed;
}

/* ==================================
   FLOATING STARS, HEARTS & SPARKLES
================================== */

#magic-layer {
  position: fixed;
  inset: 0;
  overflow: hidden;
  pointer-events: none;
  z-index: 20;
}

.magic {
  position: absolute;
  bottom: -60px;
  opacity: 0;
  user-select: none;
  animation: magicFloat linear infinite;
  filter: drop-shadow(0 0 8px #d8b56a60);
}

@keyframes magicFloat {
  0% {
    transform: translate3d(0, 0, 0) rotate(0deg) scale(.6);
    opacity: 0;
  }

  15% {
    opacity: .8;
  }

  80% {
    opacity: .6;
  }

  100% {
    transform: translate3d(40px, -115vh, 0) rotate(360deg) scale(1.3);
    opacity: 0;
  }
}

/* EXTRA CURSOR SPARKLES */

.cursor-sparkle {
  position: fixed;
  pointer-events: none;
  z-index: 99;
  color: var(--gold2);
  animation: cursorSparkle 1s ease-out forwards;
}

@keyframes cursorSparkle {
  0% {
    opacity: 1;
    transform: scale(.3) rotate(0);
  }

  100% {
    opacity: 0;
    transform: scale(1.5) rotate(90deg) translateY(-25px);
  }
}

/* ==================================
   NAVIGATION
================================== */

.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 50;
  padding: 15px 20px;
  background: #080706d9;
  backdrop-filter: blur(15px);
  border-bottom: 1px solid #d8b56a1a;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 15px;
}

.nav-brand {
  font-family: "Cormorant Garamond", serif;
  font-size: 25px;
  color: var(--gold);
  white-space: nowrap;
}

.nav-links {
  display: flex;
  gap: 22px;
  align-items: center;
}

.nav-links a {
  font-size: 10px;
  letter-spacing: 1px;
  color: #c6bcac;
  transition: .3s;
}

.nav-links a:hover {
  color: var(--gold);
}

.nav-music {
  border: 1px solid var(--gold3);
  background: transparent;
  color: var(--gold);
  padding: 9px 12px;
  font-size: 10px;
  letter-spacing: 1px;
  white-space: nowrap;
}

@media(max-width: 750px) {
  .nav-links {
    display: none;
  }

  .navbar {
    padding: 12px 16px;
  }
}

/* ==================================
   HERO
================================== */

#hero {
  min-height: 100svh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding-top: 100px;
  overflow: hidden;
}

.hero-content {
  position: relative;
  z-index: 2;
  max-width: 900px;
}

.hero-small {
  font-size: 10px;
  color: var(--gold);
  letter-spacing: 8px;
  margin-bottom: 35px;
  animation: reveal 1.5s ease both;
}

.hero-title {
  font-family: "Cormorant Garamond", serif;
  font-size: clamp(60px, 13vw, 145px);
  line-height: .82;
  font-weight: 400;
  animation: reveal 1.5s ease both;
}

.hero-title span {
  display: block;
  font-style: italic;
  margin-top: 20px;
}

.hero-subtitle {
  font-size: 11px;
  letter-spacing: 3px;
  color: #c6bba9;
  line-height: 2;
  margin-top: 35px;
}

.hero-date {
  font-size: 11px;
  letter-spacing: 6px;
  color: var(--gold);
  margin-top: 35px;
}

.hero-buttons {
  margin-top: 40px;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 12px;
}

.hero-orbit {
  position: absolute;
  width: min(80vw, 600px);
  aspect-ratio: 1;
  border: 1px solid #d8b56a12;
  border-radius: 50%;
  pointer-events: none;
  animation: orbitRotate 45s linear infinite;
}

.hero-orbit::before {
  content: "✦";
  position: absolute;
  top: 5%;
  left: 50%;
  color: var(--gold);
  font-size: 22px;
}

.hero-orbit::after {
  content: "✧";
  position: absolute;
  bottom: 8%;
  right: 10%;
  color: var(--gold2);
  font-size: 18px;
}

@keyframes orbitRotate {
  to { transform: rotate(360deg); }
}

@keyframes reveal {
  from {
    opacity: 0;
    transform: translateY(35px);
    filter: blur(8px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
    filter: blur(0);
  }
}

.hero-corner {
  position: absolute;
  width: 65px;
  height: 65px;
  border: solid var(--gold3);
  opacity: .5;
}

.hero-corner.tl {
  top: 100px;
  left: 25px;
  border-width: 1px 0 0 1px;
}

.hero-corner.tr {
  top: 100px;
  right: 25px;
  border-width: 1px 1px 0 0;
}

.hero-corner.bl {
  bottom: 25px;
  left: 25px;
  border-width: 0 0 1px 1px;
}

.hero-corner.br {
  bottom: 25px;
  right: 25px;
  border-width: 0 1px 1px 0;
}

/* ==================================
   COUNTDOWN
================================== */

.countdown-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 12px;
  max-width: 700px;
  margin: 40px auto;
}

.time-box {
  padding: 25px 10px;
  border: 1px solid var(--line);
  background: linear-gradient(145deg, #19150e, #080706);
  box-shadow: inset 0 0 25px #d8b56a05;
}

.time-box strong {
  display: block;
  font-family: "Cormorant Garamond", serif;
  font-size: clamp(35px, 8vw, 65px);
  font-weight: 400;
  color: var(--gold2);
}

.time-box span {
  font-size: 9px;
  letter-spacing: 3px;
  color: #a48b5c;
}

#countdown-message {
  text-align: center;
  font-family: "Cormorant Garamond", serif;
  font-size: 26px;
  color: var(--gold);
}

/* ==================================
   MUSIC
================================== */

.music-card {
  max-width: 750px;
  margin: auto;
  display: flex;
  align-items: center;
  gap: 18px;
  padding: 25px;
  border: 1px solid #5a4525;
  background: linear-gradient(135deg, #19150e, #090807);
}

.music-disc {
  width: 65px;
  height: 65px;
  flex-shrink: 0;
  border: 1px solid var(--gold);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 25px;
  color: var(--gold);
  background: radial-gradient(circle, #3a2b15, #080706);
}

.music-disc.playing {
  animation: rotateDisc 5s linear infinite;
}

@keyframes rotateDisc {
  to { transform: rotate(360deg); }
}

.music-info {
  flex: 1;
  min-width: 0;
}

.music-info h3 {
  font-family: "Cormorant Garamond", serif;
  font-size: 27px;
  font-weight: 500;
}

.music-info p {
  color: var(--muted);
  font-size: 11px;
  line-height: 1.7;
  margin-top: 5px;
}

.music-button {
  padding: 12px 18px;
  background: transparent;
  color: var(--gold);
  border: 1px solid var(--gold3);
  font-size: 10px;
  letter-spacing: 2px;
}

.music-button:hover {
  background: var(--gold);
  color: #000;
}

.music-progress {
  max-width: 750px;
  margin: 15px auto;
  display: flex;
  align-items: center;
  gap: 12px;
}

.music-progress input {
  flex: 1;
  accent-color: var(--gold);
}

.music-progress span {
  color: var(--muted);
  font-size: 10px;
}

.music-error {
  max-width: 750px;
  margin: 15px auto;
  text-align: center;
  color: #e8a69a;
  font-size: 12px;
  line-height: 1.8;
}

.music-error a {
  color: var(--gold);
}

/* ==================================
   GIFTS
================================== */

.gifts-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 16px;
}

.gift-card {
  position: relative;
  overflow: hidden;
  min-height: 190px;
  padding: 22px 10px;
  border: 1px solid #40321d;
  background: linear-gradient(150deg, #19150e, #090807);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 12px;
  text-align: center;
  transition: .4s;
}

.gift-card::before {
  content: "";
  position: absolute;
  top: 0;
  left: -100%;
  width: 70%;
  height: 100%;
  background: linear-gradient(90deg, transparent, #d8b56a15, transparent);
  transition: .6s;
}

.gift-card:hover::before {
  left: 130%;
}

.gift-card:hover {
  transform: translateY(-7px);
  border-color: var(--gold);
  box-shadow: 0 15px 40px #d8b56a10;
}

.gift-card.opened {
  border-color: var(--gold);
  background: linear-gradient(150deg, #292011, #100e09);
}

.gift-number {
  color: var(--gold3);
  font-size: 9px;
  letter-spacing: 3px;
}

.gift-icon {
  font-size: 40px;
  transition: .4s;
}

.gift-card:hover .gift-icon {
  transform: scale(1.15) rotate(-5deg);
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
  margin-top: 35px;
  text-align: center;
  font-size: 11px;
  letter-spacing: 3px;
  color: var(--gold);
}

.progress-track {
  height: 2px;
  max-width: 350px;
  margin: 15px auto;
  background: #292319;
}

.progress-fill {
  width: 0;
  height: 100%;
  background: var(--gold);
  transition: width .5s;
}

/* ==================================
   MODAL
================================== */

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
  position: relative;
  max-width: 550px;
  width: 100%;
  padding: 45px 30px;
  text-align: center;
  border: 1px solid var(--gold3);
  background: linear-gradient(145deg, #1b150c, #080706);
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
  color: var(--gold2);
}

.modal-content p {
  color: #c5bcae;
  font-size: 14px;
  line-height: 1.9;
  margin-top: 20px;
  white-space: pre-line;
}

.modal-close {
  position: absolute;
  top: 15px;
  right: 18px;
  background: none;
  border: none;
  color: var(--gold);
  font-size: 25px;
}

/* ==================================
   PHOTO GALLERY
================================== */

.photo-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}

.photo-frame {
  padding: 8px;
  overflow: hidden;
  border: 1px solid #4d3c20;
  background: #111;
  transition: .4s;
}

.photo-frame:hover {
  transform: translateY(-5px);
  border-color: var(--gold);
}

.photo-frame img {
  width: 100%;
  aspect-ratio: 1 / 1.15;
  object-fit: cover;
  display: block;
  filter: grayscale(15%);
  transition: .5s;
}

.photo-frame:hover img {
  filter: grayscale(0%);
  transform: scale(1.04);
}

.photo-frame p {
  font-family: "Cormorant Garamond", serif;
  color: var(--gold);
  text-align: center;
  font-size: 19px;
  padding: 12px 4px 5px;
}

/* ==================================
   MEMORY TIMELINE
================================== */

.timeline {
  max-width: 750px;
  margin: auto;
  position: relative;
}

.timeline::before {
  content: "";
  position: absolute;
  left: 22px;
  top: 0;
  bottom: 0;
  width: 1px;
  background: linear-gradient(transparent, var(--gold3), transparent);
}

.timeline-item {
  position: relative;
  padding: 0 0 45px 60px;
}

.timeline-dot {
  position: absolute;
  left: 15px;
  top: 5px;
  width: 15px;
  height: 15px;
  background: var(--gold);
  border-radius: 50%;
  box-shadow: 0 0 20px #d8b56a50;
}

.timeline-item h3 {
  font-family: "Cormorant Garamond", serif;
  font-size: 27px;
  color: var(--gold);
  font-weight: 500;
}

.timeline-item p {
  color: var(--muted);
  font-size: 13px;
  line-height: 1.9;
  margin-top: 10px;
}

/* ==================================
   LETTER
================================== */

.letter {
  max-width: 800px;
  margin: auto;
  padding: 45px;
  border: 1px solid #4b3a20;
  background: radial-gradient(ellipse at top, #4a351318, transparent 60%), #0c0b09;
  box-shadow: 0 20px 60px #0005;
}

.letter h3 {
  font-family: "Cormorant Garamond", serif;
  font-size: 34px;
  color: var(--gold);
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
  font-size: 30px;
  font-style: italic;
  color: var(--gold);
  margin-top: 30px;
}

/* ==================================
   CAKE
================================== */

.cake-area {
  text-align: center;
}

.cake {
  position: relative;
  width: 190px;
  height: 170px;
  margin: 65px auto 35px;
  filter: drop-shadow(0 15px 20px #000);
}

.cake-base {
  position: absolute;
  bottom: 0;
  width: 190px;
  height: 90px;
  background: linear-gradient(90deg, #79502b, #c89553, #80502a);
  border-radius: 8px 8px 15px 15px;
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
  width: 160px;
  height: 45px;
  background: linear-gradient(90deg, #8d592f, #e4bb78, #956033);
  border-radius: 50%;
}

.candle {
  position: absolute;
  width: 9px;
  height: 38px;
  bottom: 125px;
  left: 90px;
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
  left: 87px;
  filter: drop-shadow(0 0 12px #ff9b25);
  animation: flame 1s ease-in-out infinite alternate;
}

@keyframes flame {
  from { transform: rotate(-45deg) scale(.9); }
  to { transform: rotate(-40deg) scale(1.1); }
}

#wish-message {
  color: var(--gold);
  margin-top: 25px;
  font-family: "Cormorant Garamond", serif;
  font-size: 25px;
}

/* ==================================
   WISH GENERATOR
================================== */

.wish-box {
  max-width: 750px;
  margin: auto;
  padding: 40px 25px;
  text-align: center;
  border: 1px solid var(--line);
  background: linear-gradient(145deg, #19150e, #090807);
}

#wish-text {
  min-height: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Cormorant Garamond", serif;
  font-size: clamp(24px, 5vw, 37px);
  color: var(--gold2);
  line-height: 1.5;
}

/* ==================================
   FINAL GIFT
================================== */

.final-gift {
  max-width: 750px;
  margin: auto;
  padding: 60px 25px;
  border: 1px solid #68502a;
  background: radial-gradient(ellipse at center, #33220f40, transparent 70%);
  text-align: center;
}

.final-gift .big-icon {
  font-size: 75px;
  margin-bottom: 25px;
  animation: giftPulse 3s ease-in-out infinite;
}

@keyframes giftPulse {
  0%, 100% { transform: scale(1); }
  50% { transform: scale(1.08); }
}

.final-gift h2 {
  font-family: "Cormorant Garamond", serif;
  font-size: clamp(40px, 9vw, 80px);
  font-weight: 400;
  color: var(--gold2);
}

.final-gift p {
  color: #c4b9a6;
  font-size: 13px;
  line-height: 2;
  margin-top: 20px;
}

#final-message {
  display: none;
  margin-top: 35px;
  font-family: "Cormorant Garamond", serif;
  color: var(--gold2);
  font-size: 30px;
  line-height: 1.7;
}

footer {
  text-align: center;
  padding: 45px 20px;
  border-top: 1px solid #302719;
  color: #82786a;
  font-size: 10px;
  letter-spacing: 3px;
  line-height: 2.2;
}

footer span {
  color: var(--gold);
}

/* ==================================
   MOBILE
================================== */

@media(max-width: 750px) {
  .gifts-grid {
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
  }

  .gift-card {
    min-height: 160px;
    padding: 16px 8px;
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
    padding: 30px 22px;
  }

  section {
    padding: 75px 18px;
  }
}

@media(max-width: 420px) {
  .gifts-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .countdown-grid {
    gap: 6px;
  }

  .time-box {
    padding: 20px 4px;
  }

  .time-box span {
    font-size: 8px;
    letter-spacing: 1px;
  }

  .music-card {
    padding: 15px;
    gap: 12px;
  }

  .music-disc {
    width: 45px;
    height: 45px;
    font-size: 18px;
  }

  .music-info h3 {
    font-size: 21px;
  }

  .music-button {
    padding: 10px;
    min-width: 65px;
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

<!-- FLOATING MAGIC -->
<div id="magic-layer"></div>

<!-- NAVIGATION -->
<nav class="navbar">

  <a href="#hero" class="nav-brand">
    Bimal <span class="gold">✦</span>
  </a>

  <div class="nav-links">
    <a href="#countdown">COUNTDOWN</a>
    <a href="#music">MUSIC</a>
    <a href="#gifts">GIFTS</a>
    <a href="#memories">MEMORIES</a>
    <a href="#letter">LETTER</a>
    <a href="#final">FINAL GIFT</a>
  </div>

  <button class="nav-music" onclick="toggleMusic()">
    ♫ MUSIC
  </button>

</nav>

<!-- HERO -->
<section id="hero">

  <div class="hero-corner tl"></div>
  <div class="hero-corner tr"></div>
  <div class="hero-corner bl"></div>
  <div class="hero-corner br"></div>

  <div class="hero-orbit"></div>

  <div class="hero-content">

    <div class="hero-small">
      A CELEBRATION OF SOMEONE EXTRAORDINARY
    </div>

    <h1 class="hero-title">
      For My
      <span class="gold-text">Big Brother</span>
      <span class="gold-text">Bimal</span>
    </h1>

    <p class="hero-subtitle">
      A LITTLE SURPRISE FROM YOUR LITTLE BROTHER<br>
      MADE WITH ENDLESS LOVE
    </p>

    <div class="hero-date">
      NOVEMBER 05 · 2026
    </div>

    <div class="hero-buttons">

      <a href="#countdown" class="gold-button">
        BEGIN THE JOURNEY ✦
      </a>

      <a href="#gifts" class="gold-button">
        EXPLORE YOUR GIFTS
      </a>

    </div>

  </div>

</section>

<!-- COUNTDOWN -->
<section id="countdown">

  <div class="container">

    <div class="section-heading">

      <div class="eyebrow">
        The Moment Is Coming
      </div>

      <h2>
        Counting Down To<br>
        <span class="gold-text">Your Special Day</span>
      </h2>

      <div class="gold-line"></div>

      <p>
        Every second brings us closer to celebrating someone
        who means the world to me.
      </p>

    </div>

    <div class="countdown-grid">

      <div class="time-box">
        <strong id="days">00</strong>
        <span>DAYS</span>
      </div>

      <div class="time-box">
        <strong id="hours">00</strong>
        <span>HOURS</span>
      </div>

      <div class="time-box">
        <strong id="minutes">00</strong>
        <span>MINUTES</span>
      </div>

      <div class="time-box">
        <strong id="seconds">00</strong>
        <span>SECONDS</span>
      </div>

    </div>

    <div id="countdown-message"></div>

  </div>

</section>

<!-- MUSIC -->
<section id="music">

  <div class="container">

    <div class="section-heading">

      <div class="eyebrow">
        A Song For Every Moment
      </div>

      <h2>
        Music For <span class="gold-text">Bimal</span>
      </h2>

      <div class="gold-line"></div>

      <p id="music-description">
        A special melody while we wait for your birthday.
      </p>

    </div>

    <div class="music-card">

      <div class="music-disc" id="music-disc">
        ♫
      </div>

      <div class="music-info">

        <h3 id="music-title">
          The Countdown Song
        </h3>

        <p id="music-status">
          Your birthday surprise is getting closer.
        </p>

      </div>

      <button
        class="music-button"
        id="music-button"
        onclick="toggleMusic()">

        PLAY

      </button>

    </div>

    <div class="music-progress">

      <span id="music-current">0:00</span>

      <input
        type="range"
        id="music-seek"
        min="0"
        max="100"
        value="0"
        aria-label="Music progress">

      <span id="music-duration">0:00</span>

    </div>

    <div class="music-error" id="music-error"></div>

    <!-- YOUR EXACT MP3 FILES -->

    <audio id="song-before" loop preload="metadata">
      <source src="Song11.mp3" type="audio/mpeg">
    </audio>

    <audio id="song-after" loop preload="metadata">
      <source src="Song22.mp3" type="audio/mpeg">
    </audio>

  </div>

</section>

<!-- GIFTS -->
<section id="gifts">

  <div class="container">

    <div class="section-heading">

      <div class="eyebrow">
        Twelve Little Surprises
      </div>

      <h2>
        Open Your <span class="gold-text">Gifts</span>
      </h2>

      <div class="gold-line"></div>

      <p>
        Each gift holds a little piece of love, gratitude,
        and memories. Open every gift to discover the surprises.
      </p>

    </div>

    <div class="gifts-grid" id="gifts-grid"></div>

    <div class="gift-progress">

      <span id="opened-count">0</span> / 12 GIFTS OPENED

      <div class="progress-track">
        <div class="progress-fill" id="progress-fill"></div>
      </div>

      <p style="color:#84745b;font-size:10px;letter-spacing:1px">
        Open all 12 gifts to unlock the grand finale.
      </p>

    </div>

  </div>

</section>

<!-- MEMORIES -->
<section id="memories">

  <div class="container">

    <div class="section-heading">

      <div class="eyebrow">
        Moments That Matter
      </div>

      <h2>
        Our Little <span class="gold-text">Memories</span>
      </h2>

      <div class="gold-line"></div>

      <p>
        Different moments. Different memories.
        One beautiful bond.
      </p>

    </div>

    <div class="photo-grid">

      <div class="photo-frame">
        <img src="Nana.jpg" alt="Memory with Bimal" loading="lazy">
        <p>Our Beginning</p>
      </div>

      <div class="photo-frame">
        <img src="Nana1.jpg" alt="A special memory" loading="lazy">
        <p>Good Times</p>
      </div>

      <div class="photo-frame">
        <img src="Nana2.jpg" alt="A happy moment" loading="lazy">
        <p>Unforgettable</p>
      </div>

      <div class="photo-frame">
        <img src="Nana3.jpg" alt="Brotherhood memories" loading="lazy">
        <p>My Favourite</p>
      </div>

      <div class="photo-frame">
        <img src="Nana4.jpg" alt="A special day together" loading="lazy">
        <p>Always Together</p>
      </div>

      <div class="photo-frame">
        <img src="Nana5.jpg" alt="A memory to cherish" loading="lazy">
        <p>Forever Us</p>
      </div>

    </div>

  </div>

</section>

<!-- TIMELINE -->
<section id="timeline">

  <div class="container">

    <div class="section-heading">

      <div class="eyebrow">
        A Bond Beyond Words
      </div>

      <h2>
        Our <span class="gold-text">Story</span>
      </h2>

      <div class="gold-line"></div>

      <p>
        Some relationships don't need perfect words.
        They just need a lifetime of memories.
      </p>

    </div>

    <div class="timeline">

      <div class="timeline-item">

        <div class="timeline-dot"></div>

        <h3>The Beginning</h3>

        <p>
          From the very beginning, you were someone I could
          look up to. Having an elder brother like you has
          always been a blessing.
        </p>

      </div>

      <div class="timeline-item">

        <div class="timeline-dot"></div>

        <h3>The Little Moments</h3>

        <p>
          The laughs, the arguments, the jokes, the memories,
          and all the little things that make our bond special.
        </p>

      </div>

      <div class="timeline-item">

        <div class="timeline-dot"></div>

        <h3>The Person You Are</h3>

        <p>
          As time passes, I continue to admire your strength,
          your determination, and the person you are becoming.
        </p>

      </div>

      <div class="timeline-item">

        <div class="timeline-dot"></div>

        <h3>Forever Brothers</h3>

        <p>
          No matter where life takes us, you will always be
          my big brother, and I will always be your little brother.
        </p>

      </div>

    </div>

  </div>

</section>

<!-- LETTER -->
<section id="letter">

  <div class="container">

    <div class="section-heading">

      <div class="eyebrow">
        From My Heart
      </div>

      <h2>
        A Letter To <span class="gold-text">Bimal Bhai</span>
      </h2>

      <div class="gold-line"></div>

    </div>

    <div class="letter">

      <h3>Dear Bimal Bhai,</h3>

      <p>
        There are some people in life who make everything feel
        a little easier, a little safer, and a lot more meaningful.
        For me, you are one of those people.
      </p>

      <p>
        Having you as my big brother is one of the greatest
        blessings of my life. You have been more than just a brother.
        You have been a friend, a guide, a source of strength,
        and someone I can always look up to.
      </p>

      <p>
        I may not always say it, and sometimes I may not even
        show it, but I genuinely appreciate everything you do.
        Your presence means more to me than words can explain.
      </p>

      <p>
        On your birthday, I wish you endless happiness,
        good health, peace of mind, success in everything you do,
        and all the beautiful things this world has to offer.
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

<!-- BIRTHDAY WISH GENERATOR -->
<section id="wishes">

  <div class="container">

    <div class="section-heading">

      <div class="eyebrow">
        A Wish From The Stars
      </div>

      <h2>
        Wishes For <span class="gold-text">Your Future</span>
      </h2>

      <div class="gold-line"></div>

      <p>
        A little inspiration for your beautiful journey ahead.
      </p>

    </div>

    <div class="wish-box">

      <div id="wish-text">
        May your future shine brighter than every star in the sky.
      </div>

      <div style="margin-top:30px">

        <button class="gold-button" onclick="newWish()">
          ANOTHER WISH ✦
        </button>

      </div>

    </div>

  </div>

</section>

<!-- CAKE -->
<section id="cake">

  <div class="container">

    <div class="section-heading">

      <div class="eyebrow">
        Make A Wish
      </div>

      <h2>
        A Cake Just <span class="gold-text">For You</span>
      </h2>

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
        <div class="flame" id="flame"></div>

      </div>

      <button class="gold-button" onclick="blowCandle()">
        BLOW THE CANDLE ✦
      </button>

      <p id="wish-message"></p>

    </div>

  </div>

</section>

<!-- FINAL GIFT -->
<section id="final">

  <div class="container">

    <div class="section-heading">

      <div class="eyebrow">
        The Grand Finale
      </div>

      <h2>
        One Last <span class="gold-text">Surprise</span>
      </h2>

      <div class="gold-line"></div>

      <p>
        This one is a little more special than the rest.
      </p>

    </div>

    <div class="final-gift">

      <div class="big-icon">🎁</div>

      <h2 class="gold-text">
        For You, Bimal.
      </h2>

      <p>
        Twelve gifts. Countless memories.
        One bond that means more than anything.
      </p>

      <button
        class="gold-button filled"
        id="final-button"
        onclick="openFinalGift()"
        disabled>

        OPEN YOUR FINAL GIFT

      </button>

      <div id="final-message">

        Happy Birthday, Bimal Bhai! ❤️

        <br><br>

        <span style="font-size:20px;color:#c6b48c">

          You will always be one of the most special people
          in my life.

          May your smile never fade, your dreams never stop,
          and your heart always find happiness.

          <br><br>

          No matter where life takes us,
          we will always be brothers.

          <br><br>

          Love you forever.

        </span>

      </div>

    </div>

  </div>

</section>

<footer>

  MADE WITH <span>LOVE</span> FOR BIMAl BHAI

  <br>

  NOVEMBER 05 · 2026

  <br><br>

  A LITTLE BROTHER'S BIGGEST GIFT

</footer>

<!-- GIFT MODAL -->
<div class="modal" id="gift-modal">

  <div class="modal-content">

    <button class="modal-close" onclick="closeModal()">
      ×
    </button>

    <div class="modal-icon" id="modal-icon">
      🎁
    </div>

    <div class="eyebrow" id="modal-eyebrow">
      A LITTLE SURPRISE
    </div>

    <h2 id="modal-title">
      Your Gift
    </h2>

    <div class="gold-line"></div>

    <p id="modal-text"></p>

    <br>

    <button class="gold-button" onclick="closeModal()">
      KEEP THIS GIFT ✦
    </button>

  </div>

</div>

<script>

/* =====================================
   BIRTHDAY CONFIGURATION
===================================== */

const birthday = new Date(
  "2026-11-05T00:00:00+05:30"
).getTime();


/* =====================================
   FLOATING STARS, HEARTS & SPARKLES
===================================== */

function createMagic() {

  const layer = document.getElementById("magic-layer");

  const symbols = [
    "✦", "✧", "⋆", "✩", "♡", "♥",
    "✨", "✶", "✷", "⋆", "✧", "❤"
  ];

  for (let i = 0; i < 65; i++) {

    const item = document.createElement("span");

    item.className = "magic";

    item.textContent =
      symbols[Math.floor(Math.random() * symbols.length)];

    item.style.left = Math.random() * 100 + "%";

    item.style.fontSize =
      (9 + Math.random() * 19) + "px";

    item.style.animationDuration =
      (10 + Math.random() * 22) + "s";

    item.style.animationDelay =
      (Math.random() * 20) + "s";

    item.style.color =
      Math.random() > .5 ? "#d8b56a" : "#fff0be";

    layer.appendChild(item);

  }

}

createMagic();


/* =====================================
   MOUSE SPARKLE EFFECT
===================================== */

let lastSparkle = 0;

document.addEventListener("pointermove", function(event) {

  const now = Date.now();

  if (now - lastSparkle < 100) {
    return;
  }

  lastSparkle = now;

  const sparkle = document.createElement("span");

  sparkle.className = "cursor-sparkle";

  sparkle.textContent =
    Math.random() > .5 ? "✦" : "✧";

  sparkle.style.left = event.clientX + "px";

  sparkle.style.top = event.clientY + "px";

  sparkle.style.fontSize =
    (8 + Math.random() * 10) + "px";

  document.body.appendChild(sparkle);

  setTimeout(() => sparkle.remove(), 1000);

});


/* =====================================
   COUNTDOWN
===================================== */

function updateCountdown() {

  const difference = birthday - Date.now();

  const message =
    document.getElementById("countdown-message");

  if (difference <= 0) {

    document.getElementById("days").textContent = "00";

    document.getElementById("hours").textContent = "00";

    document.getElementById("minutes").textContent = "00";

    document.getElementById("seconds").textContent = "00";

    message.textContent =
      "Happy Birthday, Bimal Bhai! ✨";

    return;

  }

  const days = Math.floor(
    difference / (1000 * 60 * 60 * 24)
  );

  const hours = Math.floor(
    (difference / (1000 * 60 * 60)) % 24
  );

  const minutes = Math.floor(
    (difference / (1000 * 60)) % 60
  );

  const seconds = Math.floor(
    (difference / 1000) % 60
  );

  document.getElementById("days").textContent =
    String(days).padStart(2, "0");

  document.getElementById("hours").textContent =
    String(hours).padStart(2, "0");

  document.getElementById("minutes").textContent =
    String(minutes).padStart(2, "0");

  document.getElementById("seconds").textContent =
    String(seconds).padStart(2, "0");

  message.textContent =
    "A beautiful day is getting closer.";

}

updateCountdown();

setInterval(updateCountdown, 1000);


/* =====================================
   MUSIC SYSTEM
===================================== */

const songBefore =
  document.getElementById("song-before");

const songAfter =
  document.getElementById("song-after");

const musicButton =
  document.getElementById("music-button");

const musicTitle =
  document.getElementById("music-title");

const musicStatus =
  document.getElementById("music-status");

const musicDescription =
  document.getElementById("music-description");

const musicDisc =
  document.getElementById("music-disc");

const musicError =
  document.getElementById("music-error");

const musicSeek =
  document.getElementById("music-seek");

let activeSong = null;

let birthdaySongUnlocked = false;

let musicRequested = false;

let changingSong = false;


// Format seconds as minutes:seconds.
function formatTime(seconds) {

  if (!Number.isFinite(seconds)) {
    return "0:00";
  }

  const mins = Math.floor(seconds / 60);

  const secs = Math.floor(seconds % 60);

  return mins + ":" + String(secs).padStart(2, "0");

}


// Show a useful error if an MP3 fails to load.
function showMusicError(audio) {

  const filename =
    audio === songBefore ? "Song11.mp3" : "Song22.mp3";

  musicError.innerHTML =
    "Could not load <strong>" + filename + "</strong>. " +
    "Please check that it is uploaded to the same GitHub " +
    "repository folder as index.html. " +
    "<a href='" + filename + "' target='_blank'>" +
    "Test the MP3 file</a>.";

}


// Listen for audio loading errors.
songBefore.addEventListener("error", function() {

  showMusicError(songBefore);

});

songAfter.addEventListener("error", function() {

  showMusicError(songAfter);

});


// Listen for successful audio loading.
songBefore.addEventListener("canplay", function() {

  if (activeSong === songBefore) {
    musicError.textContent = "";
  }

});

songAfter.addEventListener("canplay", function() {

  if (activeSong === songAfter) {
    musicError.textContent = "";
  }

});


// Set the currently unlocked song.
function checkBirthdayMusic() {

  const birthdayStarted = Date.now() >= birthday;

  if (birthdayStarted === birthdaySongUnlocked) {
    return;
  }

  birthdaySongUnlocked = birthdayStarted;

  const previousSong = activeSong;

  const wasPlaying =
    previousSong && !previousSong.paused;

  changingSong = true;

  if (previousSong) {

    previousSong.pause();

    previousSong.currentTime = 0;

  }

  if (birthdayStarted) {

    activeSong = songAfter;

    musicTitle.textContent = "The Birthday Song";

    musicStatus.textContent =
      "Unlocked! Happy Birthday, Bimal Bhai!";

    musicDescription.textContent =
      "The birthday has arrived. Your special song is now unlocked.";

  } else {

    activeSong = songBefore;

    musicTitle.textContent = "The Countdown Song";

    musicStatus.textContent =
      "A special melody while we wait.";

    musicDescription.textContent =
      "Your birthday surprise is getting closer.";

  }

  musicDisc.classList.remove("playing");

  musicButton.textContent = "PLAY";

  changingSong = false;

  // If the previous song was playing, attempt to continue
  // with the newly unlocked song.
  if (wasPlaying && musicRequested) {

    playCurrentSong();

  }

}


// Play the currently unlocked song.
async function playCurrentSong() {

  checkBirthdayMusic();

  if (!activeSong) {
    return;
  }

  musicRequested = true;

  musicError.textContent = "";

  try {

    await activeSong.play();

    musicButton.textContent = "PAUSE";

    musicDisc.classList.add("playing");

    musicStatus.textContent =
      "Now playing your special song.";

  } catch (error) {

    musicButton.textContent = "PLAY";

    musicDisc.classList.remove("playing");

    musicStatus.textContent =
      "Tap Play to start your music.";

    if (activeSong.error) {

      showMusicError(activeSong);

    } else {

      musicError.textContent =
        "Your browser blocked automatic playback. " +
        "Tap PLAY to start the song.";

    }

  }

}


// Play or pause.
function toggleMusic() {

  checkBirthdayMusic();

  if (!activeSong) {
    return;
  }

  if (activeSong.paused) {

    playCurrentSong();

  } else {

    activeSong.pause();

    musicButton.textContent = "PLAY";

    musicDisc.classList.remove("playing");

    musicStatus.textContent =
      "Music paused.";

  }

}


// Keep the player controls synchronized.
function syncMusicControls() {

  if (!activeSong) {
    return;
  }

  if (activeSong.paused) {

    musicButton.textContent = "PLAY";

    musicDisc.classList.remove("playing");

  } else {

    musicButton.textContent = "PAUSE";

    musicDisc.classList.add("playing");

  }

}


// Update progress.
function updateMusicProgress() {

  if (!activeSong) {
    return;
  }

  const current =
    document.getElementById("music-current");

  const duration =
    document.getElementById("music-duration");

  if (Number.isFinite(activeSong.duration)) {

    musicSeek.value =
      (activeSong.currentTime / activeSong.duration) * 100;

    duration.textContent =
      formatTime(activeSong.duration);

  }

  current.textContent =
    formatTime(activeSong.currentTime);

}


songBefore.addEventListener("timeupdate", updateMusicProgress);

songAfter.addEventListener("timeupdate", updateMusicProgress);

songBefore.addEventListener("play", syncMusicControls);

songBefore.addEventListener("pause", syncMusicControls);

songAfter.addEventListener("play", syncMusicControls);

songAfter.addEventListener("pause", syncMusicControls);


// Allow seeking.
musicSeek.addEventListener("input", function() {

  if (
    activeSong &&
    Number.isFinite(activeSong.duration)
  ) {

    activeSong.currentTime =
      (Number(musicSeek.value) / 100) *
      activeSong.duration;

  }

});


// Check immediately and every second.
checkBirthdayMusic();

setInterval(checkBirthdayMusic, 1000);


/* =====================================
   12 INTERACTIVE GIFTS
===================================== */

const gifts = [

  {
    icon: "💌",
    title: "A Letter",
    subtitle: "Words from my heart",
    message:
      "Dear Bimal Bhai,\n\n" +
      "I don't always express my feelings, but I hope you know " +
      "how much you mean to me. Having you as my big brother " +
      "is something I will always be grateful for.\n\n" +
      "You are loved more than you know. ❤️"
  },

  {
    icon: "🌟",
    title: "My Respect",
    subtitle: "For the person you are",
    message:
      "One of the things I admire most about you is the person " +
      "you are becoming.\n\n" +
      "Your strength, your efforts, your determination, " +
      "and the way you keep moving forward inspire me.\n\n" +
      "I will always look up to you, Bhai."
  },

  {
    icon: "🎂",
    title: "Birthday Wish",
    subtitle: "A wish for your future",
    message:
      "May this new year of your life bring you peace, " +
      "happiness, success, good health, and countless " +
      "reasons to smile.\n\n" +
      "May every dream you hold close become a beautiful reality."
  },

  {
    icon: "🤝",
    title: "Brotherhood",
    subtitle: "A bond that never breaks",
    message:
      "Life may change. People may change. " +
      "Our paths may take us in different directions.\n\n" +
      "But one thing will always remain the same — " +
      "you are my brother, and I will always be there for you."
  },

  {
    icon: "🏆",
    title: "Your Success",
    subtitle: "You deserve the best",
    message:
      "I hope you achieve everything you have ever worked for.\n\n" +
      "I hope your hard work pays off, your sacrifices " +
      "bring beautiful results, and your future becomes " +
      "everything you have dreamed of.\n\n" +
      "I will always be proud of you."
  },

  {
    icon: "📸",
    title: "Our Memories",
    subtitle: "Moments to treasure",
    message:
      "Some of the best memories in life are the simplest ones.\n\n" +
      "The laughs, the little arguments, the silly moments, " +
      "the conversations, and everything in between.\n\n" +
      "I hope we make a million more memories together."
  },

  {
    icon: "🛡️",
    title: "My Promise",
    subtitle: "Always by your side",
    message:
      "I promise to support you whenever you need me.\n\n" +
      "I promise to celebrate your happiness, stand beside " +
      "you during difficult times, and never forget " +
      "the bond we share.\n\n" +
      "You will never have to face everything alone."
  },

  {
    icon: "🌍",
    title: "Your Dreams",
    subtitle: "Dream without limits",
    message:
      "Never stop dreaming big.\n\n" +
      "Never let fear decide your future.\n\n" +
      "You have so much potential, and I hope you always " +
      "believe in yourself as much as I believe in you."
  },

  {
    icon: "❤️",
    title: "My Gratitude",
    subtitle: "Thank you, Bhai",
    message:
      "Thank you for being a part of my life.\n\n" +
      "Thank you for the lessons, the support, the memories, " +
      "and the little things that you may not even realise " +
      "mean so much to me.\n\n" +
      "I am truly lucky to have you."
  },

  {
    icon: "☀️",
    title: "Happiness",
    subtitle: "A brighter tomorrow",
    message:
      "I hope your days are filled with laughter.\n\n" +
      "I hope your heart finds peace.\n\n" +
      "I hope you always have people around you " +
      "who genuinely care about you.\n\n" +
      "You deserve a beautiful life."
  },

  {
    icon: "👑",
    title: "My Hero",
    subtitle: "A brother like no other",
    message:
      "You don't need to be perfect to be someone I admire.\n\n" +
      "You just need to be yourself.\n\n" +
      "And that is exactly why you will always have " +
      "a special place in my heart."
  },

  {
    icon: "🎁",
    title: "The Best Gift",
    subtitle: "Having you as my brother",
    message:
      "Out of all the gifts I could ever receive in life, " +
      "having you as my big brother is one of the greatest.\n\n" +
      "No expensive gift could ever replace that.\n\n" +
      "Happy Birthday, Bimal Bhai. ❤️"
  }

];


const giftGrid =
  document.getElementById("gifts-grid");

const openedGifts = new Set();


function createGifts() {

  gifts.forEach((gift, index) => {

    const card = document.createElement("button");

    card.type = "button";

    card.className = "gift-card";

    card.innerHTML = `

      <div class="gift-number">
        GIFT ${String(index + 1).padStart(2, "0")}
      </div>

      <div class="gift-icon">
        ${gift.icon}
      </div>

      <h3>${gift.title}</h3>

      <p>${gift.subtitle}</p>

    `;

    card.addEventListener("click", function() {

      openGift(index, card);

    });

    giftGrid.appendChild(card);

  });

}


function openGift(index, card) {

  const gift = gifts[index];

  openedGifts.add(index);

  card.classList.add("opened");

  document.getElementById("modal-icon").textContent =
    gift.icon;

  document.getElementById("modal-title").textContent =
    gift.title;

  document.getElementById("modal-eyebrow").textContent =
    "GIFT " + String(index + 1).padStart(2, "0") +
    " · A LITTLE SURPRISE";

  document.getElementById("modal-text").textContent =
    gift.message;

  document.getElementById("gift-modal")
    .classList.add("show");

  updateGiftProgress();

  createConfetti(25);

}


function closeModal() {

  document.getElementById("gift-modal")
    .classList.remove("show");

}


document.getElementById("gift-modal")
  .addEventListener("click", function(event) {

    if (event.target === this) {
      closeModal();
    }

  });


function updateGiftProgress() {

  const count = openedGifts.size;

  document.getElementById("opened-count").textContent =
    count;

  document.getElementById("progress-fill").style.width =
    (count / gifts.length * 100) + "%";

  if (count === gifts.length) {

    document.getElementById("final-button").disabled = false;

    document.getElementById("final-button").textContent =
      "UNLOCK YOUR FINAL GIFT ✦";

  }

}


createGifts();


/* =====================================
   BIRTHDAY CAKE
===================================== */

let candleBlown = false;


function blowCandle() {

  const flame =
    document.getElementById("flame");

  const message =
    document.getElementById("wish-message");

  if (!candleBlown) {

    flame.style.display = "none";

    message.textContent =
      "May all your wishes come true, Bimal Bhai. ❤️";

    candleBlown = true;

    createConfetti(100);

  } else {

    flame.style.display = "block";

    message.textContent =
      "Make another beautiful wish!";

    candleBlown = false;

  }

}


/* =====================================
   WISH GENERATOR
===================================== */

const wishes = [

  "May your future shine brighter than every star in the sky.",

  "May every dream you hold become a beautiful reality.",

  "May happiness find you in every little moment.",

  "May your strength grow, your heart stay kind, and your dreams soar.",

  "May your life be filled with love, laughter, and endless success.",

  "May every new chapter bring something beautiful.",

  "May you always have the courage to chase your dreams.",

  "May peace, prosperity, and happiness follow you everywhere.",

  "May your smile never fade and your heart never lose hope.",

  "May the coming year be your most beautiful one yet."

];


function newWish() {

  const random =
    Math.floor(Math.random() * wishes.length);

  document.getElementById("wish-text").textContent =
    wishes[random];

  createConfetti(15);

}


/* =====================================
   FINAL GIFT
===================================== */

function openFinalGift() {

  if (openedGifts.size !== gifts.length) {

    alert("Open all 12 gifts first, Bimal Bhai!");

    return;

  }

  document.getElementById("final-message").style.display =
    "block";

  document.getElementById("final-button").style.display =
    "none";

  createConfetti(180);

}


/* =====================================
   GOLDEN CONFETTI
===================================== */

function createConfetti(amount) {

  const colors = [
    "#d8b56a",
    "#f8e7b0",
    "#ffffff",
    "#b58a42",
    "#f4d58d"
  ];

  for (let i = 0; i < amount; i++) {

    const confetti =
      document.createElement("div");

    confetti.style.position = "fixed";

    confetti.style.left =
      Math.random() * 100 + "vw";

    confetti.style.top = "-20px";

    confetti.style.width =
      (4 + Math.random() * 6) + "px";

    confetti.style.height =
      (6 + Math.random() * 10) + "px";

    confetti.style.background =
      colors[Math.floor(Math.random() * colors.length)];

    confetti.style.zIndex = "200";

    confetti.style.pointerEvents = "none";

    confetti.style.borderRadius = "2px";

    document.body.appendChild(confetti);

    const duration =
      2500 + Math.random() * 3500;

    const animation = confetti.animate([

      {
        transform: "translateY(0) rotate(0deg)",
        opacity: 1
      },

      {
        transform:
          "translateY(" +
          (window.innerHeight + 100) +
          "px) rotate(" +
          (360 + Math.random() * 720) +
          "deg)",

        opacity: 0.2

      }

    ], {

      duration: duration,

      easing: "ease-in"

    });

    animation.onfinish = () => confetti.remove();

  }

}


/* =====================================
   INITIALIZE
===================================== */

checkBirthdayMusic();

updateCountdown();

</script>

</body>
</html>

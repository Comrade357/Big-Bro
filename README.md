
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday Bimal Bhai ❤️</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Great+Vibes&family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>
    :root {
      --black: #080808;
      --black-soft: #111111;
      --gold: #d8b56d;
      --gold-light: #f7e5b5;
      --gold-dark: #8e6b2d;
      --white: #f7f3ea;
      --muted: #b6ad9d;
      --glass: rgba(255, 255, 255, 0.045);
      --border: rgba(216, 181, 109, 0.28);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      background:
        radial-gradient(circle at 20% 10%, rgba(216,181,109,0.08), transparent 30%),
        radial-gradient(circle at 80% 50%, rgba(216,181,109,0.05), transparent 35%),
        var(--black);
      color: var(--white);
      font-family: "Montserrat", sans-serif;
      overflow-x: hidden;
    }

    body::before {
      content: "";
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 0;
      opacity: 0.12;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 180 180' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='.8' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='.18'/%3E%3C/svg%3E");
    }

    main, section, footer, header {
      position: relative;
      z-index: 1;
    }

    button {
      font: inherit;
    }

    .gold {
      color: var(--gold);
    }

    .eyebrow {
      color: var(--gold);
      font-size: 0.72rem;
      letter-spacing: 0.32em;
      text-transform: uppercase;
      margin-bottom: 18px;
    }

    .section-title {
      font-family: "Cormorant Garamond", serif;
      font-size: clamp(2.5rem, 6vw, 5rem);
      font-weight: 500;
      line-height: 1.05;
      margin-bottom: 20px;
    }

    .section-subtitle {
      color: var(--muted);
      max-width: 650px;
      line-height: 1.8;
      margin: 0 auto;
      font-size: 0.95rem;
    }

    .center {
      text-align: center;
    }

    .gold-line {
      width: 70px;
      height: 1px;
      background: linear-gradient(90deg, transparent, var(--gold), transparent);
      margin: 25px auto;
    }

    .gold-button {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      padding: 14px 28px;
      border: 1px solid var(--gold);
      background: linear-gradient(135deg, rgba(216,181,109,0.18), rgba(216,181,109,0.04));
      color: var(--gold-light);
      border-radius: 50px;
      cursor: pointer;
      text-decoration: none;
      letter-spacing: 0.08em;
      font-size: 0.75rem;
      text-transform: uppercase;
      transition: 0.3s ease;
    }

    .gold-button:hover {
      background: var(--gold);
      color: #080808;
      transform: translateY(-3px);
      box-shadow: 0 10px 35px rgba(216,181,109,0.18);
    }

    /* Floating effects */

    #effects {
      position: fixed;
      inset: 0;
      overflow: hidden;
      pointer-events: none;
      z-index: 5;
    }

    .particle {
      position: absolute;
      bottom: -30px;
      opacity: 0;
      animation: floatUp linear forwards;
      text-shadow: 0 0 12px rgba(216,181,109,0.5);
      user-select: none;
    }

    @keyframes floatUp {
      0% {
        transform: translateY(0) rotate(0deg) scale(0.6);
        opacity: 0;
      }
      15% {
        opacity: 0.8;
      }
      80% {
        opacity: 0.65;
      }
      100% {
        transform: translateY(-110vh) rotate(360deg) scale(1.2);
        opacity: 0;
      }
    }

    /* Music player */

    .music-player {
      position: fixed;
      top: 18px;
      right: 18px;
      z-index: 20;
      display: flex;
      align-items: center;
      gap: 12px;
      padding: 11px 16px;
      border: 1px solid var(--border);
      border-radius: 50px;
      background: rgba(8,8,8,0.82);
      backdrop-filter: blur(15px);
      box-shadow: 0 8px 30px rgba(0,0,0,0.3);
    }

    .music-icon {
      color: var(--gold);
      font-size: 1.1rem;
      animation: musicPulse 2s infinite;
    }

    @keyframes musicPulse {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.15); }
    }

    .music-info {
      display: flex;
      flex-direction: column;
      gap: 3px;
    }

    .music-info strong {
      font-size: 0.72rem;
      color: var(--gold-light);
      letter-spacing: 0.04em;
    }

    .music-info span {
      font-size: 0.58rem;
      color: var(--muted);
    }

    .music-toggle {
      width: 32px;
      height: 32px;
      border: 1px solid var(--gold-dark);
      border-radius: 50%;
      background: transparent;
      color: var(--gold);
      cursor: pointer;
      font-size: 0.85rem;
    }

    /* Hero */

    .hero {
      min-height: 100vh;
      padding: 110px 20px 80px;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      overflow: hidden;
    }

    .hero::before {
      content: "";
      position: absolute;
      width: 650px;
      height: 650px;
      max-width: 100vw;
      border-radius: 50%;
      border: 1px solid rgba(216,181,109,0.08);
      box-shadow:
        0 0 0 35px rgba(216,181,109,0.018),
        0 0 0 80px rgba(216,181,109,0.012);
      pointer-events: none;
    }

    .hero-content {
      max-width: 950px;
      z-index: 2;
    }

    .hero-kicker {
      color: var(--gold);
      font-size: 0.75rem;
      letter-spacing: 0.45em;
      text-transform: uppercase;
      margin-bottom: 35px;
    }

    .hero h1 {
      font-family: "Great Vibes", cursive;
      font-size: clamp(4.2rem, 13vw, 10rem);
      font-weight: 400;
      line-height: 0.95;
      color: var(--gold-light);
      text-shadow: 0 0 40px rgba(216,181,109,0.18);
    }

    .hero h2 {
      font-family: "Cormorant Garamond", serif;
      font-size: clamp(1.4rem, 4vw, 3rem);
      font-weight: 400;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      margin-top: 28px;
    }

    .hero-description {
      color: var(--muted);
      max-width: 600px;
      margin: 30px auto;
      line-height: 1.9;
      font-size: 0.9rem;
    }

    .hero-date {
      color: var(--gold);
      letter-spacing: 0.35em;
      font-size: 0.8rem;
      margin: 25px 0 35px;
    }

    .scroll-indicator {
      position: absolute;
      bottom: 28px;
      left: 50%;
      transform: translateX(-50%);
      color: var(--gold-dark);
      font-size: 0.65rem;
      letter-spacing: 0.25em;
      text-transform: uppercase;
      animation: scrollPulse 2s infinite;
    }

    @keyframes scrollPulse {
      0%, 100% { opacity: 0.4; transform: translate(-50%, 0); }
      50% { opacity: 1; transform: translate(-50%, 7px); }
    }

    /* Countdown */

    .countdown-section {
      padding: 90px 20px;
      border-top: 1px solid rgba(216,181,109,0.1);
      border-bottom: 1px solid rgba(216,181,109,0.1);
      background: rgba(255,255,255,0.015);
    }

    .countdown {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 15px;
      margin: 45px auto 25px;
    }

    .time-box {
      width: 125px;
      padding: 25px 15px;
      border: 1px solid var(--border);
      background: linear-gradient(145deg, rgba(216,181,109,0.08), rgba(255,255,255,0.015));
      border-radius: 8px;
    }

    .time-box strong {
      display: block;
      color: var(--gold-light);
      font-family: "Cormorant Garamond", serif;
      font-size: 3rem;
      font-weight: 500;
    }

    .time-box span {
      display: block;
      color: var(--muted);
      font-size: 0.62rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      margin-top: 8px;
    }

    #countdownMessage {
      color: var(--gold);
      margin-top: 25px;
      font-family: "Cormorant Garamond", serif;
      font-size: 1.5rem;
    }

    /* Photo gallery */

    .gallery-section {
      padding: 110px 20px;
    }

    .gallery-grid {
      max-width: 1100px;
      margin: 55px auto 0;
      display: grid;
      grid-template-columns: repeat(12, 1fr);
      gap: 18px;
    }

    .gallery-card {
      position: relative;
      overflow: hidden;
      border: 1px solid var(--border);
      border-radius: 8px;
      background: #17130d;
      min-height: 260px;
    }

    .gallery-card:nth-child(1) {
      grid-column: span 7;
      min-height: 430px;
    }

    .gallery-card:nth-child(2) {
      grid-column: span 5;
      min-height: 430px;
    }

    .gallery-card:nth-child(3),
    .gallery-card:nth-child(4),
    .gallery-card:nth-child(5) {
      grid-column: span 4;
      min-height: 300px;
    }

    .gallery-card img {
      width: 100%;
      height: 100%;
      min-height: inherit;
      object-fit: cover;
      display: block;
      filter: saturate(0.8);
      transition: transform 0.7s ease, filter 0.7s ease;
    }

    .gallery-card:hover img {
      transform: scale(1.06);
      filter: saturate(1.1);
    }

    .gallery-card::after {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(0deg, rgba(0,0,0,0.4), transparent 45%);
      pointer-events: none;
    }

    .gallery-caption {
      position: absolute;
      bottom: 20px;
      left: 20px;
      z-index: 2;
      color: var(--gold-light);
      font-family: "Cormorant Garamond", serif;
      font-size: 1.4rem;
      font-style: italic;
    }

    /* Letter */

    .letter-section {
      padding: 110px 20px;
      background: linear-gradient(180deg, rgba(216,181,109,0.025), transparent);
    }

    .letter-card {
      max-width: 850px;
      margin: 50px auto 0;
      padding: clamp(25px, 6vw, 65px);
      border: 1px solid var(--border);
      background: rgba(255,255,255,0.025);
      border-radius: 10px;
      position: relative;
    }

    .letter-card::before {
      content: "❝";
      position: absolute;
      top: 10px;
      left: 25px;
      font-family: Georgia, serif;
      font-size: 5rem;
      color: rgba(216,181,109,0.15);
    }

    .letter-card p {
      color: #d6cbbb;
      font-family: "Cormorant Garamond", serif;
      font-size: clamp(1.2rem, 2.5vw, 1.55rem);
      line-height: 1.9;
      margin-bottom: 20px;
    }

    .letter-signature {
      color: var(--gold);
      font-family: "Great Vibes", cursive;
      font-size: 2.5rem;
      margin-top: 30px;
      text-align: right;
    }

    /* Timeline */

    .timeline-section {
      padding: 110px 20px;
    }

    .timeline {
      max-width: 850px;
      margin: 60px auto 0;
      position: relative;
    }

    .timeline::before {
      content: "";
      position: absolute;
      top: 0;
      bottom: 0;
      left: 50%;
      width: 1px;
      background: linear-gradient(transparent, var(--gold-dark), var(--gold), transparent);
    }

    .timeline-item {
      width: 50%;
      padding: 20px 35px;
      position: relative;
    }

    .timeline-item:nth-child(odd) {
      left: 0;
      text-align: right;
    }

    .timeline-item:nth-child(even) {
      left: 50%;
      text-align: left;
    }

    .timeline-item::after {
      content: "✦";
      position: absolute;
      top: 30px;
      color: var(--gold);
      font-size: 1rem;
    }

    .timeline-item:nth-child(odd)::after {
      right: -8px;
    }

    .timeline-item:nth-child(even)::after {
      left: -8px;
    }

    .timeline-item h3 {
      font-family: "Cormorant Garamond", serif;
      color: var(--gold-light);
      font-size: 1.6rem;
      margin-bottom: 10px;
    }

    .timeline-item p {
      color: var(--muted);
      line-height: 1.8;
      font-size: 0.85rem;
    }

    /* Gifts */

    .gifts-section {
      padding: 110px 20px;
      background: rgba(255,255,255,0.015);
    }

    .gift-progress {
      max-width: 500px;
      margin: 35px auto 15px;
    }

    .progress-label {
      display: flex;
      justify-content: space-between;
      color: var(--muted);
      font-size: 0.72rem;
      margin-bottom: 10px;
    }

    .progress-track {
      height: 5px;
      background: rgba(255,255,255,0.08);
      border-radius: 10px;
      overflow: hidden;
    }

    .progress-fill {
      height: 100%;
      width: 0%;
      background: linear-gradient(90deg, var(--gold-dark), var(--gold-light));
      transition: width 0.5s ease;
    }

    .gift-grid {
      max-width: 1100px;
      margin: 50px auto 0;
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 18px;
    }

    .gift-card {
      position: relative;
      min-height: 210px;
      padding: 25px 15px;
      border: 1px solid var(--border);
      border-radius: 8px;
      background: linear-gradient(145deg, rgba(216,181,109,0.07), rgba(255,255,255,0.015));
      cursor: pointer;
      transition: 0.3s ease;
      text-align: center;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      gap: 12px;
    }

    .gift-card:hover {
      transform: translateY(-5px);
      border-color: var(--gold);
      box-shadow: 0 15px 35px rgba(216,181,109,0.08);
    }

    .gift-card.opened {
      background: linear-gradient(145deg, rgba(216,181,109,0.13), rgba(255,255,255,0.025));
      border-color: rgba(216,181,109,0.6);
    }

    .gift-icon {
      font-size: 2.8rem;
      filter: drop-shadow(0 0 12px rgba(216,181,109,0.2));
    }

    .gift-card h3 {
      color: var(--gold-light);
      font-family: "Cormorant Garamond", serif;
      font-size: 1.35rem;
      font-weight: 500;
    }

    .gift-card p {
      color: var(--muted);
      font-size: 0.72rem;
      line-height: 1.6;
    }

    .gift-card .gift-status {
      color: var(--gold);
      font-size: 0.6rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
    }

    /* Gift modal */

    .modal {
      position: fixed;
      inset: 0;
      z-index: 50;
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      background: rgba(0,0,0,0.8);
      backdrop-filter: blur(12px);
    }

    .modal.active {
      display: flex;
    }

    .modal-content {
      width: 100%;
      max-width: 600px;
      max-height: 85vh;
      overflow-y: auto;
      padding: 45px 30px;
      border: 1px solid var(--gold);
      border-radius: 10px;
      background:
        radial-gradient(circle at top, rgba(216,181,109,0.12), transparent 50%),
        #0c0b09;
      text-align: center;
      position: relative;
      animation: modalEnter 0.35s ease;
    }

    @keyframes modalEnter {
      from { opacity: 0; transform: translateY(20px) scale(0.96); }
      to { opacity: 1; transform: translateY(0) scale(1); }
    }

    .modal-close {
      position: absolute;
      top: 15px;
      right: 18px;
      width: 35px;
      height: 35px;
      border: 1px solid var(--border);
      background: transparent;
      color: var(--gold);
      border-radius: 50%;
      cursor: pointer;
      font-size: 1.1rem;
    }

    .modal-icon {
      font-size: 3.5rem;
      margin-bottom: 20px;
    }

    .modal-content h2 {
      color: var(--gold-light);
      font-family: "Cormorant Garamond", serif;
      font-size: 2.5rem;
      font-weight: 500;
      margin-bottom: 20px;
    }

    .modal-content p {
      color: #d6cbbb;
      line-height: 1.9;
      font-size: 0.95rem;
    }

    /* Cake */

    .cake-section {
      padding: 110px 20px;
    }

    .cake {
      width: 220px;
      height: 180px;
      margin: 60px auto 35px;
      position: relative;
      cursor: pointer;
      transition: 0.3s ease;
    }

    .cake:hover {
      transform: scale(1.04);
    }

    .cake-base {
      position: absolute;
      bottom: 0;
      left: 10px;
      width: 200px;
      height: 100px;
      background: linear-gradient(135deg, #8e6b2d, #d8b56d, #8e6b2d);
      border-radius: 8px 8px 15px 15px;
      box-shadow: 0 15px 40px rgba(216,181,109,0.12);
    }

    .cake-base::before {
      content: "";
      position: absolute;
      top: 20px;
      left: 0;
      right: 0;
      height: 20px;
      background: rgba(255,255,255,0.22);
    }

    .cake-top {
      position: absolute;
      bottom: 90px;
      left: 25px;
      width: 170px;
      height: 50px;
      background: linear-gradient(135deg, #f3dfb0, #b78a42);
      border-radius: 50%;
      border: 2px solid #d8b56d;
    }

    .candle {
      position: absolute;
      bottom: 135px;
      left: 105px;
      width: 12px;
      height: 45px;
      background: repeating-linear-gradient(
        45deg,
        #f5e8c8 0 5px,
        #b78a42 5px 10px
      );
      border-radius: 3px;
    }

    .flame {
      position: absolute;
      bottom: 177px;
      left: 102px;
      width: 18px;
      height: 28px;
      background: radial-gradient(ellipse at bottom, #fff6b5, #f7a23b 60%, transparent 75%);
      border-radius: 50% 50% 40% 40%;
      animation: flameDance 0.7s infinite alternate;
      filter: drop-shadow(0 0 12px #f7a23b);
    }

    @keyframes flameDance {
      from { transform: rotate(-5deg) scale(0.95); }
      to { transform: rotate(5deg) scale(1.08); }
    }

    .cake.blown .flame {
      display: none;
    }

    .cake-message {
      color: var(--gold);
      font-family: "Cormorant Garamond", serif;
      font-size: 1.5rem;
      min-height: 35px;
      margin: 20px auto;
    }

    /* Final surprise */

    .final-section {
      padding: 110px 20px 130px;
      border-top: 1px solid rgba(216,181,109,0.1);
    }

    .final-lock {
      max-width: 700px;
      margin: 45px auto 0;
      padding: 50px 25px;
      border: 1px solid var(--border);
      border-radius: 10px;
      background: rgba(255,255,255,0.025);
      text-align: center;
    }

    .lock-icon {
      font-size: 3.5rem;
      margin-bottom: 20px;
    }

    .final-lock h3 {
      font-family: "Cormorant Garamond", serif;
      font-size: 2.2rem;
      color: var(--gold-light);
      margin-bottom: 15px;
      font-weight: 500;
    }

    .final-lock p {
      color: var(--muted);
      line-height: 1.8;
      margin-bottom: 25px;
    }

    #finalReveal {
      display: none;
      margin-top: 35px;
      padding: 35px;
      border: 1px solid var(--gold);
      border-radius: 8px;
      background: rgba(216,181,109,0.06);
    }

    #finalReveal.show {
      display: block;
      animation: modalEnter 0.5s ease;
    }

    #finalReveal h2 {
      font-family: "Great Vibes", cursive;
      font-size: clamp(3rem, 8vw, 5rem);
      color: var(--gold-light);
      font-weight: 400;
      margin-bottom: 20px;
    }

    #finalReveal p {
      font-family: "Cormorant Garamond", serif;
      color: #e4d8c3;
      font-size: 1.3rem;
      line-height: 1.9;
    }

    footer {
      padding: 30px 20px;
      border-top: 1px solid rgba(216,181,109,0.1);
      text-align: center;
      color: var(--muted);
      font-size: 0.7rem;
      letter-spacing: 0.1em;
    }

    footer span {
      color: var(--gold);
    }

    /* Responsive */

    @media (max-width: 800px) {
      .gift-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .gallery-card:nth-child(1),
      .gallery-card:nth-child(2) {
        grid-column: span 6;
        min-height: 300px;
      }

      .gallery-card:nth-child(3),
      .gallery-card:nth-child(4),
      .gallery-card:nth-child(5) {
        grid-column: span 4;
        min-height: 230px;
      }

      .time-box {
        width: 105px;
      }

      .time-box strong {
        font-size: 2.5rem;
      }
    }

    @media (max-width: 560px) {
      .music-player {
        top: 10px;
        right: 10px;
        padding: 8px 11px;
        gap: 8px;
      }

      .music-info strong {
        font-size: 0.62rem;
      }

      .music-info span {
        font-size: 0.52rem;
      }

      .hero {
        padding-top: 100px;
      }

      .hero-kicker {
        letter-spacing: 0.25em;
      }

      .countdown {
        gap: 9px;
      }

      .time-box {
        width: calc(50% - 9px);
        max-width: 140px;
        padding: 20px 10px;
      }

      .gallery-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .gallery-card:nth-child(1),
      .gallery-card:nth-child(2),
      .gallery-card:nth-child(3),
      .gallery-card:nth-child(4),
      .gallery-card:nth-child(5) {
        grid-column: span 1;
        min-height: 230px;
      }

      .gallery-card:nth-child(1) {
        grid-column: span 2;
        min-height: 350px;
      }

      .gallery-card img {
        min-height: inherit;
      }

      .timeline::before {
        left: 12px;
      }

      .timeline-item,
      .timeline-item:nth-child(odd),
      .timeline-item:nth-child(even) {
        width: 100%;
        left: 0;
        text-align: left;
        padding: 20px 20px 20px 40px;
      }

      .timeline-item:nth-child(odd)::after,
      .timeline-item:nth-child(even)::after {
        left: 4px;
        right: auto;
      }

      .gift-grid {
        gap: 12px;
      }

      .gift-card {
        min-height: 190px;
        padding: 20px 10px;
      }

      .gift-icon {
        font-size: 2.3rem;
      }

      .modal-content {
        padding: 45px 22px 30px;
      }

      .modal-content h2 {
        font-size: 2rem;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        scroll-behavior: auto !important;
        transition-duration: 0.01ms !important;
      }
    }
  </style>
</head>

<body>

  <div id="effects" aria-hidden="true"></div>

  <!-- Music: the only song on the website -->
  <div class="music-player">
    <div class="music-icon">♫</div>
    <div class="music-info">
      <strong>OUR SPECIAL SONG</strong>
      <span>Song22.mp3</span>
    </div>
    <button class="music-toggle" id="musicToggle" aria-label="Play or pause music">▶</button>
  </div>

  <audio id="birthdaySong" src="Song22.mp3" loop preload="auto"></audio>

  <main>

    <!-- HERO -->
    <section class="hero" id="home">
      <div class="hero-content">
        <p class="hero-kicker">A little world made just for you</p>

        <h1>Happy Birthday</h1>

        <h2>Dear <span class="gold">Bimal Bhai</span></h2>

        <div class="gold-line"></div>

        <p class="hero-description">
          For the person who has been more than a brother —
          a guide, a protector, a friend, and one of the most
          precious parts of my life.
        </p>

        <p class="hero-date">05 · 11 · 2026</p>

        <a href="#countdown" class="gold-button">Begin the surprise ✦</a>
      </div>

      <div class="scroll-indicator">Scroll to explore ↓</div>
    </section>

    <!-- COUNTDOWN -->
    <section class="countdown-section center" id="countdown">
      <p class="eyebrow">The special day is approaching</p>
      <h2 class="section-title">The Countdown</h2>
      <p class="section-subtitle">
        Every second brings us closer to celebrating someone truly special.
      </p>

      <div class="countdown">
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

      <p id="countdownMessage">A beautiful day is on its way ✨</p>
    </section>

    <!-- GALLERY -->
    <section class="gallery-section center" id="gallery">
      <p class="eyebrow">Moments worth keeping</p>
      <h2 class="section-title">A Gallery of <span class="gold">Memories</span></h2>
      <p class="section-subtitle">
        Some moments become memories. Some people make those memories unforgettable.
      </p>

      <div class="gallery-grid">
        <div class="gallery-card">
          <img src="Nana.jpg" alt="A special memory with Bimal" loading="lazy">
          <div class="gallery-caption">A moment to remember</div>
        </div>

        <div class="gallery-card">
          <img src="Nana2.jpg" alt="A beautiful memory" loading="lazy">
          <div class="gallery-caption">Always together</div>
        </div>

        <div class="gallery-card">
          <img src="Nana3.jpg" alt="A precious memory" loading="lazy">
          <div class="gallery-caption">The good old days</div>
        </div>

        <div class="gallery-card">
          <img src="Nana4.jpg" alt="A memory full of happiness" loading="lazy">
          <div class="gallery-caption">Little moments</div>
        </div>

        <div class="gallery-card">
          <img src="Nana5.jpg" alt="A memorable moment" loading="lazy">
          <div class="gallery-caption">Forever special</div>
        </div>
      </div>
    </section>

    <!-- LETTER -->
    <section class="letter-section center" id="letter">
      <p class="eyebrow">From my heart to yours</p>
      <h2 class="section-title">A Letter for <span class="gold">You</span></h2>
      <p class="section-subtitle">
        Some feelings are too meaningful to fit into an ordinary birthday wish.
      </p>

      <div class="letter-card">
        <p>Dear Bimal Bhai,</p>

        <p>
          On your special day, I just want to remind you how much you mean to me.
          Having you as my big brother is one of the greatest blessings of my life.
        </p>

        <p>
          Thank you for being someone I can look up to, someone whose presence
          brings strength, and someone whose place in my life can never be replaced.
        </p>

        <p>
          I may not always say it, but I appreciate every little thing you do.
          Your support, your care, your guidance, and even the little moments
          we share mean more than words can explain.
        </p>

        <p>
          May this new year of your life bring you peace, happiness, good health,
          success, and everything your heart has been wishing for.
          May every dream you carry become a beautiful reality.
        </p>

        <p>
          No matter how much life changes, one thing will always remain the same:
          I will always be proud to call you my brother.
        </p>

        <p>
          Happy Birthday, Bhai. Keep smiling, keep shining, and keep being
          the wonderful person you are.
        </p>

        <div class="letter-signature">With love, always ❤️</div>
      </div>
    </section>

    <!-- TIMELINE -->
    <section class="timeline-section center" id="memories">
      <p class="eyebrow">A journey of memories</p>
      <h2 class="section-title">Our Little <span class="gold">Timeline</span></h2>
      <p class="section-subtitle">
        Not just years passing by — a collection of moments that made life special.
      </p>

      <div class="timeline">
        <div class="timeline-item">
          <h3>The Beginning</h3>
          <p>
            The beginning of a bond that would become one of the most meaningful
            parts of our lives.
          </p>
        </div>

        <div class="timeline-item">
          <h3>Growing Together</h3>
          <p>
            Learning, laughing, making memories, and discovering that family
            is one of life's greatest gifts.
          </p>
        </div>

        <div class="timeline-item">
          <h3>Through Every Season</h3>
          <p>
            The good days, the difficult days, and all the little moments in between —
            we keep moving forward.
          </p>
        </div>

        <div class="timeline-item">
          <h3>Today & Always</h3>
          <p>
            Celebrating you today and wishing you countless more years of love,
            laughter, and unforgettable memories.
          </p>
        </div>
      </div>
    </section>

    <!-- GIFTS -->
    <section class="gifts-section center" id="gifts">
      <p class="eyebrow">A collection of little surprises</p>
      <h2 class="section-title">12 Gifts, <span class="gold">12 Wishes</span></h2>
      <p class="section-subtitle">
        Every gift holds a little message. Open all twelve to unlock the final surprise.
      </p>

      <div class="gift-progress">
        <div class="progress-label">
          <span>Gifts discovered</span>
          <span id="giftCount">0 / 12</span>
        </div>
        <div class="progress-track">
          <div class="progress-fill" id="progressFill"></div>
        </div>
      </div>

      <div class="gift-grid" id="giftGrid"></div>
    </section>

    <!-- CAKE -->
    <section class="cake-section center" id="cakeSection">
      <p class="eyebrow">Make a birthday wish</p>
      <h2 class="section-title">A Cake Just <span class="gold">For You</span></h2>
      <p class="section-subtitle">
        Close your eyes, make a wish, and tap the cake to blow out the candle.
      </p>

      <div class="cake" id="cake" role="button" tabindex="0" aria-label="Blow out the birthday candle">
        <div class="cake-base"></div>
        <div class="cake-top"></div>
        <div class="candle"></div>
        <div class="flame"></div>
      </div>

      <p class="cake-message" id="cakeMessage">Make a wish, Bhai ✨</p>

      <button class="gold-button" id="wishButton">Make a Wish</button>
    </section>

    <!-- FINAL SURPRISE -->
    <section class="final-section center" id="final">
      <p class="eyebrow">One last surprise</p>
      <h2 class="section-title">Something <span class="gold">Special</span></h2>
      <p class="section-subtitle">
        The final surprise is waiting. It opens when all twelve gifts have been discovered.
      </p>

      <div class="final-lock">
        <div class="lock-icon" id="lockIcon">🔒</div>
        <h3 id="finalTitle">A Surprise Is Waiting</h3>
        <p id="finalDescription">
          Open all 12 gifts above to unlock this final birthday message.
        </p>

        <button class="gold-button" id="unlockButton" disabled>
          Unlock the Surprise
        </button>

        <div id="finalReveal">
          <h2>Happy Birthday, Bhai!</h2>
          <p>
            You are not just my big brother — you are a part of my heart,
            my strength, and one of the greatest blessings in my life.
            <br><br>
            May your life always be filled with happiness, peace, success,
            love, and beautiful memories.
            <br><br>
            Whatever happens, wherever life takes us,
            I will always be grateful to have you as my brother.
            <br><br>
            This little website is just a small reminder of a very big feeling:
            <br><br>
            <strong class="gold">You are loved more than you know. ❤️</strong>
          </p>
        </div>
      </div>
    </section>

  </main>

  <footer>
    Made with <span>♥</span> for Bimal Bhai · 05 November 2026
  </footer>

  <!-- GIFT MODAL -->
  <div class="modal" id="giftModal" role="dialog" aria-modal="true" aria-labelledby="modalTitle">
    <div class="modal-content">
      <button class="modal-close" id="modalClose" aria-label="Close gift">×</button>
      <div class="modal-icon" id="modalIcon">🎁</div>
      <h2 id="modalTitle">A Special Gift</h2>
      <p id="modalMessage"></p>
    </div>
  </div>

  <script>
    /* -----------------------------------------
       MUSIC PLAYER
       Only Song22.mp3 is used on this website.
    ----------------------------------------- */

    const birthdaySong = document.getElementById("birthdaySong");
    const musicToggle = document.getElementById("musicToggle");

    musicToggle.addEventListener("click", async () => {
      if (birthdaySong.paused) {
        try {
          await birthdaySong.play();
          musicToggle.textContent = "Ⅱ";
        } catch (error) {
          musicToggle.textContent = "▶";
          alert("Please check that Song22.mp3 is in the same folder as index.html.");
        }
      } else {
        birthdaySong.pause();
        musicToggle.textContent = "▶";
      }
    });

    birthdaySong.addEventListener("play", () => {
      musicToggle.textContent = "Ⅱ";
    });

    birthdaySong.addEventListener("pause", () => {
      musicToggle.textContent = "▶";
    });

    /* -----------------------------------------
       FLOATING HEARTS, STARS & SPARKLES
    ----------------------------------------- */

    const effects = document.getElementById("effects");

    const particleSymbols = ["✦", "✧", "♡", "♥", "⋆", "✨", "✶"];
    const particleColors = ["#d8b56d", "#f7e5b5", "#b99550", "#fff0c8"];

    function createParticle() {
      const particle = document.createElement("span");
      particle.className = "particle";

      particle.textContent =
        particleSymbols[Math.floor(Math.random() * particleSymbols.length)];

      particle.style.left = Math.random() * 100 + "%";
      particle.style.fontSize = (Math.random() * 16 + 8) + "px";
      particle.style.color =
        particleColors[Math.floor(Math.random() * particleColors.length)];

      const duration = Math.random() * 9 + 8;
      particle.style.animationDuration = duration + "s";

      effects.appendChild(particle);

      setTimeout(() => {
        particle.remove();
      }, duration * 1000);
    }

    for (let i = 0; i < 25; i++) {
      setTimeout(createParticle, i * 250);
    }

    setInterval(createParticle, 450);

    /* -----------------------------------------
       COUNTDOWN
       Birthday: November 5, 2026
       India Standard Time: UTC+05:30
    ----------------------------------------- */

    const birthdayDate = new Date("2026-11-05T00:00:00+05:30").getTime();

    const daysElement = document.getElementById("days");
    const hoursElement = document.getElementById("hours");
    const minutesElement = document.getElementById("minutes");
    const secondsElement = document.getElementById("seconds");
    const countdownMessage = document.getElementById("countdownMessage");

    function updateCountdown() {
      const now = Date.now();
      const distance = birthdayDate - now;

      if (distance <= 0) {
        daysElement.textContent = "00";
        hoursElement.textContent = "00";
        minutesElement.textContent = "00";
        secondsElement.textContent = "00";

        countdownMessage.textContent = "Happy Birthday, Bimal Bhai! 🎉";
        return;
      }

      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor((distance / (1000 * 60 * 60)) % 24);
      const minutes = Math.floor((distance / (1000 * 60)) % 60);
      const seconds = Math.floor((distance / 1000) % 60);

      daysElement.textContent = String(days).padStart(2, "0");
      hoursElement.textContent = String(hours).padStart(2, "0");
      minutesElement.textContent = String(minutes).padStart(2, "0");
      secondsElement.textContent = String(seconds).padStart(2, "0");
    }

    updateCountdown();
    setInterval(updateCountdown, 1000);

    /* -----------------------------------------
       12 INTERACTIVE GIFTS
    ----------------------------------------- */

    const gifts = [
      {
        icon: "💛",
        title: "A Wish",
        short: "A wish from my heart",
        message:
          "May your life be filled with endless happiness, good health, peace, and success. May every new day bring you a reason to smile."
      },
      {
        icon: "🌟",
        title: "A Star",
        short: "You deserve to shine",
        message:
          "You deserve every beautiful thing life has to offer. Keep shining in your own way, Bhai. The world is better with your light in it."
      },
      {
        icon: "🤝",
        title: "A Promise",
        short: "Always by your side",
        message:
          "No matter where life takes us, you will always have someone who cares for you, believes in you, and wishes the very best for you."
      },
      {
        icon: "📸",
        title: "A Memory",
        short: "Moments that stay forever",
        message:
          "Some memories never fade. They become a part of who we are. I hope we keep creating beautiful memories together for many years to come."
      },
      {
        icon: "🛡️",
        title: "A Blessing",
        short: "For your strength",
        message:
          "May you always have the courage to face every challenge, the wisdom to choose your path, and the strength to keep moving forward."
      },
      {
        icon: "🌹",
        title: "A Thank You",
        short: "For everything you do",
        message:
          "Thank you for being you. Thank you for your care, your support, your guidance, and all the little things that make such a big difference."
      },
      {
        icon: "☀️",
        title: "A Smile",
        short: "A little happiness",
        message:
          "I hope this birthday brings you a thousand reasons to smile. And even on ordinary days, I hope happiness finds its way to you."
      },
      {
        icon: "🎯",
        title: "A Dream",
        short: "May your dreams come true",
        message:
          "May every dream you have been working toward become reality. May your efforts be rewarded and your future be brighter than you imagine."
      },
      {
        icon: "🕊️",
        title: "Peace",
        short: "A peaceful year ahead",
        message:
          "May your heart always find peace, your mind find clarity, and your life find the balance and happiness you truly deserve."
      },
      {
        icon: "💎",
        title: "A Reminder",
        short: "You are precious",
        message:
          "Never forget how valuable you are. You make a difference in the lives of the people around you, especially in mine."
      },
      {
        icon: "🎂",
        title: "A Celebration",
        short: "Today is all about you",
        message:
          "Today is a celebration of your life, your kindness, your strength, and all the wonderful things that make you the person you are."
      },
      {
        icon: "❤️",
        title: "My Love",
        short: "The most important gift",
        message:
          "The best gift I can give you is a simple truth: I love you, Bhai. I am proud of you, grateful for you, and always wishing the best for you."
      }
    ];

    const giftGrid = document.getElementById("giftGrid");
    const giftCount = document.getElementById("giftCount");
    const progressFill = document.getElementById("progressFill");

    const giftModal = document.getElementById("giftModal");
    const modalClose = document.getElementById("modalClose");
    const modalIcon = document.getElementById("modalIcon");
    const modalTitle = document.getElementById("modalTitle");
    const modalMessage = document.getElementById("modalMessage");

    const openedGifts = new Set();

    function renderGifts() {
      giftGrid.innerHTML = "";

      gifts.forEach((gift, index) => {
        const card = document.createElement("button");
        card.type = "button";
        card.className = "gift-card";
        card.setAttribute("aria-label", "Open gift " + (index + 1));

        if (openedGifts.has(index)) {
          card.classList.add("opened");
        }

        card.innerHTML = `
          <div class="gift-icon">${gift.icon}</div>
          <h3>${gift.title}</h3>
          <p>${gift.short}</p>
          <span class="gift-status">
            ${openedGifts.has(index) ? "✦ Discovered" : "Tap to open"}
          </span>
        `;

        card.addEventListener("click", () => openGift(index));
        giftGrid.appendChild(card);
      });
    }

    function openGift(index) {
      const gift = gifts[index];

      openedGifts.add(index);

      modalIcon.textContent = gift.icon;
      modalTitle.textContent = gift.title;
      modalMessage.textContent = gift.message;

      giftModal.classList.add("active");

      updateGiftProgress();
      renderGifts();
    }

    function updateGiftProgress() {
      const count = openedGifts.size;
      const percentage = (count / gifts.length) * 100;

      giftCount.textContent = count + " / " + gifts.length;
      progressFill.style.width = percentage + "%";

      const unlockButton = document.getElementById("unlockButton");
      const lockIcon = document.getElementById("lockIcon");
      const finalTitle = document.getElementById("finalTitle");
      const finalDescription = document.getElementById("finalDescription");

      if (count === gifts.length) {
        unlockButton.disabled = false;
        unlockButton.textContent = "Open Your Final Surprise";
        unlockButton.style.opacity = "1";
        unlockButton.style.cursor = "pointer";

        lockIcon.textContent = "🔓";
        finalTitle.textContent = "All Gifts Discovered!";
        finalDescription.textContent =
          "You found every little surprise. Your final birthday message is ready.";
      } else {
        unlockButton.disabled = true;
        unlockButton.textContent = "Unlock the Surprise";
        unlockButton.style.opacity = "0.45";
        unlockButton.style.cursor = "not-allowed";

        lockIcon.textContent = "🔒";
        finalTitle.textContent = "A Surprise Is Waiting";
        finalDescription.textContent =
          "Open all 12 gifts above to unlock this final birthday message.";
      }
    }

    function closeGiftModal() {
      giftModal.classList.remove("active");
    }

    modalClose.addEventListener("click", closeGiftModal);

    giftModal.addEventListener("click", (event) => {
      if (event.target === giftModal) {
        closeGiftModal();
      }
    });

    document.addEventListener("keydown", (event) => {
      if (event.key === "Escape") {
        closeGiftModal();
      }
    });

    renderGifts();
    updateGiftProgress();

    /* -----------------------------------------
       BIRTHDAY CAKE & WISH
    ----------------------------------------- */

    const cake = document.getElementById("cake");
    const cakeMessage = document.getElementById("cakeMessage");
    const wishButton = document.getElementById("wishButton");

    let candleBlown = false;

    function blowCandle() {
      if (candleBlown) {
        cakeMessage.textContent = "Your wish is on its way, Bhai ❤️";
        return;
      }

      candleBlown = true;
      cake.classList.add("blown");

      cakeMessage.textContent =
        "May your wish come true. Happy Birthday, Bhai! ✨";

      wishButton.textContent = "Wish Made ❤️";

      for (let i = 0; i < 25; i++) {
        setTimeout(createParticle, i * 60);
      }
    }

    cake.addEventListener("click", blowCandle);

    cake.addEventListener("keydown", (event) => {
      if (event.key === "Enter" || event.key === " ") {
        event.preventDefault();
        blowCandle();
      }
    });

    wishButton.addEventListener("click", blowCandle);

    /* -----------------------------------------
       FINAL SURPRISE UNLOCK
    ----------------------------------------- */

    const unlockButton = document.getElementById("unlockButton");
    const finalReveal = document.getElementById("finalReveal");

    unlockButton.addEventListener("click", () => {
      if (openedGifts.size !== gifts.length) {
        return;
      }

      finalReveal.classList.add("show");
      unlockButton.textContent = "Surprise Unlocked ❤️";
      unlockButton.disabled = true;

      document.getElementById("final").scrollIntoView({
        behavior: "smooth",
        block: "center"
      });

      for (let i = 0; i < 35; i++) {
        setTimeout(createParticle, i * 80);
      }
    });
  </script>

</body>
</html>

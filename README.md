<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Happy Anniversary BeckySweetChips 🎉</title>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Playfair+Display:wght@500&family=Quicksand:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Quicksand', sans-serif;
      background: linear-gradient(135deg, #ff7e5f, #feb47b);
      color: #fff;
      overflow-x: hidden;
      animation: fadeIn 2s ease-in;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    .container {
      max-width: 850px;
      margin: 60px auto;
      background: rgba(255, 255, 255, 0.15);
      padding: 40px;
      border-radius: 25px;
      text-align: center;
      box-shadow: 0px 8px 25px rgba(0, 0, 0, 0.3);
      backdrop-filter: blur(8px);
      position: relative;
      z-index: 2;
      animation: slideUp 1.5s ease-out;
    }

    @keyframes slideUp {
      from { transform: translateY(50px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3em;
      margin-bottom: 0.3em;
      text-shadow: 2px 2px 10px rgba(0,0,0,0.3);
    }

    h2 {
      font-weight: 600;
      font-size: 1.5em;
      margin-bottom: 1.2em;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: #fff8dc;
    }

    p {
      font-size: 1.2em;
      line-height: 1.8;
      margin-bottom: 1em;
    }

    .poem {
      font-style: italic;
      margin-top: 40px;
      background: rgba(255, 255, 255, 0.18);
      padding: 25px;
      border-radius: 15px;
      box-shadow: inset 0 0 20px rgba(255, 255, 255, 0.3);
      animation: glow 3s infinite alternate;
    }

    .poem h3 {
      margin-bottom: 15px;
      font-family: 'Playfair Display', serif;
      font-size: 1.6em;
    }

    @keyframes glow {
      from { box-shadow: inset 0 0 10px rgba(255,255,255,0.2); }
      to { box-shadow: inset 0 0 25px rgba(255,255,255,0.5); }
    }

    /* Signature style */
    .signature {
      margin-top: 50px;
      font-family: 'Great Vibes', cursive;
      font-size: 2.2em;
      color: gold;
      text-shadow: 1px 1px 8px rgba(0,0,0,0.4);
      animation: pulse 2s infinite;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.05); }
      100% { transform: scale(1); }
    }

    /* Floating hearts */
    .heart {
      position: fixed;
      width: 22px;
      height: 22px;
      background: rgba(255,255,255,0.9);
      clip-path: polygon(50% 0%, 61% 10%, 70% 25%, 75% 40%, 74% 55%, 67% 67%, 50% 90%, 33% 67%, 26% 55%, 25% 40%, 30% 25%, 39% 10%);
      animation: float 6s linear infinite;
      z-index: 1;
    }

    @keyframes float {
      0% {
        transform: translateY(100vh) scale(0.8);
        opacity: 0;
      }
      50% {
        opacity: 1;
      }
      100% {
        transform: translateY(-10vh) scale(1.3);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Happy 2nd Anniversary 🎉</h1>
    <h2>BeckySweetChips 🥔✨</h2>

    <p>My Love,</p>
    <p>
      Today, your business turns 2 years old, and my heart is full of pride. I have watched you 
      start with just a dream, and I’ve seen you fight, struggle, and rise above challenges most 
      people would have given up on. You have built something beautiful with your own hands, 
      with your sweat, your sleepless nights, and your unshakable courage.
    </p>
    <p>
      Baby, this 2-year journey is not just about your business. It’s a story of who you are — 
      a strong, powerful, and unstoppable woman. I’m blessed to witness your growth, and I 
      promise I’ll always be here, cheering you on, reminding you how amazing you are, and 
      loving you every step of the way.
    </p>

    <div class="poem">
      <h3>Two Years Strong</h3>
      <p>
        Two years ago, you planted a seed,<br>
        With hope in your heart, and faith you would lead.<br>
        Through trials and tears, you chose not to fall,<br>
        You built a dream, and you gave it your all.<br><br>
        Your journey inspires, your courage shines bright,<br>
        You turn the darkest struggles into light.<br>
        My love, my pride, forever you’ll be,<br>
        A Queen, a fighter, an angel to me.
      </p>
    </div>

    <div class="signature">
      With all my heart,<br>
      Your Loving OLASUNKANMI
    </div>
  </div>

  <!-- floating hearts generator -->
  <script>
    function createHeart() {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = 4 + Math.random() * 4 + "s";
      document.body.appendChild(heart);
      setTimeout(() => {
        heart.remove();
      }, 9000);
    }
    setInterval(createHeart, 500);
  </script>
</body>
</html>

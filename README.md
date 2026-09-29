
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>For You 💙</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Georgia, "Times New Roman", serif;
      background: #07111f;
      color: #f5f7fb;
      overflow-x: hidden;
    }

    /* ---------- BACKGROUND ---------- */

    .stars {
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 0;
      background:
        radial-gradient(circle at 20% 20%, rgba(80,140,255,.18), transparent 25%),
        radial-gradient(circle at 80% 70%, rgba(255,180,80,.10), transparent 25%);
    }

    .stars::before,
    .stars::after {
      content: "";
      position: absolute;
      inset: 0;
      background-image:
        radial-gradient(circle, white 1px, transparent 1px),
        radial-gradient(circle, rgba(255,255,255,.6) 1px, transparent 1px);
      background-size: 80px 80px, 130px 130px;
      background-position: 10px 20px, 50px 70px;
      opacity: .25;
    }

    section {
      position: relative;
      z-index: 1;
      min-height: 100vh;
      padding: 70px 25px;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .container {
      width: 100%;
      max-width: 650px;
      text-align: center;
    }

    /* ---------- HERO ---------- */

    .hero {
      min-height: 100vh;
      flex-direction: column;
    }

    .small-text {
      font-size: 14px;
      letter-spacing: 4px;
      text-transform: uppercase;
      opacity: .65;
      margin-bottom: 25px;
    }

    h1 {
      font-size: clamp(42px, 12vw, 75px);
      font-weight: normal;
      margin-bottom: 25px;
    }

    .gold {
      color: #e8c875;
    }

    .hero p {
      font-size: 19px;
      line-height: 1.8;
      opacity: .8;
    }

    .scroll {
      margin-top: 70px;
      font-size: 13px;
      opacity: .5;
      animation: bounce 2s infinite;
    }

    @keyframes bounce {
      50% {
        transform: translateY(10px);
      }
    }

    /* ---------- STORY ---------- */

    .card {
      background: rgba(255,255,255,.055);
      border: 1px solid rgba(255,255,255,.1);
      border-radius: 24px;
      padding: 35px 25px;
      backdrop-filter: blur(10px);
      box-shadow: 0 20px 60px rgba(0,0,0,.25);
    }

    .card h2 {
      font-size: 32px;
      font-weight: normal;
      margin-bottom: 25px;
    }

    .card p {
      font-size: 17px;
      line-height: 1.9;
      color: rgba(255,255,255,.82);
    }

    /* ---------- MEMORY ---------- */

    .memory {
      margin-top: 30px;
      padding: 22px;
      border-left: 2px solid #e8c875;
      text-align: left;
      background: rgba(255,255,255,.035);
      border-radius: 0 15px 15px 0;
    }

    .memory strong {
      display: block;
      color: #e8c875;
      margin-bottom: 8px;
    }

    /* ---------- REVEAL ---------- */

    .reveal-text {
      font-size: 21px;
      line-height: 1.9;
      margin: 30px 0;
    }

    .heart {
      font-size: 55px;
      animation: heartbeat 1.5s infinite;
      margin-bottom: 25px;
    }

    @keyframes heartbeat {
      0%, 100% {
        transform: scale(1);
      }

      50% {
        transform: scale(1.12);
      }
    }

    /* ---------- FINAL ---------- */

    .final h2 {
      font-size: 40px;
      font-weight: normal;
      margin-bottom: 25px;
    }

    .question {
      font-size: 24px;
      line-height: 1.6;
      margin: 30px 0;
    }

    .buttons {
      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
      margin-top: 35px;
    }

    button {
      border: none;
      padding: 15px 25px;
      border-radius: 50px;
      font-size: 16px;
      cursor: pointer;
      transition: .3s;
    }

    .yes {
      background: #e8c875;
      color: #07111f;
    }

    .yes:hover {
      transform: scale(1.06);
    }

    .think {
      background: rgba(255,255,255,.08);
      color: white;
      border: 1px solid rgba(255,255,255,.15);
    }

    .response {
      margin-top: 30px;
      min-height: 40px;
      font-size: 18px;
      color: #e8c875;
    }

    footer {
      position: relative;
      z-index: 1;
      text-align: center;
      padding: 30px;
      font-size: 12px;
      opacity: .4;
    }

    /* ---------- MOBILE ---------- */

    @media(max-width:500px) {

      section {
        padding: 60px 20px;
      }

      .card {
        padding: 30px 20px;
      }

      .card h2 {
        font-size: 28px;
      }

      .card p {
        font-size: 16px;
      }

      .question {
        font-size: 21px;
      }
    }
  </style>
</head>

<body>

  <div class="stars"></div>

  <!-- HERO -->

  <section class="hero">

    <div class="container">

      <div class="small-text">
        A little something for you
      </div>

      <h1>
        Hey, <span class="gold">Vani...</span>
      </h1>

      <p>
        This isn't a normal webpage.<br>
        And maybe this isn't a normal message either.
      </p>

      <div class="scroll">
        ↓ scroll slowly ↓
      </div>

    </div>

  </section>


  <!-- STORY -->

  <section>

    <div class="container">

      <div class="card">

        <h2>
          How this started...
        </h2>

        <p>
          I still remember the first time I properly noticed you.
          It wasn't some dramatic movie moment.
          It was just a simple moment...
          but somehow, I remembered it.
        </p>

        <div class="memory">

          <strong>One classroom. One laptop. One small moment.</strong>

          And somehow, that small moment became the beginning
          of me noticing you more and more.

        </div>

        <div class="memory">

          <strong>Then came the conversations.</strong>

          Slowly, talking to you became something I genuinely
          looked forward to.

        </div>

      </div>

    </div>

  </section>


  <!-- FEELINGS -->

  <section>

    <div class="container">

      <div class="card">

        <div class="heart">💙</div>

        <h2>
          Somewhere along the way...
        </h2>

        <p class="reveal-text">

          You became someone I genuinely care about.

          <br><br>

          I like talking to you.
          I like knowing more about you.
          I like the person you are.

          <br><br>

          And eventually I realised...

          <br><br>

          <span class="gold">
            I like you.
          </span>

        </p>

      </div>

    </div>

  </section>


  <!-- IMPORTANT MESSAGE -->

  <section>

    <div class="container">

      <div class="card">

        <h2>
          But there's something important...
        </h2>

        <p>

          I'm not making this page because I expect
          you to give me an answer immediately.

          <br><br>

          I just wanted you to know what I feel.

          <br><br>

          You don't have to say anything just because
          I made this.

          <br><br>

          Take your time.
          Be honest.
          Be yourself.

        </p>

      </div>

    </div>

  </section>


  <!-- FINAL QUESTION -->

  <section class="final">

    <div class="container">

      <div class="card">

        <div class="heart">💙</div>

        <h2>
          So...
        </h2>

        <p class="question">

          Would you like to give
          <br>
          <span class="gold">us</span>
          a chance?

        </p>

        <p>
          Whatever your answer is,
          I'll respect it.
        </p>

        <div class="buttons">

          <button class="yes" onclick="sayYes()">
            Yes ❤️
          </button>

          <button class="think" onclick="takeTime()">
            Let me think 🌸
          </button>

        </div>

        <div class="response" id="response"></div>

      </div>

    </div>

  </section>


  <footer>
    Made with honesty, not pressure. 💙
  </footer>


  <script>

    function sayYes() {

      document.getElementById("response").innerHTML =
        "Then maybe this is the beginning of something beautiful. 💙";

    }

    function takeTime() {

      document.getElementById("response").innerHTML =
        "Take all the time you need. I'll be happy to hear from you whenever you're ready. 🌸";

    }

  </script>

</body>
</html>
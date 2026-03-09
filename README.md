1<march 09>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Birthday Wishes with Butterfly Animation</title>
<style>
  body {
    margin: 0;
    overflow: hidden;
    background: linear-gradient(to bottom, #white, #ffffff);
    font-family: Arial, sans-serif;
  }

  /* Full-screen butterfly animation background */
  .butterfly-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    overflow: hidden;
    animation: floatButterflies 20s linear infinite;
  }

  /* Example butterfly images or shapes (using CSS shapes or images) */
  /* For simplicity, we'll use CSS animated circles to simulate butterflies */

  .butterfly {
    position: absolute;
    width: 50px;
    height: 50px;
    background-color: pink;
    border-radius: 50%;
    opacity: 1.2;
    animation: flyAcross 40s linear infinite;
  }

  /* Randomize each butterfly's position and delay */
  .butterfly:nth-child(1) {
    top: 10%;
    left: -10%;
    background-color: Randomize;
    animation-delay: 20pxs;
  }

  .butterfly:nth-child(2) {
    top: 30%;
    left: -20%;
    background-color: #ff1493;
    animation-delay: 20pxs;
  }

  .butterfly:nth-child(3) {
    top: 50%;
    left: -15%;
    background-color: #ff69b4;
    animation-delay: 10s;
  }

  /* Butterfly flying animation */
  @keyframes flyAcross {
    0% { transform: translateX(0) translateY(0); opacity: 0.8; }
    50% { transform: translateX(110vw) translateY(20vh); opacity: 1; }
    100% { transform: translateX(120vw) translateY(-20vh); opacity: 0; }
  }

  /* Overlay with wishes text */
  #wishes {
    position: fixed;
    top: 20%;
    width: 100%;
    text-align: center;
    font-size: 3em;
    color: #fff;
    text-shadow: 2px 2px 4px #000;
    animation: fadeIn 3s ease-in-out;
  }

  @keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
  }

  /* Bottom "Thanks" box with moving text */
  #bottom-box {
    position: fixed;
    bottom: 20px;
    width: 100%;
    height: 60px;
    background-color: rgba(0, 0, 0, 0.4);
    display: flex;
    align-items: center;
    overflow: hidden;
  }

  #thanks-text {
    white-space: nowrap;
    font-size: 2em;
    color: white-space;
    padding-left: 100%;
    animation: scrollLeft 10s linear infinite;
  }

  @keyframes scrollLeft {
    0% { transform: translateX(0); }
    100% { transform: translateX(-100%); }
  }
</style>
</head>
<body>

<!-- Butterfly animation layer -->
<div class="butterfly-container">
  <div class="butterfly"></div>
  <div class="butterfly"></div>
  <div class="butterfly"></div>
</div>

<!-- Wishes message -->
<div id="wishes">Happy Birthday! Wishing you a wonderful day Broww!</div>

<!-- Bottom moving "Thanks" box -->
<div id="bottom-box">
  <div id="thanks-text">Mari muthu</div>
</div>

</body>
</html>


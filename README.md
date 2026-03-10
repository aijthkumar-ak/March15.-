<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Happy Birthday Wishes</title>
<style>
  /* Reset and basic styles */
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    background: linear-gradient(135deg, #ffe6f0, #ffe6e6);
    font-family: 'Arial', sans-serif;
    overflow: hidden;
    height: 100vh;
    width: 100vw;
  }

  /* Full screen message */
  .container {
    position: relative;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 20px;
    z-index: 2;
  }

  h1 {
    font-size: 3em;
    color: #d6336c;
    margin-bottom: 20px;
    text-shadow: 2px 2px 4px #fff;
  }

  /* Butterfly styles */
  .butterfly {
    position: absolute;
    width: 60px;
    height: 60px;
    background-image: url('https://i.imgur.com/6V0T0sL.png'); /* Butterfly image URL, replace if needed */
    background-size: contain;
    background-repeat: no-repeat;
    animation: flyAround 20s linear infinite;
  }

  @keyframes flyAround {
    0% {
      transform: translate(0, 0) scale(1);
    }
    25% {
      transform: translate(80vw, 10vh) scale(1.2);
    }
    50% {
      transform: translate(0, 80vh) scale(1);
    }
    75% {
      transform: translate(-80vw, 10vh) scale(0.8);
    }
    100% {
      transform: translate(0, 0) scale(1);
    }
  }

  /* Love balloon styles */
  .balloon {
    position: absolute;
    width: 50px;
    height: 70px;
    background-image: url('https://i.imgur.com/6R0L8L2.png'); /* Balloon image URL, replace if needed */
    background-size: contain;
    background-repeat: no-repeat;
    animation: floatUp 15s ease-in-out infinite;
  }

  @keyframes floatUp {
    0% {
      transform: translateY(100vh) scale(0.8);
      opacity: 0;
    }
    10% {
      opacity: 1;
    }
    100% {
      transform: translateY(-10vh) scale(1);
      opacity: 0;
    }
  }

  /* Slideshow styles */
  .slideshow {
    position: absolute;
    bottom: 20px;
    width: 80%;
    max-width: 800px;
    height: 200px;
    overflow: hidden;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    z-index: 2;
  }

  .slides {
    display: flex;
    width: calc(100% * 5); /* 5 slides */
    animation: slide 20s infinite linear;
  }

  .slide {
    flex: 1 0 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.8em;
    background-color: rgba(255,255,255,0.8);
    padding: 20px;
    box-shadow: inset 0 0 10px rgba(0,0,0,0.1);
  }

  @keyframes slide {
    0% { transform: translateX(0); }
    20% { transform: translateX(0); }
    25% { transform: translateX(-100%); }
    45% { transform: translateX(-100%); }
    50% { transform: translateX(-200%); }
    70% { transform: translateX(-200%); }
    75% { transform: translateX(-300%); }
    95% { transform: translateX(-300%); }
    100% { transform: translateX(0); }
  }

</style>
</head>
<body>

<div class="container">
  <h1>Happy Birthday!</h1>
</div>

<!-- Butterflies -->
<div class="butterfly" style="top:10%; left:5%; animation-delay: 0s;"></div>
<div class="butterfly" style="top:20%; left:80%; animation-delay: 5s; animation-duration: 25s;"></div>
<div class="butterfly" style="top:70%; left:10%; animation-delay: 10s; animation-duration: 30s;"></div>
<div class="butterfly" style="top:50%; left:50%; animation-delay: 15s; animation-duration: 20s;"></div>

<!-- Love balloons -->
<div class="balloon" style="bottom:10%; left:10%; background-image: url('https://i.imgur.com/4BJ8IW1.png'); animation-delay: 0s;"></div>
<div class="balloon" style="bottom:15%; left:70%; background-image: url('https://i.imgur.com/4BJ8IW1.png'); animation-delay: 3s;"></div>
<div class="balloon" style="bottom:20%; left:30%; background-image: url('https://i.imgur.com/4BJ8IW1.png'); animation-delay: 6s;"></div>
<div class="balloon" style="bottom:12%; left:55%; background-image: url('https://i.imgur.com/4BJ8IW1.png'); animation-delay: 9s;"></div>

<!-- Slideshow -->
<div class="slideshow">
  <div class="slides">
    <div class="slide">Wishing You a Day Filled with Love & Happiness!</div>
    <div class="slide">May All Your Dreams Come True!</div>
    <div class="slide">Have a Wonderful Birthday!</div>
    <div class="slide">Celebrate and Make Memories!</div>
    <div class="slide">Enjoy Your Special Day!</div>
  </div>
</div>

</body>
</html>

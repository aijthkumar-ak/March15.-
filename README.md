<>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Birthday Wishes</title>
<style>
  body {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100vh;
    margin: 30;
    font-family: Arial, sans-serif;
  }
  #top {
    text-align: center;
    padding: 20px;
    font-size: 66px;
    height: 150px;
  }
  #bottom {
    text-align: center;
    padding: 20px;
    font-size: 20px;
    background-color🤸‍♂️;
  }
</style>
</head>
<body>

<div id="Top">
  <span id="wish"></span>
</div>

<div id="bottom">
  Happiest Day sowmi
</div>

<script>
  const wishes = [
    "🎀Happy Birthday Sowmiiiiiyaa💖!",
    "📍Wishing you a wonderful year a head!🎁",
    "Many happy returns of the Day🎀!",
    "💭Enjoy your special day!",
    "Cheers to you another Year!",
    " ✨💕Marakkamaa Arrkadu Briyani Vangii Koduuu!😁😁"
  ];

  let currentIndex = 0;
  const wishElement = document.getElementById('wish');

  function showNextWish() {
    wishElement.textContent = wishes[currentIndex];
    currentIndex = (currentIndex + 1) % wishes.length;
  }

  // Rotate wishes every 2 seconds
  setInterval(showNextWish, 2000);

  // Show the first wish immediately
  showNextWish();
</script>

</body>
</html>

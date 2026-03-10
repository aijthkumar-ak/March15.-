<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Happy Birthday Animation</title>
<style>
  /* Reset and full layout */
  body {
    margin: 0;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    background-color: #ffe6e6;
    font-family: Arial, sans-serif;
    overflow: hidden;
  }

  /* Animated "Happy Birthday" text at top */
  .happy-birthday {
    font-size: 2em;
    color: #ff69b4;
    animation: bounce 2s infinite alternate;
    margin-top: 20px;
  }

  /* Center area for any other content if needed */
  .center {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  /* Butterfly at bottom */
  .butterfly {
    font-size: 5em;
    /* Optional: add some animation to the butterfly */
    animation: flutter 3s infinite alternate ease-in-out;
  }

  /* Moving "Thanks" text at bottom, moving up and down */
  .thanks {
    font-size: 2em;
    color: #ff69b4;
    animation: moveUpDown 2s infinite ease-in-out;
    margin-bottom: 20px;
  }

  /* Animations */

  @keyframes bounce {
    0% { transform: translateY(0); }
    100% { transform: translateY(-10px); }
  }

  @keyframes moveUpDown {
    0% { transform: translateY(0); }
    50% { transform: translateY(-20px); }
    100% { transform: translateY(0); }
  }

  @keyframes flutter {
    0% { transform: rotate(0deg); }
    50% { transform: rotate(10deg); }
    100% { transform: rotate(-10deg); }
  }
</style>
</head>
<body>

  <!-- Top animated "Happy Birthday" -->
  <div class="happy-birthday">Happy Birthday</div>

  <!-- Optional center content -->
  <div class="center"></div>

  <!-- Bottom butterfly -->
  <div class="butterfly">🦋</div>

  <!-- "Thanks" moving up and down -->
  <div class="thanks">Thanks</div>

</body>
</html>

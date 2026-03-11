<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Birthday Love Animation</title>

<style>

body{
  margin:0;
  height:100vh;
  display:flex;
  flex-direction:column;
  justify-content:space-between;
  align-items:center;
  background:#fff0f5;
  font-family:Arial, sans-serif;
  text-align:center;
}

/* Top Birthday Text */
.top-text{
  font-size:40px;
  color:#ff1493;
  margin-top:20px;
  font-weight:bold;
}

/* Heart Animation */
.heart{
  position:relative;
  width:100px;
  height:100px;
  background:red;
  transform:rotate(-45deg);
  animation:pulse 1.5s infinite;
}

.heart:before,
.heart:after{
  content:"";
  position:absolute;
  width:100px;
  height:100px;
  background:red;
  border-radius:50%;
}

.heart:before{
  top:-50px;
  left:0;
}

.heart:after{
  left:50px;
  top:0;
}

/* Pulse Animation */
@keyframes pulse{
  0%,100%{ transform:rotate(-45deg) scale(1); }
  50%{ transform:rotate(-45deg) scale(1.2); }
}

/* Bottom Moving Message Box */
.message-box{
  background:white;
  padding:15px 30px;
  border-radius:20px;
  box-shadow:0 0 10px rgba(0,0,0,0.2);
  margin-bottom:40px;
  font-size:20px;
  color:#ff1493;
  animation:moveMsg 2s infinite alternate;
}

/* Move up and down */
@keyframes moveMsg{
  from{ transform:translateY(0); }
  to{ transform:translateY(-20px); }
}

</style>
</head>

<body>

<div class="top-text">🎉 Happy Birthday 🎉</div>

<div class="heart"></div>

<div class="message-box">Hi 💖</div>

</body>
</html>

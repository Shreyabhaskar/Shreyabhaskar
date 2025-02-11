<!DOCTYPE html>
<html>
<head>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');
    body {
      background-color: black;
      color: #00ff00;
      font-family: 'Press Start 2P', cursive;
      text-align: center;
    }
    .container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .avatar {
      width: 100px;
      height: 100px;
      background: url('https://api.dicebear.com/7.x/pixel-art/svg?seed=Shreya') no-repeat center;
      background-size: cover;
      border: 4px solid #00ff00;
      border-radius: 10px;
      margin-bottom: 20px;
    }
    .typewriter {
      overflow: hidden;
      border-right: 4px solid #00ff00;
      white-space: nowrap;
      width: 20ch;
      animation: typing 3s steps(20, end) forwards, blink 0.5s infinite;
    }
    @keyframes typing {
      from { width: 0; }
      to { width: 20ch; }
    }
    @keyframes blink {
      50% { border-color: transparent; }
    }
    .lights {
      display: flex;
      gap: 10px;
      margin-top: 20px;
    }
    .light {
      width: 10px;
      height: 10px;
      background-color: red;
      border-radius: 50%;
      animation: flicker 1s infinite alternate;
    }
    .light:nth-child(2) { animation-delay: 0.2s; background-color: yellow; }
    .light:nth-child(3) { animation-delay: 0.4s; background-color: cyan; }
    .light:nth-child(4) { animation-delay: 0.6s; background-color: magenta; }
    .light:nth-child(5) { animation-delay: 0.8s; background-color: lime; }
    @keyframes flicker {
      0% { opacity: 0.3; }
      100% { opacity: 1; }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="avatar"></div>
    <div class="typewriter">Hello! I'm Shreya Bhaskar 🚀</div>
    <div class="lights">
      <div class="light"></div>
      <div class="light"></div>
      <div class="light"></div>
      <div class="light"></div>
      <div class="light"></div>
    </div>
  </div>
</body>
</html>

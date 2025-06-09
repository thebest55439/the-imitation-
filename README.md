<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .container {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      padding: 20px;
    }
    .image-box {
      text-align: center;
    }
    .t-rex {
      filter: grayscale(100%) brightness(150%);
      transform: rotate(10deg);
      box-shadow: 0 0 10px #00ff00, 0 0 20px #00ff00;
    }
    .stage {
      filter: sepia(60%) contrast(120%);
      position: relative;
    }
    .stage::after {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: radial-gradient(circle, transparent 50%, rgba(0, 0, 0, 0.5) 100%);
      pointer-events: none;
    }
    .penguins {
      filter: blur(2px) hue-rotate(90deg);
      border: 5px solid #fff;
    }
    .seagull {
      filter: drop-shadow(5px 5px 5px #000);
      transform: scale(1.2);
      transition: transform 0.3s;
    }
    .football-field {
      position: relative;
      filter: brightness(120%) saturate(150%);
    }
    .football-field img.tic-tac-toe {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 50%;
      opacity: 0.7;
      filter: hue-rotate(180deg);
    }
    .butterfly {
      filter: contrast(150%) hue-rotate(-30deg);
      box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.5);
      border-radius: 10px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="image-box">
      <img src="dinosaur.png" alt="dinosaur.png" class="dinosaur.png">
    </div>
    <div class="image-box">
      <img src="theater_stage.jpg" alt="theater_stage.jpg" class="theater_stage.jpg">
    </div>
    <div class="image-box">
      <img src="penguins.jpg" alt="Penguins" class="penguins">
    </div>
    <div class="image-box">
      <img src="seagull.png" alt="Seagull" class="seagull">
    </div>
    <div class="image-box">
      <img src="football_field.jpg" alt="Football Field" class="football-field">
      <img src="tic-tac-toe.png" alt="Tic Tac Toe" class="tic-tac-toe">
    </div>
    <div class="image-box">
      <img src="butterfly.jpg" alt="Butterfly" class="butterfly">
    </div>
  </div>
</body>
</html>

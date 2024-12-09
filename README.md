<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Score Counter</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #f3f3f3;
    }

    .score-counter {
      position: absolute;
      top: 10px;
      right: 10px;
      font-size: 24px;
      background: #333;
      color: #fff;
      padding: 5px 10px;
      border-radius: 5px;
    }

    button {
      font-size: 20px;
      padding: 10px 20px;
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <div class="score-counter">Score: <span id="score">0</span></div>
  <button id="pressMeButton" onclick="increaseScore()">Press Me</button>

  <script>
    let score = 0;

    function increaseScore() {
      score += 1;
      document.getElementById('score').textContent = score;
    }
  </script>
</body>
</html>

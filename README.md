# Des-will-u
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Ruth, Will You Be My Girlfriend?</title>
  <style>
    body {
      background: linear-gradient(135deg, #ffe6f0, #ffcccc);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      text-align: center;
      color: #333;
      margin: 0;
      padding: 0;
    }

    .container {
      padding: 60px 20px;
      max-width: 700px;
      margin: auto;
    }

    h1 {
      font-size: 3em;
      margin-bottom: 20px;
    }

    p {
      font-size: 1.5em;
      margin-bottom: 30px;
    }

    .heart {
      font-size: 80px;
      color: red;
      animation: beat 1s infinite;
    }

    @keyframes beat {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }

    .btn-yes, .btn-no {
      padding: 15px 30px;
      margin: 15px;
      font-size: 1.2em;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .btn-yes {
      background-color: #ff4d88;
      color: white;
    }

    .btn-no {
      background-color: #ccc;
      color: #333;
    }

    .btn-yes:hover {
      background-color: #e6005c;
    }

    .btn-no:hover {
      background-color: #aaa;
    }

    .response {
      font-size: 1.6em;
      margin-top: 30px;
      display: none;
    }
  </style>
</head>
<body>

  <div class="container">
    <div class="heart">❤️</div>
    <h1>Hi Ruth Deseree Ruelo</h1>
    <p>Will you make me the happiest person alive<br>and be my girlfriend?</p>
    <button class="btn-yes" onclick="answerYes()">Yes 💘</button>
    <button class="btn-no" onclick="answerNo()">No 😢</button>

    <div class="response" id="response"></div>
  </div>

  <script>
    function answerYes() {
      document.getElementById("response").style.display = "block";
      document.getElementById("response").innerHTML = "YAY! 💖 You just made my heart explode with happiness!";
    }

    function answerNo() {
      document.getElementById("response").style.display = "block";
      document.getElementById("response").innerHTML = "Oh no 😭 I still think you're amazing, Ruth.";
    }
  </script>

</body>
</html>

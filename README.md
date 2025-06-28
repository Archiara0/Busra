<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Barışalım mı? ❤️</title>
  <style>
    body {
      text-align: center;
      font-family: 'Comic Sans MS', sans-serif;
      background-color: #ffe6e6;
      padding-top: 100px;
    }

    h1 {
      font-size: 32px;
      color: #c2185b;
    }

    button {
      font-size: 20px;
      padding: 10px 20px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      margin: 20px;
      transition: 0.3s;
    }

    #yesBtn {
      background-color: #4caf50;
      color: white;
    }

    #noBtn {
      background-color: #f44336;
      color: white;
      position: absolute;
    }
  </style>
</head>
<body>

  <h1>Benimle barışır mısın? ❤️</h1>

  <button id="yesBtn" onclick="yesClicked()">Evet</button>
  <button id="noBtn" onmouseover="moveButton()">Hayır</button>

  <script>
    function moveButton() {
      const button = document.getElementById('noBtn');
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 100);
      button.style.left = `${x}px`;
      button.style.top = `${y}px`;
    }

    function yesClicked() {
      document.body.innerHTML = "<h1>Yaşasın! ❤️ Barıştık!</h1>";
    }
  </script>

</body>
</html>

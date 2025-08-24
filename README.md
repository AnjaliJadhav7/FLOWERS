<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Flower Greeting Card</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(to top, #ca6bfa, #ee9ca7);
      overflow: hidden;
      font-family: "Segoe UI", sans-serif;
    }
    h1 {
      color: white;
      font-size: 2em;
      text-shadow: 2px 2px 6px black;
      position: relative;
      z-index: 10;
      text-align: center;
    }
    .flower {
      position: absolute;
      font-size: 1em;
      animation: fall linear infinite;
    }
    @keyframes fall {
      from { transform: translateY(-10vh) rotate(0deg); }
      to { transform: translateY(110vh) rotate(360deg); }
    }
  </style>
</head>
<body>
  <h1>🪻 FLOWER APOLOGIZING PAGE🌼<br> 🌷Sorry for not giving the chapter earlier, my flowers 🌸.</h1>

  <script>
    function createFlower() {
      const flower = document.createElement("div");
      flower.classList.add("flower");
      flower.innerHTML = ["🌸","🌺","🌻","🌹","🌷"][Math.floor(Math.random()*5)];
      flower.style.left = Math.random() * 100 + "vw";
      flower.style.animationDuration = (Math.random() * 3 + 3) + "s";
      document.body.appendChild(flower);

      setTimeout(() => { flower.remove(); }, 6000);
    }
    setInterval(createFlower, 300);
  </script>
</body>
</html>
    

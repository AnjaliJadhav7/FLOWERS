
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Flower Apologizing Page 🌸</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      background: linear-gradient(to bottom right, #ff9a9e, #fad0c4, #fad0c4, #fbc2eb);
      font-family: Arial, sans-serif;
      overflow: hidden;
    }

    h1 {
      font-size: 2.5rem;
      color: white;
      text-shadow: 2px 2px 6px #000;
      margin-bottom: 20px;
    }

    p {
      font-size: 1.5rem;
      color: #fff;
      text-shadow: 1px 1px 5px #000;
    }

    /* Floating flowers */
    .flower {
      position: absolute;
      font-size: 1.5rem;
      animation: float 10s linear infinite;
    }

    @keyframes float {
      from { transform: translateY(100vh); opacity: 1; }
      to { transform: translateY(-10vh); opacity: 0.8; }
    }
  </style>
</head>
<body>
  <div>
    <h1>🪻 Flower Apologizing Page 🌸</h1>
    <p>🌷 Sorry for not giving the chapter earlier, my flowers 🌺</p>
  </div>

  <script>
    const emojis = ["🌹","🌷","🌸","🌼","💮","🌻","🌺"];
    for (let i = 0; i < 30; i++) {
      let flower = document.createElement("div");
      flower.className = "flower";
      flower.innerHTML = emojis[Math.floor(Math.random() * emojis.length)];
      flower.style.left = Math.random() * 100 + "vw";
      flower.style.animationDuration = (Math.random() * 5 + 5) + "s";
      flower.style.fontSize = (Math.random() * 20 + 20) + "px";
      document.body.appendChild(flower);
    }
  </script>
</body>
</html>

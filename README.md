# Samir
valentine.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Be My Valentine 💘</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #ff4d6d, #ffb3c6);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Segoe UI', sans-serif;
      color: #fff;
    }

    .card {
      background: rgba(255, 255, 255, 0.15);
      padding: 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 20px 40px rgba(0,0,0,0.2);
      width: 320px;
    }

    h1 {
      margin-bottom: 10px;
      font-size: 28px;
    }

    p {
      font-size: 18px;
      margin-bottom: 30px;
    }

    .buttons {
      position: relative;
      height: 80px;
    }

    button {
      padding: 12px 28px;
      border: none;
      border-radius: 30px;
      font-size: 16px;
      cursor: pointer;
      transition: 0.2s ease;
    }

    #yesBtn {
      background: #ff1e56;
      color: white;
      margin-right: 10px;
    }

    #yesBtn:hover {
      background: #e6003f;
    }

    #noBtn {
      background: #ffc2d1;
      color: #a1002d;
      position: absolute;
    }

    .love {
      font-size: 22px;
      margin-top: 20px;
      display: none;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Hey Samir 💖</h1>
    <p>Will you be my Valentine?</p>

    <div class="buttons">
      <button id="yesBtn" onclick="yesClicked()">Yes 💕</button>
      <button id="noBtn">No 🙈</button>
    </div>

    <div class="love" id="loveMsg">
      Yayyy! 💘 I knew you’d say yes 😍
    </div>
  </div>

  <script>
    const noBtn = document.getElementById("noBtn");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 60 - 30;
      noBtn.style.transform = `translate(${x}px, ${y}px)`;
    });

    function yesClicked() {
      document.getElementById("loveMsg").style.display = "block";
    }
  </script>

</body>
</html>


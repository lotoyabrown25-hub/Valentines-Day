index.html
<!DOCTYPE html>
<html>
<head>
  <title>Lance, Be My Valentine? 💖</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      background: linear-gradient(to right, #ff758c, #ff7eb3);
      height: 100vh;
      overflow: hidden;
      color: white;
    }

    h1 {
      margin-top: 100px;
      font-size: 38px;
    }

    button {
      padding: 15px 30px;
      font-size: 20px;
      border: none;
      border-radius: 12px;
      cursor: pointer;
      margin: 20px;
      transition: 0.3s;
    }

    #yesBtn {
      background-color: white;
      color: #ff4d6d;
      font-weight: bold;
    }

    #noBtn {
      background-color: #ff4d6d;
      color: white;
      position: absolute;
    }

    #message {
      font-size: 28px;
      margin-top: 40px;
      font-weight: bold;
    }
  </style>
</head>

<body>

<h1>Alanzo 💕 (aka my Lance 🥰)<br><br>
Will you be my Valentine? 💘</h1>

<button id="yesBtn">YES OF COURSE 😍</button>
<button id="noBtn">No 😢</button>

<div id="message"></div>

<script>
  const noBtn = document.getElementById("noBtn");
  const yesBtn = document.getElementById("yesBtn");
  const message = document.getElementById("message");

  noBtn.addEventListener("mouseover", function() {
    const x = Math.random() * (window.innerWidth - 100);
    const y = Math.random() * (window.innerHeight - 100);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
  });

  yesBtn.addEventListener("click", function() {
    message.innerHTML = "YAYYYY LANCE!!! 💖🥹 You just made me the happiest girlfriend ever! I love you so much! 💕💋";
  });
</script>

</body>
</html>

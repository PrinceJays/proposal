<!DOCTYPE html>
<html>
<head>
  <title>Letter for My Budi ❤️</title>
  <style>
    body {
      background: linear-gradient(to right, #ffafbd, #ffc3a0);
      font-family: 'Georgia', serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      text-align: center;
      color: #4b0082;
      padding: 20px;
    }

    #letterBox {
      background: rgba(255,255,255,0.8);
      padding: 30px;
      border-radius: 15px;
      width: 90%;
      max-width: 500px;
      box-shadow: 0 0 20px rgba(0,0,0,0.2);
    }

    button {
      padding: 10px 20px;
      font-size: 18px;
      margin-top: 20px;
      border-radius: 8px;
      border: none;
      cursor: pointer;
      background-color: #ff4d6d;
      color: white;
    }
  </style>
</head>
<body>

<div id="letterBox">
  <div id="pageText">Dear Iksha budu,<br><br>Do you know someone is thinking of you right now? 😌</div>
  <button id="nextBtn">Next ❤️</button>
</div>

<script>
  const pages = [
    "Since the day we started talking i found my wife that day, you became my wifey for my whole life .",
    "Every moment with you feels like need more time to spend with you always in my entire life …",
    "I realized something very important…",
    "My Budi, Iksha Thamsang, will you be my velentine forever in my entire life? 💍❤️"
  ];

  let currentPage = 0;
  const pageText = document.getElementById("pageText");
  const nextBtn = document.getElementById("nextBtn");

  nextBtn.addEventListener("click", () => {
    if (currentPage < pages.length) {
      pageText.innerHTML = pages[currentPage];
      currentPage++;
      if (currentPage === pages.length) {
        nextBtn.innerText = "YES 💖";
        nextBtn.onclick = () => {
          alert("She said YES! 💍🎉 My Budi ❤️");
        };
      }
    }
  });
</script>

</body>
</html>

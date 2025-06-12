# 5-Tl
İlk Ozel oyun 
<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no" />
<title>5 TL Oyun</title>
<style>
  body {
    margin: 0; padding: 0; font-family: Arial, sans-serif; background: linear-gradient(135deg, #74ebd5, #ACB6E5);
    display: flex; flex-direction: column; align-items: center; justify-content: center; height: 100vh;
    user-select: none;
  }
  #game-container {
    background: white; border-radius: 15px; box-shadow: 0 4px 15px rgba(0,0,0,0.2);
    width: 320px; max-width: 90vw; padding: 20px; text-align: center;
  }
  #money-img {
    width: 150px; cursor: pointer;
  }
  button {
    margin: 10px; padding: 10px 20px; font-size: 1rem; border-radius: 10px;
    border: none; background: #4CAF50; color: white; cursor: pointer;
  }
  button:active {
    background: #388E3C;
  }
  #message {
    margin-top: 15px; font-size: 1.2rem; color: #333;
  }
</style>
</head>
<body>

<div id="game-container">
  <img id="money-img" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/33/TL5_2019.png/220px-TL5_2019.png" alt="5 TL" />
  <div>
    <button id="mini1">Mini Oyun 1</button>
    <button id="mini2">Mini Oyun 2</button>
    <button id="mini3">Mini Oyun 3</button>
    <button id="mini4">Mini Oyun 4</button>
    <button id="mini5">Mini Oyun 5</button>
  </div>
  <div id="message">Tıklayın ve mini oyunlardan birini seçin!</div>
</div>

<audio id="click-sound" src="https://actions.google.com/sounds/v1/cartoon/clang_and_wobble.ogg"></audio>

<script>
  const moneyImg = document.getElementById('money-img');
  const message = document.getElementById('message');
  const clickSound = document.getElementById('click-sound');

  moneyImg.addEventListener('click', () => {
    clickSound.play();
    message.textContent = "5 TL'ye tıkladınız!";
  });

  // Mini oyunlar örneği - basit alert mesajları
  document.getElementById('mini1').addEventListener('click', () => {
    alert('Mini Oyun 1: Hızlı Tıklama!');
  });
  document.getElementById('mini2').addEventListener('click', () => {
    alert('Mini Oyun 2: Sayı Tahmin Et!');
  });
  document.getElementById('mini3').addEventListener('click', () => {
    alert('Mini Oyun 3: Hafıza Oyunu!');
  });
  document.getElementById('mini4').addEventListener('click', () => {
    alert('Mini Oyun 4: Renk Eşleştir!');
  });
  document.getElementById('mini5').addEventListener('click', () => {
    alert('Mini Oyun 5: Labirent!');
  });
</script>

</body>
</html>

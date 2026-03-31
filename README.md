***Welcome to My Corner of the World***🧭  
Contact me📮: 3870045464@qq.com

### Birdwatching Section
![照片描述](小天鹅.JPG)
*A Small Swan I took in Minjiang Wetland Park*

### ACGN Section
![照片描述](塑心壁纸1.png)
*My favorite ACGN character - Virtuosa from Arknights*

### Small Games  
<br>
<br>
<hr>
<div align="center">
  <h3>🎉 猜数字小游戏 🎉</h3>
  <p>我想了一个 1 到 100 之间的数字，你能猜出来吗？</p>
  <input type="number" id="guessInput" min="1" max="100" placeholder="输入你的猜测">
  <button onclick="checkGuess()">猜一下！</button>
  <p id="message" style="margin-top: 10px; font-weight: bold;"></p>
  <button onclick="resetGame()" style="display: none; background-color: #f44336; color: white; padding: 8px 15px; border: none; border-radius: 4px; cursor: pointer;">再玩一次</button>
</div>

<script>
  let randomNumber = Math.floor(Math.random() * 100) + 1;
  let attempts = 0;
  const guessInput = document.getElementById('guessInput');
  const message = document.getElementById('message');
  const resetButton = document.querySelector('.reset-button'); // 使用类选择器

  // 将 resetGame 按钮的 id 修改为类，并将其赋值给 resetButton
  document.querySelector('button[onclick="resetGame()"]').classList.add('reset-button');

  function checkGuess() {
    const userGuess = Number(guessInput.value);
    attempts++;

    if (isNaN(userGuess) || userGuess < 1 || userGuess > 100) {
      message.textContent = '请输入 1 到 100 之间的一个有效数字！';
      return;
    }

    if (userGuess === randomNumber) {
      message.textContent = `恭喜你！你在 ${attempts} 次尝试后猜对了数字 ${randomNumber}！`;
      message.style.color = 'green';
      guessInput.disabled = true;
      document.querySelector('button[onclick="checkGuess()"]').disabled = true;
      document.querySelector('.reset-button').style.display = 'inline-block';
    } else if (userGuess < randomNumber) {
      message.textContent = '太小了！再猜大一点。';
      message.style.color = 'orange';
    } else {
      message.textContent = '太大了！再猜小一点。';
      message.style.color = 'orange';
    }
  }

  function resetGame() {
    randomNumber = Math.floor(Math.random() * 100) + 1;
    attempts = 0;
    message.textContent = '';
    message.style.color = 'black';
    guessInput.value = '';
    guessInput.disabled = false;
    document.querySelector('button[onclick="checkGuess()"]').disabled = false;
    document.querySelector('.reset-button').style.display = 'none';
  }
</script>
<br>
<hr>

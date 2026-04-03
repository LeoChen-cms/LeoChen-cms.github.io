***Welcome to My Corner of the World***🧭  
Contact me📮: 3870045464@qq.com

### Birdwatching Section

**2026/01/21 中国，福建，福州，马尾闽江滨**

---

**2026/01/23 中国，福建，福州，森林公园与塔礁洲湿地**

---

**2026/01/25 中国，福建省，福州，连江，山堂村**

![北红尾鸲](北红尾鸲.JPG)  
*&nbsp;&nbsp;Daurian Redstart; Phoenicurus auroreus; 北红尾鸲*
<br><br>

![树麻雀](树麻雀.JPG)  
*&nbsp;&nbsp;Eurasian Tree Sparrow; Passer montanus; 树麻雀*
<br><br>

![棕背伯劳](棕背伯劳.JPG)  
*&nbsp;&nbsp;Long-tailed Shrike; Lanius schach; 棕背伯劳*
<br><br>

![牛背鹭](牛背鹭.JPG)  
*&nbsp;&nbsp;Cattle Egret; Bubulcus ibis; 牛背鹭*
<br><br>

![白鹤](白鹤.JPG)  
*&nbsp;&nbsp;Siberian Crane; Grus leucogeranus; 白鹤*
<br><br>

![黑喉石鵖](<黑喉石鵖 (2).JPG>)  
*&nbsp;&nbsp;Common Stonechat; Saxicola torquata; 黑喉石鵖*
<br><br>

---

**2026/02/07-08 中国，福建，福州，兴化湾与闽江湿地保护区**


### ACGN Section
![塑心壁纸](塑心壁纸1.png)
*My favorite ACGN character - Virtuosa from Arknights*

### Small Games  
<br>
<hr>
<div align="center" style="padding: 20px; background-color: #f9f9f9; border-radius: 10px;">
  <h3 style="color: #2a7ae2;">🎉 猜数字小游戏 🎉</h3>
  <p>我想了一个 1 到 100 之间的数字，你能猜出来吗？</p>
  
  <input type="number" id="guessInput" min="1" max="100" placeholder="1-100" 
         style="width: 100px; padding: 10px; margin: 10px; border: 1px solid #ccc; border-radius: 5px;">
  
  <button onclick="checkGuess()" 
          style="padding: 10px 20px; background-color: #2a7ae2; color: white; border: none; border-radius: 5px; cursor: pointer;">
    猜一下！
  </button>
  
  <p id="message" style="margin-top: 15px; font-weight: bold; min-height: 24px;"></p>
  
  <button id="resetBtn" onclick="resetGame()" 
          style="display: none; background-color: #f44336; color: white; padding: 10px 20px; border: none; border-radius: 5px; cursor: pointer;">
    再玩一次
  </button>
</div>

<script>
  let randomNumber = Math.floor(Math.random() * 100) + 1;
  let attempts = 0;

  function checkGuess() {
    const input = document.getElementById('guessInput');
    const msg = document.getElementById('message');
    const resetBtn = document.getElementById('resetBtn');
    const userGuess = Number(input.value);
    attempts++;

    if (!input.value || userGuess < 1 || userGuess > 100) {
      msg.textContent = '请输入 1-100 的数字！';
      msg.style.color = 'red';
      return;
    }

    if (userGuess === randomNumber) {
      msg.textContent = `🎊 猜对了！答案是 ${randomNumber}，用了 ${attempts} 次。`;
      msg.style.color = 'green';
      input.disabled = true;
      resetBtn.style.display = 'inline-block';
    } else if (userGuess < randomNumber) {
      msg.textContent = '小了点，再试试？';
      msg.style.color = 'orange';
    } else {
      msg.textContent = '大了点，再试试？';
      msg.style.color = 'orange';
    }
  }

  function resetGame() {
    randomNumber = Math.floor(Math.random() * 100) + 1;
    attempts = 0;
    const input = document.getElementById('guessInput');
    const msg = document.getElementById('message');
    const resetBtn = document.getElementById('resetBtn');
    input.value = '';
    input.disabled = false;
    msg.textContent = '';
    resetBtn.style.display = 'none';
  }
</script>
<hr>

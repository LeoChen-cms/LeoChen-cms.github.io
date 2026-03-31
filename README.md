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


<br>
<hr>
<div align="center" style="padding: 20px; background-color: #f0f7ff; border: 2px solid #2a7ae2; border-radius: 12px; font-family: 'Microsoft YaHei', sans-serif;">
  <h3 style="color: #2a7ae2; margin-bottom: 10px;">🐉 成语接龙大挑战</h3>
  
  <p id="game-status" style="font-size: 1.1em; color: #333;">
    我先开路：<strong style="color: #e91e63; font-size: 1.2em;">一心一意</strong>
  </p>

  <input type="text" id="idiom-input" placeholder="请输入四字成语" 
         style="width: 220px; padding: 12px; margin: 10px; border: 1px solid #2a7ae2; border-radius: 6px; outline: none; font-size: 16px;">
  
  <button onclick="playIdiom()" 
          style="padding: 12px 25px; background-color: #2a7ae2; color: white; border: none; border-radius: 6px; cursor: pointer; font-size: 16px; transition: 0.3s;">
    提交接龙
  </button>

  <p id="msg" style="margin-top: 15px; color: #666; font-weight: bold; min-height: 24px;"></p>
  
  <div id="history-box" style="margin-top: 10px; font-size: 0.9em; color: #888;"></div>
</div>

<script>
  // 基础词库（电脑会从这里找词回敬你）
  let history = ["一心一意"];
 const library = [
    "意气风发", "发愤图强", "强词夺理", "理直气壮", "壮志凌云", "云淡风轻", "轻而易举", "举一反三", "三思而行", "行云流水",
    "水到渠成", "成王败寇", "扣人心弦", "闲情逸致", "志同道合", "合家欢乐", "乐此不疲", "疲惫不堪", "堪当重任", "任重道远",
    "远见卓识", "识全大局", "局促不安", "安分守己", "己所不欲", "欲罢不能", "能者多劳", "劳苦功高", "高瞻远瞩", "瞩目惊心",
    "心猿意马", "马到成功", "功德圆满", "满腹经纶", "纶音佛语", "语重心长", "长篇大论", "论功行赏", "赏心悦目", "目瞪口呆",
    "呆头呆脑", "脑满肠肥", "肥马轻裘", "裘马轻狂", "狂风暴雨", "雨过天晴", "晴天霹雳", "霹雳手段", "段数极高", "高山流水",
    "水涨船高", "高不可攀", "攀龙附凤", "凤毛麟角", "角逐中原", "原形毕露", "露天荧屏", "平步青云", "云消雾散", "散步赏花",
    "花好月圆", "圆满结束", "束手无策", "策马奔腾", "腾云驾雾", "雾里看花", "花言巧语", "语惊四座", "座无虚席", "席卷天下",
    "下不为例", "例直禁简", "简明扼要", "要言不烦", "烦躁不安", "安居乐业", "业精于勤", "勤能补拙", "拙嘴笨舌", "舌战群儒",
    "儒雅随和", "和衷共济", "济济一堂", "堂堂正正", "正大光明", "明察秋毫", "毫发无伤", "伤天害理", "理屈词穷", "穷途末路",
    "路不拾遗", "遗臭万年", "年富力强", "强弩之末", "末学肤受", "受宠若惊", "惊天动地", "地久天长", "长治久安", "安如泰山",
    "山清水秀", "秀色可餐", "餐风露宿", "宿怨未解", "解决问题", "题名榜首", "首屈一指", "指点江山", "山外有山", "山穷水尽",
    "尽力而为", "为人师表", "表里如一", "一心一意", "意气用事", "事半功倍", "倍道而行", "行善积德", "德才兼备", "备受瞩目",
    "目光如炬", "炬火照天", "天外有天", "天经地义", "义愤填膺", "膺惩暴行", "行动果敢", "敢作敢当", "当机立断", "断章取义",
    "义正辞严", "严阵以待", "待人接物", "物极必反", "反复无常", "常胜将军", "军令如山", "山高水远", "远走高飞", "飞黄腾达",
    "达官显贵", "贵在坚持", "持之以恒", "恒河沙数", "数不胜数", "数一数二", "二龙戏珠", "珠光宝气", "气吞山河", "河清海晏",
    "晏然自若", "若无其事", "事在人为", "为人正直", "直截了当", "当之无愧", "愧不敢当", "当红炸子", "子虚乌有", "有目共睹",
    "睹物思人", "人山人海", "海枯石烂", "烂醉如泥", "泥沙俱下", "下落不明", "明争暗斗", "斗志昂扬", "扬长避短", "短小精悍",
    "悍然不顾", "顾影自怜", "怜香惜玉", "玉石俱焚", "焚膏继晷", "晷刻不离", "离心离德", "德高望重", "重整旗鼓", "鼓舞人心",
    "心驰神往", "往事如烟", "烟消云散", "散入帘栊", "栊间风月", "月落星沉", "沉鱼落雁", "雁过留声", "声名狼藉", "藉草攀花",
    "花丛觅句", "句读不全", "全心全意", "意乱情迷", "迷途知返", "返老还童", "童心未泯", "泯灭人性", "性格开朗", "朗朗乾坤"
  ];

  function playIdiom() {
    const inputField = document.getElementById('idiom-input');
    const input = inputField.value.trim();
    const msg = document.getElementById('msg');
    const status = document.getElementById('game-status');
    const historyBox = document.getElementById('history-box');
    
    // 1. 校验长度
    if (input.length !== 4) {
      msg.innerText = "❌ 请输入四个字的成语哦！";
      msg.style.color = "red";
      return;
    }

    // 2. 校验首尾字（这里取上一个词的最后一个字）
    const lastIdiom = history[history.length - 1];
    if (input[0] !== lastIdiom[lastIdiom.length - 1]) {
      msg.innerText = `❌ 不对哦，要以“${lastIdiom[lastIdiom.length - 1]}”开头！`;
      msg.style.color = "red";
      return;
    }

    // 3. 用户接龙成功
    history.push(input);
    
    // 4. 电脑寻找匹配的词
    let response = library.find(word => word[0] === input[input.length - 1]);
    
    if (response) {
      history.push(response);
      status.innerHTML = `你接：<strong>${input}</strong> | 我接：<strong style="color: #e91e63;">${response}</strong>`;
      msg.innerText = "✅ 接得好！请继续。";
      msg.style.color = "green";
    } else {
      status.innerHTML = `你接：<strong>${input}</strong>`;
      msg.innerText = "🔥 太厉害了，我接不上了，你赢了！";
      msg.style.color = "#ff9800";
    }

    inputField.value = "";
    historyBox.innerText = "接龙轨迹: " + history.join(" > ");
  }
</script>
<br>
<hr>

## 公平性 ##

### 1. 公平的亂數算灋： ###

TRON Go平臺的所有遊戲都是基於部署在波場的智慧合約來實現的，平臺無法干預亂數的結果，從而保證了遊戲的公平性，用戶可以放心體驗平臺的遊戲內容。亂數算灋如下：


**Slot:<br>**
randomNum = sha256(sign(address + bet_amount + bet_count + randNonce + timestamp)<br>
randNonce++<br>
randomNum = sha256(sign(randNonce + randomNum + timestamp) Mod 24<br>

**Dice:<br>**
randomNum = sha256(sign(address + bet_amount + bet_count + randNonce + timestamp)<br>
randNonce++<br>
randomNum = sha256(sign(randNonce + randomNum + timestamp) Mod 100<br>

### 2. 可驗證的交易資訊： ###

TRON Go平臺上所有遊戲中產生的投注記錄，都會在相應遊戲下方的投注記錄中顯示，我們在每一筆投注記錄的後方放置了交易査詢的入口，用戶可點擊跳轉到波場公鏈，查看交易詳情。
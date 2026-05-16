# Velvet 21 · Blackjack

單檔案瀏覽器版 21 點，賭場質感 UI + 監控台統計賭徒每一步動作。

## 玩法
打開 `index.html` 即可。沒有伺服器、沒有相依，全部跑在瀏覽器。

- **籌碼下注**：點 LL / MAIN BET / BUSTER 圈切換押注區，點下方籌碼丟上桌面
- **動作鍵**：`H` Hit · `S` Stand · `D` Double · `P` Split · `R` Surrender · `Enter` Deal · `M` Monitor

## 規則
- 牌靴：**7 副**（364 張），發出 52 張就重洗（低滲透）
- 莊家 **H17**（軟 17 補牌）
- Blackjack 賠 **3:2**
- 允許 Double after Split、Late Surrender
- 同點兩張可 Split（最多拆一次）
- A 拆牌每手只發一張

## Side Bets
- **Lucky Lucky**（前三張就結算，A 可作 1 或 11）：同花 7-7-7 / 200:1，同花 6-7-8 / 100:1，雜色 7-7-7 / 50:1，同花 21 / 20:1，雜色 6-7-8 / 10:1，21 / 3:1，20 / 2:1，19 / 2:1
- **Buster Blackjack**（莊家爆牌張數）：3 張 2:1，4 張 4:1，5 張 18:1，6 張 50:1，7 張 250:1，8+ 張 800:1

## 監控台 (M 鍵打開)
- Session：時間、手牌數、勝率、連敗、每小時燒錢、追注偵測
- Lifetime（存 localStorage，跨 session 累積）：投注總額、淨損益、莊家賺走、實際莊家優勢、最長連敗、重新發錢次數
- 賭癮指數 / 回本機率
- 現實對照：你輸的錢可以買多少杯珍奶 / 支 iPhone
- Activity log（終端機風格）

## 多巴胺套件
贏錢時：金色 `+$N` 浮字、bankroll 滾動上升＋金光、大獎光暈擴散。

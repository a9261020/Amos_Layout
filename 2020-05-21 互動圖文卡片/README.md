# 2020-05-21 互動圖文卡片

![成品](./completed.jpg)

## 重點整理

- transition: width 1s 0.2s

第一個時間是轉場的時間(轉場要花多久跑完)  
第二個時間是延遲時間(轉場多久後開始)

- position:absolute

會往上找父層的定位，如果都沒有定位的話，會找到視窗去(不是 html 或 body，而是當前的視窗)，所以通常父層會定位 position:relative，讓他可以根據父層做定位變化

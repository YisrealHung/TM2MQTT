# TM2MQTT
結合Teachable Machine 與MQTT 功能，將訓練好的模型連結與MQTT 相關資訊輸入後，可將影像推論結果轉換成訊息並發佈至MQTT Topic。
<p align="center">
  <img src="https://github.com/YisrealHung/TM2MQTT/blob/main/album/00.png" width="800"/>
</p>

# 支援
* Image Project
* Pose Project

# 使用步驟
1. 使用Teachable Machine 訓練一個model，並按下Export Model。
<p align="center">
  <img src="https://github.com/YisrealHung/TM2MQTT/blob/main/album/01.png" width="800"/>
</p>

2. 於Tensorflow.js 頁面按下Upload my model 並等待連結出現後，按下Copy 複製model 的連結。
<p align="center">
  <img src="https://github.com/YisrealHung/TM2MQTT/blob/main/album/02.png" width="800"/>
</p>

3. 將整個專案Clone 到自己的電腦，依照自己在Teachable Machine 訓練的專案類型，選擇image.html 或是pose.html。
<p align="center">
  <img src="https://github.com/YisrealHung/TM2MQTT/blob/main/album/03.png" width="800"/>
</p>

4. 打開網頁後填入model 連結，與MQTT 相關資訊，網頁內MQTT Server 預設是連接HiveMQ，使用HiveMQ 的使用者不用更改欄位。
<p align="center">
  <img src="https://github.com/YisrealHung/TM2MQTT/blob/main/album/04.png" width="800"/>
</p>

5. 設定完畢後按下Webcam 按鈕開啟攝影機，然後按下Connect 連接MQTT，即可看到影像與推論結果，還有目前Topic 發送狀況。
<p align="center">
  <img src="https://github.com/YisrealHung/TM2MQTT/blob/main/album/05.png" width="800"/>
</p>

推論結果達70%以上才會發送訊息至Topic，並且不會一直發送。

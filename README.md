# HTML-class-S35
2024/9/12首次上課，目標：HTML網頁設計練習
- 學習資料來源```[https://www.tcsh.hlc.edu.tw/ischool/public/resource_view/openfid.php?id=4239](https://www.tcsh.hlc.edu.tw/ischool/public/resource_view/openfid.php?id=4324)```
## 基礎認知
- html 網站主體通常為一```index.html```之檔案且調用元素需在```<html>```檔案之資料夾中或使用URL連結
## 基本結構
```
<html>
  <title> 網站標題 </title>
  <body>
    網站本體內容
  </body>
</html>
```
## 常用(基本)語法與擴充屬性
- ### ```<html> </html>```網頁架構
#### 整個網頁的程式碼都會在此框架內
- ### ```<title> </title>```網頁標題
#### 設定網頁在瀏覽器標籤中的名稱
- ### ```<body> </body>```網頁主體
  - #### 網頁主體顯示的文字、圖片、超連結都在這裡設定
  - bgcolor=```<color>``` 設定背景顏色
    - 附加於```<body>```後，顏色可用簡單文字描述如"green","lightgreen"等也可使用色號精確定義
  - text="color" 設定文字顏色
    - 同上且可同時設定，指令間需空格
  - background = ```<image file name>``` 設定背景圖片
    - 會覆蓋掉bgcolor的設定，二者不相容
    - 在圖片無法填滿視窗時預設採用重複拼貼，建議使用重複性高的圖片或先確認比例
    - 使用的背景圖片檔需與```index.html```位於相同資料夾
- ### ```<a> </a>```超連結設定
  - #### 將前後包圍的原素設為超連結
  - href = ```<URL>```指向路徑
    - 加綴於```<a>```內，設定點擊超連結後前往的路徑
  - target = ```<開啟方式/位置>``` 設定超連結開啟方法
    - 常用為```<target = _blank>``` 功能在新分頁開啟超連結
    - 如果網頁有進行分割則可透過此指令設定開啟超連結的區塊
- ### ```<img>```插入圖片
   - #### 可以設為超連結
   - src=```<URL>``` 插入圖片網址or路徑
   - width=```<寬度>```、height=```<高度>``` 設定圖片寬、高（單位為px）
   - border=```<寬>``` 設定圖片邊框粗細（預設=0，少用到）
   - title=```<"文字">```圖片標示，游標停在圖片上時顯示
   - alt=```<"文字">```圖片替代文字，URL掛掉或圖片無法正常顯示時出現
- ### ```<br>```換行
  - 類似enter鍵用法
- ### ```<table></table>```表格
  - #### ```<tr></tr>``` 一組為一列(橫)，夾在```<table>```間 
  - #### ```<td></td>``` 一組為一儲存格，夾在```<tr>```間
    - bgcolor=```<color>```設定該格背景顏色
    - align=```<對齊方式>``` 設定格內文字對齊方式
  - border=```<寬>``` 設定表格格線粗細，預設為0建議設1以上
- ### ```<font></font>``` 文字設定
  - color=```<color>``` 設定顏色
  - size=```<size>``` 設定文字大小，默認為3
  - #### ```<i>``` 設為斜體
  - #### ```<b>``` 設為粗體
  - #### ```<u>``` 底線
- ### ```<marquee></marquee>```跑馬燈效果
  - direction=```<方向>``` 字幕移動方向，可設定為up,dun(下),left,right
  - align=```<對齊方式>``` 字幕對齊方式，可設為top,midden,botton
  - scrollamount=```<speed>``` 字幕移速，通常設在1~10的範圍
  - height=```<高>```、width=```<寬>``` 老朋友，字幕寬高設定
  - behavior=```<行為>``` 字幕行為
    - ```<alternate>``` 重複來回
    - ```<slide>``` 跑入後停止
  - bgcolor=```<color>```
- ### ```<form></form>```表單(輸入)內容
  ` action=```<URL>``` 處理資料的.php檔案位置
  - method=```<post/get>``` 資料獲取(傳送)方式
    - ```<post>``` 較為隱蔽，傳送時網址不變
    - ```<get>``` 傳送資料可能導致網址變化而洩漏
  - #### ```<input>```輸入單元
    - type=```<type>``` 輸入類型
      - ```<text>``` 普通文字
      - ```<password>``` 密碼，會隱藏
      - ```<radio>``` 單選選項(圓)，在多個擁有相同```name```的選項中擇一
      - ```<checkbox>``` 核取方塊(多選)
      - ```<file>``` 上傳檔案按鈕
      - ```<submit>``` 送出表單按鈕
      - ```<reset>``` 重設表單按鈕
      - ```<color>``` 選取顏色
      - ```<date>``` 選取日齊
      - ```<email>``` 電子郵件特化
      - ```<number>``` 數字特化
      - ```<range>``` 拉條選項，使用```max```和```min```設定範圍
      - 族繁不及備載
    - name="name" 選項名稱
    - vaule="name" 設定按鈕名稱


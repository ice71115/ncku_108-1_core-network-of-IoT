# LAB1_Guess_number(GuessTheNumber.aia)

## 目標:
	隨機生成一個1~100之間的整數，讓使用者透過textbox輸入要猜測的數字，並且提示遊戲進度。
## 作法or步驟:
                 判斷正確的整數與使用者輸入的整數大小，並輸出區間

# LAB1_Post_text(HttpPostApplication.aia)
## 目標:
    將textbox中的文字，經由HTTP POST的方式傳到自己定義的node-red server，並將回傳的response放置到畫面上。

## 作法or步驟:
                  將使用者輸入的名字轉成json格式，並傳到server，並等待server回傳

# LAB1_flow(Lab1_flow.json)

## 目標:
    接收來自LAB1_POST_text的http request，回傳"Hello"加上收到訊息name
    
## 作法or步驟:
                  將收到的json格式 轉成使用者的名稱 並在前面加入hellp

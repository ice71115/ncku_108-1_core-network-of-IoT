# 檔案說明:
    LAB5.aia:負責控制lamp與顯示lamp 狀態的app，
	flow.json:負責轉傳app與om2m間的訊息
# LAB5
## 目標:
    使用任意方法完成以下:
    1. 分別控制 LAMP_0 的開/關、LAMP_1 的開/關、ALL_ON、ALL_OFF 共六個動作
    2. 在 APP 上，顯示當前燈泡的狀態 (主動 or 被動皆可)

## 作法or步驟:  
    node red接收app傳來了post請求，並轉傳到om2m，來控制LAMP_0與LAMP_1開關
	並對LAMP_0與LAMP_1資源訂閱，資料更新後om2m會傳送通知到node red，再利用node red 的context flow儲存兩個燈的狀態
	如果app傳送get請求lamp_status資訊，node red 會回傳 儲存的lamp資訊
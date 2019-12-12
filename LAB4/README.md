
# 檔案說明:
    GA.json:GA的flow
	NA.json:NA的flow
	ServerLocation.aia:一個APP，可以將自己位置傳到GA，也能傳送GET 取得NA位置
# LAB4_GA with Node-red
## 目標:
    使用 node-red 分別建立以下
	  1. Create a "Location_Gateway_Application" Application on OM2M
		2. Create a "DESCRIPTOR" container on OM2M
		    3. Create a "DESCRIPTOR contentInsances" on OM2M
		4. Create a "DATA" container on OM2M
			5. Create a "DATA contentInsances" (for testing) on OM2M
    6. Create a http node to forward data to GSCL

## 作法or步驟:  
    建立Application、DESCRIPTOR container、DATA container、來儲存手機位置資訊 
    
# LAB4_App inventor Sender
## 目標:
    須完成兩個功能
      1.讀取手機(or 模擬器)的location sensor
      2.將其值交給 GA(node-red)
 
## 作法or步驟:  
    先取得手機的位置，再以POST請求 傳給GA
       
# LAB4_NA with Node-red
# 目標:
    使用 node-red 建立以下
    1. Create a "Location_Network_Application" Application on OM2M
    2. Subscribe new contentInsatnace in the   gscl/Location_Gateway_Application/DATA  on OM2M and save recive notify
    3. Create a http node to response previously save data
    
## 作法or步驟:  
    建立Application與Subscribe 訂閱存放在gscl的經緯度資訊，並存在NA上
    
    
# LAB4_APP Inventor reciver
## 目標:
    須完成兩個功能
      1. http get NA(node-red) 上儲存的 data
      2. 將該 data 用來啟動 google map 並顯示位子
      
## 作法or步驟:  
    以GET請求NA回傳DATA，並在GOOGLE map上顯示位置

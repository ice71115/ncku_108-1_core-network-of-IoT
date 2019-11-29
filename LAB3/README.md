# LAB3_OM2M with Postman
## 目標:
    使用Postman分別建立以下Entities
	1. Create a "MY_SENSOR" Application
		2. Create a "DESCRIPTOR" container
			3. Create a "DESCRIPTOR contentInsances"
		4. Create a "DATA" container
			5. Create a "DATA contentInsances"
			6. Create a "Subscription" contact to localhost:1400/monitor

## 作法or步驟:
                  使用Postman建立好以上Entities後，只要建立新的"DATA contentInsances"，GA就會通知monitor收到的"DATA contentInsances"



# LAB3_OM2M  GA with Node-red
## 目標:
    使用 node-red 在GSCL分別建立以下 Entities
	1. Create a "MY_SENSOR" Application
		2. Create a "DESCRIPTOR" container
			3. Create a "DESCRIPTOR contentInsances"
		4. Create a "DATA" container
			5. Create a "DATA contentInsances"
	6. 在 GA(node-red) 開啟 /sensorData Server 負責轉傳 data 到 OM2M
	

## 作法or步驟:
		Create a "MY_SENSOR" Application
		Create a "DESCRIPTOR" container
		Create a "DESCRIPTOR contentInsances"
		Create a "DATA" container
		Create a "DATA contentInsances"
		建立好以上Entities後，GA可將收到的data作處理，並建立"DATA contentInsances"
		
		





# LAB3_OM2M  NA with Node-red
## 目標:
    	

    使用 node-red 在 NSCL 分別建立以下 Entities
	1. Create a "MY_NETWORK_APPLICATION"
	2. Subscribe new contentInsatnace in the   gscl/MYSENSOR/DATA 並儲存
	3. 開啟 /getxmlfile Server 負責讀取先前儲存的資料
    
## 作法or步驟:
		NA藉由訂閱方式將gscl/MYSENSOR/DATA中新的contentInsatnace 儲存起來
		並可用get方法讀取
	

# LAB2_Get_Sensor_Value(GetSensorValues.aia)
## 目標:
    按下按鈕時，抓取手機上的三種sensor，Accelerometer、OrientationSensor、LocationSensor
    
## 作法or步驟:
    取得手機的資訊，並輸出
    
    
    
# LAB2_Show_Location_on_Google.aia(ServerLocation.aia)
##目標:
    實現五個功能，1.抓取LocationSensor(GPS) 2.將1中的值傳到node-red顯示 3.讀取server存放的location資料 4(5).將1(3)中的資料用google map定位 

## 作法or步驟:
    得到手機目前的gps位置，傳給server，
    讀取server回傳的json格式，轉換成經緯度，並在google map 上定位 
    
    
    
    
# LAB2_flow.json(server.json)
##目標:
    1.接受來自app的訊息，並回復response，2.回傳在server儲存的location data
    
## 作法or步驟:
    接收手機傳的gps位址的post，與接收手機的get 並回傳server的gps位址 

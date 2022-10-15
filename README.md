
# PERT/CPM
![PERT/CPM](PERT.jpg "PERT")
***




# 甘特圖
```mermaid
gantt
    title 甘特圖
    section 研擬計畫
    1天:a1, 2022-10-03, 1d
    
    section 任務分配
    4天:a2,after a1  , 4d
    
    section 取得硬體
    17天:a3,after a1  , 17d
    
    section 程式開發
    70天:a4,after a2  , 70d 
    
    section 安裝軟體
    10天:a5,after a3  , 10d
    
    section 程式測試
    30天:a6,after a4  , 30d
    
    section 撰寫使用手冊
    25天:a7,after a5  , 25d
    
    section 轉換檔案
    20天:a8,after a5  , 20d
    
    section 系統測試
    25天:a9,after a6  , 25d
    
    section 使用者訓練
    20天:a10,after a7, 20d
    
    section 使用者測試
    25天:a11,after a9, 25d
```
# 關鍵路徑
---
![CPM_img 圖](關鍵.jpg)
***


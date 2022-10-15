
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
```graphviz
digraph {
	node[shape=record];
	rankdir="LR";
    no1 [label = "取得授權 | 編號:1 | 開始:第1天 | 結束:第1天 | 需時:1天"]
    no2 [label = "聘僱分析師 | 編號:2 | 開始:第2天 | 結束:5 | 需時:4天"]
    no3 [label = "規劃訓練 | 編號:3 | 開始:第2天 | 結束:第18天 | 需時:17天"]
    no4 [label = "安排後勤 | 編號:4 | 開始:第6天 | 結束:第75天 | 需時:70天"]
    no5 [label = "宣告訓練 | 編號:5 | 開始:第19天 | 結束:第28天 | 需時:10天"]
    no6 [label = "聘僱分析師 | 編號:6 | 開始:第76天 | 結束:105 | 需時:30天"]
    no7 [label = "聘僱分析師 | 編號:7 | 開始:第29天 | 結束:53 | 需時:25天"]
    no8 [label = "聘僱分析師 | 編號:8 | 開始:第29天 | 結束:48 | 需時:20天"]
    no9 [label = "聘僱分析師 | 編號:9 | 開始:第106天 | 結束:130 | 需時:25天"]
    no10 [label = "聘僱分析師 | 編號:10 | 開始:第54天 | 結束:73 | 需時:25天"]
    no11 [label = "聘僱分析師 | 編號:11 | 開始:第131天 | 結束:155 | 需時:25天"]
    no1->no2
    no1->no3
    no2->no4
    no3->no5
    no4->no6
    no6->no9
    no9->no11
    no5->no7
    no5->no8
    no7->no10
    no8->no10
    no10->no11
    
}



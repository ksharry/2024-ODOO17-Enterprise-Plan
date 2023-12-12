## 差異系列-ODOO17企業版-MPS

## 總表
![Alt text](https://github.com/ksharry/2024-ODOO17-Enterprise-Plan/blob/main/pic/F171301.png?raw=true)

## 名詞介紹
1. 主生產排成（Master Production Schedule，簡稱MPS），為根據銷售訂單或預測得到的對產品（獨立需求物料）的需求清單，即在某一個時間點對產品的需求量。主生產計畫的訂立必須考量到可能的客戶訂單、目前未完成的訂單、可用資源的數量、現有能力、管理階層的目標等等。
2. 物資需求計劃(Manufacturing Resources Planning，簡稱MRP)：系統透過現有的單據資訊，計算供給與需求的量，如果供給與需求不匹配時，就會提出建議的資訊，例如缺料情況、交期建議修改..等，讓各單位透過系統更容易了解缺口並進行調整的一套計算方式。
3. 粗略產能規劃(Rough-Cut Capacity Planning，簡稱RCCP)，探究其處理過程，主要是將成品的生產計畫，轉換成為相對應的工作能力需求，ODOO設定式透過每日的最高產能。

## 設定
1. 可以根據設定開啟

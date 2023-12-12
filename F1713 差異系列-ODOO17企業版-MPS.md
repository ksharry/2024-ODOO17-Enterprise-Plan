## 差異系列-ODOO17企業版-MPS

## 總表
![Alt text](https://github.com/ksharry/2024-ODOO17-Enterprise-Plan/blob/main/pic/F171301.png?raw=true)

## 名詞介紹
1. 主生產排成（Master Production Schedule，簡稱MPS），為根據銷售訂單或預測得到的對產品（獨立需求物料）的需求清單，即在某一個時間點對產品的需求量。主生產計畫的訂立必須考量到可能的客戶訂單、目前未完成的訂單、可用資源的數量、現有能力、管理階層的目標等等。
2. 物資需求計劃(Manufacturing Resources Planning，簡稱MRP)：系統透過現有的單據資訊，計算供給與需求的量，如果供給與需求不匹配時，就會提出建議的資訊，例如缺料情況、交期建議修改..等，讓各單位透過系統更容易了解缺口並進行調整的一套計算方式。
3. 粗略產能規劃(Rough-Cut Capacity Planning，簡稱RCCP)，探究其處理過程，主要是將成品的生產計畫，轉換成為相對應的工作能力需求，ODOO設定式透過每日的最高產能。

## 設定
![Alt text](https://github.com/ksharry/2024-ODOO17-Enterprise-Plan/blob/main/pic/F171302.png?raw=true)
1. 根據製造週期去設定
   + 日
   + 周
   + 月
![Alt text](https://github.com/ksharry/2024-ODOO17-Enterprise-Plan/blob/main/pic/F171303.png?raw=true)
2. 設定MPS規則
   + 設定安全庫存
   + 設定最高產量
   + 如設定BOM表，可自動產算下階。

## 實際運算
#### 計畫式生產
![Alt text](https://github.com/ksharry/2024-ODOO17-Enterprise-Plan/blob/main/pic/F171304.png?raw=true)
1. 根據預測，展開每周的計畫內容。

#### 接單式生產
![Alt text](https://github.com/ksharry/2024-ODOO17-Enterprise-Plan/blob/main/pic/F171305.png?raw=true)
1. 根據訂單，展開每周的計畫內容

#### 實際運算-混合式生產
![Alt text](https://github.com/ksharry/2024-ODOO17-Enterprise-Plan/blob/main/pic/F171306.png?raw=true)
1. 根據共用性產品，展開每周的計畫內容，期望縮短製造週期。
2. 根據訂單，展開每周計畫。

#### 如果運算要進行修改，如何處理
![Alt text](https://github.com/ksharry/2024-ODOO17-Enterprise-Plan/blob/main/pic/F171307.png?raw=true)
1. 可透過補充的數字，串查已產生的單據
   + 過高可以重新補充
   + 過低請進行取消，重新產生新的MPS單據。

## 小結
1. 版本需求，目前僅能查看一次的需求。
   + 不同職能需求
   + 不同預測需求
2. 訂單預測與產能規劃設定比較簡單。
3. 建議可以產出單次橫向的料號與總需求表，較容易查看單次情況。

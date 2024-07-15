---
title: Amazon sales channel — 價格規則範例
description: 若要協助您為Amazon清單設計定價規則，請根據常見案例檢閱這些範例。
feature: Sales Channels, Price Rules
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 1%

---

# 價格規則範例

## 標準價格規則範例

### 捨棄後續規則

捨棄後續規則的功能是定價規則內的一項絕佳功能，可防止多個定價規則棧疊並提供意想不到的額外折扣。 若要捨棄後續規則，訂價規則必須使用在[訂價規則一般設定](./pricing-rule-general-settings.md)的&#x200B;_[!UICONTROL Priority]_區段中設定的優先順序。

如果&#x200B;**[!UICONTROL Discard Subsequent Rules]**&#x200B;設定為`Yes`，則優先順序較低（數字較高）的規則不會套用至符合資格的產品。

例如，假設有三個定價規則：

| 範例 | 規則名稱 | 優先順序 | 捨棄後續規則 |
|---------|-----------------------|----------|-------------------------|
| 1 | 優惠季商品10%優惠 | 1 | 否 |
| 2 | 2美元優惠銷售產品 | 2 | 是 |
| 3 | 所有產品5%優惠 | 3 | 否 |

此情境中，規則#1和#2會套用至合格產品。 規則#3僅適用於規則#2中未包含的合格產品，因為其優先順序低於範例#2，且&#x200B;**[!UICONTROL Discard Subsequent Rules]**&#x200B;設定為`Yes`。 因此，銷售類別中符合資格的產品可享有10%的折扣，以及Amazon上市價格的$2優惠。

### 套用兩個標準價格規則

| 欄位 | 設定 — 規則1 | 設定 — 規則2 |
|--------------------------------|---------------------|-----------------------|
| [!UICONTROL Rule Name] | 規則–1 | 規則–2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | 標準價格規則 | 標準價格規則 |
| [!UICONTROL Price action] | 減少依據 | 減少依據 |
| [!UICONTROL Apply] | 套用為百分比 | 套用為固定金額 |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### 產品1

價格：45.49美元

套用規則1：$45.49 x (0.9) = $40.94

套用規則2：$40.94 - $10.00 = $30.94

套用規則1和規則2後的最終價格： $30.94

#### 產品2

價格：47.76美元

套用規則1：$47.76 x (0.9) = $42.98

套用規則2：$42.98 - $10.00 = $32.98

套用規則1和規則2後的最終價格： $32.98

## 智慧型重新訂價規則範例

### 含底價的Buy Box價格Source =價格

| 欄位 | 設定 |
|--------------------------------------|----------------------------|
| [!UICONTROL Rule Name] | 規則–1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 智慧型重新訂價規則 |
| [!UICONTROL Competitor Price Source] | 使用「Buy Box」價格 |
| [!UICONTROL Price Action] | 比對競爭者價格 |
| [!UICONTROL Floor Price Source] | 價格 |
| [!UICONTROL Floor Price Action] | 符合 |

#### 產品1

價格：15美元

來自Amazon的[Buy Box](./buy-box-competitor-pricing.md)價格： $10

由於[Buy Box](./buy-box-competitor-pricing.md)的價格低於原始價格，因此產品會以原始價格列出。

套用規則後的最終價格：$15

#### 產品2

價格：5美元

來自Amazon的[Buy Box](./buy-box-competitor-pricing.md)價格： $10

由於[Buy Box](./buy-box-competitor-pricing.md)的價格大於原始價格，因此產品會以[Buy Box](./buy-box-competitor-pricing.md)的價格列出。

套用規則後的最終價格： $10

### 含底價的Buy Box價格Source =價格與20%的價格降低

| 欄位 | 設定 |
|--------------------------------------|----------------------------|
| [!UICONTROL Rule Name] | 規則–1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 智慧型重新訂價規則 |
| [!UICONTROL Competitor Price Source] | 使用「Buy Box」價格 |
| [!UICONTROL Price Action] | 比對競爭者價格 |
| [!UICONTROL Floor Price Source] | 價格 |
| [!UICONTROL Floor Price Action] | 減少依據 |
| [!UICONTROL Apply] | 以百分比套用 |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### 產品1

價格：$20

計算的底價：$16

來自Amazon的[Buy Box](./buy-box-competitor-pricing.md)價格： $15

由於[Buy Box](./buy-box-competitor-pricing.md)價格小於計算的[樓面價格](./floor-price.md)，因此產品會以計算的[樓面價格](./floor-price.md)列出。

套用規則後的最終價格：$16

#### 產品2

價格：15美元

已計算[底價](./floor-price.md)： $12

來自Amazon的[Buy Box](./buy-box-competitor-pricing.md)價格： $15

由於[Buy Box](./buy-box-competitor-pricing.md)價格大於計算的[樓面價格](./floor-price.md)，因此產品會以[Buy Box](./buy-box-competitor-pricing.md)價格列出。

套用規則後的最終價格：$15

#### 產品3

價格：17美元

計算底價：$13.60

來自Amazon的[Buy Box](./buy-box-competitor-pricing.md)價格： $15

由於[Buy Box](./buy-box-competitor-pricing.md)價格大於計算的[樓面價格](./floor-price.md)，因此產品會以[Buy Box](./buy-box-competitor-pricing.md)價格列出。

套用規則後的最終價格：$15

### 最低價格，包含所有競爭者的價格並使用所有競爭者的產品條件

| 欄位 | 設定 |
|----------------------------------------|-----------------------------------------|
| [!UICONTROL Rule Name] | 規則–1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 智慧型重新訂價規則 |
| [!UICONTROL Competitor Price Source] | 使用最低競爭者價格 |
| [!UICONTROL Minimum Positive Feedback] | 所有競爭者價格 |
| [!UICONTROL Conditional Variance] | 使用所有競爭者的產品條件 |
| [!UICONTROL Price Action] | 比對競爭者價格 |
| [!UICONTROL Floor Price Source] | 價格 |
| [!UICONTROL Floor Price Action] | 符合 |

| 價格 | 條件 |
|-------|-----------------|
| 17美元 | 新增 |
| 15美元 | 新增 |
| 14美元 | 已使用；非常好 |
| 13美元 | 已使用；良好 |

#### 產品1

價格：$10

條件：新增

因為新條件的競爭者最低價格是$15，所以產品價格為$15。

套用規則後的最終價格：$15

#### 產品2

價格：$10

條件：已使用；可接受

由於「已使用」狀況的[最低競爭者價格](./lowest-competitor-pricing.md)為$13，因此產品上市價格為$13。

套用規則後的最終價格：$13

### 結合上限價格、幣別兌換及VAT的智慧型重新訂價規則

| 欄位 | 設定 |
|-----------------------------------|---------------|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | $10 |
| [!UICONTROL Currency conversion] | 1.25歐元：1美元 |

[歐洲(VAT)市場的最高價格](./optional-ceiling-price.md)：$10 x 1.25 = $12.50

當點選歐洲(VAT)市場中的[最高價格](./optional-ceiling-price.md)時，就會計算並新增VAT。

加值後最終價格：$12.50 x (1.1) = $13.75

### 結合多重訂價規則、上限價格、幣別兌換及VAT

#### 智慧型訂價規則（來自上一個範例）

| 欄位 | 設定 |
|----------------------|---------------|
| 優先順序 | 1 |
| VAT | 10% |
| 最高價格來源 | $10 |
| 貨幣轉換 | 1.25歐元：1美元 |

[歐洲(VAT)市場的最高價格](./optional-ceiling-price.md)：$10 x 1.25 = $12.50

加值後最終價格：$12.50 x (1.1) = $13.75

#### 標準訂價規則

| 欄位 | 設定 |
|--------------------------------|-----------------------|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | 增加方式 |
| [!UICONTROL Apply] | 套用為固定金額 |
| [!UICONTROL Adjustment Amount] | $5.00 |

當達到[最高價格](./optional-ceiling-price.md)時，標準訂價規則會套用至智慧型訂價規則之上。

套用標準訂價規則後的最終價格：$13.75 + $5.00 = $18.75

### 價格調整

在此範例中，最具競爭力的價格是透過檢視Amazon [競爭者的最低價格](./lowest-competitor-pricing.md)來定義，有95%的正面意見回饋，以及最低意見回饋1,000個商家評論。

![價格調整範例](assets/amazon-price-adjustment-example.png){width="600" zoomable="yes"}

根據這些引數執行搜尋之後，競爭價格會回到$25。

從這裡，根據此最低價格，有三個不同的[價格規則動作](./pricing-rule-actions.md)選擇。

| 欄位 | 說明 |
|--------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | 選項：<ul><li>**[!UICONTROL Decrease By]** — 此選項會減少您的上市價格，相對於[最低競爭者價格](./lowest-competitor-pricing.md)。</li><li>**[!UICONTROL Increase By]** — 此選項會提高您的刊登價格，相對於[最低競爭者價格](./lowest-competitor-pricing.md)。</li><li>**[!UICONTROL Match Competitor Price]** — 此選項會變更您的Amazon上市價格，以根據引數符合最低價格。 在範例中，Amazon的掛牌價為$25。</li></ul> |
| [!UICONTROL Apply] | 選項：以百分比沖銷/以固定金額沖銷 |
| [!UICONTROL Adjustment Amount] | 用於定義要套用之折扣的百分比或固定金額的數值。 <br>這些選擇會取得最低價格，並將其設定為低於$0.01的價格。 |

### 底價

| 欄位 | 設定 |
|--------------------------------------|---------------------|
| [!UICONTROL Floor Price Source] | 成本= $5 |
| [!UICONTROL Floor Price Action] | 增加方式 |
| [!UICONTROL Apply] | 套用為百分比 |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[底價](./floor-price.md)計算=底價Source `$5` x底價調整金額`5%` = $5.25

套用智慧型定價規則時，若成本為$5美元，此特定產品的上市價格會低於$5.25。

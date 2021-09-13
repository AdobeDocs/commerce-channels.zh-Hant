---
title: 價格規則範例
description: 若要協助您設計Amazon清單的定價規則，請根據常見案例檢閱這些範例。
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# 價格規則範例

## 標準價格規則範例

### 捨棄後續規則

捨棄後續規則的能力，是定價規則中的絕佳功能，可防止多個定價規則堆疊，並提供非預期的額外折扣。 要放棄後續規則，定價規則必須使用[定價規則一般設定](./pricing-rule-general-settings.md)的&#x200B;_[!UICONTROL Priority]_部分中設定的優先順序。

如果將&#x200B;**[!UICONTROL Discard Subsequent Rules]**&#x200B;設為`Yes`，優先順序較低（數字較高）的規則不適用於符合條件的產品。

例如，假設有三個定價規則：

| 範例 | 規則名稱 | 優先順序 | 捨棄後續規則 |
|----------|----|----|----|
| 3 | 銷售產品優惠10% | 3 | 否 |
| 2 | $2銷售產品 | 2 | 是 |
| 3 | 佔所有產品的5% | 3 | 否 |

在此案例中，#1和#2則適用於合格產品。 規則#3僅適用於規則#2中未包含的合格產品，因為其優先順序比範例#2低，且&#x200B;**[!UICONTROL Discard Subsequent Rules]**&#x200B;設為`Yes`。 因此，銷售類別中的合格產品將獲得10%的折扣，並獲得Amazon上市價格的2美元折扣。

### 應用兩個標準價格規則

| 欄位 | 設定 — 規則1 | 設定 — 規則2 |
|----------|----|----|
| [!UICONTROL Rule Name] | 規則1 | 規則2 |
| [!UICONTROL Priority] | 3 | 2 |
| [!UICONTROL Rule Type] | 標準價格規則 | 標準價格規則 |
| [!UICONTROL Price action] | 減少者 | 減少者 |
| [!UICONTROL Apply] | 以百分比方式應用 | 以固定金額應用 |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### 產品1

價格：US$45.49

規則1已應用：$45.49 x(0.9)= $40.94

第2條適用：40.94美元 — 10.00美元= 30.94美元

適用規則1和規則2之後的最終價格：US$30.94

#### 產品2

價格：US$47.76

規則1已應用：$47.76 x(0.9)= $42.98

第2條適用：42.98美元 — 10.00美元= 32.98美元

適用規則1和規則2之後的最終價格：US$32.98

## 智慧重新定價規則範例

### Buy Box價格（含底價來源）=價格

| 欄位 | 設定 |
|----------|----|
| [!UICONTROL Rule Name] | 規則1 |
| [!UICONTROL Priority] | 3 |
| [!UICONTROL Rule Type] | 智慧重新定價規則 |
| [!UICONTROL Competitor Price Source] | 使用「Buy Box」價格 |
| [!UICONTROL Price Action] | 符合競爭者價格 |
| [!UICONTROL Floor Price Source] | 價格 |
| [!UICONTROL Floor Price Action] | 符合 |

#### 產品1

價格：15美元

[向](./buy-box-competitor-pricing.md) Amazon購買Boxprice:10美元

由於[Buy Box](./buy-box-competitor-pricing.md)價格低於原價，因此產品按原價列出。

套用規則後的最終價格：15美元

#### 產品2

價格：5美元

[向](./buy-box-competitor-pricing.md) Amazon購買Boxprice:10美元

由於[Buy Box](./buy-box-competitor-pricing.md)價格大於原始價格，因此產品以[Buy Box](./buy-box-competitor-pricing.md)價格列出。

套用規則後的最終價格：10美元

### Buy Box價格與最低價格來源=價格和20%的降價

| 欄位 | 設定 |
|----------|----|
| [!UICONTROL Rule Name] | 規則1 |
| [!UICONTROL Priority] | 3 |
| [!UICONTROL Rule Type] | 智慧重新定價規則 |
| [!UICONTROL Competitor Price Source] | 使用「Buy Box」價格 |
| [!UICONTROL Price Action] | 符合競爭者價格 |
| [!UICONTROL Floor Price Source] | 價格 |
| [!UICONTROL Floor Price Action] | 減少者 |
| [!UICONTROL Apply] | 以百分比形式應用 |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### 產品1

價格：20美元

計算底價：16美元

[向](./buy-box-competitor-pricing.md) Amazon購買Boxprice:15美元

由於[Buy Box](./buy-box-competitor-pricing.md)價格小於「計算[樓價](./floor-price.md)」，因此產品將按「計算[樓價](./floor-price.md)」列出。

套用規則後的最終價格：16美元

#### 產品2

價格：15美元

計算的[樓價](./floor-price.md):12美元

[向](./buy-box-competitor-pricing.md) Amazon購買Boxprice:15美元

由於[Buy Box](./buy-box-competitor-pricing.md)價格大於計算[樓價](./floor-price.md)，因此產品以[Buy Box](./buy-box-competitor-pricing.md)價格列出。

套用規則後的最終價格：15美元

#### 產品3

價格：17美元

計算底價：US$13.60

[向](./buy-box-competitor-pricing.md) Amazon購買Boxprice:15美元

由於[Buy Box](./buy-box-competitor-pricing.md)價格大於計算[樓價](./floor-price.md)，因此產品以[Buy Box](./buy-box-competitor-pricing.md)價格列出。

套用規則後的最終價格：15美元

### 所有競爭者的價格的最低價格和使用所有競爭者的產品條件

| 欄位 | 設定 |
|----------|-----|
| [!UICONTROL Rule Name] | 規則1 |
| [!UICONTROL Priority] | 3 |
| [!UICONTROL Rule Type] | 智慧重新定價規則 |
| [!UICONTROL Competitor Price Source] | 使用最低競爭者價格 |
| [!UICONTROL Minimum Positive Feedback] | 所有競爭者價格 |
| [!UICONTROL Conditional Variance] | 使用所有競爭者的產品條件 |
| [!UICONTROL Price Action] | 符合競爭者價格 |
| [!UICONTROL Floor Price Source] | 價格 |
| [!UICONTROL Floor Price Action] | 符合 |

| 價格 | 條件 |
|----------|----|
| 17美元 | 新增 |
| 15美元 | 新增 |
| 14美元 | 已使用；很好 |
| 13美元 | 已使用；好 |

#### 產品1

價格：10美元

條件：新增

因為「新」條件的競爭者最低價格是$15，所以產品的標價是$15。

套用規則後的最終價格：15美元

#### 產品2

價格：10美元

條件：已使用；可接受

因為「已使用」條件的[最低競爭者價格](./lowest-competitor-pricing.md)為$13，所以該產品以$13列出。

套用規則後的最終價格：13美元

### 結合最高價格、貨幣轉換和增值稅的智慧重新定價規則

| 欄位 | 設定 |
|----------|-----|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | 10美元 |
| [!UICONTROL Currency conversion] | 1.25歐元：1美元 |

[歐](./optional-ceiling-price.md) 洲(VAT)市場的最高價格：$10 x 1.25 = $12.50

當歐洲(VAT)市場中的[最高價格](./optional-ceiling-price.md)被點擊時，將計算並添加VAT。

增值稅後最終價格：$12.50 x(1.1)= $13.75

### 結合多個定價規則、最高價格、貨幣轉換和增值稅

#### 智慧定價規則（來自上一個範例）

| 欄位 | 設定 |
|----------|----|
| 優先順序 | 3 |
| 增值稅 | 10% |
| 最高價格來源 | 10美元 |
| 貨幣轉換 | 1.25歐元：1美元 |

[歐](./optional-ceiling-price.md) 洲(VAT)市場的最高價格：$10 x 1.25 = $12.50

增值稅後最終價格：$12.50 x(1.1)= $13.75

#### 標準定價規則

| 欄位 | 設定 |
|----------|-----|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | 增加者 |
| [!UICONTROL Apply] | 以固定金額應用 |
| [!UICONTROL Adjustment Amount] | 5.00美元 |

當[最高價格](./optional-ceiling-price.md)點擊時，在智慧定價規則的頂端套用標準定價規則。

套用標準定價規則後的最終價格：$13.75 + $5.00 = $18.75

### 價格調整

在此範例中，最具競爭力的價格是透過查看Amazon [競爭者的最低價格](./lowest-competitor-pricing.md)、95%的正反饋和1,000個商家評論的最低反饋計數來定義。

![價格調整實例](assets/amazon-price-adjustment-example.png)

根據這些參數運行此搜索後，競爭價格會回到25美元。

從這裡，有三個不同的[價格規則操作](./pricing-rule-actions.md)選項，它們基於此最低價格。

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Price Action] | 選項：<ul><li>**[!UICONTROL Decrease By]**  — 此選項會降低您的上市價格，而非 [最低競爭者價格](./lowest-competitor-pricing.md)。</li><li>**[!UICONTROL Increase By]**  — 此選項會比競爭者最低的價格 [提高您的上市價格](./lowest-competitor-pricing.md)。</li><li>**[!UICONTROL Match Competitor Price]**  — 此選項會變更您的Amazon上市價格，以根據參數來比對最低價格。在此範例中，Amazon的上市價格為$25。</li></ul> |
| [!UICONTROL Apply] | 選項：以百分比形式應用/以固定金額形式應用 |
| [!UICONTROL Adjustment Amount] | 定義要套用折扣的百分比或固定金額的數值。 <br>這些選擇將使價格降至最低，並將價格設定為低於0.01美元。 |

### 最低價格

| 欄位 | 設定 |
|----------|----|
| [!UICONTROL Floor Price Source] | 成本= 5美元 |
| [!UICONTROL Floor Price Action] | 增加者 |
| [!UICONTROL Apply] | 以百分比方式應用 |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[最低](./floor-price.md) 價計算=最低價源 `$5` x最低調整 `5%` 金額= $5.25

套用智慧型定價規則時，成本為$5時，此特定產品的上市價格確實會低於$5.25。

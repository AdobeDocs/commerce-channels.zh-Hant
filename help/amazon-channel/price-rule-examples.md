---
title: 價格規則示例
description: 為幫助您設計Amazon清單的定價規則，請根據常見方案查看這些示例。
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# 價格規則示例

## 標準價格規則示例

### 放棄後續規則

放棄後續規則的能力是定價規則內的一個強大功能，它防止了多個定價規則堆疊並提供意外的附加折扣。 要放棄後續規則，定價規則必須使用在 _[!UICONTROL Priority]_部分 [定價規則常規設定](./pricing-rule-general-settings.md)。

如果 **[!UICONTROL Discard Subsequent Rules]** 設定為 `Yes`，優先順序較低（數字較高）的規則不適用於合格產品。

例如，假設有三個定價規則：

| 示例 | 規則名稱 | 優先順序 | 放棄後續規則 |
|----------|----|----|----|
| 1 | 10%的銷售產品 | 1 | 否 |
| 2 | 2美元的銷售產品 | 2 | 是 |
| 3 | 所有產品的5% | 3 | 否 |

在此方案中，規則#1和#2適用於合格產品。 規則#3僅適用於規則#2中未包含的合格產品，因為它的優先順序低於#2例和 **[!UICONTROL Discard Subsequent Rules]** 設定為 `Yes`。 因此，銷售類別中的合格產品將獲得10%的折扣，並享受Amazon上市價2美元的折扣。

### 應用兩個標準價格規則

| 欄位 | 設定 — 規則1 | 設定 — 規則2 |
|----------|----|----|
| [!UICONTROL Rule Name] | 規則1 | 規則2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | 標準價格規則 | 標準價格規則 |
| [!UICONTROL Price action] | 減少者 | 減少者 |
| [!UICONTROL Apply] | 按百分比應用 | 應用為固定金額 |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### 產品1

價格：US$45.49

應用規則1:$45.49 x(0.9)= $40.94

應用規則2:40.94美元 — 10.00美元= 30.94美元

應用規則1和規則2之後的最終價格：US$30.94

#### 產品2

價格：US$47.76

應用規則1:$47.76 x(0.9)= $42.98

應用規則2:42.98美元 — 10.00美元= 32.98美元

應用規則1和規則2之後的最終價格：US$32.98

## 智慧重定價規則示例

### Buy Box價格，最低價格來源=價格

| 欄位 | 設定 |
|----------|----|
| [!UICONTROL Rule Name] | 規則1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 智慧重定價規則 |
| [!UICONTROL Competitor Price Source] | 使用「Buy Box」價格 |
| [!UICONTROL Price Action] | 匹配競爭對手價格 |
| [!UICONTROL Floor Price Source] | 價格 |
| [!UICONTROL Floor Price Action] | 匹配 |

#### 產品1

價格：15美元

[Buy Box](./buy-box-competitor-pricing.md) 來自Amazon的價格：10美元

因為 [Buy Box](./buy-box-competitor-pricing.md) 價格低於原價，按原價列出。

應用規則後的最終價格：15美元

#### 產品2

價格：$5

[Buy Box](./buy-box-competitor-pricing.md) 來自Amazon的價格：10美元

因為 [Buy Box](./buy-box-competitor-pricing.md) 價格大於原價，產品按 [Buy Box](./buy-box-competitor-pricing.md) 價格。

應用規則後的最終價格：10美元

### Buy Box價格，底價來源=價格和降價20%

| 欄位 | 設定 |
|----------|----|
| [!UICONTROL Rule Name] | 規則1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 智慧重定價規則 |
| [!UICONTROL Competitor Price Source] | 使用「Buy Box」價格 |
| [!UICONTROL Price Action] | 匹配競爭對手價格 |
| [!UICONTROL Floor Price Source] | 價格 |
| [!UICONTROL Floor Price Action] | 減少者 |
| [!UICONTROL Apply] | 按百分比應用 |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### 產品1

價格：20美元

計算底價：16美元

[Buy Box](./buy-box-competitor-pricing.md) 來自Amazon的價格：15美元

因為 [Buy Box](./buy-box-competitor-pricing.md) 價格小於已計算 [底價](./floor-price.md)，產品列在「已計算」 [底價](./floor-price.md)。

應用規則後的最終價格：16美元

#### 產品2

價格：15美元

已計算 [底價](./floor-price.md):12美元

[Buy Box](./buy-box-competitor-pricing.md) 來自Amazon的價格：15美元

因為 [Buy Box](./buy-box-competitor-pricing.md) 價格大於已計算 [底價](./floor-price.md)，產品在 [Buy Box](./buy-box-competitor-pricing.md) 價格。

應用規則後的最終價格：15美元

#### 產品3

價格：17美元

計算底價：13.60美元

[Buy Box](./buy-box-competitor-pricing.md) 來自Amazon的價格：15美元

因為 [Buy Box](./buy-box-competitor-pricing.md) 價格大於已計算 [底價](./floor-price.md)，產品在 [Buy Box](./buy-box-competitor-pricing.md) 價格。

應用規則後的最終價格：15美元

### 所有競爭對手的價格和使用所有競爭對手的產品條件的最低價格

| 欄位 | 設定 |
|----------|-----|
| [!UICONTROL Rule Name] | 規則1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 智慧重定價規則 |
| [!UICONTROL Competitor Price Source] | 使用最低競爭對手價格 |
| [!UICONTROL Minimum Positive Feedback] | 所有競爭對手的價格 |
| [!UICONTROL Conditional Variance] | 使用所有競爭對手的產品條件 |
| [!UICONTROL Price Action] | 匹配競爭對手價格 |
| [!UICONTROL Floor Price Source] | 價格 |
| [!UICONTROL Floor Price Action] | 匹配 |

| 價格 | 條件 |
|----------|----|
| $17 | 新建 |
| $15 | 新建 |
| $14 | 已用；非常好 |
| $13 | 已用；好 |

#### 產品1

價格：10美元

條件：新建

由於新條件下最低的競爭對手價格為$15，因此產品的標價為$15。

應用規則後的最終價格：15美元

#### 產品2

價格：10美元

條件：已用；可接受

因為 [最低競爭對手價格](./lowest-competitor-pricing.md) 對於「已使用」條件為$13，產品以$13列出。

應用規則後的最終價格：13美元

### 結合最高價格、幣種折換和增值稅的智慧重新定價規則

| 欄位 | 設定 |
|----------|-----|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | $10 |
| [!UICONTROL Currency conversion] | 1.25歐元：1美元 |

[上限價格](./optional-ceiling-price.md) 在歐洲(VAT)市場：$10 x 1.25 = $12.50

當 [上限](./optional-ceiling-price.md) 在歐洲(VAT)市場受到衝擊時，計算並添加VAT。

增值稅後最終價格：$12.50 x(1.1)= $13.75

### 組合多個定價規則、最高價格、幣種折換和增值稅

#### 智慧定價規則（來自上例）

| 欄位 | 設定 |
|----------|----|
| 優先順序 | 1 |
| 增值稅 | 10% |
| 上限價格來源 | $10 |
| 貨幣兌換 | 1.25歐元：1美元 |

[上限價格](./optional-ceiling-price.md) 在歐洲(VAT)市場：$10 x 1.25 = $12.50

增值稅後最終價格：$12.50 x(1.1)= $13.75

#### 標準定價規則

| 欄位 | 設定 |
|----------|-----|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | 增加者 |
| [!UICONTROL Apply] | 應用為固定金額 |
| [!UICONTROL Adjustment Amount] | $5.00 |

當 [上限](./optional-ceiling-price.md) 在智慧定價規則的基礎上應用標準定價規則。

應用標準定價規則後的最終價格：13.75美元+ 5.00美元= 18.75美元

### 價格調整

在此示例中，最具競爭力的價格是通過查看Amazon [競爭對手的最低價格](./lowest-competitor-pricing.md) 95%的正反饋和1000個商家評論的最低反饋。

![價格調整示例](assets/amazon-price-adjustment-example.png)

根據這些參數運行此搜索後，競爭價格回升至25美元。

從這裡，有三種 [價格規則操作](./pricing-rule-actions.md) 基於最低價格的選擇。

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Price Action] | 選項：<ul><li>**[!UICONTROL Decrease By]**  — 此選項將您的上市價格相對於 [最低競爭對手價格](./lowest-competitor-pricing.md)。</li><li>**[!UICONTROL Increase By]**  — 此選項可提高您的上市價格， [最低競爭對手價格](./lowest-competitor-pricing.md)。</li><li>**[!UICONTROL Match Competitor Price]**  — 此選項將更改您的Amazon上市價格，以根據參數匹配最低價格。 在示例中，Amazon的上市價為$25。</li></ul> |
| [!UICONTROL Apply] | 選項：按百分比應用/按固定金額應用 |
| [!UICONTROL Adjustment Amount] | 用於定義要應用的折扣的百分比或固定金額的數值。 <br>這些選擇會使價格降到最低，並將價格設定為低0.01美元。 |

### 底價

| 欄位 | 設定 |
|----------|----|
| [!UICONTROL Floor Price Source] | 成本= 5美元 |
| [!UICONTROL Floor Price Action] | 增加者 |
| [!UICONTROL Apply] | 按百分比應用 |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[底價](./floor-price.md) 計算=底價來源 `$5` x底部調整金額 `5%` = 5.25美元

應用智慧定價規則時，當成本為$5時，它確實允許此特定產品的上市價格低於$5.25。

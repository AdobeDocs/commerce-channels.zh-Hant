---
title: Amazon銷售管道 — 價格優先順序邏輯
description: Amazon sales channel會套用優先順序來決定Amazon清單的已公佈價格。
feature: Sales Channels, Price Rules
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 4%

---

# 價格優先順序邏輯

在下列範例中，系統如何判斷您應發佈$31.99、$24.99或$27.99？

![商務價格範圍](assets/amazon-price-scope.png){width="400"}

若要在產品位於兩個網站且每個網站的價格各不相同的情況下判斷要使用的價格，請使用價格優先順序邏輯(由以下專案決定： [排序順序](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) 值)。

若要檢視商店的排序順序，請前往 **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** 在 _管理員_ 側欄。 在 _[!UICONTROL Web Site]_欄中，按一下網站名稱。 此_[!UICONTROL Web Site Information]_ 頁面顯示 _[!UICONTROL Sort Order]_網站的設定，可決定網站的優先順序。 值 `1` 表示最高優先順序。

如果產品價格設為 `Use Default`，系統會退回預設價格值，而非網站價格值。

## 範例1

|         | 網站優先順序 | 價格（網站） | 使用預設 |
|---------|------------------|-----------------|-------------|
| 預設 | 0 | $31.99 | — |
| 商店1 | 1 | $24.99 | 否 |
| 商店2 | 2 | $27.99 | 是 |

- 此 **[!UICONTROL Magento Price Source]** (定義於 [上市價格](./listing-price.md) 設為 `Price` 屬性。
- 檢視網站優先順序最高的網站，也就是「商店1」(由 [排序順序](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) 值)。
- 由於商店1設為使用網站價格（使用預設值=否），因此公佈價格為$24.99美元。

## 範例2

|         | 網站優先順序 | 價格網站 | 使用預設 |
|---------|------------------|---------------|-------------|
| 預設 | 0 | $31.99 | -- |
| 商店1 | 1 | $24.99 | 是 |
| 商店2 | 2 | $27.99 | 否 |

- 此 **[!UICONTROL Magento Price Source]** (定義於 [上市價格](./listing-price.md) 設為 `Price` 屬性。
- 檢視網站優先順序最高的網站，也就是「商店1」(由 [排序順序](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) 值)。
- 自從商店1 **不是** 設定為使用網站價格（使用預設值=是），以排序順序檢視下一個網站。
- 自從商店2 **是** 設定為使用網站價格（使用預設值=否），公佈價格為$27.99。

## 範例3

|         | 網站優先順序 | 價格網站 | 使用預設 |
|---------|------------------|---------------|-------------|
| 預設 | 0 | $31.99 | $30.00 |
| 商店1 | 1 | $24.99 | -- |
| 商店2 | 2 | $27.99 | $20.00 |

此範例新增非價格值，如果您為_選取其他值，則會使用此值[!UICONTROL Magento Price Source_] (定義於 [上市價格](./listing-price.md) 設定)。 非價格值一律會使用價格作為遞補價格。

- 此 **[!UICONTROL Magento Price Source]** (定義於 [[!UICONTROL Listing Price]](./listing-price.md) settings)設為 `Non-Price`.
- 檢視網站優先順序最高的網站，也就是 `Store 1`(由定義 [排序順序](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) 值)。
- 自從商店1 **不是** 設定為使用 `Non-Price` 屬性，以排序順序檢視下一個網站。
- 自從商店2 **是** 設定為使用 `Non-Price` 屬性（非價格） [網站] = $20.00)，公佈價格為$20.00。

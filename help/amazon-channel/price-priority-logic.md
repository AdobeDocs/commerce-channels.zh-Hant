---
title: Amazon銷售管道 — 價格優先順序邏輯
description: Amazon sales channel會套用優先順序來決定Amazon清單的已公佈價格。
feature: Sales Channels, Price Rules
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 2%

---

# 價格優先順序邏輯

在下列範例中，系統如何判斷您應發佈$31.99、$24.99或$27.99？

![Commerce價格範圍](assets/amazon-price-scope.png){width="400"}

若要在產品位於兩個網站且每個網站的價格各異時決定使用哪個價格，請使用價格優先順序邏輯（由[排序順序](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)值決定）。

若要檢視商店的排序順序，請前往&#x200B;_管理員_&#x200B;側邊欄中的&#x200B;**[!UICONTROL Stores]** > **[!UICONTROL All Stores]**。 在&#x200B;_[!UICONTROL Web Site]_欄中按一下網站名稱。_[!UICONTROL Web Site Information]_&#x200B;頁面顯示網站的&#x200B;_[!UICONTROL Sort Order]_設定，此設定決定網站的優先順序。 值`1`表示最高優先順序。

如果產品價格設為`Use Default`，則會退回預設價格值，而非網站價格值。

## 範例1

|         | 網站優先順序 | 價格（網站） | 使用預設 |
|---------|------------------|-----------------|-------------|
| 預設 | 0 | 31.99美元 | — |
| 商店1 | 1 | 24.99美元 | 否 |
| 商店2 | 2 | 27.99美元 | 是 |

- **[!UICONTROL Magento Price Source]** （定義在您的[清單價格](./listing-price.md)中）已設定為`Price`屬性。
- 檢視網站優先順序最高的網站，即「商店1」（由[排序順序](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)值定義）。
- 由於商店1設為使用網站價格（使用預設值=否），因此公佈價格為$24.99美元。

## 範例2

|         | 網站優先順序 | 價格網站 | 使用預設 |
|---------|------------------|---------------|-------------|
| 預設 | 0 | 31.99美元 | — |
| 商店1 | 1 | 24.99美元 | 是 |
| 商店2 | 2 | 27.99美元 | 否 |

- **[!UICONTROL Magento Price Source]** （定義在您的[清單價格](./listing-price.md)中）已設定為`Price`屬性。
- 檢視網站優先順序最高的網站，其優先順序為商店1 （由[排序順序](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)值定義）。
- 由於商店1 **未設定為使用網站價格（使用預設值=是），**&#x200B;請依照排序順序檢視下一個網站。
- 由於商店2的&#x200B;**設定為**&#x200B;使用網站價格（使用預設值=否），因此公佈價格為$27.99美元。

## 範例3

|         | 網站優先順序 | 價格網站 | 使用預設 |
|---------|------------------|---------------|-------------|
| 預設 | 0 | 31.99美元 | $30.00 |
| 商店1 | 1 | 24.99美元 | — |
| 商店2 | 2 | 27.99美元 | 20.00美元 |

此範例新增非價格值，如果您為_[!UICONTROL Magento Price Source_]選取其他值（已在您的[清單價格](./listing-price.md)設定中定義），則會使用此值。 非價格值一律會使用價格作為遞補價格。

- **[!UICONTROL Magento Price Source]** （在[[!UICONTROL Listing Price]](./listing-price.md)設定中定義）設定為`Non-Price`。
- 檢視網站優先順序最高的網站，其為`Store 1` （由[排序順序](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)值定義）。
- 由於商店1 **未設定為使用`Non-Price`屬性，**&#x200B;請依照排序順序檢視下一個網站。
- 由於商店2的&#x200B;**已設定為**&#x200B;使用`Non-Price`屬性（非價格[網站] = $20.00），因此公佈價格為$20.00。

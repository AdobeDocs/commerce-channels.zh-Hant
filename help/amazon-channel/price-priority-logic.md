---
title: 價格優先順序邏輯
description: Amazon銷售管道會在決定Amazon上市的已發佈價格時套用優先順序。
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 4%

---

# 價格優先順序邏輯

在以下範例中，系統如何判斷您應發佈$31.99、$24.99或$27.99?

![商務價格範圍](assets/amazon-price-scope.png)

若要在兩個網站上使用產品且每個網站的價格不同時，決定使用哪個價格，請使用價格優先順序邏輯（由[排序順序](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}值決定）。

若要檢視您商店的排序順序，請前往&#x200B;_Admin_&#x200B;側邊欄中的&#x200B;**[!UICONTROL Stores]** > **[!UICONTROL All Stores]**。 在&#x200B;_[!UICONTROL Web Site]_欄中，按一下網站名稱。_[!UICONTROL Web Site Information]_&#x200B;頁面顯示網站的&#x200B;_[!UICONTROL Sort Order]_設定，該設定決定網站的優先順序。 值`1`表示最高優先順序。

如果產品價格設為`Use Default`，則會回落為預設價格值，而非網站價格值。

## 範例1

|  | 網站優先順序 | 價格（網站） | 使用預設值 |
|---|---|---|---|
| 預設 | 0 | US$31.99 | — |
| 商店1 | 3 | US$24.99 | 否 |
| 商店2 | 2 | US$27.99 | 是 |

- **[!UICONTROL Magento Price Source]**（在[Listing Price](./listing-price.md)中定義）設定為`Price`屬性。
- 查看網站優先順序最高的網站，即「商店1」（由[排序順序](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}值定義）。
- 由於Store 1設定為使用網站價格（使用預設值=否），因此發佈的價格為$24.99。

## 範例2

|  | 網站優先順序 | 價格網站 | 使用預設值 |
|---|---|---|---|
| 預設 | 0 | US$31.99 | — |
| 商店1 | 3 | US$24.99 | 是 |
| 商店2 | 2 | US$27.99 | 否 |

- **[!UICONTROL Magento Price Source]**（在[Listing Price](./listing-price.md)中定義）設定為`Price`屬性。
- 查看網站優先順序最高的網站，即「商店1」（由[排序順序](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}值定義）。
- 由於商店1 **未設為使用網站價格（使用預設=是），因此請按排序順序查看下一個網站。**
- 由於Store 2 **是**&#x200B;設為使用網站價格（使用預設值=否），因此發佈價格為$27.99。

## 範例3

|  | 網站優先順序 | 價格網站 | 使用預設值 |
|---|---|---|---|
| 預設 | 0 | US$31.99 | US$30.00 |
| 商店1 | 3 | US$24.99 | — |
| 商店2 | 2 | US$27.99 | US$20.00 |

此示例添加了非價格值，如果您為_[!UICONTROL Magento Price Source_]（在[Listing Price](./listing-price.md)設定中定義）選擇其他值，則會使用該值。 非價格值一律以價格作為備援價格。

- **[!UICONTROL Magento Price Source]**（在[[!UICONTROL Listing Price]](./listing-price.md)設定中定義）設為`Non-Price`。
- 查看網站優先順序最高的網站，其為`Store 1`（由[排序順序](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;}值定義）。
- 由於Store 1 **未設定為使用`Non-Price`屬性，因此請按排序順序查看下一個網站。**
- 由於Store 2 **是**&#x200B;設為使用`Non-Price`屬性（非價格[Website] = $20.00），因此發佈價格為$20.00。

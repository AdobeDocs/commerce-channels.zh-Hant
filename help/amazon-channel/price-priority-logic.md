---
title: 價格優先順序邏輯
description: Amazon銷售渠道於釐定Amazon上市之已公佈價格時應用優先次序。
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 4%

---

# 價格優先順序邏輯

在以下示例中，系統如何確定您是否應發佈$31.99、$24.99或$27.99?

![商業價格範圍](assets/amazon-price-scope.png)

要確定在兩個網站上使用的產品價格，並且每個網站的價格不同，請使用價格優先順序邏輯(由 [排序順序](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){target="_blank"} 值)。

要查看商店的排序順序，請轉到 **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** 的 _管理_ 工具欄。 在 _[!UICONTROL Web Site]_列，按一下網站名稱。 的_[!UICONTROL Web Site Information]_ 頁面顯示 _[!UICONTROL Sort Order]_設定，它確定網站的優先順序。 值 `1` 表示最高優先順序。

如果產品價格設定為 `Use Default`，它會回落到預設價格值而不是網站價格值。

## 示例1

|  | 網站優先順序 | 價格（網站） | 使用預設值 |
|---|---|---|---|
| 預設 | 0 | $31.99 | -- |
| 儲存1 | 1 | $24.99 | 否 |
| 儲存2 | 2 | $27.99 | 是 |

- 的 **[!UICONTROL Magento Price Source]** (定義於 [上市價格](./listing-price.md) 設定為 `Price` 屬性。
- 查看網站優先順序最高的網站，即第1商店(由 [排序順序](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){target="_blank"} 值)。
- 由於「應用商店1」設定為使用網站價格（使用預設值=否），因此發佈的價格為$24.99。

## 示例2

|  | 網站優先順序 | 價格網站 | 使用預設值 |
|---|---|---|---|
| 預設 | 0 | $31.99 | -- |
| 儲存1 | 1 | $24.99 | 是 |
| 儲存2 | 2 | $27.99 | 否 |

- 的 **[!UICONTROL Magento Price Source]** (定義於 [上市價格](./listing-price.md) 設定為 `Price` 屬性。
- 查看網站優先順序最高的網站，即第1商店(由 [排序順序](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){target="_blank"} 值)。
- 自儲存1 **不是** 設定為使用網站價格（使用預設值=是），按排序順序查看下一個網站。
- 自儲存2 **是** 設定為使用網站價格（使用預設值=否），發佈的價格為$27.99。

## 示例3

|  | 網站優先順序 | 價格網站 | 使用預設值 |
|---|---|---|---|
| 預設 | 0 | $31.99 | $30.00 |
| 儲存1 | 1 | $24.99 | -- |
| 儲存2 | 2 | $27.99 | $20.00 |

此示例將添加非價格值，如果為_選擇另一個值，則使用該值[!UICONTROL Magento Price Source_] (定義於 [上市價格](./listing-price.md) )。 非價格值始終使用價格作為回退價格。

- 的 **[!UICONTROL Magento Price Source]** (定義於 [[!UICONTROL Listing Price]](./listing-price.md) 設定)設定為 `Non-Price`。
- 查看網站優先順序最高的網站， `Store 1`(由 [排序順序](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){target="_blank"} 值)。
- 自儲存1 **不是** 設定為使用 `Non-Price` 屬性，按排序順序查看下一個網站。
- 自儲存2 **是** 設定為使用 `Non-Price` 屬性（非價格） [網站] = 20.00美元)，發佈價格為20.00美元。

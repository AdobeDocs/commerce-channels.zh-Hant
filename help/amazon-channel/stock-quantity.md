---
title: 庫存/數量
description: 控制將產品數量詳細資訊從Commerce商店同步到 [!DNL Amazon Seller Central] 帳戶，更新庫存/數量設定。
redirect_from: /sales-channels/asc/ob-stock-quantity.html
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# 庫存/數量

*[!UICONTROL Stock/Quantity]* 設定是儲存清單設定的一部分。 從 [儲存儀表板](./amazon-store-dashboard.md)。

這些設定用於同步您的產品數量詳細資訊 [!DNL Commerce] 儲存到您的 [!DNL Amazon Seller Central] 帳戶。 此工具功能強大，可通過向購買者顯示緊急情況，同時保持庫存有條不紊，用於附加廣告。 例如，一些商戶的倉庫中可能存有150件特定SKU的物品，並希望確保Amazon購物者能夠購買他們的所有庫存。 其他商家可能希望一次只列出一個商品，以便給最終用戶造成稀缺感。 在此情況下，設定 *[!UICONTROL Maximum Listed Quantity]* 至 `1`。

數量是區域屬性，並基於 **[!UICONTROL Amazon Marketplace Country]** 設定定義 [儲存整合](./store-integration.md)。 當對產品數量進行更改時，該更改將影響共用該產品的所有Amazon清單 [!DNL Amazon Seller SKU] 在你Amazon的店裡賣的。 對共用的更改 [!DNL Amazon Seller SKU] 在美國，不會影響你為另一個國家設立的Amazon店。 整合的第一個Amazon商店（具有最早的建立日期）控制數量設定中的優先順序。

>[!NOTE]
>
>對於Adobe Commerce和Magento Open Source2.3.x用戶，Amazon銷售渠道支援使用Inventory management擴展，而不需要任何附加設定。 請參閱 [管理庫存](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target="_blank"}。

## 配置庫存/數量設定 {#configure-stock--quantity-settings}

1. 按一下 **[!UICONTROL Listing Settings]** 在商店儀表板上。

1. 展開 **[!UICONTROL Stock / Quantity]** 的子菜單。

1. 對於 **[!UICONTROL Out-of-Stock Threshold]** （必需），輸入產品最小數量的數值，以使產品符合其Amazon清單的條件。

   預設值為 `0`。 如果 [!DNL Commerce] 產品庫存低於此數量，相應的Amazon上市不符合通過Amazon銷售的條件。

1. 對於 **[!UICONTROL Maximum Listed Quantity]** （必需），輸入要在Amazon清單中顯示的數量的數值。

   此設定以輸入的值列出所有符合條件的Amazon清單。 銷售物料時，Amazon清單數量不會更改。 即使您的實際產品數量高於或低於此值，可用清單數量也始終使用此值。 此設定通常在您不管理產品庫存時使用。 例如，您的產品中可能包含數量為80的產品 [!DNL Commerce] 目錄。 設定為 `10`,Amazon清單始終顯示 `10` 產品銷售時不變。

1. 對於 **[!UICONTROL "Do Not Manage Stock" Quantity]** （必需），輸入要為您的Amazon清單顯示的數量值。

   Amazon要求您發佈可用數量。 對於 [!DNL Commerce] 設定為不管理庫存，但您希望將其列在Amazon的產品中，將在此處輸入可用數量後發佈該清單。

1. 完成後，按一下 **[!UICONTROL Save listing settings]**。

![庫存/數量設定](assets/amazon-stock-quantity.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | 輸入產品最小數量的數值，以使產品符合其Amazon清單的條件(預設值為 `0`)。<br><br>如果 [!DNL Commerce] 產品庫存低於此數量，相應的Amazon上市不符合通過Amazon銷售的條件。 |
| [!UICONTROL Maximum Listed Quantity] | 輸入要在Amazon清單中顯示的數量的數值。<br><br>銷售物料時，Amazon清單將重新發佈此處輸入的數量。 此設定通常在您不管理產品庫存時使用。<br><br>例如，您將「列出的數量最大值」輸入為 `10`。 產品的實際數量是 `80`。 因為您已將此值設定為 `10`,Amazon清單始終顯示 `10`。 即使庫存數量較少，也始終以定義的值顯示可用數量。 |
| [!UICONTROL "Do Not Manage Stock" Quantity] | 為您的Amazon清單輸入顯示數量的值。<br><br>Amazon要求您發佈可用數量。 對於 [!DNL Commerce] 設定為不管理庫存，但您希望將其列在Amazon的產品中，此清單將以此處輸入的可用數量發佈。 |

**快速訪問** - [!UICONTROL Listing Settings] 節

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## 示例：列出的最大數量

銷售物料時，Amazon清單將重新確定此數量。

例如，如果 *[!UICONTROL Maximum Listed Quantity]* 如 `12`,Amazon清單顯示的數量為12，即使產品 [!DNL Commerce] 80的數量：

![最大列出數量示例1](assets/amazon-max-listed-quantity.png)

如果你 *[!UICONTROL Maximum Listed Quantity]* 如 `1`，所有合格產品都列有 `1`。 銷售物料時，系統將查找 [!DNL Commerce] 產品，如果存在額外庫存，則用數量 `1`。

對於通常訂購數量為1的產品，此選項可能非常有價值。 這也增加了購物者在查看你的Amazon上市時的緊迫性。

![最大列出數量示例2](assets/amazon-max-listed-quantity-1.png)

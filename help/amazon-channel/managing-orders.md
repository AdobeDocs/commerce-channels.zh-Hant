---
title: 管理訂單
description: 您可以在「訂單設定」中啟用訂單匯入，以便從商務管理員輕鬆管理Amazon訂單。
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 管理訂單

您可以在[儲存控制面板](./amazon-store-dashboard.md)的&#x200B;_[!UICONTROL Recent Orders]_區段或_[!UICONTROL Amazon orders]_&#x200B;頁面（亦稱為&#x200B;_[!UICONTROL All Orders]_檢視）中，檢視從Amazon收到的Amazon訂單資訊。

如何管理Amazon訂單，取決於您的[訂單設定](./order-settings.md#configure-order-settings)中是啟用還是停用訂單匯入。

## 啟用訂單導入

在[儲存整合](./store-integration.md)之後，預設情況下，[**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings)設定為`Enabled`。 使用此設定，會為您的Amazon訂單建立對應的[!DNL Commerce]訂單，並可在[[!DNL Commerce] Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}工作流程中管理。

>[!NOTE]
>
>無論訂單匯入設定為何，在[store integration](./store-integration.md)之前，您的[!DNL Amazon Seller Central]帳戶中存在的Amazon訂單都不會匯入。

匯入的Amazon訂單在[[!DNL Commerce] Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}工作流程中進行管理，就像其他[!DNL Commerce]商店一樣。 按一下&#x200B;*[!UICONTROL Order Number]*&#x200B;欄中的Amazon訂單編號，開啟[[!DNL Commerce] order process](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target=&quot;_blank&quot;}中的訂單。 請參閱[檢視Amazon訂單](./amazon-orders-all.md)。

### 訂單導入流程

在Amazon上下訂單並啟用[order import](./order-settings.md)後，以下過程將開始。

| 變更 | 動作 |
|---|---|
| 對Amazon下單。 | <ul><li>Amazon會將順序狀態設為`Pending`。</li><li>訂單資訊將發送到[!DNL Commerce]。</li><li>將順序新增至狀態為`Pending`的&#x200B;[_Amazon訂單_&#x200B;表](./amazon-orders-all.md)。</li></ul> |
| Amazon將訂單狀態變更為`Unshipped`。 | <ul><li>狀態更改將發送到[!DNL Commerce]。</li><li>在&#x200B;[_Amazon訂單_&#x200B;表](./amazon-orders-all.md)中，訂單狀態變更為`Unshipped`。</li><li>在[[!DNL Commerce] orders workflow](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}中，建立具有`Processing`狀態的相應[!DNL Commerce]順序。</li></ul> |
| 在[[!DNL Commerce] orders workflow](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}中，會處理[!DNL Commerce]訂單，且狀態會變更為`Shipped`。 | <ul><li>在&#x200B;[_Amazon訂單_&#x200B;表](./amazon-orders-all.md)中，訂單狀態變更為`Shipped`。</li><li>在下一個cron作業中，訂單狀態在[[!DNL Commerce] orders workflow](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}中變更為`Complete`。</li></ul> |

### 訂單建立封鎖程式

有一些情況會阻止建立相應的[!DNL Commerce]順序。 [!DNL Commerce] 系統不會針對發生下列任何問題時收到的訂單建立訂單。

| 藍本 | 解決方案 |
|---|---|
| [!DNL Commerce]目錄中不存在該項。 | [在目錄](./creating-assigning-catalog-products.md) 中建立 [!DNL Commerce] 產品， [並手](./creating-assigning-catalog-products.md) 動將其與產品配對。 |
| 目錄中的項目已停用。 | 請確定已啟用[產品狀態](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;}。 |
| 訂購的物料無存貨。 | 更新或配置數量和源的[產品選項](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;}。 |

當無法匯入訂單時，螢幕頂端會顯示類似下列的系統訊息：

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

問題解決後，會在下次同步時建立[!DNL Commerce]順序。

## 禁用訂單導入

如果您不想在[!DNL Commerce]中匯入和管理Amazon訂單，可將[**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings)設定變更為`Disabled`。 此設定表示從Amazon收到新訂單時，不會建立對應的[!DNL Commerce]訂單。

停用後，從Amazon收到的訂單資訊會顯示在存放區控制面板的&#x200B;_[!UICONTROL Recent Orders]_區段和_[!UICONTROL All Orders]_&#x200B;檢視中。 此訂單資訊僅供查看，您必須在[!DNL Amazon Seller Central]中管理這些訂單。 若要開啟[!DNL Amazon Seller Central]中的訂單詳細資訊，請按一下&#x200B;_[!UICONTROL Order Number]_欄中的Amazon訂單編號。

另請參閱[查看Amazon訂單](./amazon-orders-all.md)、[查看Amazon訂單詳細資訊](./amazon-order-details.md)和[常見訂單處理任務](./common-order-processing.md)。

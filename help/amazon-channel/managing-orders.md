---
title: 管理Amazon訂單
description: 您可以在「訂單設定」中啟用訂單匯入，以便更輕鬆地從Commerce管理員管理Amazon訂單。
feature: Sales Channels, Orders
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 管理Amazon訂單

從Amazon收到的資料中，您可以在[存放區儀表板](./amazon-store-dashboard.md)的&#x200B;_[!UICONTROL Recent Orders]_區段或_[!UICONTROL Amazon orders]_&#x200B;頁面（也稱為&#x200B;_[!UICONTROL All Orders]_檢視）上檢視您的Amazon訂單資訊。

您管理Amazon訂單的方式取決於您的[訂單設定](./order-settings.md#configure-order-settings)中是否啟用或停用訂單匯入。

## 啟用訂單匯入

在[存放區整合](./store-integration.md)之後，[**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings)設定預設為`Enabled`。 透過此設定，可為您的Amazon訂單建立對應的[!DNL Commerce]訂單，並可在[[!DNL Commerce] 訂單](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)工作流程中進行管理。

>[!NOTE]
>
>無論您的訂單匯入設定為何，在您的[存放區整合](./store-integration.md)之前存在於您[!DNL Amazon Seller Central]帳戶中的Amazon訂單都不會匯入。

匯入的Amazon訂單在[[!DNL Commerce] 訂單](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)工作流程中進行管理，就像您的其他[!DNL Commerce]存放區一樣。 按一下&#x200B;*[!UICONTROL Order Number]*&#x200B;欄中的Amazon訂單編號以開啟[[!DNL Commerce] 訂單程式](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-view-descriptions)中的訂單。 請參閱[檢視Amazon訂單](./amazon-orders-all.md)。

### 訂單匯入程式

在Amazon上下達訂單，並啟用[訂單匯入](./order-settings.md)時，下列程式就會開始。

| 變更 | 動作 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 在Amazon下訂單。 | <ul><li>Amazon將訂單狀態設為`Pending`。</li><li>訂單資訊已傳送至[!DNL Commerce]。</li><li>訂單已新增至&#x200B;[_Amazon訂單_&#x200B;資料表](./amazon-orders-all.md)，且狀態為`Pending`。</li></ul> |
| Amazon會將訂單狀態變更為`Unshipped`。 | <ul><li>狀態變更已傳送至[!DNL Commerce]。</li><li>在&#x200B;[_Amazon訂單_&#x200B;資料表](./amazon-orders-all.md)中，訂單狀態變更為`Unshipped`。</li><li>在[[!DNL Commerce] 訂單工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)中，已建立具有`Processing`狀態的對應[!DNL Commerce]訂單。</li></ul> |
| 在[[!DNL Commerce] 訂單工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)中，已處理[!DNL Commerce]訂單且狀態變更為`Shipped`。 | <ul><li>在&#x200B;[_Amazon訂單_&#x200B;資料表](./amazon-orders-all.md)中，訂單狀態變更為`Shipped`。</li><li>在下一個cron工作上，[[!DNL Commerce] 訂單工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)中的訂單狀態變更為`Complete`。</li></ul> |

### 訂單建立封鎖程式

有一些案例會阻止建立對應的[!DNL Commerce]順序。 未針對發生下列任何問題時收到的訂單建立[!DNL Commerce]個訂單。

| 情境 | 解決方案 |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 專案不存在於[!DNL Commerce]目錄中。 | [在您的[!DNL Commerce]目錄中建立產品](./creating-assigning-catalog-products.md)，並[手動比對](./creating-assigning-catalog-products.md)該產品與產品。 |
| 目錄中的專案已停用。 | 請確定[產品狀態](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html)已啟用。 |
| 訂購料號無庫存。 | 更新或設定數量與來源的[產品選項](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html)。 |

當無法匯入訂單時，類似下列的系統訊息會出現在畫面頂端：

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

問題解決後，會在下次同步處理時建立[!DNL Commerce]訂單。

## 已停用訂單匯入

如果您不想要在[!DNL Commerce]中匯入及管理您的Amazon訂單，您可以將[**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings)設定變更為`Disabled`。 此設定表示從Amazon收到新訂單時，不會建立對應的[!DNL Commerce]訂單。

停用時，從Amazon收到的訂單資訊會顯示在商店儀表板的&#x200B;_[!UICONTROL Recent Orders]_區段和_[!UICONTROL All Orders]_&#x200B;檢視中。 此訂單資訊僅供檢視，您必須在[!DNL Amazon Seller Central]中管理這些訂單。 若要在[!DNL Amazon Seller Central]中開啟訂單詳細資料，請按一下&#x200B;_[!UICONTROL Order Number]_欄中的Amazon訂單編號。

另請參閱[檢視Amazon訂單](./amazon-orders-all.md)、[檢視Amazon訂單詳細資料](./amazon-order-details.md)和[常見訂單處理工作](./common-order-processing.md)。

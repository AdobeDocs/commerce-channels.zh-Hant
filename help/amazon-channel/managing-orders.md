---
title: 管理訂單
description: 您可以在「訂單設定」中啟用訂單匯入，以便從商務管理員輕鬆管理Amazon訂單。
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 1d1b888db4de4f6e3658af768cd6f5cf30828788
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 管理訂單

您可以在以下位置檢視從Amazon收到的Amazon訂單資訊： _[!UICONTROL Recent Orders]_區段 [儲存儀表板](./amazon-store-dashboard.md) 或_[!UICONTROL Amazon orders]_ 頁面(又稱為 _[!UICONTROL All Orders]_檢視)。

如何管理Amazon訂單，取決於您的 [順序設定](./order-settings.md#configure-order-settings).

## 啟用訂單導入

之後 [商店整合](./store-integration.md), [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 設定 `Enabled` 依預設。 使用此設定，會對應 [!DNL Commerce] 系統會為您的Amazon訂單建立訂單，並可在 [[!DNL Commerce] 訂購](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}工作流程。

>[!NOTE]
>
>無論訂單匯入設定為何，Amazon訂單都存在於 [!DNL Amazon Seller Central] 帳戶 [商店整合](./store-integration.md) 未匯入。

匯入的Amazon訂單會在 [[!DNL Commerce] 訂購](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}工作流，就像您的其他工作流 [!DNL Commerce] 商店。 按一下 *[!UICONTROL Order Number]* 欄以開啟 [[!DNL Commerce] 訂單處理](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target=&quot;_blank&quot;}。 請參閱 [檢視Amazon訂單](./amazon-orders-all.md).

### 訂單導入流程

下訂單時，Amazon和 [訂單匯入](./order-settings.md) 啟用後，下列程式就會開始。

| 變更 | 動作 |
|---|---|
| 對Amazon下單。 | <ul><li>Amazon將訂單狀態設為 `Pending`.</li><li>訂單資訊傳送至 [!DNL Commerce].</li><li>訂單已新增至 [_Amazon訂購_ 表格](./amazon-orders-all.md) 帶 `Pending` 狀態。</li></ul> |
| Amazon將訂單狀態變更為 `Unshipped`. | <ul><li>狀態變更會傳送至 [!DNL Commerce].</li><li>在 [_Amazon訂購_ 表格](./amazon-orders-all.md)，訂單狀態會變更為 `Unshipped`.</li><li>在 [[!DNL Commerce] 訂購工作流](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}，對應的 [!DNL Commerce] 使用 `Processing` 狀態。</li></ul> |
| 在 [[!DNL Commerce] 訂購工作流](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}, [!DNL Commerce] 處理訂單，且狀態變更為 `Shipped`. | <ul><li>在 [_Amazon訂購_ 表格](./amazon-orders-all.md)，訂單狀態會變更為 `Shipped`.</li><li>在下一個cron作業上，訂單狀態會變更為 `Complete` 在 [[!DNL Commerce] 訂購工作流](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}。</li></ul> |

### 訂單建立封鎖程式

有些情況會防止建立對應的 [!DNL Commerce] 順序。 [!DNL Commerce] 系統不會針對發生下列任何問題時收到的訂單建立訂單。

| 藍本 | 解決方案 |
|---|---|
| 項目不存在於 [!DNL Commerce] 目錄。 | [建立產品](./creating-assigning-catalog-products.md) 在 [!DNL Commerce] 目錄和 [手動比對](./creating-assigning-catalog-products.md) 它和產品。 |
| 目錄中的項目已停用。 | 請確定 [產品狀態](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target=&quot;_blank&quot;}已啟用。 |
| 訂購的物料無存貨。 | 更新或設定 [產品選項](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target=&quot;_blank&quot;}表示數量和來源。 |

當無法匯入訂單時，螢幕頂端會顯示類似下列的系統訊息：

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

問題解決後， [!DNL Commerce] 下次同步時會建立訂單。

## 禁用訂單導入

如果您不想在 [!DNL Commerce]，您可以變更 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 設定為 `Disabled`. 此設定表示從Amazon收到新訂單時，會對應 [!DNL Commerce] 不會建立訂單。

停用時，從Amazon收到的訂單資訊會顯示在 _[!UICONTROL Recent Orders]_儲存控制面板的區段中_[!UICONTROL All Orders]_ 檢視。 此訂單資訊僅供檢視，您必須在 [!DNL Amazon Seller Central]. 要在中開啟訂單詳細資訊，請執行以下操作： [!DNL Amazon Seller Central]，按一下 _[!UICONTROL Order Number]_欄。

另請參閱 [檢視Amazon訂單](./amazon-orders-all.md), [檢視Amazon訂單詳細資料](./amazon-order-details.md)，和 [常見訂單處理任務](./common-order-processing.md).

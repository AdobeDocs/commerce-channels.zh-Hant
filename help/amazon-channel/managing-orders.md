---
title: 管理Amazon訂單
description: 您可以在「訂單設定」中啟用訂單匯入，以便更輕鬆地從商務管理員管理您的Amazon訂單。
feature: Sales Channels, Orders
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 管理Amazon訂單

從Amazon接收到Amazon訂單資訊後，您可在以下網址檢視： _[!UICONTROL Recent Orders]_的區段 [存放區儀表板](./amazon-store-dashboard.md) 或在_[!UICONTROL Amazon orders]_ 頁面(也稱為 _[!UICONTROL All Orders]_檢視)。

您管理Amazon訂單的方式，取決於您的訂單匯入是否啟用 [訂單設定](./order-settings.md#configure-order-settings).

## 啟用訂單匯入

晚於 [存放區整合](./store-integration.md)，則 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 設定為 `Enabled` 依預設。 透過此設定，對應至 [!DNL Commerce] 系統會為您的Amazon訂單建立訂單，並可於以下位置管理： [[!DNL Commerce] 訂購](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) 工作流程。

>[!NOTE]
>
>無論您的訂單匯入設定為何，您電腦中現有的Amazon訂單 [!DNL Amazon Seller Central] 您之前的帳戶 [存放區整合](./store-integration.md) 不會匯入。

匯入的Amazon訂單管理於 [[!DNL Commerce] 訂購](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) 工作流程，就像您的其他工作流程一樣 [!DNL Commerce] 商店。 Amazon按一下 *[!UICONTROL Order Number]* 欄以開啟中的順序 [[!DNL Commerce] 訂購流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-view-descriptions). 另請參閱 [檢視Amazon訂單](./amazon-orders-all.md).

### 訂單匯入程式

在Amazon上下達訂單時，以及 [訂單匯入](./order-settings.md) 已啟用，下列程式將開始。

| 變更 | 動作 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 在Amazon下訂單。 | <ul><li>Amazon將訂單狀態設為 `Pending`.</li><li>訂單資訊已傳送至 [!DNL Commerce].</li><li>訂單已新增至 [_Amazon訂單_ 表格](./amazon-orders-all.md) 與 `Pending` 狀態。</li></ul> |
| Amazon會將訂單狀態變更為 `Unshipped`. | <ul><li>狀態變更已傳送至 [!DNL Commerce].</li><li>在 [_Amazon訂單_ 表格](./amazon-orders-all.md)，訂單狀態會變更為 `Unshipped`.</li><li>在 [[!DNL Commerce] 訂單工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)，對應 [!DNL Commerce] 訂單是使用 `Processing` 狀態。</li></ul> |
| 在 [[!DNL Commerce] 訂單工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)，則 [!DNL Commerce] 訂單已處理且狀態已變更為 `Shipped`. | <ul><li>在 [_Amazon訂單_ 表格](./amazon-orders-all.md)，訂單狀態會變更為 `Shipped`.</li><li>在下一個cron作業中，訂單狀態將變更為 `Complete` 在 [[!DNL Commerce] 訂單工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).</li></ul> |

### 訂單建立封鎖程式

有一些案例會阻止建立對應的 [!DNL Commerce] 訂購。 [!DNL Commerce] 當發生下列任何問題時，不會為收到的訂單建立訂單。

| 情境 | 解決方案 |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 此專案不存在於 [!DNL Commerce] 目錄。 | [建立產品](./creating-assigning-catalog-products.md) 在您的 [!DNL Commerce] 目錄和 [手動比對](./creating-assigning-catalog-products.md) 它對應到產品。 |
| 目錄中的專案已停用。 | 確定 [產品狀態](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) 已啟用。 |
| 訂購料號無庫存。 | 更新或設定 [產品選項](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) 數量與來源。 |

當無法匯入訂單時，類似下列的系統訊息會出現在畫面頂端：

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

問題解決後， [!DNL Commerce] 訂單會在下次同步處理時建立。

## 已停用訂單匯入

如果您不想在中匯入及管理您的Amazon訂單 [!DNL Commerce]，您可以變更 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 將設為 `Disabled`. 此設定表示從Amazon收到新訂單時，需對應至 [!DNL Commerce] 未建立訂單。

停用時，從Amazon收到的訂單資訊會出現在 _[!UICONTROL Recent Orders]_區段和_[!UICONTROL All Orders]_ 檢視。 此訂單資訊僅供檢視，您必須管理下列訂單： [!DNL Amazon Seller Central]. 若要在中開啟訂單詳細資料，請執行下列步驟： [!DNL Amazon Seller Central]，按一下中的Amazon訂單編號 _[!UICONTROL Order Number]_欄。

另請參閱 [檢視Amazon訂單](./amazon-orders-all.md)， [檢視Amazon訂單詳細資料](./amazon-order-details.md)、和 [常見訂單處理作業](./common-order-processing.md).

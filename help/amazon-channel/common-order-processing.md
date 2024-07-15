---
title: 常見Amazon訂單處理任務
description: 使用為Amazon訂單建立的對應 [!DNL Commerce] 訂單，在[!UICONTROL Commerce]管理員中管理訂單活動和處理。
feature: Sales Channels, Orders
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 常見Amazon訂單處理任務

[Commerce訂單處理](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)可以管理您的Amazon訂單，包括傳送電子郵件給買家、完成訂單（出貨）、簽發信用額度/退款、新增註解等等。 若要管理您的Amazon訂單，您的&#x200B;[**匯入Amazon訂單**](./order-settings.md)&#x200B;設定必須設為`Enabled`，以便在收到Amazon訂單時建立對應的[!DNL Commerce]訂單。 Amazon訂單資訊會顯示在商店儀表板的&#x200B;*[!UICONTROL Recent Orders]*&#x200B;區段中。

啟用後，會為Amazon訂單建立對應的[!DNL Commerce]訂單，且Amazon訂單編號會顯示在&#x200B;_[!UICONTROL Order Number]_欄中。 如果已建立對應的[!DNL Commerce]訂單，請按一下訂單編號，以在[Commerce訂單處理](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)頁面中開啟訂單。 您可以像處理其他[[!DNL Commerce] 訂單一樣管理訂單](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)。

[!DNL Commerce]訂單編號未顯示&#x200B;_[!UICONTROL Recent Orders]_資訊。 只有當您按一下商店儀表板上的訂單編號，並在[Commerce訂單處理](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)中開啟訂單時，才會顯示Commerce訂單編號。 檢視[!DNL Commerce]訂單時，Amazon訂單編號會出現在&#x200B;*[!UICONTROL Payment & Shipping Method]*區段中。 它還包含&#x200B;*[!UICONTROL View or Cancel Amazon Order]*和&#x200B;*[!UICONTROL View all Amazon Orders]*的選項（視訂單送貨狀態而定）。

請參閱[取消未送出的訂單](./cancel-unshipped-order.md)。

![Commerce訂單中的Amazon訂單資訊](assets/amazon-order-number-payment-info.png){width="500"}

處理Amazon訂單時，Amazon銷售管道會更新訂單資訊，並將其與您的[!DNL Amazon Seller Central]帳戶同步。 您的cron設定會決定訂單資訊在Amazon與Amazon銷售管道之間同步的頻率。

常見的Commerce [訂單處理](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)工作包括：

- [排序動作](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions)
- [訂單搜尋](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [處理訂單](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
   - [檢視訂單](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
   - [處理訂單](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
   - [訂單與帳戶資訊](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
   - [地址資訊](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
   - [付款與送貨方式](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
   - [檢閱訂購的專案](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)
- [簽發退款](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [履行/運送訂單](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [建立發票](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [取消未出貨的訂單](./cancel-unshipped-order.md)

>[!NOTE]
>
>如果訂單處於`Unshipped`狀態，您可以在[[!UICONTROL Amazon Order Details]](./amazon-order-details.md)頁面上[取消Amazon訂單](./cancel-unshipped-order.md)。 如果訂單已出貨，則無法取消。

請參閱[Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations)。

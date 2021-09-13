---
title: 常見訂單處理任務
description: 使用對應的 [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] 管理。
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# 常見訂單處理任務

[[!DNL Commerce] 訂單處理](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}可管理您的Amazon訂單，包括寄送電子郵件給買家、履行訂單（運送）、核發信用/退款、新增評論等。若要管理Amazon訂單，您的&#x200B;[**匯入Amazon訂單**](./order-settings.md)&#x200B;設定必須設為`Enabled`，以便在收到Amazon訂單時建立對應的[!DNL Commerce]訂單。 Amazon訂單資訊會顯示在存放區控制面板的&#x200B;*[!UICONTROL Recent Orders]*&#x200B;區段中。

啟用後，會為Amazon訂單建立對應的[!DNL Commerce]訂單，而Amazon訂單編號會顯示在&#x200B;_[!UICONTROL Order Number]_欄中。 如果建立了相應的[!DNL Commerce]順序，請按一下訂單編號以開啟[!DNL Commerce] [訂單處理](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}頁面中的訂單。 您可以像處理其他[[!DNL Commerce] 訂單一樣管理訂單](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}。

[!DNL Commerce]訂單編號未隨&#x200B;_[!UICONTROL Recent Orders]_資訊顯示。 [!DNL Commerce]訂單編號僅在您按一下商店控制面板上的訂單編號，並在[[!DNL Commerce] 訂單處理](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}中開啟訂單時顯示。 檢視[!DNL Commerce]順序時，Amazon訂單編號會顯示在&#x200B;*[!UICONTROL Payment & Shipping Method]*區段中。 它還包括&#x200B;*[!UICONTROL View or Cancel Amazon Order]*和&#x200B;*[!UICONTROL View all Amazon Orders]*的選項，具體取決於訂單發運狀態。

請參閱[取消未發運的訂單](./cancel-unshipped-order.md)。

![Amazon商務訂單中的訂單資訊](assets/amazon-order-number-payment-info.png)

處理Amazon訂單時，Amazon銷售管道會更新訂單資訊並與您的[!DNL Amazon Seller Central]帳戶同步。 您的cron設定會決定在Amazon和Amazon銷售管道之間同步訂單資訊的頻率。

常見[!DNL Commerce] [訂單處理](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}任務包括：

- [訂購操作](https://docs.magento.com/user-guide/sales/order-actions.html){target=&quot;_blank&quot;}
- [訂購搜索](https://docs.magento.com/user-guide/sales/orders-search.html){target=&quot;_blank&quot;}
- [處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}
   - [檢視順序](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target=&quot;_blank&quot;}
   - [處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target=&quot;_blank&quot;}
   - [訂單和帳戶資訊](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target=&quot;_blank&quot;}
   - [地址資訊](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target=&quot;_blank&quot;}
   - [付款和運送方法](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target=&quot;_blank&quot;}
   - [查看已排序的項](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target=&quot;_blank&quot;}
- [核發貸項/退款](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target=&quot;_blank&quot;}
- [履行/發運訂單](https://docs.magento.com/user-guide/sales/shipments-create.html){target=&quot;_blank&quot;}
- [建立發票](https://docs.magento.com/user-guide/sales/invoice-create.html){target=&quot;_blank&quot;}
- [取消未發運的訂單](./cancel-unshipped-order.md)

>[!NOTE]
>
>如果訂單處於`Unshipped`狀態，您可以在[[!UICONTROL Amazon Order Details]](./amazon-order-details.md)頁面上[取消Amazon訂單](./cancel-unshipped-order.md)。 如果訂單已發運，則無法取消。

請參閱[商務訂單管理](https://docs.magento.com/user-guide/sales/order-management.html){target=&quot;_blank&quot;}。

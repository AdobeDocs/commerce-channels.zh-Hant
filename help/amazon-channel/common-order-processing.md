---
title: 普通訂單處理任務
description: 使用相應 [!DNL Commerce] 為Amazon訂單建立的訂單，以管理訂單活動和處理 [!UICONTROL Commerce] 管理員。
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 普通訂單處理任務

[[!DNL Commerce] 訂單處理](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} 可以管理您的Amazon訂單，包括給買家發送電子郵件、完成訂單（發運）、發放信用額度/退款、添加評論等。 為了管理您的Amazon訂單， [**導入Amazon訂單**](./order-settings.md) 設定必須設定為 `Enabled` 這樣對應 [!DNL Commerce] 在收到Amazon訂單時建立訂單。 Amazon訂單資訊顯示於 *[!UICONTROL Recent Orders]* 的子菜單。

啟用時，相應 [!DNL Commerce] 為Amazon訂單建立訂單，Amazon訂單編號顯示在 _[!UICONTROL Order Number]_的雙曲餘切值。 如果對應 [!DNL Commerce] 訂單已建立，按一下訂單編號以在 [!DNL Commerce] [訂單處理](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} page. You can manage the order as you do your other [[!DNL Commerce] order processing](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}。

的 [!DNL Commerce] 訂單編號不顯示 _[!UICONTROL Recent Orders]_的下界。 的 [!DNL Commerce] 訂單編號僅在您按一下商店控制面板上的訂單編號並開啟訂單時顯示 [[!DNL Commerce] 訂單處理](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}。 查看 [!DNL Commerce] 訂單，Amazon訂單號顯示在&#x200B;*[!UICONTROL Payment & Shipping Method]*的子菜單。 它還包括&#x200B;*[!UICONTROL View or Cancel Amazon Order]*和&#x200B;*[!UICONTROL View all Amazon Orders]*，具體取決於訂單發運狀態。

請參閱 [取消未發運訂單](./cancel-unshipped-order.md)。

![Amazon商務訂單中的訂單資訊](assets/amazon-order-number-payment-info.png)

處理Amazon訂單時，Amazon銷售渠道會更新訂單資訊並與您的 [!DNL Amazon Seller Central] 帳戶。 您的cron設定確定訂單資訊在Amazon和Amazon銷售渠道之間同步的頻率。

常用 [!DNL Commerce] [訂單處理](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} 任務包括：

- [訂單操作](https://docs.magento.com/user-guide/sales/order-actions.html){target="_blank"}
- [訂單搜索](https://docs.magento.com/user-guide/sales/orders-search.html){target="_blank"}
- [處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}
   - [查看訂單](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target="_blank"}
   - [處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target="_blank"}
   - [訂單和帳戶資訊](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target="_blank"}
   - [地址資訊](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target="_blank"}
   - [付款和發運方法](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target="_blank"}
   - [複查訂購的物料](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target="_blank"}
- [發放貸項/退款](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target="_blank"}
- [履行/發運訂單](https://docs.magento.com/user-guide/sales/shipments-create.html){target="_blank"}
- [建立發票](https://docs.magento.com/user-guide/sales/invoice-create.html){target="_blank"}
- [取消未發運訂單](./cancel-unshipped-order.md)

>[!NOTE]
>
>如果訂單在 `Unshipped` 狀態，您可以 [取消Amazon訂單](./cancel-unshipped-order.md) 的 [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) 的子菜單。 如果訂單已發運，則無法取消。

請參閱 [商務訂單管理](https://docs.magento.com/user-guide/sales/order-management.html){target="_blank"}。

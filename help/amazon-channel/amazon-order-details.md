---
title: Amazon訂單詳細資料
description: 在Adobe Commerce或Magento Open Source管理員中檢視您Amazon Marketplace訂單的詳細資料。
feature: Sales Channels, Orders
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Amazon訂單詳細資料

![Amazon訂單詳細資料](assets/amazon-order-details-header.png){width="600" zoomable="yes"}

## 檢視Amazon訂單詳細資料

1. 按一下商店資訊卡上的&#x200B;**[!UICONTROL View Store]**。

1. 在&#x200B;_[!UICONTROL Recent Orders]_區段中，按一下訂單編號。

   _[!UICONTROL Amazon Order Details]_頁面隨即開啟。

>[!NOTE]
>
>如果您已在[訂單設定](./order-settings.md)中啟用訂單匯入，且訂單已由Amazon (FBA)](./fulfilled-by.md)履行[，則訂單詳細資料中可能會顯示某些欄位的虛擬資料。 Amazon不會針對FBA訂單傳送下列資料。
>
> - `AddressType`
> - `AddressLine1`
> - `AddressLine2`
> - `AddressLine3`
> - `BuyerName`
> - `Phone`
> - `PurchaseOrderNumber`
> - `RecipientName`
> - `CustomizedURL`
> - `GiftMessageText`

### 訂單與出貨詳細資訊頁標

_[!UICONTROL Order and Shipping Details]_索引標籤會顯示從Amazon收到的詳細訂單資訊。

>[!IMPORTANT]
>
>Amazon接受無法匯入Amazon sales channel的非標準地址資訊，因此導致某些訂單的州/國家/地區代碼無法正確更新。 若要更正地址錯誤，可在訂單詳細資料中編輯下列欄位：
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`
>
>編輯後別忘了按一下&#x200B;**儲存順序**。

![訂單與送貨詳細資料](assets/amazon-order-details.png){width="600" zoomable="yes"}

### 「訂購專案」標籤

_[!UICONTROL Order Items]_索引標籤會顯示從Amazon收到的所有與Amazon訂單相關聯的專案。

![訂單專案詳細資料](assets/amazon-order-item-details.png){width="600" zoomable="yes"}

### 「追蹤」標籤

_[!UICONTROL Tracking]_索引標籤會顯示與Amazon訂單相關聯的追蹤資訊。

![追蹤詳細資料](assets/amazon-order-tracking-details.png){width="600" zoomable="yes"}

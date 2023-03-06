---
title: Amazon訂單詳細資料
description: 在Adobe Commerce或Magento Open Source管理員中檢視Amazon Marketplace訂單的詳細資訊。
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Amazon訂單詳細資料

![Amazon訂單詳細資料](assets/amazon-order-details-header.png)

## 檢視Amazon訂單詳細資訊

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 在 _[!UICONTROL Recent Orders]_區段，按一下訂單編號。

   此 _[!UICONTROL Amazon Order Details]_頁面開啟。

>[!NOTE]
>
>如果您的 [順序設定](./order-settings.md) 順序是 [由Amazon(FBA)履行](./fulfilled-by.md)，您可能會在訂單詳細資料中看到某些欄位的虛擬資料。 Amazon不會針對FBA訂單傳送下列資料。
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


### 訂單和發運詳細資訊標籤

此 _[!UICONTROL Order and Shipping Details]_標籤會顯示從Amazon收到的詳細訂單資訊。

>[!IMPORTANT]
>
>Amazon接受無法匯入至Amazon銷售管道的非標準位址資訊，因此某些訂單無法正確更新狀態/國家/地區代碼。 要更正地址錯誤，可在訂單詳細資訊中編輯以下欄位：
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`
>
>別忘了按一下 **儲存順序** 進行編輯之後。

![訂單和發運詳細資訊](assets/amazon-order-details.png)

### 訂單項目標籤

此 _[!UICONTROL Order Items]_標籤會顯示從Amazon收到的與Amazon訂單相關聯的所有項目。

![訂單項目詳細資訊](assets/amazon-order-item-details.png)

### 追蹤標籤

此 _[!UICONTROL Tracking]_索引標籤會顯示與Amazon訂單相關的追蹤資訊。

![追蹤詳細資料](assets/amazon-order-tracking-details.png)

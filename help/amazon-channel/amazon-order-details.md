---
title: Amazon訂單詳細資料
description: 在「Amazon商務」或「Magento Open Source管理員」中檢視Adobe Marketplace訂單的詳細資訊。
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Amazon訂單詳細資料

![Amazon訂單詳細資料](assets/amazon-order-details-header.png)

## 檢視Amazon訂單詳細資訊

1. 按一下儲存卡上的&#x200B;**[!UICONTROL View Store]**。

1. 在&#x200B;_[!UICONTROL Recent Orders]_區段中，按一下訂單編號。

   _[!UICONTROL Amazon Order Details]_頁面隨即開啟。

>[!NOTE]
>
>如果您已在[訂單設定](./order-settings.md)中啟用訂單匯入，且訂單為[由Amazon(FBA)](./fulfilled-by.md)履行，則訂單詳細資料中某些欄位可能會顯示虛擬資料。 Amazon不會針對FBA訂單傳送下列資料。
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

_[!UICONTROL Order and Shipping Details]_標籤會顯示從Amazon收到的詳細訂單資訊。

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
>編輯後，別忘了按一下&#x200B;**儲存順序**。

![訂單和發運詳細資訊](assets/amazon-order-details.png)

### 訂單項目標籤

_[!UICONTROL Order Items]_索引標籤會顯示從Amazon收到的與Amazon訂單相關聯的所有項目。

![訂單項目詳細資訊](assets/amazon-order-item-details.png)

### 追蹤標籤

_[!UICONTROL Tracking]_標籤會顯示與Amazon順序相關的追蹤資訊。

![追蹤詳細資料](assets/amazon-order-tracking-details.png)

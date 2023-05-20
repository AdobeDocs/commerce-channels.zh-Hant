---
title: Amazon訂單詳細資訊
description: 在Adobe Commerce或Magento Open Source管理員中查看您的Amazon市場訂單的詳細資訊。
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Amazon訂單詳細資訊

![Amazon訂單詳細資訊](assets/amazon-order-details-header.png)

## 查看Amazon訂單詳細資訊

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 在 _[!UICONTROL Recent Orders]_的上界。

   的 _[!UICONTROL Amazon Order Details]_的上界。

>[!NOTE]
>
>如果您的 [訂單設定](./order-settings.md) 命令是 [由Amazon履行](./fulfilled-by.md)，您可能會在訂單詳細資訊中看到某些欄位的虛資料。 Amazon不發送FBA訂單的以下資料。
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

的 _[!UICONTROL Order and Shipping Details]_的子菜單。

>[!IMPORTANT]
>
>Amazon接受無法導入Amazon銷售渠道的非標準地址資訊，從而阻止某些訂單的州/國家代碼正確更新。 要更正地址錯誤，可以按順序詳細編輯以下欄位：
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`
>
>不要忘記按一下 **保存訂單** 編輯。

![訂單和發運詳細資訊](assets/amazon-order-details.png)

### 「訂單項」頁籤

的 _[!UICONTROL Order Items]_頁籤顯示從Amazon接收的與Amazon訂單關聯的所有項目。

![訂單物料詳細資訊](assets/amazon-order-item-details.png)

### 跟蹤頁籤

的 _[!UICONTROL Tracking]_頁籤顯示與Amazon訂單關聯的跟蹤資訊。

![跟蹤詳細資訊](assets/amazon-order-tracking-details.png)

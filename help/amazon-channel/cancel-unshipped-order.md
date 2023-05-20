---
title: 取消未發運訂單
description: 通過您的Amazon取消待定或部分發運（未發運）訂單 [!DNL Seller Central] 帳戶。
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# 取消未發運訂單

Amazon訂單只有在 `Unshipped` 狀態。 如果訂單處於待定狀態或部分發運（未發運），則只能通過您的 [!DNL Amazon Seller Central] 帳戶。 如果已發運該物料，則還必須在您的 [!DNL Amazon Seller Central] 帳戶。

>[!NOTE]
>
>對於除取消訂單外的任務：
>
>- 如果 [訂單導入](./order-settings.md) 啟用，訂單在 [[!DNL Commerce] 訂單工作流](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}。
>- 如果 [訂單導入](./order-settings.md) 已禁用，您必須在 [!DNL Amazon Seller Central]。


## 取消訂單 `Unshipped` 狀態

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 在 _[!UICONTROL Recent Orders]_在「儲存」面板的「區域」中，按一下訂單號。

   的 _[!UICONTROL Amazon Order Details]_的子菜單。

1. 按一下 **[!UICONTROL Cancel Order]** 的子菜單。

   此選項僅對中的訂單顯示 `Unshipped` 狀態。

1. 對於 **[!UICONTROL Reason for cancellation]**，也請參見Wiki頁。

1. 按一下 **[!UICONTROL Confirm]**。

   訂單已取消，狀態更新為 `Canceled` 的下界。

取消通知將發送給您 [!DNL Amazon Seller Central] 並通知與訂單關聯的客戶。 相應的狀態 [!DNL Commerce] 順序，如果有，則更改 `Complete`。

---
title: 取消未發運的訂單
description: 通過您的Amazon取消待定或部分發運（未發運）訂單 [!DNL Seller Central] 帳戶。
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 取消未發運的訂單

Amazon訂單只有在 `Unshipped` 狀態。 如果訂單待定或部分發運（未發運），則只能通過 [!DNL Amazon Seller Central] 帳戶。 如果已發運項目，則還必須在 [!DNL Amazon Seller Central] 帳戶。

>[!NOTE]
>
>對於取消訂單以外的任務：
>
>- 若您有 [訂單匯入](./order-settings.md) 啟用時，會在 [[!DNL Commerce] 訂購工作流](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}。
>- 若 [訂單匯入](./order-settings.md) 停用時，您必須在 [!DNL Amazon Seller Central].


## 取消訂單 `Unshipped` 狀態

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 在 _[!UICONTROL Recent Orders]_區段，按一下訂單編號。

   此 _[!UICONTROL Amazon Order Details]_頁。

1. 按一下 **[!UICONTROL Cancel Order]** 的下一頁。

   此選項只會針對 `Unshipped` 狀態。

1. 針對 **[!UICONTROL Reason for cancellation]**，選擇選項。

1. 按一下 **[!UICONTROL Confirm]**.

   訂單被取消，且狀態更新為 `Canceled` 在訂單詳細資料中。

取消通知會傳送至您的 [!DNL Amazon Seller Central] 帳戶，並會通知與訂單相關聯的客戶。 對應之 [!DNL Commerce] 順序，若有，則變更為 `Complete`.

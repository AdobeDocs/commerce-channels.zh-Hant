---
title: 取消未發運的訂單
description: 通過您的Amazon [!DNL Seller Central] 帳戶取消待定或部分發運（未發運）訂單。
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 取消未發運的訂單

Amazon訂單只有在處於`Unshipped`狀態時才能取消。 如果訂單待定或已部分發運（未發運），則只能通過您的[!DNL Amazon Seller Central]帳戶取消訂單。 如果已發運該物料，則還必須在[!DNL Amazon Seller Central]帳戶中處理退貨和交換。

>[!NOTE]
>
>對於取消訂單以外的任務：
>
>- 如果您已啟用[order import](./order-settings.md)，則訂單會在[[!DNL Commerce] orders workflow](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}中管理。
>- 如果[order import](./order-settings.md)被禁用，您必須在[!DNL Amazon Seller Central]中管理訂單。


## 取消`Unshipped`狀態中的訂單

1. 按一下儲存卡上的&#x200B;**[!UICONTROL View Store]**。

1. 在商店控制面板的&#x200B;_[!UICONTROL Recent Orders]_區段中，按一下訂單編號。

   此時將顯示&#x200B;_[!UICONTROL Amazon Order Details]_頁。

1. 按一下標題列中的&#x200B;**[!UICONTROL Cancel Order]**。

   此選項僅針對處於`Unshipped`狀態的訂單顯示。

1. 對於&#x200B;**[!UICONTROL Reason for cancellation]**，選擇一個選項。

1. 按一下&#x200B;**[!UICONTROL Confirm]**。

   訂單被取消，訂單詳細資訊中的狀態更新為`Canceled`。

取消通知將發送到您的[!DNL Amazon Seller Central]帳戶，並且與訂單關聯的客戶也會收到通知。 相應[!DNL Commerce]順序的狀態（如果有）更改為`Complete`。

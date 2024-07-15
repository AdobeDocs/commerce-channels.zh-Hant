---
title: 取消未出貨的Amazon訂單
description: 透過您的Amazon [!DNL Seller Central] 帳戶取消擱置或部份出貨（未出貨）的訂單。
feature: Sales Channels, Orders, Shipping/Delivery
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 取消未出貨的Amazon訂單

Amazon訂單處於`Unshipped`狀態時才能取消。 如果訂單擱置或部份出貨（未出貨），則只能透過您的[!DNL Amazon Seller Central]帳戶取消訂單。 如果專案已出貨，您也必須在[!DNL Amazon Seller Central]帳戶中處理退貨與交換。

>[!NOTE]
>
>對於取消訂單以外的工作：
>
>- 如果您已啟用[訂單匯入](./order-settings.md)，則會在[[!DNL Commerce] 訂單工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)中管理訂單。
>- 如果[訂單匯入](./order-settings.md)已停用，您必須在[!DNL Amazon Seller Central]中管理您的訂單。

## 取消狀態為`Unshipped`的訂單

1. 按一下商店資訊卡上的&#x200B;**[!UICONTROL View Store]**。

1. 在商店儀表板的&#x200B;_[!UICONTROL Recent Orders]_區段中，按一下訂單編號。

   _[!UICONTROL Amazon Order Details]_頁面隨即顯示。

1. 按一下標題列中的&#x200B;**[!UICONTROL Cancel Order]**。

   此選項僅針對`Unshipped`狀態的訂單顯示。

1. 針對&#x200B;**[!UICONTROL Reason for cancellation]**，選擇一個選項。

1. 按一下&#x200B;**[!UICONTROL Confirm]**。

   訂單已取消，訂單詳細資料中的狀態已更新為`Canceled`。

取消通知已傳送至您的[!DNL Amazon Seller Central]帳戶，同時也會通知與訂單相關聯的客戶。 對應[!DNL Commerce]訂單的狀態（如果有的話）變更為`Complete`。

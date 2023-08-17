---
title: 處理訂單
description: '''送貨與取消說明 [!DNL Walmart Marketplace] Adobe Commerce和Magento Open Source的訂單。'
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# 處理訂單

晚於 [!DNL Walmart Marketplace] 訂單已確認並成功傳送至 [!DNL Channel Manager]，您會使用 [Commerce訂單管理](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#orders-workspace) 以處理訂單。

Channel Manager將更新同步到 [!DNL Walmart Marketplace] 以確保訂單狀態與出貨資訊來自 [!DNL Commerce] 符合在中追蹤的資料 [!DNL Walmart Marketplace].

* **訂單出貨** — 沃爾瑪要求所有出貨都有追蹤編號。 如果部份料號缺貨，您可以建立部份出貨，以傳送目前可用的料號。 在您提交出貨之後，訂單更新會同步化至 [!DNL Walmart Marketplace]. 然後，沃爾瑪會通知客戶訂單狀態和運送細節。

* **訂單取消** — 當您取消 [!DNL Walmart Marketplace] 訂單，沃爾瑪要求取消原因，包含在寄給客戶的訂單取消通知中。 取消原因也會顯示在 [!DNL Commerce] 訂單付款資訊。 在您提交取消之後，庫存更新會同步到 [!DNL Walmart Marketplace]. 然後，沃爾瑪會通知客戶訂單狀態和運送細節。

  在店面，您必須取消整個訂單。 [!DNL Commerce] 不允許部分取消。

* **退款請求** — 如果要求沃爾瑪商店退貨以取得已出貨的訂單，則 [!UICONTROL Status details] 包含回訪連結。 退貨與退款管理自 [傳回](return-refund-orders.md) 儀表板。

當處理商務訂單且 [!DNL Channel Manager] 將出貨、部份出貨及取消更新成功同步至 [!DNL Walmart Marketplace]，訂單處理完成。 已出貨訂單的退貨請求與退款管理自 [傳回](return-refund-orders.md) 儀表板。

>[!NOTE]
>
> 同步處理訂單更新最多可能需要五分鐘 [!DNL Walmart Marketplace]. 若要檢查訂單狀態，請返回 [!DNL Channel Manager] 訂單頁面。

## 出貨訂單

1. 在「管理員」中，選取 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. 選取銷售管道商店的眼睛圖示，以開啟商店檢視。

1. 要檢視 [!DNL Walmart Marketplace] 訂購，選取 **[!UICONTROL Orders]**.

1. 在「訂單」表格中，選取 **[!UICONTROL Commerce Order Number]**.

1. 透過選取「 」，建立並提交全部或部份訂單的出貨 **[!UICONTROL Ship]**.

   ![的商務訂單詳細資料檢視 [!DNL Walmart Marketplace] 訂購](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

   * 選擇出貨承運商，並透過選取 **[!UICONTROL Add tracking number]**.

     ![的商務訂單詳細資料檢視 [!DNL Walmart Marketplace] 訂購](assets/order-shipment-add-tracking-number.png){width="600" zoomable="yes"}

   * 視需要完成其餘的送貨表格。 另請參閱 [[!DNL Shipping an Order]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-ship.html) 以取得詳細指示。

1. 提交出貨後，追蹤 [訂單狀態](manage-orders.md#about-order-status) 在 [!DNL Channel Manager] 以確認已傳送更新至 [!DNL Walmart Marketplace].

訂單出貨後，您可以處理完整或部份退款，從 [!DNL Channel Manager] 針對訂單中包含的專案，根據從收到的退貨請求 [!DNL Walmart Marketplace]. 另請參閱 [退貨與退款訂單](return-refund-orders.md).

## 取消訂單

1. 在「管理員」中，選取 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. 選取銷售管道商店的眼睛圖示，開啟商店檢視。

1. 要檢視 [!DNL Walmart Marketplace] 訂購，選取*[!UICONTROL Orders]**。

1. 在「訂單」表格中，開啟 [訂單詳細資訊頁面](manage-orders.md#view-order-detail) 藉由選取 **[!UICONTROL Commerce Order Number]** 以取消訂單。

   ![的商務訂單詳細資料檢視[!DNL Walmart Marketplace]訂購](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

1. 取消訂單。

   * 選取 **取消** 從「訂單詳細資料」功能表。

   * 在 [!UICONTROL Cancel Order] 表單，選取 **[!UICONTROL Cancellation reason]**.

   ![的商務訂單詳細資料檢視 [!DNL Walmart Marketplace] 訂購](assets/cancel-order-reason-selector.png){width="600" zoomable="yes"}

   * 選取 **[!UICONTROL Cancel Order]**.

1. 提交取消後，追蹤 [訂單狀態](manage-orders.md#about-order-status) 在 [!DNL Channel Manager] 以確認已傳送更新至 [!DNL Walmart Marketplace].

## 修正訂單錯誤

在訂單同步處理期間，可能會發生下列錯誤： [!DNL Walmart Marketplace]，或在出貨、部份出貨及取消的訂單更新處理期間。

如果出貨、部份出貨或取消更新的同步化作業失敗， [!DNL Channel Manager] 訂單頁面會顯示 _錯誤_ 訂單的狀態。 為確保出貨資訊和訂單取消資訊能正確反映在Walmart Marketplace帳戶中，請手動更新您網站上的訂單。 [!DNL Walmart Marketplace] 商店。



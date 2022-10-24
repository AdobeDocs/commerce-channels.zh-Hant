---
title: 處理訂單
description: '''運送和取消指示 [!DNL Walmart Marketplace] Adobe Commerce和Magento Open Source的訂單。'
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: 958f91f0303b823f164e60e56d8dbe4e8c2380f6
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---

# 處理訂單

之後 [!DNL Walmart Marketplace] 已確認訂單，並已成功傳送至 [!DNL Channel Manager]，您使用 [商務訂單管理](https://docs.magento.com/user-guide/sales/orders-workspace.html) 來處理訂單。

Channel Manager會將更新同步至 [!DNL Walmart Marketplace] 確保訂單狀態和發運資訊 [!DNL Commerce] 符合 [!DNL Walmart Marketplace].

* **訂單發運** — 沃爾瑪要求所有貨物的跟蹤編號。 如果某些物料無存貨，您可以建立部分發運以發送當前可用的物料。 在您提交發運後，訂單更新將同步到 [!DNL Walmart Marketplace]. 然後，沃爾瑪會通知客戶訂單狀態和發貨詳細資訊。

* **訂單取消** — 當您取消 [!DNL Walmart Marketplace] 訂單，沃爾瑪要求取消原因，該原因包含在發送給客戶的訂單取消通知中。 取消原因也會顯示在 [!DNL Commerce] 訂單付款資訊。 提交取消後，庫存更新將同步到 [!DNL Walmart Marketplace]. 然後，沃爾瑪會通知客戶訂單狀態和發貨詳細資訊。

   在店面，您必須取消整筆訂單。 [!DNL Commerce] 不允許部分取消。

* **退款請求** — 如果要求Walmart Marketplace退回發貨訂單， [!UICONTROL Status details] 包含傳回的連結。 退貨和退款由 [傳回](return-refund-orders.md) 控制面板。

處理商務訂單時，並 [!DNL Channel Manager] 成功將發運、部分發運和取消更新同步到 [!DNL Walmart Marketplace]，訂單處理完成。 發運訂單的退貨請求和退款可從 [傳回](return-refund-orders.md) 控制面板。

>[!NOTE]
>
> 訂單更新最多可能需要5分鐘才能同步至 [!DNL Walmart Marketplace]. 要檢查訂單狀態，請返回 [!DNL Channel Manager] 訂購頁面。

## 發運訂單

1. 在管理員中，選取 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. 選取銷售管道商店的眼睛圖示，以開啟商店檢視。

1. 要查看 [!DNL Walmart Marketplace] 訂購，選擇 **[!UICONTROL Orders]**.

1. 在「訂單」(Orders)表格中，通過選擇 **商務訂單編號**.

1. 通過選擇 **[!UICONTROL Ship]**.

   ![的商務訂單詳細資訊視圖 [!DNL Walmart Marketplace] 訂購](assets/order-detail-with-external-order-id.png)

   * 選擇發運承運商，並通過選擇 **[!UICONTROL Add tracking number]**.

      ![的商務訂單詳細資訊視圖 [!DNL Walmart Marketplace] 訂購](assets/order-shipment-add-tracking-number.png)


   * 視需要填寫其餘的運送表單。 請參閱 [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) 以取得詳細指示。

1. 提交裝運後，跟蹤 [訂單狀態](manage-orders.md#about-order-status) in [!DNL Channel Manager] 驗證是否已將更新發送至 [!DNL Walmart Marketplace].

發運訂單後，您可以處理 [!DNL Channel Manager] 根據從收到的回訪請求 [!DNL Walmart Marketplace]. 請參閱 [退貨訂單](return-refund-orders.md).

## 取消訂單

1. 在管理員中，選取 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. 選取銷售管道商店的眼睛圖示，以開啟商店檢視。

1. 要查看 [!DNL Walmart Marketplace] 訂購，選擇*[!UICONTROL *Orders]**。

1. 在「訂單」表格中，開啟 [訂購詳細資訊頁面](manage-orders.md#view-order-detail) 選取 **商務訂單編號** 來取消。

   ![的商務訂單詳細資訊視圖[!DNL Walmart Marketplace]訂購](assets/order-detail-with-external-order-id.png)

1. 取消訂單。

   * 選擇 **取消** 從「訂單詳細資訊」菜單。

   * 在 [!UICONTROL Cancel Order] 表單中 **取消原因**.
   ![的商務訂單詳細資訊視圖 [!DNL Walmart Marketplace] 訂購](assets/cancel-order-reason-selector.png)

   * 選擇 **取消訂單**.


1. 提交取消後，追蹤 [訂單狀態](manage-orders.md#about-order-status) in [!DNL Channel Manager] 驗證是否已將更新發送至 [!DNL Walmart Marketplace].

## 修正訂單錯誤

在訂單同步過程中，可能會發生錯誤 [!DNL Walmart Marketplace]，或在訂單更新流程中，對發運、部分發運和取消進行更新。

如果發運、部分發運或取消更新的同步操作失敗，則 [!DNL Channel Manager] 訂單頁面顯示 _錯誤_ 訂單的狀態。 為確保發運資訊和訂單取消資訊準確反映在Walmart Marketplace帳戶中，請在您的 [!DNL Walmart Marketplace] 儲存。



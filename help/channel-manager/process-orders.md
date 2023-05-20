---
title: 處理訂單
description: '''裝運和取消說明 [!DNL Walmart Marketplace] Adobe Commerce和Magento Open Source的命令。'
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---

# 處理訂單

之後 [!DNL Walmart Marketplace] 已確認訂單，並已成功發送至 [!DNL Channel Manager]，則 [商務訂單管理](https://docs.magento.com/user-guide/sales/orders-workspace.html) 處理訂單。

Channel Manager將更新同步到 [!DNL Walmart Marketplace] 確保訂單狀態和發運資訊 [!DNL Commerce] 與 [!DNL Walmart Marketplace]。

* **訂單發運** — 沃爾瑪要求所有發貨的跟蹤編號。 如果某些物料缺貨，您可以建立部分發運以發送當前可用的物料。 提交發運後，訂單更新將同步到 [!DNL Walmart Marketplace]。 然後，沃爾瑪會通知客戶訂單狀態和發貨詳細資訊。

* **訂單取消** — 當取消 [!DNL Walmart Marketplace] 而沃爾瑪則要求在發送給客戶的訂單取消通知中包含取消原因。 取消原因也顯示在 [!DNL Commerce] 訂單付款資訊。 提交取消後，庫存更新將同步到 [!DNL Walmart Marketplace]。 然後，沃爾瑪會通知客戶訂單狀態和發貨詳細資訊。

   在店面，必須取消整個訂單。 [!DNL Commerce] 不允許部分取消。

* **退款請求** — 如果需要Walmart Marketplace退回已發運訂單， [!UICONTROL Status details] 包含到返回的連結。 退貨和退款由 [返回](return-refund-orders.md) 控制項欄。

處理和處理Commerce訂單時 [!DNL Channel Manager] 成功將裝運、部分裝運和取消更新同步到 [!DNL Walmart Marketplace]，訂單處理完成。 從管理 [返回](return-refund-orders.md) 控制項欄。

>[!NOTE]
>
> 要同步到的訂單更新最多需要五分鐘 [!DNL Walmart Marketplace]。 要檢查訂單狀態，請返回至 [!DNL Channel Manager] 訂單頁。

## 發運訂單

1. 在管理員中，選擇 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**。

1. 通過為銷售渠道商店選擇眼睛表徵圖開啟商店視圖。

1. 查看 [!DNL Walmart Marketplace] 訂單，選擇 **[!UICONTROL Orders]**。

1. 在「訂單」表中，通過選擇 **商業訂單編號**。

1. 通過選擇 **[!UICONTROL Ship]**。

   ![Oracle Commerce Order Detail視圖 [!DNL Walmart Marketplace] 訂單](assets/order-detail-with-external-order-id.png)

   * 選擇發運承運人並通過選擇 **[!UICONTROL Add tracking number]**。

      ![Oracle Commerce Order Detail視圖 [!DNL Walmart Marketplace] 訂單](assets/order-shipment-add-tracking-number.png)


   * 根據需要填寫其餘的裝運單。 請參閱 [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) 的上界。

1. 提交發運後，跟蹤 [訂單狀態](manage-orders.md#about-order-status) 在 [!DNL Channel Manager] 驗證更新已發送到 [!DNL Walmart Marketplace]。

發運訂單後，您可以處理來自 [!DNL Channel Manager] 根據從以下地址接收的退貨請求 [!DNL Walmart Marketplace]。 請參閱 [退貨訂單](return-refund-orders.md)。

## 取消訂單

1. 在管理員中，選擇 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**。

1. 通過為銷售渠道商店選擇眼睛表徵圖開啟商店視圖。

1. 查看 [!DNL Walmart Marketplace] 訂單，選擇*[!UICONTROL *Orders]**。

1. 在「訂單」表中，開啟 [訂單詳細資訊頁面](manage-orders.md#view-order-detail) 選擇 **商業訂單編號** 訂單。

   ![Oracle Commerce Order Detail視圖[!DNL Walmart Marketplace]訂單](assets/order-detail-with-external-order-id.png)

1. 取消訂單。

   * 選擇 **取消** 按鈕。

   * 在 [!UICONTROL Cancel Order] ，請選擇 **取消原因**。
   ![Oracle Commerce Order Detail視圖 [!DNL Walmart Marketplace] 訂單](assets/cancel-order-reason-selector.png)

   * 選擇 **取消訂單**。


1. 提交取消後，跟蹤 [訂單狀態](manage-orders.md#about-order-status) 在 [!DNL Channel Manager] 驗證更新已發送到 [!DNL Walmart Marketplace]。

## 修復訂單錯誤

在訂單同步過程中可能發生錯誤 [!DNL Walmart Marketplace]或在發運、部分發運和取消的訂單更新過程中。

如果發運、部分發運或取消更新的同步操作失敗， [!DNL Channel Manager] 訂單頁顯示 _錯誤_ 訂單的狀態。 為確保發運資訊和訂單取消資訊準確反映在Walmart Marketplace帳戶中，請手動更新您的訂單 [!DNL Walmart Marketplace] 商店。



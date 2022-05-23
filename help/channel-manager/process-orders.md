---
title: 處理訂單
description: 發運和取消說明 [!DNL Walmart Marketplace] Adobe Commerce和Magento Open Source。
source-git-commit: 5670639697550b2d7fee67dd29be9c6278d5782b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# 處理訂單

如果您使用Adobe Commerce和Magento Open Source訂單管理管理 [!DNL Commerce] 商店銷售，您處理 [!DNL Walmart Marketplace] Commerce的訂單。

在Commerce中處理訂單時，Channel Manager將更新同步到 [!DNL Walmart Marketplace]。 此更新確保Commerce的產品庫存和訂單狀態與在 [!DNL Walmart Marketplace] 並通知沃爾瑪將訂單狀態和發貨資訊發送給客戶。

>[!NOTE]
>
> 最多5分鐘，訂單更新可同步到 [!DNL Walmart Marketplace]。 要檢查訂單狀態，請返回至 [!DNL Channel Manager] 命令。

## 發運訂單

從Commerce發運訂單時，使用 [[!DNL Commerce Order Management] 發運工作流](https://docs.magento.com/user-guide/sales/order-ship.html)。 提交訂單後，更新將同步到 [!DNL Walmart Marketplace]。 然後，沃爾瑪會通知客戶訂單狀態和發貨詳細資訊。

**先決條件**

在發運訂單之前，驗證 [通道運輸設定和承運人配置](map-shipping-carriers.md) 見 [!DNL Walmart Marketplace requirements]。

### 建立並提交發運

當您發運 [!DNL Walmart Marketplace] 訂單 [!DNL Commerce]，必須添加跟蹤編號。 客戶從中接收的發運通知中接收跟蹤編號 [!DNL Walmart]。

1. 在管理員中，選擇 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 開啟 [!UICONTROL Channel Manager Marketplace Stores] 的子菜單。

1. 通過為銷售渠道商店選擇眼睛表徵圖開啟商店視圖。

1. 查看 [!DNL Walmart Marketplace] 訂單，選擇*[!UICONTROL *Orders]**。

1. 在「訂單」表中，通過選擇 **商業訂單編號**。

1. 通過選擇 **[!UICONTROL Ship]**。

   - 要選擇發運承運人並添加跟蹤編號，請選擇 **[!UICONTROL Add tracking number]**。

   - 根據需要填寫其餘的裝運單。 請參閱 [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) 的上界。

1. 提交發運後，跟蹤 [訂單狀態](manage-orders.md#about-order-status) 在 [!DNL Channel Manager] 驗證更新已發送到 [!DNL Walmart Marketplace]。

## 取消訂單

當取消 [!DNL Walmart Marketplace] 而沃爾瑪則要求取消訂單。 當訂單取消更新到沃爾瑪時，取消原因被包括在發送給客戶的取消通知中。

取消原因也顯示在 [!DNL Commerce] 訂單付款資訊。

1. 在管理員中，選擇 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 開啟 [!UICONTROL Channel Manager Marketplace Stores] 的子菜單。

1. 通過為銷售渠道商店選擇眼睛表徵圖開啟商店視圖。

1. 查看 [!DNL Walmart Marketplace] 訂單，選擇*[!UICONTROL *Orders]**。

1. 在「訂單」表中，通過選擇 **商業訂單編號** 訂單。

   ![Walmart Marketplace訂單的「商務訂單」詳細資訊視圖](assets/order-detail-with-external-order-id.png)

1. 取消訂單。

   - 選擇 **取消** 按鈕。

   - 在「取消訂單」窗體中，選擇 **取消原因**。

      ![Walmart Marketplace訂單的「商務訂單」詳細資訊視圖](assets/order-detail-with-external-order-id.png)

   - 選擇 **取消訂單**。

1. 驗證是否已將更新發送到 [!DNL Walmart Marketplace] 通過檢查 [訂單狀態](manage-orders.md#about-order-status) 在 [!DNL Channel Manager]。

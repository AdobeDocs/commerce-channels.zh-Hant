---
title: '"管理 [!DNL Walmart Marketplace] 訂單"'
description: '"查看和管理 [!DNL Walmart Marketplace] 訂單 [!DNL Channel Manager] Adobe Commerce和Magento Open Source。」'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: eb57189ed866fffa064867d1de5ae9db5b32e283
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 0%

---

# 管理 [!DNL Walmart Marketplace] 訂單

[!DNL Walmart Marketplace] 訂單資料 [!DNL Commerce] 產品自動同步 [!DNL Channel Manager] 後 [!DNL Walmart] 處理訂單。

在Commerce端，成功的同步將觸發以下操作：

- [!DNL Channel Manager] 向沃爾瑪發出訂單確認。

- 根據沃爾瑪訂單建立相應的商務訂單。

- 更新的訂單資訊顯示在 [!DNL Channel Manager] 訂單控制板。

在店面管理員中，您可以查看 [!DNL Channel Manager] 透過開設銷售渠道店及選擇 **[!UICONTROL Orders]**。

![要管理的Channel Manager訂單視圖 [!DNL Walmart Marketplace] 訂單](assets/orders-dashboard-view.png)

>[!NOTE]
>
>最多需要35分鐘 [!DNL Walmart Marketplace] 顯示順序 [!DNL Channel Manager] 清單。 [!DNL Walmart] 需要大約30分鐘來處理傳入的訂單，並將其發送到 [!DNL Channel Manager]。 在Channel Manager收到訂單後，在Adobe Commerce或Magento Open Source中建立和顯示訂單大約需要5分鐘。

## 訂單控制項和列說明

下表說明了可用於訂單的控制項和列。

**控制項[!UICONTROL Orders]**
| **控制項**                    | **說明**                                                                                                                                                                                                                                                                  | |—| | [!UICONTROL Filter orders]     |通過選擇以下選項之一對視圖進行排序 [!UICONTROL Order Status] 卡片。                                                                                                                                                                                                           | |錯誤描述 |提供有關訂單的「錯誤」狀態的詳細資訊。                                                                                                                                                                                                            | | [!UICONTROL View order detail] |要查看訂單詳細資訊，請選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 的子菜單。 然後，使用 [!DNL Commerce] 訂單選項以處理訂單。                                                                                                                    | | [!UICONTROL Channel Settings]  |要修改渠道配置，請選擇渠道Walmart連接憑據、映射的屬性或發運標識符，設定選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 的子菜單。 然後，使用 [!DNL Commerce] 訂單選項以處理訂單。 |


**列說明**

| 欄位 | 說明 |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Walmart Order Number] | 在中分配給訂單的採購訂單編號 [!DNL Walmart Marketplace]。 當訂單最初導入到 [!DNL Channel Manager]，僅 [!DNL Walmart] 此時將顯示訂單編號。 當 [!DNL Commerce] 建立順序， [!DNL Walmart] 訂單號儲存在 [!UICONTROL External ID] 產品屬性。 |
| [!DNL Commerce] 訂單編號 | 分配給 [!DNL Commerce] 根據 [!DNL Walmart Marketplace] 命令。 |
| 項目 | 訂購的物料數 [!DNL Walmart Marketplace]。 |
| [!UICONTROL Order Value] | 訂購物料的總成本。 |
| [!UICONTROL Date Ordered] | 訂單提交日期 [!DNL Walmart Marketplace]。 |
| [!UICONTROL Ship By Date] | 訂單必須發運的日期才能滿足 [!DNL Walmart Marketplace] 要求。 |
| [!UICONTROL Deliver By Date] | 必須將訂單交付給客戶以滿足要求的日期 [!DNL Walmart Marketplace] UTC格式的要求。 |
| [!UICONTROL Ship Method] | 的 [[!DNL Walmart Marketplace] 裝運方法](https://sellerhelp.walmart.com/s/guide?article=000007893) 的下界。 |
| [!UICONTROL Last Update At] | 指示上次在中更新訂單資料的時間的時間戳 [!DNL Channel Manager] 的子菜單。 |
| [!UICONTROL Status] | 指示中的當前訂單狀態 [!DNL Commerce] 訂單工作流。 從導入的訂單的初始狀態 [!DNL Walmart Marketplace] 是 _開啟_。 處理和更新Commerce訂單時會發生其他狀態更新 [!DNL Channel Manager] 成功將裝運、部分裝運和取消更新同步到 [!DNL Walmart Marketplace]。 |
| [!UICONTROL Error Description] | 提供有關訂單的詳細資訊 _[!UICONTROL Error]_狀態。 |

## 訂單狀態


[!UICONTROL Order Status] 提供有關 [!DNL Walmart Marketplace] 從Adobe Commerce或Magento Open Source處理訂單。 訂單狀態更新發生於 [!DNL Channel Manager] 從其中一個接收更新的訂單資訊 [!DNL Walmart Marketplace] 或 [!DNL Commerce] 訂單制度。 訂單可以具有以下狀態：

- **[!UICONTROL Shipped]** — 已從 [!DNL Commerce] 商店。 當命令發出時， [!DNL Channel Manager] 將更新發送到 [!DNL Walmart Marketplace] 更新Walmart上的發運狀態，並提供發運的訂單跟蹤編號。

- **[!UICONTROL Partially Shipped]** — 某些物料標籤為已發運，而其他物料等待發運的訂單。 訂單發運中的物料時， [!DNL Channel Manager] 將更新發送到 [!DNL Walmart Marketplace] 更新在Walmart上單獨發運的發運狀態，並提供發運的訂單跟蹤編號。

- **[!UICONTROL Canceled]** — 已從 [!DNL Commerce] 商店。

   訂單取消完成後， [!DNL Commerce] 庫存數量更新以反映退回的物料。 然後， [!DNL Channel Manager] 將更新同步到 [!DNL Walmart Marketplace]。

- **[!UICONTROL Error]** — 有錯誤的訂單。 訂單更新操作失敗時可能出錯。 例如，如果 [!DNL Channel Manager] 無法從沃爾瑪獲得新訂單。 如果 [!DNL Channel Manager] 無法將訂單發運或取消更新發送到 [!DNL Walmart Marketplace]。 如果操作失敗，「訂單」頁將顯示 _錯誤_ 訂單的狀態。 有關詳細資訊，請參閱 [修復訂單錯誤](process-orders.md#fix-shipping-and-cancelation-errors)。

- **[!UICONTROL Error description]** — 提供有關因資訊缺失或值無效、發運詳細資訊不正確或訂單取消失敗等問題而發生的訂單錯誤的詳細資訊。 說明有助於確定在 [!DNL Commerce] 實例或 [!DNL Walmart Marketplace]。

>[!NOTE]
>
>如果訂單物料以多發運方式發送，則訂單狀態為 [!DNL Channel Manager] 反映最後一個可用訂單狀態。 例如，如果第一個物料發運，並且在將訂單更新同步到時不返回任何錯誤 [!DNL Channel Manager] 和 [!DNL Walmart Marketplace]，也請參見Wiki頁。 [!DNL Channel Manager] 訂單狀態為 _[!UICONTROL Partially Shipped]_。  如果第二個物料已發運並 [!C渠道經理] 返回錯誤，訂單狀態更新到_[!UICONTROL Error]_。

## 審閱訂單

1. 在管理員中，選擇 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 開啟 [!UICONTROL Channel Manager Marketplace Stores] 的子菜單。

1. 通過在儲存條目行中選擇眼睛表徵圖來開啟儲存視圖。

1. 要查看訂單資訊，請選擇*[!UICONTROL *Orders]**。

1. 通過檢查 **[狀態](#about-order-status)** 列中的設定。

## 查看訂單詳細資訊

在從市場接收訂單並導入Adobe Commerce或Magento Open Source後，使用 [!DNL Commerce] 訂單ID查看Adobe Commerce的訂單。

從 **[!UICONTROL Orders]**，選擇 **[!UICONTROL Commerce Order Number]** 開啟 [!DNL Commerce] 訂單詳細資訊。

![Oracle Commerce Order Detail視圖 [!DNL Walmart Marketplace] 訂單](assets/order-detail-with-external-order-id.png)

在Commerce商店中，從 [!DNL Walmart Marketplace] 在訂單資料中包含以下附加資訊：

- **付款資訊和發運方法** — 從Walmart導入的訂單包括以下付款和發運欄位的值：

   - **[!UICONTROL Offline Channel Payment]** — 表示訂單付款由 [!DNL Walmart Marketplace]。

   - **[!UICONTROL External Order Number]** — 顯示 [!DNL Walmart Marketplace] 訂單編號。

   - **[!UICONTROL Channel Shipping - Value]** — 指示通過以下方式處理運費 [!DNL Walmart Marketplace]。

   - **[!UICONTROL Cancellation Reason]** — 僅當從導入的訂單 [!DNL Walmart Marketplace] 已取消。 取消原因包括：

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]


---
title: '"管理 [!DNL Walmart Marketplace] 訂單"'
description: '"查看和管理 [!DNL Walmart Marketplace] 訂單 [!DNL Channel Manager] Adobe Commerce和Magento Open Source。」'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: e3b12c9ce1ad4b5be17284e98956a773d7ccca24
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 管理 [!DNL Walmart Marketplace] 訂單

[!DNL Walmart Marketplace] 訂單 [!DNL Commerce] 產品清單自動同步 [!DNL Channel Manager] 後 [!DNL Walmart] 處理訂單。 同步完成後，您可以通過選擇 **[!UICONTROL Orders]** 從連接的通道儲存視圖 [!DNL Channel Manager]。

![要管理的Channel Manager訂單視圖 [!DNL Walmart Marketplace] 訂單](assets/orders-dashboard-view.png)

>[!NOTE]
>
>最多需要35分鐘 [!DNL Walmart Marketplace] 顯示順序 [!DNL Channel Manager] 清單。 [!DNL Walmart] 需要大約30分鐘來處理傳入的訂單，並將其發送到 [!DNL Channel Manager]。 在Channel Manager收到訂單後，在Adobe Commerce或Magento Open Source中建立和顯示訂單大約需要5分鐘。

## 審閱訂單

1. 在管理員中，選擇 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 開啟 [!UICONTROL Channel Manager Marketplace Stores] 的子菜單。

1. 通過在儲存條目行中選擇鉛筆表徵圖開啟儲存視圖。

1. 要查看訂單資訊，請選擇*[!UICONTROL *Orders]**。

1. 通過檢查 **[狀態](#about-order-status)** 列中的設定。

## 查看訂單詳細資訊

在從市場接收訂單並導入Adobe Commerce或Magento Open Source後，使用 [!DNL Commerce] 訂單ID查看Adobe Commerce的訂單。

從 **[!UICONTROL Orders]**，選擇 **[!UICONTROL Commerce Order Number]** 開啟 [!DNL Commerce] 訂單詳細資訊。

![Oracle Commerce Order Detail視圖 [!DNL Walmart Marketplace] 訂單](assets/order-detail-with-external-order-id.png)

### 訂單控制項和列說明

下表說明了可用於訂單的控制項和列。

**控制項[!UICONTROL Orders]**
| **控制項**                    | **說明**                                                                                                                                               | |—| | [!UICONTROL Filter orders]     |通過選擇以下選項之一對視圖進行排序 [!UICONTROL Order Status] 卡片。                                                                                        | |錯誤消息詳細資訊 |懸停在 [!UICONTROL Error Status] 的子菜單。                                                                      | | [!UICONTROL View order detail] |要查看訂單詳細資訊，請選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 的子菜單。 然後，使用 [!DNL Commerce] 訂單選項以處理訂單。 |

**列說明**

| 欄位 | 說明 |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL  Walmart Order Number] | 在中分配給訂單的採購訂單編號 [!DNL Walmart Marketplace]。 當訂單最初導入到 [!DNL Channel Manager]，僅 [!DNL Walmart] 此時將顯示訂單編號。 當 [!DNL Commerce] 建立順序， [!DNL Walmart] 訂單號儲存在 [!UICONTROL External ID] 產品屬性。 |
| [!DNL Commerce]  訂單編號 | 分配給 [!DNL Commerce]  根據 [!DNL Walmart Marketplace] 命令。 |
| 項目 | 訂購的物料數 [!DNL Walmart Marketplace]。 |
| [!UICONTROL Order Value] | 訂購物料的總成本。 |
| [!UICONTROL Date Created] | 在 [!DNL Walmart Marketplace]。 |
| [!UICONTROL Ship By Date] | 訂單必須發運的日期才能滿足 [!DNL Walmart Marketplace] 要求。 |
| [!UICONTROL Deliver By Date] | 必須將訂單交付給客戶以滿足要求的日期 [!DNL Walmart Marketplace] 要求。 |
| [!UICONTROL Last Update At] | 指示上次在中更新訂單資料的時間的時間戳 [!DNL Channel Manager] |
| [!UICONTROL Status] | 指示中的當前訂單狀態 [!DNL Commerce] 訂單工作流。 成功將產品添加到時的狀態更新 [!DNL Channel Manager] 當你把產品 [!DNL Walmart Marketplace]。 如果操作失敗，則清單顯示「錯誤」狀態。 修復錯誤後， [!DNL Channel Manager] 重試該操作並更新狀態。 |
| [!UICONTROL Error Description] | 提供有關訂單的詳細資訊 *錯誤* 狀態。 |

### 關於訂單狀態


[!UICONTROL Order Status] 提供有關 [!DNL Walmart Marketplace] 從Adobe Commerce或Magento Open Source處理訂單。 訂單狀態更新發生於 [!DNL Channel Manager] 從其中一個接收更新的訂單資訊 [!DNL Walmart Marketplace] 或 [!DNL Commerce] 訂單制度。 訂單可以具有以下狀態：

* **[!UICONTROL Open]** — 從 [!DNL Walmart Marketplace] 準備在Adobe Commerce或Magento Open Source接受審查和處理。

   在客戶從 [!DNL Walmart Marketplace]，在連接通道的順序工作區中顯示開啟順序可能需要35分鐘。 [!DNL Commerce] 需要大約30分鐘來處理傳入的訂單，並將其發送到 [!DNL Channel Manager]。 在Channel Manager收到訂單後，建立和顯示 [!DNL Commerce] 命令。

* **[!UICONTROL Processed]** — 已發運、取消或退回的訂單 [!DNL Commerce] 商店。

   要顯示所有已發運、已取消和已退回的訂單，請選擇 **已處理** 狀態卡。

* **[!UICONTROL Canceled]** — 已從 [!DNL Commerce] 商店。

   訂單取消完成後， [!DNL Commerce] 庫存數量更新以反映退回的物料。 然後， [!DNL Channel Manager] 將更新同步到 [!DNL Walmart Marketplace]。

* **[!UICONTROL Refunded]** — 已從 [!DNL Commerce] 商店。

   退款完成後， [!DNL Commerce] 更新庫存數量以反映退款項目。 然後， [!DNL Channel Manager] 將更新同步到 [!DNL Walmart Marketplace]。

* **[!UICONTROL Error]** — 有錯誤的訂單。 訂單更新操作失敗時可能出錯。 例如，如果 [!DNL Channel Manager] 無法從沃爾瑪獲得新訂單。 如果 [!DNL Channel Manager] 無法將訂單發運或取消更新發送到 [!DNL Walmart Marketplace]。

* **[!UICONTROL Error description]** — 提供有關因資訊缺失或值無效、發運詳細資訊不正確或訂單取消失敗等問題而發生的訂單錯誤的詳細資訊。 說明有助於確定在 [!DNL Commerce] 實例或 [!DNL Walmart Marketplace]。

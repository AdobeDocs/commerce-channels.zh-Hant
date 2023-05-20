---
title: '''查看和管理訂單 [!DNL Channel Manager]"'
description: '''查看和管理 [!DNL Walmart Marketplace] 訂單 [!DNL Channel Manager] Adobe Commerce和Magento Open Source。'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# 查看和跟蹤訂單 [!DNL Channel Manager]

[!DNL Walmart Marketplace] 訂單資料 [!DNL Commerce] 產品自動同步 [!DNL Channel Manager] 後 [!DNL Walmart] 處理訂單。

在 [!DNL Commerce] 另外，成功的同步將觸發以下操作：

- [!DNL Channel Manager] 向沃爾瑪發出訂單確認。

- 對應 [!DNL Commerce] 訂單是根據沃爾瑪的訂單建立的。

- 更新的訂單資訊顯示在 [!DNL Channel Manager] 訂單控制板。

在店面管理員中，您可以查看 [!DNL Channel Manager] 透過開設銷售渠道店及選擇 **[!UICONTROL Orders]**。

![要管理的Channel Manager訂單視圖 [!DNL Walmart Marketplace] 訂單](assets/orders-dashboard-view.png)

>[!NOTE]
>
>最多需要35分鐘 [!DNL Walmart Marketplace] 顯示順序 [!DNL Channel Manager] 清單。 [!DNL Walmart] 需要大約30分鐘來處理傳入的訂單，並將其發送到 [!DNL Channel Manager]。 在Channel Manager收到訂單後，在Adobe Commerce或Magento Open Source中建立和顯示訂單大約需要5分鐘。

## 訂單控制項和列說明

下表說明了可用於訂單的控制項和列。

**控制項[!UICONTROL Orders]**

<table>
<tr>
<td><strong>控制項</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>通過選擇 [!UICONTROL Order Status] 卡片。</td>
</tr>
<tr>
<td>狀態詳細資訊</td>
<td>提供有關訂單錯誤和退貨請求的資訊。 要查看訂單的退貨資訊和退款狀態，請選擇 <strong>[!UICONTROL Return requested]</strong> 要開啟的文本 [!UICONTROL Returns] 控制項欄。</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>要查看訂單詳細資訊，請選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 的子菜單。 然後，使用 [!DNL Commerce] 訂單選項以處理訂單。</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>要修改渠道配置，請選擇渠道Walmart連接憑據、映射屬性或發運標識符，設定選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 的子菜單。 然後，使用 [!DNL Commerce] 訂單選項以處理訂單。</td>
</tr>
</table>


**列說明**

<table>
<tr>
<td>欄位</td>
<td>說明</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>在中分配給訂單的採購訂單編號 [!DNL Walmart Marketplace]。 當訂單最初導入到 [!DNL Channel Manager]，僅 [!DNL Walmart] 此時將顯示訂單編號。 當 [!DNL Commerce] 建立順序， [!DNL Walmart] 訂單號儲存在 [!UICONTROL External ID] 產品屬性。</td>
</tr>
<tr>
<td>[!DNL Commerce] 訂單號</td>
<td>分配給 [!DNL Commerce] 根據 [!DNL Walmart Marketplace] 命令。</td>
</tr>
<tr>
<td>項目</td>
<td>訂購的物料數 [!DNL Walmart Marketplace]。</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>訂購物料的總成本。</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>將訂單提交至 [!DNL Walmart Marketplace] 轉換為本地時區。</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>訂單必須發運的日期才能滿足 [!DNL Walmart Marketplace] 要求轉換為本地時區。
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>必須將訂單交付給客戶以滿足的日期 [!DNL Walmart Marketplace] 要求轉換為本地時區。</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>[[!DNL Walmart Marketplace] 發運方法](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29已為訂單選定。</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>指示上次在中更新訂單資料的時間的時間戳 [!DNL Channel Manager] 轉換為本地時區。</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>指示中的當前訂單狀態 [!DNL Commerce] 訂單工作流。 從導入的訂單的初始狀態 [!DNL Walmart Marketplace] 為_Open_。 當 [!DNL Commerce] 處理和 [!DNL Channel Manager] 成功將裝運、部分裝運和取消更新同步到 [!DNL Walmart Marketplace]。</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>提供有錯誤或退款請求的訂單的詳細資訊。</td>
</tr>
</table>

## 訂單狀態

[!UICONTROL Order Status] 提供有關 [!DNL Walmart Marketplace] 從Adobe Commerce或Magento Open Source處理訂單。 訂單狀態更新發生於 [!DNL Channel Manager] 從其中一個接收更新的訂單資訊 [!DNL Walmart Marketplace] 或 [!DNL Commerce] 訂單制度。 訂單可以具有以下狀態：

- **[!UICONTROL Shipped]** — 已從 [!DNL Commerce] 商店。 當命令發出時， [!DNL Channel Manager] 將更新發送到 [!DNL Walmart Marketplace] 更新Walmart上的發運狀態，並提供發運的訂單跟蹤編號。 在訂單發運後，如果沃爾瑪發出退貨授權表，訂單項目可以部分或全部退還。 請參閱 [退貨和退款](return-refund-orders.md)。

- **[!UICONTROL Partially Shipped]** — 某些物料標籤為已發運，而其他物料等待發運的訂單。 訂單發運中的物料時， [!DNL Channel Manager] 將更新發送到 [!DNL Walmart Marketplace] 要將發運狀態更新為 _[!DNL Partially Shipped]_提供裝運的訂單跟蹤編號。

- **[!UICONTROL Canceled]** — 已從 [!DNL Commerce] 商店。

   訂單取消完成後， [!DNL Commerce] 庫存數量更新以反映退回的物料。 然後， [!DNL Channel Manager] 將更新同步到 [!DNL Walmart Marketplace]。

- **[!UICONTROL Return requested]** — 如果Walmart Marketplace請求退回已發運的訂單， `Return requested` 連結顯示在 [!UICONTROL Status details] 的雙曲餘切值。 選擇連結將開啟 [!UICONTROL Returns] 控制面板以查看退貨並管理退款流程。

- **[!UICONTROL Error]** — 有錯誤的訂單。 訂單更新操作失敗時可能出錯。 例如，如果 [!DNL Channel Manager] 無法從沃爾瑪獲得新訂單。 如果 [!DNL Channel Manager] 無法將訂單發運或取消更新發送到 [!DNL Walmart Marketplace]。 如果操作失敗，「訂單」頁將顯示 _錯誤_ 訂單的狀態。 有關詳細資訊，請參閱 [修復訂單錯誤](process-orders.md#fix-shipping-and-cancelation-errors)。

- **[!UICONTROL Status details]** — 提供有關由於資訊丟失或值無效、發運詳細資訊不正確或訂單取消失敗等問題而發生的訂單錯誤的詳細資訊。 說明有助於確定在 [!DNL Commerce] 實例或 [!DNL Walmart Marketplace]。

>[!NOTE]
>
>如果訂單物料以多發運方式發送，則訂單狀態為 [!DNL Channel Manager] 反映最後一個可用訂單狀態。 例如，如果第一個物料發運，並且在將訂單更新同步到時不返回任何錯誤 [!DNL Channel Manager] 和 [!DNL Walmart Marketplace]，也請參見Wiki頁。 [!DNL Channel Manager] 訂單狀態為 _[!UICONTROL Partially Shipped]_。 如果第二個物料已發運並 [!DNL Channel Manager] 返回錯誤，訂單狀態更新到_[!UICONTROL Error]_。

## 審閱訂單

1. 在管理員中，選擇 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 開啟 [!UICONTROL Channel Manager Marketplace Stores] 的子菜單。

1. 通過在儲存條目行中選擇眼睛表徵圖來開啟儲存視圖。

1. 要查看訂單資訊，請選擇*[!UICONTROL *Orders]**。

1. 通過檢查 **[狀態](#order-status)** 的雙曲餘切值。

## 複查訂單詳細資訊

在從市場接收訂單並導入到您的銷售渠道商店後，使用 [!DNL Commerce] 訂單ID用於查看Adobe Commerce中的訂單詳細資訊。

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

- **訂購的物料** — 本節列出所有Commerce訂單上的訂單項。 的 [!UICONTROL Qty] 列提供訂單物料的狀態歷史記錄。 例如，如果訂單已開票、發運和退款，則您可以看到狀態轉變。

   ![訂單詳細資訊訂購物料狀態歷史記錄 [!DNL Walmart Marketplace] 訂單](assets/order-detail-status-history.png)

通過選擇 [!UICONTROL Invoice] 和 [!UICONTROL Credit Memo] 選項。 您還可以從 [[!UICONTROL Returns]](return-refund-orders.md) 銷售渠道商店中的儀表板。

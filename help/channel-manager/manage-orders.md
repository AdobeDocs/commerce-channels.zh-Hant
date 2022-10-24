---
title: '查看和管理訂單 [!DNL Channel Manager]'
description: '''檢視和管理 [!DNL Walmart Marketplace] 訂購 [!DNL Channel Manager] Adobe Commerce和Magento Open Source。'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 1180c86ee8f087a2fef84d84171d77fd5b33164b
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# 查看和跟蹤訂單 [!DNL Channel Manager]

[!DNL Walmart Marketplace] 訂購資料 [!DNL Commerce] 產品會自動同步至 [!DNL Channel Manager] after [!DNL Walmart] 處理訂單。

在 [!DNL Commerce] 此外，成功的同步會觸發下列動作：

- [!DNL Channel Manager] 向沃爾瑪發出命令確認。

- 對應的 [!DNL Commerce] 訂單是從沃爾瑪的訂單中建立的。

- 更新的訂單資訊會顯示在 [!DNL Channel Manager] 訂單控制面板。

在店面管理員中，您可以從 [!DNL Channel Manager] 開啟銷售渠道商店並選擇 **[!UICONTROL Orders]**.

![要管理的管道管理員訂單檢視 [!DNL Walmart Marketplace] 訂購](assets/orders-dashboard-view.png)

>[!NOTE]
>
>最多需要35分鐘 [!DNL Walmart Marketplace] 顯示順序 [!DNL Channel Manager] 訂單清單。 [!DNL Walmart] 大約需要30分鐘來處理傳入的訂單，並將它們發送到 [!DNL Channel Manager]. 管道管理員收到訂單後，大約需要再花五分鐘的時間，才能在Adobe Commerce或Magento Open Source中建立和顯示訂單。

## 訂購控制項和列說明

下表說明了「訂單」可用的控制項和列。

**的控制[!UICONTROL Orders]**

<table>
<tr>
<td><strong>控制</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>選取以下任一項目，以排序檢視 [!UICONTROL Order Status] 卡片。</td>
</tr>
<tr>
<td>狀態詳細資訊</td>
<td>提供訂單錯誤和退貨請求的相關資訊。 要查看訂單的退貨資訊和退款狀態，請選擇 <strong>[!UICONTROL Return requested]</strong> 要開啟的文字 [!UICONTROL Returns] 控制面板。</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>要查看訂單詳細資訊，請選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 表格。 然後，使用 [!DNL Commerce] 處理訂單的訂單選項。</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>要修改渠道配置，請選擇渠道Walmart連接憑據、映射屬性或發運標識符，設定選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 表格。 然後，使用 [!DNL Commerce] 處理訂單的訂單選項。</td>
</tr>
</table>


**欄說明**

<table>
<tr>
<td>欄位</td>
<td>說明</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>在 [!DNL Walmart Marketplace]. 訂單最初匯入至 [!DNL Channel Manager]，僅 [!DNL Walmart] 訂單編號隨即顯示。 當 [!DNL Commerce] 訂單建立後， [!DNL Walmart] 訂單編號儲存在 [!UICONTROL External ID] 產品屬性。</td>
</tr>
<tr>
<td>[!DNL Commerce] 訂單編號</td>
<td>分配給 [!DNL Commerce] 從 [!DNL Walmart Marketplace] 順序。</td>
</tr>
<tr>
<td>項目</td>
<td>訂購的物料數 [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>訂購物料的總成本。</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>提交訂單的日期 [!DNL Walmart Marketplace] 轉換為當地時區。</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>必須發運訂單以滿足的日期 [!DNL Walmart Marketplace] 需求轉換為當地時區。
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>必須將訂單交付給客戶以滿足的日期 [!DNL Walmart Marketplace] 需求轉換為當地時區。</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>[[!DNL Walmart Marketplace] 發運方法](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29已為訂單選擇。</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>時間戳記，指出上次在 [!DNL Channel Manager] 轉換為當地時區。</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>指示 [!DNL Commerce] 訂購工作流程。 從導入的訂單的初始狀態 [!DNL Walmart Marketplace] 為_Open_。 當 [!DNL Commerce] 處理訂單， [!DNL Channel Manager] 成功將發運、部分發運和取消更新同步到 [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>提供有錯誤或退款請求的訂單的詳細資訊。</td>
</tr>
</table>

## 訂單狀態

[!UICONTROL Order Status] 提供 [!DNL Walmart Marketplace] 從Adobe Commerce或Magento Open Source管理的訂單。 訂單狀態更新發生於 [!DNL Channel Manager] 從其中一個接收更新的訂單資訊 [!DNL Walmart Marketplace] 或 [!DNL Commerce] 訂購系統。 訂單可具有下列狀態：

- **[!UICONTROL Shipped]** — 已從 [!DNL Commerce] 儲存。 當訂單出貨時， [!DNL Channel Manager] 將更新傳送至 [!DNL Walmart Marketplace] 要更新Walmart上的發運狀態，並提供發運的訂單跟蹤編號。 在訂單發運後，如果沃爾瑪發出「退貨授權表」，訂單項目可以部分或完全退貨。 請參閱 [退貨與退款](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]** — 某些物料標籤為已發運，而其他物料等待發運的訂單。 當訂單中的物料發運時， [!DNL Channel Manager] 將更新傳送至 [!DNL Walmart Marketplace] 要將發運狀態更新為 _[!DNL Partially Shipped]_提供裝運的訂單跟蹤編號。

- **[!UICONTROL Canceled]** — 已從 [!DNL Commerce] 儲存。

   訂單取消完成後， [!DNL Commerce] 庫存數量更新以反映退貨。 然後， [!DNL Channel Manager] 將更新同步至 [!DNL Walmart Marketplace].

- **[!UICONTROL Return requested]** — 如果Walmart Marketplace請求退回已發運的訂單項目， `Return requested` 連結會顯示在 [!UICONTROL Status details] 欄。 選取連結會開啟 [!UICONTROL Returns] 控制面板來檢視退貨及管理退款流程。

- **[!UICONTROL Error]** — 有錯誤的訂單。 訂單更新操作失敗時可能會發生錯誤。 例如，若 [!DNL Channel Manager] 無法收到沃爾瑪的新訂單。 如果 [!DNL Channel Manager] 無法將訂單發運或取消更新發送到 [!DNL Walmart Marketplace]. 如果操作失敗，「訂購」頁面會顯示 _錯誤_ 訂單的狀態。 如需詳細資訊，請參閱 [修正訂單錯誤](process-orders.md#fix-shipping-and-cancelation-errors)。

- **[!UICONTROL Status details]** — 提供有關訂單錯誤的詳細資訊，這些錯誤是由於缺少資訊或值無效、發運詳細資訊不正確或訂單取消失敗等問題而發生的。 說明有助於判斷 [!DNL Commerce] 例項或 [!DNL Walmart Marketplace].

>[!NOTE]
>
>如果訂單物料以多個發運發送，則訂單狀態為 [!DNL Channel Manager] 會反映最後可用的訂單狀態。 例如，如果第一個項目發貨，且訂單更新同步至時未傳回任何錯誤 [!DNL Channel Manager] 和 [!DNL Walmart Marketplace], [!DNL Channel Manager] 訂單狀態為 _[!UICONTROL Partially Shipped]_. 如果已發運第二個物料，並且 [!DNL Channel Manager] 傳回錯誤，順序狀態會更新為_[!UICONTROL Error]_.

## 審核訂單

1. 在管理員中，選取 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 開啟 [!UICONTROL Channel Manager Marketplace Stores] 頁面。

1. 在商店登入列中選取眼睛圖示，以開啟商店檢視。

1. 要查看訂單資訊，請選擇*[!UICONTROL *Orders]**。

1. 取得訂單的相關資訊，並透過檢查 **[狀態](#order-status)** 欄。

## 查看訂單詳細資訊

從市集收到訂單並匯入至您的銷售管道商店後，請使用 [!DNL Commerce] 訂單ID可在Adobe Commerce中檢視訂單詳細資料。

從 **[!UICONTROL Orders]**，請選取 **[!UICONTROL Commerce Order Number]** 開啟 [!DNL Commerce] 訂單詳細資料。

![的商務訂單詳細資訊視圖 [!DNL Walmart Marketplace] 訂購](assets/order-detail-with-external-order-id.png)

在「商務」店面中，從 [!DNL Walmart Marketplace] 訂單資料中包含下列其他資訊：

- **付款資訊和發運方法** — 從Walmart導入的訂單包括以下付款和發運欄位的值：

   - **[!UICONTROL Offline Channel Payment]** — 指示離線處理訂單付款的方式 [!DNL Walmart Marketplace].

   - **[!UICONTROL External Order Number]** — 顯示 [!DNL Walmart Marketplace] 訂單編號。

   - **[!UICONTROL Channel Shipping - Value]** — 表示運費是通過 [!DNL Walmart Marketplace].

   - **[!UICONTROL Cancellation Reason]** — 只有從導入的訂單 [!DNL Walmart Marketplace] 已取消。 取消原因包括：

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **訂購的物料** — 本節列出所有Commerce訂單上的訂單項。 此 [!UICONTROL Qty] 欄提供訂單項目的狀態歷史記錄。 例如，如果訂單已開具發票、已發運和已退貨，您可以看到狀態轉變。

   ![訂單詳細資訊訂購物料狀態歷史記錄 [!DNL Walmart Marketplace] 訂購](assets/order-detail-status-history.png)

通過選擇 [!UICONTROL Invoice] 和 [!UICONTROL Credit Memo] 選項。 您也可以直接從 [[!UICONTROL Returns]](return-refund-orders.md) 控制面板。




---
title: 退貨與退款訂單
description: 針對收到的退貨請求發出全部或部分退款的指示 [!DNL Walmart Marketplace] 從 [!DNL Channel Manager] 適用於Adobe Commerce和Magento Open Source。
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1184'
ht-degree: 0%

---

# 退貨與退款訂單

當採購員要求退貨購買到的訂單料號時 [!DNL Walmart Marketplace]，Walmart會建立退貨要求。 [!DNL Channel Manager] 會監控這些要求的市集管道，並自動將傳回要求資訊同步至管道管理員。

在Commerce端，傳回要求會起始下列工作流程：

1. Channel Manager會建立具有已接收狀態的對應傳回要求，並新增傳回ID編號([!UICONTROL RMA #])到 [!UICONTROL Returns] 儀表板。 在 [!DNL Orders] 儀表板，與退貨更新相關聯的訂單狀態詳細資訊，以包含 [!UICONTROL Return requested] 檢視及處理退貨的連結。

1. 商戶會在下列步驟之後建立「銷退折讓單」，以處理與退貨相關的退款 [Adobe Commerce退款工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html). 所有退款均使用離線方式處理。

1. [!DNL Channel Manager] 將退款更新傳送至Walmart marketplace，以便更新退貨狀態，反映Adobe Commerce已完成的退款。

在店面管理員中，您可以透過開啟銷售管道商店並選取「 」，檢視及處理「管道管理員」的退貨 **[!UICONTROL Returns]**.

![「管道經理退貨」儀表板可針對收到的退貨請求處理退款 [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>您只能處理已出貨訂單的退款。 在 [!DNL Channel Manager]，訂單狀態必須為 [!UICONTROL Shipped]. 在 [!DNL Walmart Marketplace] 賣家帳戶，訂單必須為 [!UICONTROL Delivered].

## 傳回控制項和資料行說明

下清單格說明可用的控制項與欄 [!DNL Channel Manager] 會傳回。

**控制項[!UICONTROL Returns]**

<table>
<tr>
<td><strong>控制</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>選取其中一個以篩選檢視 [!UICONTROL Return Status] 卡片。</td>
</tr>
<tr>
<td>狀態詳細資訊</td>
<td>對於含有以下各項的傳回專案： [!UICONTROL Received] 或 [!UICONTROL Refunded] 狀態，您可以在「狀態明細」欄位中選取連結的文字，來建立或檢視退款的銷退折讓單。</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>若要檢視訂單詳細資料，請選取 [!DNL Commerce] 中的訂單編號 [!UICONTROL Order] 表格以開啟Commerce訂單。</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>若要修改通道組態，請選取通道Walmart連線認證、對應的屬性或出貨識別碼，設定請選取 [!DNL Commerce] 中的訂單編號 [!UICONTROL Order] 表格。 然後，使用 [!DNL Commerce] 訂單選項以處理訂單。</td>
</tr>
</table>

**欄說明**

<table>
<tr>
<td><strong>欄位</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>與從收到的退貨要求相關聯的退貨商品授權號碼 [!DNL Walmart Marketplace]. 此號碼是由Walmart Marketplace產生 [!UICONTROL Returns] 當退貨程式啟動時。</td>
</tr>
<tr>
<td>[!DNL Commerce] 訂單編號</td>
<td>此 [!DNL Commerce] 與Walmart Marketplace的退貨要求中所包含的專案相關聯的訂單編號。 選取訂單編號，以檢視訂單詳細資料。</td>
</tr>
<tr>
<td>已要求</td>
<td>要求退貨的日期 [!DNL Walmart Marketplace]
轉換為當地時間。</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>必須退款才能達到的退款日期 [!DNL Walmart Marketplace] [需求](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f)轉換為當地時間。</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>列出退貨中所列各料號的SKU與數量。</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>退回專案要退款的總值。</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>指示中目前的傳回狀態 [!DNL Commerce] 回訪工作流程 — <i>已接收</i>， <i>已退款</i>，或 <i>錯誤</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>針對已接收與已退款的退貨分錄，狀態詳細資料會提供存取退款處理之銷退折讓單的連結。 如果期間發生錯誤 [!DNL Channel Manager] Adobe Commerce與之間的同步程式 [!DNL Walmart marketplace]，此欄位提供錯誤說明。</td>
</tr>
</table>

## 傳回狀態

[!UICONTROL Return Status] 提供目前狀態的相關資訊 [!DNL Walmart Marketplace] 從Adobe Commerce或Magento Open Source管理的傳回請求。

傳回狀態更新發生於 [!DNL Channel Manager] 接收來自的傳回要求 [!DNL Walmart Marketplace] 或當 [!DNL Commerce] 已建立銷退折讓單，以處理退回料號的退款。

傳回可具有下列狀態：

* **[!UICONTROL Received]** — 這是從收到的傳回要求的初始狀態 [!DNL Walmart Marketplace] 商店。 商家可以選取以下專案，以處理退貨 **[!UICONTROL Create credit memo]** 在 [!UICONTROL Status details].

* **[!UICONTROL Refunded]** — 表示已建立銷退折讓單，以發放退回專案的退款。 商戶可藉由選取「 」，檢視退款資訊 **[!UICONTROL View credit memo]** 在 [!UICONTROL Status details].

* **[!UICONTROL Error]** — 傳回含有錯誤的請求。 當來自Walmart的傳回要求遺失或不正確的資料時，可能會發生錯誤。 或者，如果 [!DNL Channel Manager] 無法傳送退款更新通知給Walmart。

## 傳回案例

以下案例說明如何針對不同的退貨請求型別發放退款 [!DNL Channel Manager].

* **完整退貨** — 如果Walmart Marketplace退貨請求是針對訂單中的所有專案，請更新銷退折讓單數量，以退回所有專案。

* **部分傳回** — 如果「沃爾瑪市集」退貨請求只針對某些訂單專案，請只針對要退款的專案更新銷退折讓單數量。

* **已透過沃爾瑪市集退款** — 在某些情況下，退款會在以下日期處理： [!DNL Walmart Marketplace] 在「管道管理員」中處理傳回之前。 例如，如果Commerce訂單未在Walmart要求的48小時退款處理期間內退款，則Walmart會自動退款。 發生此情況時，「管道管理員」仍會將退貨請求同步至Adobe Commerce，因此您可以處理退貨並簽發銷退折讓單。 此工作流程可確保中的訂單詳細資料 [!DNL Commerce] 符合Walmart Marketplace中的訂單資訊。

>[!NOTE]
>
> 退款更新最多可能需要5分鐘的時間才能同步至 [!DNL Walmart Marketplace]. 您可從「 」檢查目前的回訪狀態 [!DNL Channel Manager] [!UICONTROL Returns] 儀表板。

## 處理退款請求

1. 開啟 [!UICONTROL Returns] 您的sales channel商店的儀表板。

   * 在「管理員」中，選取 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * 選取銷售管道商店的眼睛圖示，以開啟商店檢視。

   * 您可以選取 **[!UICONTROL Returns]** 標籤。

     您也可以從以下位置存取傳回資訊 [!UICONTROL Orders] 頁面。 尋找 [!UICONTROL Shipped] 有退貨請求的訂單。 然後，選取 `Return requested` 中的連結 [!UICONTROL Status Details] 欄，以檢視及處理請求。

1. 從「傳回」表格中，尋找含有下列專案的傳回： *[!UICONTROL Received]* 狀態。

1. 在料號欄位中，複查訂單料號清單與要退款的數量。

1. 藉由簽發銷退折讓單來處理退款。

   * 從 [!UICONTROL Status Details] 欄，選取 **[!UICONTROL Create credit memo]** 以開啟訂單詳細資訊頁面 [!DNL Commerce].

     如果訂單尚未開立商業發票，「訂單明細」頁面會顯示錯誤訊息，提示您建立訂單。 選取 **[!UICONTROL Create invoice]**. 然後 [建立並儲存發票](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html).

   * 在訂單詳細資訊頁面上，選取 **[!UICONTROL Credit Memo]**.

   * 在 [!UICONTROL Items to Refund] 的區段 [!UICONTROL Credit Memo]，更新 **[!UICONTROL Qty to refund]** 和 **[!UICONTROL Return to Stock]** 退貨要求中包含之專案的資訊。

     請確定只傳回要求中列出的專案。

   * 若要新增註解，請在 **[!UICONTROL Credit Memo Comments]**

   * 選取 **[!UICONTROL Refund Offline]**.

完成退款後， [!DNL Channel Manager] 更新中的傳回狀態 [!UICONTROL Returns] 報告面板至 [!UICONTROL Refunded] 並將更新同步至Walmart，以更新Marketplace中的退貨狀態。


## 檢視退貨的退款資訊

您可以檢視退貨請求與退款處理的相關資訊，請參閱 [!UICONTROL Returns] 儀表板。

1. 開啟您銷售管道商店的「退貨」儀表板。

   * 在「管理員」中，選取 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * 選取銷售管道商店的眼睛圖示，以開啟商店檢視。

   * 選取 **[!UICONTROL Returns]**.

1. 選取「 」以檢視退款的訂單 **[!UICONTROL Refunded]** 狀態卡。

1. 選取以檢視退貨的退款明細 **[!UICONTROL View credit memo]**.

   ![用於退款的銷退折讓單 [!DNL Walmart Marketplace] 訂購](assets/refund-credit-memo-for-marketplace-order.png){width="600" zoomable="yes"}

>[!NOTE]
>
>訂單退款後， [!UICONTROL Orders] 儀表板未顯示傳回資訊。 若要檢視退貨資訊，請使用 [!DNL Channel Manager] 傳回儀表板。 您也可以從「訂單詳細資料」頁面取得更詳細的退貨與退款資訊。

## 修正傳回錯誤

從收到傳回資訊時，可能會發生錯誤 [!DNL Walmart Marketplace]，或當 [!DNL Channel Manager] 從同步狀態更新 [!DNL Commerce] 至 [!DNL Walmart Marketplace].

如果傳回更新的同步化作業失敗， [!DNL Channel Manager] 傳回控制面板顯示 *[!UICONTROL Error]* 退貨專案的狀態。 為確保退貨和退款資訊準確反映在Walmart Marketplace帳戶中，請手動更新 [!DNL Walmart Marketplace] 商店。

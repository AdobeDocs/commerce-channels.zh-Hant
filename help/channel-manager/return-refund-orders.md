---
title: 退貨與退款訂單
description: 針對從 [!DNL Walmart Marketplace] 接收的Adobe Commerce和Magento Open Source的 [!DNL Channel Manager] 退貨要求發出全部或部分退款的指示。
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# 退貨與退款訂單

當買家要求退貨透過[!DNL Walmart Marketplace]購買的訂單專案時，Walmart會建立退貨要求。 [!DNL Channel Manager]會監視這些要求的市集管道，並自動將傳回要求資訊同步至管道管理員。

在Commerce端，傳回要求會起始下列工作流程：

1. 管道管理員會建立具有已接收狀態的對應傳回要求，並將傳回識別碼([!UICONTROL RMA #])新增到[!UICONTROL Returns]儀表板。 在[!DNL Orders]儀表板上，與退貨更新相關之訂單的狀態詳細資訊將包含[!UICONTROL Return requested]連結，以檢視及處理退貨。

1. 商家在[Adobe Commerce退款工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html)之後建立「銷退折讓單」，以處理與退貨相關的退款。 所有退款均使用離線方式處理。

1. [!DNL Channel Manager]傳送退款更新至Walmart Marketplace，以便更新退貨狀態，反映Adobe Commerce已完成的退款。

在店面管理員中，您可以透過開啟銷售管道商店並選取&#x200B;**[!UICONTROL Returns]**&#x200B;來檢視及處理管道管理員的退貨。

![管道管理員退款儀表板，用於處理從[!DNL Walmart Marketplace]](assets/returns-dashboard-view.png){width="600" zoomable="yes"}收到的退款要求

>[!NOTE]
>
>您只能處理已出貨訂單的退款。 在[!DNL Channel Manager]中，訂單狀態必須為[!UICONTROL Shipped]。 在[!DNL Walmart Marketplace]賣家帳戶中，訂單必須為[!UICONTROL Delivered]。

## 傳回控制項和資料行說明

下清單格說明[!DNL Channel Manager]傳回可用的控制項與資料行。

[!UICONTROL Returns]**的**&#x200B;控制項

<table>
<tr>
<td><strong>控制</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>選取[!UICONTROL Return Status]張卡片之一，以篩選檢視。</td>
</tr>
<tr>
<td>狀態詳細資訊</td>
<td>針對狀態為[!UICONTROL Received]或[!UICONTROL Refunded]的退貨專案，您可以在「狀態詳細資料」欄中選取連結的文字，建立或檢視退款的銷退折讓單。</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>若要檢視訂單詳細資料，請選取[!UICONTROL Order]表格中的[!DNL Commerce]訂單編號以開啟Commerce訂單。</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>若要修改通道組態，請選取通道Walmart連線認證、對應的屬性或送貨識別碼，設定請在[!UICONTROL Order]表格中選取[!DNL Commerce]訂單編號。 然後，使用[!DNL Commerce]訂單選項來處理訂單。</td>
</tr>
</table>

**資料行說明**

<table>
<tr>
<td><strong>欄位</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>與從[!DNL Walmart Marketplace]收到的退貨要求相關聯的退貨商品授權號碼。 此號碼是由Walmart Marketplace [!UICONTROL Returns]在啟動退貨程式時產生。</td>
</tr>
<tr>
<td>[!DNL Commerce] 訂單編號</td>
<td>與Walmart Marketplace退貨要求中所包含的專案相關聯的[!DNL Commerce]訂單編號。 選取訂單編號，以檢視訂單詳細資料。</td>
</tr>
<tr>
<td>已要求</td>
<td>要求傳回的日期為[!DNL Walmart Marketplace]
轉換為當地時間。</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>必須退款以符合[!DNL Walmart Marketplace] [需求](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f)的日期，已轉換為當地時間。</td>
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
<td>指示[!DNL Commerce]傳回工作流程中的目前傳回狀態 — <i>已接收</i>、<i>已退款</i>或<i>錯誤</i>。</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>針對已接收與已退款的退貨分錄，狀態詳細資料會提供存取退款處理之銷退折讓單的連結。 如果在Adobe Commerce與[!DNL Walmart marketplace]之間的[!DNL Channel Manager]同步處理過程中發生錯誤，此欄位將提供錯誤說明。</td>
</tr>
</table>

## 傳回狀態

[!UICONTROL Return Status]提供從Adobe Commerce或Magento Open Source管理的[!DNL Walmart Marketplace]個傳回要求之目前狀態的資訊。

當[!DNL Channel Manager]收到來自[!DNL Walmart Marketplace]的退貨要求或建立[!DNL Commerce]銷退折讓單以處理退貨專案的退款時，就會發生退貨狀態更新。

傳回可具有下列狀態：

* **[!UICONTROL Received]** — 這是從[!DNL Walmart Marketplace]存放區接收的傳回要求的初始狀態。 商家可以選取[!UICONTROL Status details]中的&#x200B;**[!UICONTROL Create credit memo]**&#x200B;來處理退款。

* **[!UICONTROL Refunded]** — 表示已建立銷退折讓單以發放退回專案的退款。 商戶可以在[!UICONTROL Status details]中選取&#x200B;**[!UICONTROL View credit memo]**&#x200B;以檢視退款資訊。

* **[!UICONTROL Error]** — 傳回含有錯誤的請求。 當來自Walmart的傳回要求遺失或不正確的資料時，可能會發生錯誤。 或者，如果[!DNL Channel Manager]無法傳送退款更新通知給Walmart。

## 傳回案例

下列案例說明如何針對[!DNL Channel Manager]中不同型別的退貨請求發放退款。

* **完整退貨** — 如果Walmart Marketplace退貨要求適用於訂單中的所有專案，請更新銷退折讓單數量以退款所有專案。

* **部份退貨** — 如果沃爾瑪市集退貨要求只針對某些訂單專案，請只針對要退款的專案更新銷退折讓單數量。

* **退貨已透過Walmart Marketplace退款** — 在某些情況下，退款會在[!DNL Walmart Marketplace]處理，然後再於「通路管理員」處理退款。 例如，如果Commerce訂單未在Walmart要求的48小時退款處理期間內退款，Walmart會自動退款。 發生此情況時，「管道管理員」仍會將退貨請求同步至Adobe Commerce，因此您可以處理退貨並簽發銷退折讓單。 此工作流程會確保[!DNL Commerce]中的訂單詳細資料符合Walmart Marketplace中的訂單資訊。

>[!NOTE]
>
> 退款更新最多可能需要5分鐘的時間才能同步處理至[!DNL Walmart Marketplace]。 您可以從[!DNL Channel Manager] [!UICONTROL Returns]儀表板檢查目前的傳回狀態。

## 處理退款請求

1. 開啟您銷售管道商店的[!UICONTROL Returns]儀表板。

   * 從Admin中，選取&#x200B;**[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**。

   * 選取銷售管道商店的眼睛圖示，以開啟商店檢視。

   * 您可以選取&#x200B;**[!UICONTROL Returns]**&#x200B;索引標籤來檢閱退貨。

     您也可以從[!UICONTROL Orders]頁面存取傳回資訊。 尋找具有退貨請求的[!UICONTROL Shipped]訂單。 然後，選取[!UICONTROL Status Details]欄中的`Return requested`連結以檢視及處理要求。

1. 從Returns表格中，尋找狀態為&#x200B;*[!UICONTROL Received]*&#x200B;的傳回。

1. 在料號欄位中，複查訂單料號清單與要退款的數量。

1. 藉由簽發銷退折讓單來處理退款。

   * 從[!UICONTROL Status Details]欄中選取&#x200B;**[!UICONTROL Create credit memo]**&#x200B;以在[!DNL Commerce]中開啟訂單詳細資料頁面。

     如果訂單尚未開立商業發票，「訂單明細」頁面會顯示錯誤訊息，提示您建立訂單。 選取&#x200B;**[!UICONTROL Create invoice]**。 然後，[建立並儲存發票](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html)。

   * 在訂單詳細資訊頁面上，選取&#x200B;**[!UICONTROL Credit Memo]**。

   * 在[!UICONTROL Credit Memo]的[!UICONTROL Items to Refund]區段中，更新傳回要求中包含之專案的&#x200B;**[!UICONTROL Qty to refund]**&#x200B;與&#x200B;**[!UICONTROL Return to Stock]**&#x200B;資訊。

     請確定只傳回要求中列出的專案。

   * 若要新增註解，請在&#x200B;**[!UICONTROL Credit Memo Comments]**&#x200B;中輸入文字

   * 選取&#x200B;**[!UICONTROL Refund Offline]**。

完成退款後，[!DNL Channel Manager]會將[!UICONTROL Returns]儀表板中的退貨狀態更新為[!UICONTROL Refunded]，並將更新同步至Walmart，以更新市集中的退貨狀態。


## 檢視退貨的退款資訊

您可以從[!UICONTROL Returns]儀表板檢視退貨請求和退款處理的相關資訊。

1. 開啟您銷售管道商店的「退貨」儀表板。

   * 從Admin中，選取&#x200B;**[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**。

   * 選取銷售管道商店的眼睛圖示，以開啟商店檢視。

   * 選取&#x200B;**[!UICONTROL Returns]**。

1. 選取&#x200B;**[!UICONTROL Refunded]**&#x200B;狀態卡以檢視已退款的訂單。

1. 選取&#x200B;**[!UICONTROL View credit memo]**，檢視退貨的退款詳細資料。

   ![退款[!DNL Walmart Marketplace]訂單之退回專案的銷退折讓單](assets/refund-credit-memo-for-marketplace-order.png){width="600" zoomable="yes"}

>[!NOTE]
>
>訂單退款後，[!UICONTROL Orders]儀表板不會顯示退貨資訊。 若要檢視退貨資訊，請使用[!DNL Channel Manager]退貨儀表板。 您也可以從「訂單詳細資料」頁面取得更詳細的退貨與退款資訊。

## 修正傳回錯誤

從[!DNL Walmart Marketplace]收到傳回資訊時，或當[!DNL Channel Manager]將狀態更新從[!DNL Commerce]同步到[!DNL Walmart Marketplace]時，可能會發生錯誤。

如果傳回更新的同步化作業失敗，[!DNL Channel Manager]傳回儀表板會顯示傳回專案的&#x200B;*[!UICONTROL Error]*&#x200B;狀態。 為了確保退貨和退款資訊準確反映在Walmart Marketplace帳戶中，請手動更新[!DNL Walmart Marketplace]商店中的訂單。

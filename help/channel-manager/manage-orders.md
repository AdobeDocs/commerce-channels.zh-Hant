---
title: '檢視及管理來自 [!DNL Channel Manager]的訂單'
description: '檢視並管理 [!DNL Channel Manager] 的Adobe Commerce和Magento Open Source [!DNL Walmart Marketplace] 訂單。'
feature: Sales Channels, Orders
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

# 從[!DNL Channel Manager]檢視及追蹤訂單

[!DNL Walmart]處理訂單後，[!DNL Commerce]產品的[!DNL Walmart Marketplace]訂單資料會自動同步至[!DNL Channel Manager]。

在[!DNL Commerce]端，成功的同步處理會觸發下列動作：

- [!DNL Channel Manager]傳送訂單確認給Walmart。

- 從Walmart訂單建立對應的[!DNL Commerce]訂單。

- 更新的訂單資訊會顯示在[!DNL Channel Manager]訂單儀表板上。

在店面管理員中，您可以透過開啟銷售管道商店並選取&#x200B;**[!UICONTROL Orders]**&#x200B;來檢視[!DNL Channel Manager]的訂單資料。

![管道管理員訂單檢視以管理[!DNL Walmart Marketplace]個訂單](assets/orders-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>[!DNL Walmart Marketplace]訂單可能需要35分鐘的時間才會顯示在[!DNL Channel Manager]訂單清單中。 [!DNL Walmart]大約需要30分鐘來處理傳入的訂單，並將它們傳送到[!DNL Channel Manager]。 Channel Manager收到訂單後，大約需要5分鐘才能在Adobe Commerce或Magento Open Source中建立並顯示訂單。

## 訂單控制項與欄位說明

下清單格說明「訂單」可用的控制項與欄位。

[!UICONTROL Orders]**的**&#x200B;控制項

<table>
<tr>
<td><strong>控制</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>選取[!UICONTROL Order Status]張卡片之一來排序檢視。</td>
</tr>
<tr>
<td>狀態詳細資訊</td>
<td>提供有關訂單錯誤和退貨請求的資訊。 若要檢視訂單的退貨資訊和退款狀態，請選取<strong>[!UICONTROL Return requested]</strong>文字以開啟[!UICONTROL Returns]儀表板。</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>若要檢視訂單詳細資料，請在[!UICONTROL Order]表格中選取[!DNL Commerce]訂單編號。 然後，使用[!DNL Commerce]訂單選項來處理訂單。</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>若要修改通道組態，請選取通道Walmart連線認證、對應的屬性或送貨識別碼，設定請在[!UICONTROL Order]表格中選取[!DNL Commerce]訂單編號。 然後，使用[!DNL Commerce]訂單選項來處理訂單。</td>
</tr>
</table>


**資料行說明**

<table>
<tr>
<td>欄位</td>
<td>說明</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>在[!DNL Walmart Marketplace]中指派給訂單的採購單編號。 當訂單最初匯入至[!DNL Channel Manager]時，只顯示[!DNL Walmart]訂單編號。 建立[!DNL Commerce]訂單時，[!DNL Walmart]訂單編號會儲存在[!UICONTROL External ID]產品屬性中。</td>
</tr>
<tr>
<td>[!DNL Commerce] 訂單編號</td>
<td>指派給從[!DNL Walmart Marketplace]訂單建立的[!DNL Commerce]訂單的編號。</td>
</tr>
<tr>
<td>專案</td>
<td>在[!DNL Walmart Marketplace]上訂購的專案數。</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>訂購料號的總成本。</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>將訂單提交至[!DNL Walmart Marketplace]的日期已轉換為當地時區。</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>訂單必須寄出以符合轉換為當地時區的[!DNL Walmart Marketplace]需求的日期。
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>訂單必須遞送給客戶以符合轉換為當地時區的[!DNL Walmart Marketplace]要求的日期。</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>為訂單選取的[[!DNL Walmart Marketplace]送貨方法](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29)。</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>表示上次將訂單資料在[!DNL Channel Manager]中更新為當地時區的時間戳記。</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>指示[!DNL Commerce]訂單工作流程中的目前訂單狀態。 從[!DNL Walmart Marketplace]匯入之訂單的初始狀態為_Open_。 當處理[!DNL Commerce]個訂單且[!DNL Channel Manager]成功同步處理[!DNL Walmart Marketplace]的裝運、部分裝運和取消更新時，會發生其他狀態更新。</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>提供有關出現錯誤或退款請求的訂單的詳細資訊。</td>
</tr>
</table>

## 訂單狀態

[!UICONTROL Order Status]提供有關從Adobe Commerce或Magento Open Source管理的[!DNL Walmart Marketplace]個訂單之目前狀態的資訊。 當[!DNL Channel Manager]從[!DNL Walmart Marketplace]或[!DNL Commerce]訂單系統收到更新的訂單資訊時，就會發生訂單狀態更新。 訂單可以有下列狀態：

- **[!UICONTROL Shipped]** — 已從[!DNL Commerce]存放區出貨的訂單。 當訂單出貨時，[!DNL Channel Manager]會傳送更新給[!DNL Walmart Marketplace]，以更新Walmart上的出貨狀態，並提供出貨的訂單追蹤編號。 訂單出貨後，如果沃爾瑪簽發「退貨商品授權」表單，訂單專案可以部份或全部退款。 請參閱[退貨與退款](return-refund-orders.md)。

- **[!UICONTROL Partially Shipped]** — 有些料號標示為已出貨，而其他料號則等待出貨的訂單。 當訂單中的專案出貨時，[!DNL Channel Manager]傳送更新給[!DNL Walmart Marketplace]，以將出貨狀態更新為Walmart上的&#x200B;_[!DNL Partially Shipped]_，並提供出貨的訂單追蹤號碼。

- **[!UICONTROL Canceled]** — 已從[!DNL Commerce]存放區取消的訂單。

  訂單取消完成後，[!DNL Commerce]庫存數量會更新以反映傳回的專案。 然後，[!DNL Channel Manager]將更新同步到[!DNL Walmart Marketplace]。

- **[!UICONTROL Return requested]** — 如果Walmart Marketplace要求退回已出貨的訂單專案，則[!UICONTROL Status details]欄中會顯示`Return requested`連結。 選取連結會開啟[!UICONTROL Returns]儀表板以檢視退款並管理退款程式。

- **[!UICONTROL Error]** — 有錯誤的訂單。 訂單更新作業失敗時可能會發生錯誤。 例如，如果[!DNL Channel Manager]無法從Walmart收到新訂單，就會發生錯誤。 如果[!DNL Channel Manager]無法傳送訂單出貨或取消更新至[!DNL Walmart Marketplace]，也可能發生這種情況。 如果作業失敗，「訂單」頁面會顯示訂單的&#x200B;_錯誤_&#x200B;狀態。 如需詳細資訊，請參閱[修正訂單錯誤](process-orders.md#fix-shipping-and-cancellation-errors)。

- **[!UICONTROL Status details]** — 提供因遺失資訊或無效值、不正確的出貨詳細資訊或訂單取消失敗等問題而發生訂單錯誤的相關資訊。 說明可協助判斷[!DNL Commerce]執行個體或[!DNL Walmart Marketplace]上是否發生錯誤。

>[!NOTE]
>
>如果訂單料號是以多筆出貨方式傳送，[!DNL Channel Manager]中的訂單狀態會反映最後一個可用的訂單狀態。 例如，如果第一個專案出貨，且在訂單更新同步處理至[!DNL Channel Manager]和[!DNL Walmart Marketplace]時未傳回任何錯誤，則[!DNL Channel Manager]訂單狀態為&#x200B;_[!UICONTROL Partially Shipped]_。 如果第二個專案已送出，[!DNL Channel Manager]傳回錯誤，則訂單狀態會更新為_[!UICONTROL Error]_。

## 檢閱訂單

1. 從Admin中，選取&#x200B;**[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**&#x200B;以開啟[!UICONTROL Channel Manager Marketplace Stores]頁面。

1. 選取商店專案列中的眼睛圖示，開啟商店檢視。

1. 若要檢視訂單資訊，請選取*[!UICONTROL *Orders]**。

1. 請檢查&#x200B;**[狀態](#order-status)**&#x200B;資料行，以取得訂單的相關資訊，並決定後續步驟。

## 檢閱訂單詳細資料

收到來自市集的訂單並匯入您的銷售管道商店後，請使用[!DNL Commerce]訂單ID在Adobe Commerce中檢視訂單詳細資料。

從&#x200B;**[!UICONTROL Orders]**&#x200B;中，選取&#x200B;**[!UICONTROL Commerce Order Number]**&#x200B;以開啟[!DNL Commerce]訂單詳細資料。

[!DNL Walmart Marketplace]訂單的![Commerce訂單詳細資料檢視](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

在Commerce店面中，從[!DNL Walmart Marketplace]匯入的訂單在訂單資料中包含下列額外資訊：

- **付款資訊與送貨方式** — 從Walmart匯入的訂單包含下列付款與送貨欄位的值：

   - **[!UICONTROL Offline Channel Payment]** — 表示[!DNL Walmart Marketplace]已離線處理訂單付款。

   - **[!UICONTROL External Order Number]** — 顯示[!DNL Walmart Marketplace]訂單編號。

   - **[!UICONTROL Channel Shipping - Value]** — 表示已透過[!DNL Walmart Marketplace]處理運費。

   - **[!UICONTROL Cancellation Reason]** — 此欄位只有在從[!DNL Walmart Marketplace]匯入的訂單取消時才會顯示。 取消原因包括：

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **訂購的專案** — 此區段會列出所有Commerce訂單上的訂購專案。 [!UICONTROL Qty]欄提供訂單專案的狀態歷史記錄。 例如，如果訂單已開立商業發票、出貨及退款，您就可以檢視狀態轉換。

  ![訂單詳細資訊訂購專案狀態歷史記錄[!DNL Walmart Marketplace]個訂單](assets/order-detail-status-history.png){width="600" zoomable="yes"}

從瀏覽功能表中選取[!UICONTROL Invoice]和[!UICONTROL Credit Memo]選項，以檢視專案發票和退款詳細資料。 您也可以直接從Sales Channel商店的[[!UICONTROL Returns]](return-refund-orders.md)儀表板存取銷退折讓單。

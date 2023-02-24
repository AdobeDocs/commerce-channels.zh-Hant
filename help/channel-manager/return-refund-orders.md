---
title: 退貨訂單和退款訂單
description: 關於對從以下網站收到的返還請求發出全額或部分退款的指示 [!DNL Walmart Marketplace] 從 [!DNL Channel Manager] Adobe Commerce和Magento Open Source。
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# 退貨訂單和退款訂單

當採購員請求退貨時， [!DNL Walmart Marketplace]，沃爾瑪會建立回訪請求。 [!DNL Channel Manager] 監控這些請求的市集管道，並自動將傳回請求資訊同步至管道管理員。

在商務端，傳回請求會起始下列工作流程：

1. 管道管理員會建立具有接收狀態的對應傳回請求，並新增傳回ID號碼([!UICONTROL RMA #]) [!UICONTROL Returns] 控制面板。 在 [!DNL Orders] 控制面板，與回訪更新相關聯的順序的狀態詳細資料，以包含 [!UICONTROL Return requested] 連結以檢視及處理傳回。

1. 商家通過在 [Adobe Commerce退款工作流程](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow). 所有退款都使用離線方法處理。

1. [!DNL Channel Manager] 向沃爾瑪市場發送退款更新，以便更新退貨狀態，以反映從Adobe Commerce獲得的已完成退款。

在店面管理員中，您可以開啟銷售管道商店並選取 **[!UICONTROL Returns]**.

![Channel Manager返回控制面板以處理從接收的回訪請求的退款 [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png)

>[!NOTE]
>
>您只能處理已發運訂單的退款。 在 [!DNL Channel Manager]，訂單狀態必須是 [!UICONTROL Shipped]. 在 [!DNL Walmart Marketplace] 賣方帳戶，訂單必須 [!UICONTROL Delivered].

## 傳回控制項和欄說明

下表說明可用於 [!DNL Channel Manager] 傳回。

**的控制[!UICONTROL Returns]**

<table>
<tr>
<td><strong>控制</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>選取以下任一項目以篩選檢視 [!UICONTROL Return Status] 卡片。</td>
</tr>
<tr>
<td>狀態詳細資訊</td>
<td>對於具有 [!UICONTROL Received] 或 [!UICONTROL Refunded] 狀態，您可以通過在「狀態詳細資訊」列中選擇連結的文本來建立或查看退款的貸項通知單。</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>要查看訂單詳細資訊，請選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 表格來開啟商務順序。</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>要修改渠道配置，請選擇渠道Walmart連接憑據、映射屬性或發運標識符，設定選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 表格。 然後，使用 [!DNL Commerce] 處理訂單的訂單選項。</td>
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
<td>與從接收的退貨請求相關聯的退貨授權號 [!DNL Walmart Marketplace]. 這個數字是由Walmart Marketplace生成的 [!UICONTROL Returns] 當返回進程啟動時。</td>
</tr>
<tr>
<td>[!DNL Commerce] 訂單編號</td>
<td>此 [!DNL Commerce] 與來自Walmart Marketplace的退貨請求中包含的物料相關的訂單號。 通過選擇訂單編號查看訂單詳細資訊。</td>
</tr>
<tr>
<td>已請求</td>
<td>在 [!DNL Walmart Marketplace]
轉換為當地時間。</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>返回必須退回的日期 [!DNL Walmart Marketplace] [需求](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f)轉換為當地時間。</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>列出退貨中所列每個項目的SKU和數量。</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>退回項目要退回的總值。</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>指示 [!DNL Commerce] 返回工作流程 — <i>已接收</i>, <i>已退回</i>，或 <i>錯誤</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>對於已接收和已退回的退貨條目，狀態詳細資訊提供了訪問貸項通知單以進行退款處理的連結。 若 [!DNL Channel Manager] Adobe Commerce和 [!DNL Walmart marketplace]，此欄位會提供錯誤說明。</td>
</tr>
</table>

## 返回狀態

[!UICONTROL Return Status] 提供 [!DNL Walmart Marketplace] 傳回從Adobe Commerce或Magento Open Source管理的請求。

當 [!DNL Channel Manager] 接收來自 [!DNL Walmart Marketplace] 或 [!DNL Commerce] 系統會建立貸項通知單以處理退回項目的退款。

傳回的狀態如下：

* **[!UICONTROL Received]** — 這是從 [!DNL Walmart Marketplace] 儲存。 商家可以通過選擇 **[!UICONTROL Create credit memo]** 在 [!UICONTROL Status details].

* **[!UICONTROL Refunded]** — 指示已建立貸項通知單以為退回的物料發放退款。 商戶可以通過選擇 **[!UICONTROL View credit memo]** 在 [!UICONTROL Status details].

* **[!UICONTROL Error]** — 傳回有錯誤的請求。 當來自沃爾瑪的返回請求缺少或資料不正確時，可能會發生錯誤。 或者，如果 [!DNL Channel Manager] 無法將退款更新通知發送到沃爾瑪。

## 傳回案例

以下案例說明如何針對不同類型的回傳請求，從 [!DNL Channel Manager].

* **完整回訪** — 如果Walmart Marketplace退貨請求是訂單中所有物料的退貨請求，請更新貸項通知單數量以退還所有物料。

* **部分返回** — 如果Walmart Marketplace僅對某些訂單項進行退貨請求，則僅對要退貨的項更新貸項通知單數量。

* **已通過Walmart Marketplace退回** — 在某些情況下， [!DNL Walmart Marketplace] 在「管道管理員」中處理傳回前。 例如，如果在沃爾瑪要求的48小時退款處理窗口內未退回商務訂單，則沃爾瑪會自動退款訂單。 發生此情況時，管道管理員仍會將回訪請求同步至Adobe Commerce，以便您處理回訪並核發貸項通知單。 此工作流程可確保 [!DNL Commerce] 與沃爾瑪市場中的訂單資訊匹配。

>[!NOTE]
>
> 退款更新最多需要5分鐘，才能同步至 [!DNL Walmart Marketplace]. 您可以從 [!DNL Channel Manager] [!UICONTROL Returns] 控制面板。

## 處理退款請求

1. 開啟 [!UICONTROL Returns] 銷售管道商店的控制面板。

   * 在管理員中，選取 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * 選取銷售管道商店的眼睛圖示，以開啟商店檢視。

   * 您可以選取 **[!UICONTROL Returns]** 標籤。

      您也可以從 [!UICONTROL Orders] 頁面。 尋找 [!UICONTROL Shipped] 具有退貨請求的訂單。 然後，選取 `Return requested` 連結 [!UICONTROL Status Details] 欄來檢視及處理請求。

1. 從「傳回」表格中，尋找含有 *[!UICONTROL Received]* 狀態。

1. 從「項目」列中，複查訂單項目清單和要退款的數量。

1. 通過發出貸項通知單處理退款。

   * 從 [!UICONTROL Status Details] 欄，選擇 **[!UICONTROL Create credit memo]** 要開啟「訂單詳細資訊」頁，請在 [!DNL Commerce].

      如果尚未開具訂單發票，則「訂單詳細資訊」頁將顯示一條錯誤消息，提示您建立訂單。 選擇 **[!UICONTROL Create invoice]**. 然後， [建立並保存發票](https://docs.magento.com/user-guide/sales/invoices.html).

   * 在訂單詳細資訊頁面上，選擇 **[!UICONTROL Credit Memo]**.

   * 在 [!UICONTROL Items to Refund] 區段 [!UICONTROL Credit Memo]，請更新 **[!UICONTROL Qty to refund]** 和 **[!UICONTROL Return to Stock]** 返回請求中包含的項的資訊。

      請確定只傳回傳回請求中列出的項目。

   * 要添加註釋，請在 **[!UICONTROL Credit Memo Comments]**

   * 選擇 **[!UICONTROL Refund Offline]**.

完成退款後， [!DNL Channel Manager] 更新 [!UICONTROL Returns] 控制面板 [!UICONTROL Refunded] 並將更新同步至沃爾瑪，以更新市場中的退貨狀態。


## 查看退貨的退款資訊

您可以透過 [!UICONTROL Returns] 控制面板。

1. 開啟銷售渠道商店的「退貨」控制面板。

   * 在管理員中，選取 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * 選取銷售管道商店的眼睛圖示，以開啟商店檢視。

   * 選擇 **[!UICONTROL Returns]**.

1. 通過選擇 **[!UICONTROL Refunded]** 狀態卡。

1. 通過選擇 **[!UICONTROL View credit memo]**.

   ![要退款的退回項的貸項通知單 [!DNL Walmart Marketplace] 訂購](assets/refund-credit-memo-for-marketplace-order.png)

>[!NOTE]
>
>訂單退款後， [!UICONTROL Orders] 控制面板未顯示傳回資訊。 若要檢視傳回資訊，請使用 [!DNL Channel Manager] 傳回控制面板。 「訂單詳細資訊」頁還提供更詳細的退貨和退款資訊。

## 修正傳回錯誤

從接收返回資訊時，可能會發生錯誤 [!DNL Walmart Marketplace]，或 [!DNL Channel Manager] 同步狀態更新 [!DNL Commerce] to [!DNL Walmart Marketplace].

如果返回更新的同步操作失敗，則 [!DNL Channel Manager] 傳回控制面板顯示 *[!UICONTROL Error]* 返回條目的狀態。 為確保退貨和退款資訊準確反映在Walmart Marketplace帳戶中，請手動更新您 [!DNL Walmart Marketplace] 儲存。

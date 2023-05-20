---
title: 退貨和退款訂單
description: 關於為從以下地址收到的退回請求發放全額或部分退款的說明 [!DNL Walmart Marketplace] 從 [!DNL Channel Manager] Adobe Commerce和Magento Open Source。
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# 退貨和退款訂單

當採購員請求退回通過 [!DNL Walmart Marketplace],Walmart會建立退貨請求。 [!DNL Channel Manager] 監視這些請求的市場渠道，並自動將返回請求資訊同步到Channel Manager。

在Commerce方面，返回請求將啟動以下工作流：

1. Channel Manager建立具有接收狀態的相應返回請求並添加返回ID號([!UICONTROL RMA #]) [!UICONTROL Returns] 控制項欄。 在 [!DNL Orders] 控制板，與返回更新關聯的訂單的狀態詳細資訊，以包括 [!UICONTROL Return requested] 連結以查看和處理返回。

1. 商家通過在以下項後建立貸項通知單來處理與退貨關聯的退款 [Adobe Commerce退款工作流](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow)。 所有退款都使用離線方法處理。

1. [!DNL Channel Manager] 向沃爾瑪市場發送退款更新，以便更新退貨狀態，以反映從Adobe Commerce獲得的已完成退款。

在店面管理員中，您可以通過開啟銷售渠道商店並選擇 **[!UICONTROL Returns]**。

![Channel Manager返回儀表板以處理從接收的退貨請求的退款 [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png)

>[!NOTE]
>
>您只能處理已發運訂單的退款。 在 [!DNL Channel Manager]，訂單狀態必須為 [!UICONTROL Shipped]。 在 [!DNL Walmart Marketplace] 賣家帳戶，訂單必須 [!UICONTROL Delivered]。

## 返回控制項和列說明

下表介紹了可用於 [!DNL Channel Manager] 返回。

**控制項[!UICONTROL Returns]**

<table>
<tr>
<td><strong>控制項</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>通過選擇 [!UICONTROL Return Status] 卡片。</td>
</tr>
<tr>
<td>狀態詳細資訊</td>
<td>對於返回條目 [!UICONTROL Received] 或 [!UICONTROL Refunded] 狀態，您可以通過在「狀態詳細資訊」列中選擇連結文本來建立或查看退款的貸項通知單。</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>要查看訂單詳細資訊，請選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 的子菜單。</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>要修改渠道配置，請選擇渠道Walmart連接憑據、映射屬性或發運標識符，設定選擇 [!DNL Commerce] 訂單編號 [!UICONTROL Order] 的子菜單。 然後，使用 [!DNL Commerce] 訂單選項以處理訂單。</td>
</tr>
</table>

**列說明**

<table>
<tr>
<td><strong>欄位</strong></td>
<td><strong>說明</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>與從接收的退貨請求關聯的退貨授權號 [!DNL Walmart Marketplace]。 此數字由Walmart Marketplace生成 [!UICONTROL Returns] 啟動返回進程時。</td>
</tr>
<tr>
<td>[!DNL Commerce] 訂單號</td>
<td>的 [!DNL Commerce] 與來自沃爾瑪市場的退貨請求中包含的物料關聯的訂單號。 通過選擇訂單編號查看訂單詳細資訊。</td>
</tr>
<tr>
<td>請求</td>
<td>在 [!DNL Walmart Marketplace]
轉換為本地時間。</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>返還必須返還的日期 [!DNL Walmart Marketplace] [requirements](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f)轉換為本地時間。</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>列出退貨中列出的每件產品的SKU和數量。</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>退回項目應退還的總值。</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>指示中的當前返回狀態 [!DNL Commerce] 返回工作流 — <i>已接收</i>。 <i>已退款</i>或 <i>錯誤</i>。</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>對於已接收和已退回的退貨條目，狀態詳細資訊提供了訪問貸項通知單以進行退款處理的連結。 如果在 [!DNL Channel Manager] Adobe Commerce與DNA的同步過程 [!DNL Walmart marketplace]，此欄位提供錯誤說明。</td>
</tr>
</table>

## 返回狀態

[!UICONTROL Return Status] 提供有關 [!DNL Walmart Marketplace] 返回從Adobe Commerce或Magento Open Source管理的請求。

返回狀態更新發生於 [!DNL Channel Manager] 從 [!DNL Walmart Marketplace] 或 [!DNL Commerce] 建立貸項通知單以處理退回物料的退款。

退貨可以具有以下狀態：

* **[!UICONTROL Received]** — 這是從 [!DNL Walmart Marketplace] 商店。 商戶可以通過選擇 **[!UICONTROL Create credit memo]** 的 [!UICONTROL Status details]。

* **[!UICONTROL Refunded]** — 表示已建立貸項通知單以為返回的物料發放退款。 商戶可以通過選擇 **[!UICONTROL View credit memo]** 的 [!UICONTROL Status details]。

* **[!UICONTROL Error]** — 返回有錯誤的請求。 當來自沃爾瑪的返回請求丟失或資料不正確時，可能會發生錯誤。 或者，如果 [!DNL Channel Manager] 無法向沃爾瑪發送退款更新通知。

## 返回方案

以下方案說明如何為來自的不同類型的退貨請求發放退款 [!DNL Channel Manager]。

* **完全返回** — 如果Walmart Marketplace的退貨請求針對訂單中的所有物料，請更新貸項通知單數量以退還所有物料。

* **部分返回** — 如果Walmart Marketplace僅對某些訂單物料發出退貨請求，則僅對要退還的物料更新貸項通知單數量。

* **已通過沃爾瑪市場退還退貨** — 在某些情況下，將在 [!DNL Walmart Marketplace] 在Channel Manager中處理返回之前。 例如，如果在沃爾瑪要求的48小時退款處理窗口內未退回商務訂單，沃爾瑪將自動退還訂單。 在發生這種情況時，Channel Manager仍將將退貨請求同步到Adobe Commerce，以便您可以處理退貨並發放貸項通知單。 此工作流確保中的訂單詳細資訊 [!DNL Commerce] 與沃爾瑪市場的訂單資訊相匹配。

>[!NOTE]
>
> 退款更新要同步到最多需要5分鐘 [!DNL Walmart Marketplace]。 您可以從 [!DNL Channel Manager] [!UICONTROL Returns] 控制項欄。

## 處理退款請求

1. 開啟 [!UICONTROL Returns] 銷售渠道商店的儀表板。

   * 在管理員中，選擇 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**。

   * 通過為銷售渠道商店選擇眼睛表徵圖開啟商店視圖。

   * 通過選擇 **[!UICONTROL Returns]** 頁籤。

      您還可以從 [!UICONTROL Orders] 的子菜單。 查找 [!UICONTROL Shipped] 有退貨請求的訂單。 然後，選擇 `Return requested` 連結 [!UICONTROL Status Details] 的子菜單。

1. 從「返回」(Returns)表中，查找帶有 *[!UICONTROL Received]* 狀態。

1. 在「物料」列中，複查要退款的訂單物料和數量清單。

1. 通過發出貸項通知單處理退款。

   * 從 [!UICONTROL Status Details] 列，選擇 **[!UICONTROL Create credit memo]** 開啟「訂單詳細資訊」頁 [!DNL Commerce]。

      如果訂單尚未開票，則「訂單詳細資訊」頁將顯示一條錯誤消息，提示您建立一個。 選擇 **[!UICONTROL Create invoice]**。 然後， [建立並保存發票](https://docs.magento.com/user-guide/sales/invoices.html)。

   * 在「訂單詳細資訊」頁上，選擇 **[!UICONTROL Credit Memo]**。

   * 在 [!UICONTROL Items to Refund] 的下界 [!UICONTROL Credit Memo]，更新 **[!UICONTROL Qty to refund]** 和 **[!UICONTROL Return to Stock]** 返回請求中包含的項的資訊。

      確保僅返回返回返回請求中列出的項。

   * 要添加註釋，請在 **[!UICONTROL Credit Memo Comments]**

   * 選擇 **[!UICONTROL Refund Offline]**。

退款完成後， [!DNL Channel Manager] 更新 [!UICONTROL Returns] 儀表板 [!UICONTROL Refunded] 並將更新同步到沃爾瑪以更新市場中的退貨狀態。


## 查看退貨的退款資訊

您可以從中查看有關退貨請求和退款處理的資訊 [!UICONTROL Returns] 控制項欄。

1. 開啟銷售渠道商店的退貨面板。

   * 在管理員中，選擇 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**。

   * 通過為銷售渠道商店選擇眼睛表徵圖開啟商店視圖。

   * 選擇 **[!UICONTROL Returns]**。

1. 通過選擇 **[!UICONTROL Refunded]** 狀態卡。

1. 通過選擇 **[!UICONTROL View credit memo]**。

   ![要退款的退回物料的貸項通知單 [!DNL Walmart Marketplace] 訂單](assets/refund-credit-memo-for-marketplace-order.png)

>[!NOTE]
>
>訂單退還後， [!UICONTROL Orders] 儀表板不顯示返回資訊。 要查看退貨資訊，請使用 [!DNL Channel Manager] 返回儀表板。 更詳細的退貨和退款資訊也可從訂單詳細資訊頁面獲得。

## 修復返回錯誤

當從接收返回資訊時，可能會發生錯誤 [!DNL Walmart Marketplace]或 [!DNL Channel Manager] 同步狀態更新 [!DNL Commerce] 至 [!DNL Walmart Marketplace]。

如果返回更新的同步操作失敗， [!DNL Channel Manager] 返回儀表板顯示 *[!UICONTROL Error]* 返回條目的狀態。 為確保退貨和退款資訊準確反映在Walmart Marketplace帳戶中，請手動更新您的 [!DNL Walmart Marketplace] 商店。

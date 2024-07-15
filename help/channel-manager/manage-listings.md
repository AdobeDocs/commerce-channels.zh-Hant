---
title: 管理清單
description: '使用Adobe Commerce和Magento Open Source的管道管理員管理 [!DNL Commerce] 商店的銷售管道清單。'
feature: Sales Channels, Merchandising, Products
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# 管理清單

從管道管理員UI管理[!DNL Walmart Marketplace]銷售管道的產品清單。

個別清單的狀態表示產品在[!DNL Channel Manager]工作流程中的位置，因此您可以決定後續步驟並解決任何錯誤。

已連線銷售管道的![清單頁面](assets/listings-dashboard-view.png){width="500" zoomable="yes"}

您可以從「清單」檢視完成下列作業。

* 檢視目前清單
* 排序及篩選清單
* 新增產品
* 比對產品
* 追蹤清單狀態
* 檢閱錯誤狀態清單的錯誤說明

## 檢視產品清單

1. 從管理員移至&#x200B;[!UICONTROL **行銷** > **管道管理員**]。

1. 從「商店」清單中，選取商店專案列中的眼睛圖示，以開啟商店檢視。

1. 選取&#x200B;[!UICONTROL **清單**]。

1. 選取&#x200B;*清單*&#x200B;表格中的任何欄標題，以排序&#x200B;*清單*&#x200B;檢視。

1. 選取其中一個狀態計數卡片，以篩選&#x200B;*清單*&#x200B;檢視。

1. 選取&#x200B;**重新整理產品**，以重設排序順序並移除篩選器。

## 新增[!DNL Commerce]產品至管道管理員

完成下列作業，建立[!DNL Walmart Marketplace]管道的產品分類：

* [將產品從您的 [!DNL Commerce] 產品目錄新增至 [!DNL Channel Manager]](add-products-to-channel-store.md)

* [對應目錄屬性](map-catalog-attributes.md#configure-product-attribute-settings)

## 符合[!DNL Walmart]上的產品

您可以使用產品比對或手動上傳新產品的產品清單，在[!DNL Walmart Marketplace]上建立產品優惠方案。

* **[符合Walmart上的產品](connect-listings-to-marketplace.md)** — 更新銷售相同產品的現有清單，將產品清單從您的頻道連結到[!DNL Walmart Marketplace]。 符合條件是由您管道的[屬性對應組態](map-catalog-attributes.md)所決定。

* **[手動上傳新清單](connect-listings-to-marketplace.md#upload-new-product-listings)** — 對於不符合[!DNL Walmart Marketplace]上現有清單的產品，請使用[!DNL Walmart]產品類別Excel範本來大量上傳產品清單。

## 列出控制項與欄位說明

下清單格說明[!UICONTROL Listings]可用的控制項與資料行。

[!UICONTROL Listings]**的**&#x200B;控制項

| **控制項** | **描述** |
|----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | 開啟[!UICONTROL Admin Product Catalog]頁面，以選取要新增至您的[!DNL Walmart Marketplace]分類的產品，或更新產品屬性以符合Walmart Marketplace的清單要求。 |
| [!UICONTROL Match products on Walmart] | 選取一或多個處於[!UICONTROL Draft]狀態的產品後，選取[!UICONTROL Match products on Walmart]以檢查可新增至現有[!DNL Walmart Marketplace]清單的產品優惠方案。 |
| [!UICONTROL Refresh products] | 以最新的清單和狀態更新顯示。 此控制項也會將清單檢視重設為預設的排序順序，並移除任何篩選器。 |
| [!UICONTROL Filter by *狀態*] | 選取「清單」表格上方的其中一個狀態卡，僅顯示具有特定狀態的清單。 選取&#x200B;**[!UICONTROL Refresh products]**&#x200B;以移除篩選器。 |
| [!UICONTROL Sort products] | 選取任何欄標題，變更清單的排序順序。 |


**資料行說明**

| **欄位** | **描述** |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | 來自[!DNL Commerce]商店目錄的產品名稱。 |
| [!UICONTROL SKU (Unique ID)] | 指派給[!DNL Commerce]目錄中產品的SKU。 |
| [!UICONTROL  Quantity] | Adobe Commerce或Magento Open Source中可用的庫存量。 |
| [!UICONTROL Price] | [!DNL Commerce]商店目錄中的產品價格。 目錄價格更新會同步至Channel Manager，然後傳送至[!DNL Walmart Marketplace]，讓列出的專案顯示目前的價格。 |
| [!UICONTROL Status] | 指示[!DNL Commerce]訂單工作流程中的目前訂單狀態。 當您成功將產品新增到[!DNL Channel Manager]以及當您符合市場上的產品時，狀態會更新。 如果作業失敗，清單會顯示錯誤狀態。 修正錯誤後，[!DNL Channel Manager]會重試操作並更新狀態。 |
| [!UICONTROL Error Description] | 提供狀態為`[!DNL Error]`之產品的其他錯誤資訊。 |

### 關於清單狀態

在清單工作區中，「狀態」標籤會顯示產品在[!DNL Channel Manager]工作流程中的位置，讓您可以決定後續步驟並解決錯誤。 清單可以有下列狀態標籤：

* **[!UICONTROL Draft]** — 識別尚未[提交至 [!DNL Walmart] 以符合](connect-listings-to-marketplace.md#match-products)的產品。

* **[!UICONTROL Processing]** — 識別在[!DNL Walmart Marketplace]上提交比對的產品。 產品會維持在&#x200B;*處理*&#x200B;狀態，直到[!DNL Walmart]傳回HTTP狀態訊息，指出比對是否成功，或是否有錯誤為止。 最多可能需要30分鐘，才能在[!DNL Walmart Marketplace]上完成比對作業。

* **[!UICONTROL Match]** — 識別[!DNL Walmart]上已成功比對的產品。

  當產品屬性值（例如UPC代碼）與現有[!DNL Walmart Marketplace]清單中的UPC值相符時，就會有相符專案。 當產品符合時，Commerce產品選件會新增至現有清單。

  檢查[[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items)儀表板以檢閱更新的產品清單，並驗證產品詳細資料、價格和存貨數量。

* **[!UICONTROL Match - Match in Stage]** — 識別[!DNL Walmart]上相符的產品，直到[!DNL Walmart Marketplace]存放區上線後才能連線。 具有此狀態的產品會在[!DNL Walmart Marketplace]存放區上線時自動連線。

* **[!UICONTROL Error]** — 識別不符合現有[!DNL Walmart Marketplace]清單的產品。

* **[!UICONTROL Error description]** — 提供有關清單錯誤的詳細資訊。

  解決錯誤後，請重新提交產品以進行比對。 請參閱[產品比對錯誤疑難排解](connect-listings-to-marketplace.md#troubleshoot-product-match-errors)。

---
title: 管理清單
description: '''管理 [!DNL Commerce] 與Channel Manager for Adobe Commerce和Magento Open Source一起儲存。'
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 0%

---

# 管理清單

管理 [!DNL Walmart Marketplace] 銷售管道。

個別清單的狀態會指出產品在 [!DNL Channel Manager] 工作流程，以便您決定後續步驟並解決任何錯誤。

![已連接銷售渠道的清單頁](assets/listings-dashboard-view.png)

您可以從清單檢視中完成下列工作。

* 查看當前清單
* 排序和篩選清單
* 新增產品
* 匹配產品
* 跟蹤清單狀態
* 查看狀態為錯誤的清單的錯誤說明

## 檢視產品清單

1. 從管理員，前往 [!UICONTROL **行銷** > **管道管理員**].

1. 從「商店」清單中，選擇商店條目行中的眼睛表徵圖以開啟商店視圖。

1. 選擇 [!UICONTROL **清單**].

1. 排序 *清單* 檢視，方法是選取 *清單* 表格。

1. 篩選 *清單* 選取其中一個狀態計數卡即可檢視。

1. 重設排序順序並移除篩選器，方法是選取 **重新整理產品**.

## 新增 [!DNL Commerce] 產品至Channel Manager

為 [!DNL Walmart Marketplace] 通道，方法如下：

* [從 [!DNL Commerce] 產品目錄 [!DNL Channel Manager]](add-products-to-channel-store.md)

* [映射目錄屬性](map-catalog-attributes.md#configure-product-attribute-settings)

## 在上匹配產品 [!DNL Walmart]

您可以在 [!DNL Walmart Marketplace] 使用產品比對，或手動上傳新產品的產品清單。

* **[沃爾瑪配貨](connect-listings-to-marketplace.md)** — 將產品清單從您的渠道連接到 [!DNL Walmart Marketplace] 更新銷售相同產品的現有清單。 符合條件由 [屬性映射配置](map-catalog-attributes.md) 為您的頻道。

* **[手動上傳新清單](connect-listings-to-marketplace.md#upload-new-product-listings)** — 若產品與上的現有清單不符 [!DNL Walmart Marketplace]，請使用 [!DNL Walmart] 產品類別Excel範本，以大量上傳產品清單。

## 列出控制項和列說明

下表說明可用於 [!UICONTROL Listings].

**的控制[!UICONTROL Listings]**

| **控制** | **說明** |
|----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | 開啟 [!UICONTROL Admin Product Catalog] 頁面，以選取要新增至您的產品 [!DNL Walmart Marketplace] 分類，或更新產品屬性以符合Walmart Marketplace的清單要求。 |
| [!UICONTROL Match products on Walmart] | 選取一或多個產品後， [!UICONTROL Draft] 狀態，選擇 [!UICONTROL Match products on Walmart] 來檢查可新增至現有 [!DNL Walmart Marketplace] 清單。 |
| [!UICONTROL Refresh products] | 使用最新清單和狀態更新顯示。 此控制項也會將清單檢視重設為預設排序順序，並移除任何篩選器。 |
| [!UICONTROL Filter by *狀態*] | 通過選擇清單表上方的狀態卡之一，僅顯示具有特定狀態的清單。 選取 **[!UICONTROL Refresh products]**. |
| [!UICONTROL Sort products] | 通過選擇任何列標題來更改清單的排序順序。 |


**欄說明**

| **欄位** | **說明** |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | 來自的產品名稱 [!DNL Commerce] 儲存目錄。 |
| [!UICONTROL SKU (Unique ID)] | 指派給 [!DNL Commerce] 目錄。 |
| [!UICONTROL  Quantity] | Adobe Commerce或Magento Open Source中可用的庫存量。 |
| [!UICONTROL Price] | 來自 [!DNL Commerce] 儲存目錄。 目錄價格更新會同步至管道管理員，然後傳送至 [!DNL Walmart Marketplace]  讓列出的項目顯示目前的價格。 |
| [!UICONTROL Status] | 指示 [!DNL Commerce] 訂購工作流程。 成功將產品新增至時，狀態會更新 [!DNL Channel Manager] 當你在市場上匹配產品時。 如果操作失敗，清單會顯示錯誤狀態。 修正錯誤後， [!DNL Channel Manager] 重試操作並更新狀態。 |
| [!UICONTROL Error Description] | 提供產品的其他錯誤資訊， `[!DNL Error]` 狀態。 |

### 關於清單狀態

在清單工作區中，狀態標籤會顯示產品在 [!DNL Channel Manager] 工作流程，以便您決定後續步驟並解決錯誤。 清單可以有下列狀態標籤：

* **[!UICONTROL Draft]** — 識別尚未 [已提交 [!DNL Walmart] 匹配](connect-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]** — 識別提交以進行比對的產品 [!DNL Walmart Marketplace]. 產品仍保留在 *處理* 狀態直到 [!DNL Walmart] 傳回HTTP狀態訊息，指出相符是否成功，或是否發生錯誤。 匹配操作最多需要30分鐘才能完成 [!DNL Walmart Marketplace].

* **[!UICONTROL Match]** — 標識成功匹配的產品 [!DNL Walmart].

   當產品屬性值（例如UPC代碼）與現有產品中的UPC值匹配時，就會發生匹配 [!DNL Walmart Marketplace] 清單。 產品符合時，商務產品選件會新增至現有清單。

   檢查 [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) 控制面板，以檢查更新的產品清單，並驗證產品詳細資訊、價格和存貨數量。

* **[!UICONTROL Match - Match in Stage]** — 標識在上匹配的產品 [!DNL Walmart] 直到 [!DNL Walmart Marketplace] 商店已上線。 具有此狀態的產品會在 [!DNL Walmart Marketplace] 商店上線。

* **[!UICONTROL Error]** — 標識與現有產品不匹配的產品 [!DNL Walmart Marketplace] 清單。

* **[!UICONTROL Error description]** — 提供有關清單錯誤的詳細資訊。

   解決錯誤後，重新提交產品以進行匹配。 請參閱 [疑難排解產品比對錯誤](connect-listings-to-marketplace.md#troubleshoot-product-match-errors).

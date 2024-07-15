---
title: 不完整的Amazon清單
description: Amazon sales channel提供[!UICONTROL Incomplete]標籤，協助您識別並符合未完成Amazon清單的資格要求。
feature: Sales Channels, Products
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# 不完整的Amazon清單

_[!UICONTROL Incomplete]_索引標籤會列出符合您Amazon適用性要求的[!DNL Commerce]目錄產品（定義於您的[清單規則](./listing-rules.md)），但遺失Amazon所需的資訊(例如Amazon ASIN或定義的產品條件)。

清單未完成的可能原因有四種，每種原因都由其狀態來識別。

| 狀態 | 原因 | 動作 |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 缺少條件 | Amazon接受各種條件的清單（例如&#x200B;_New_、_Refluished_、_Used： Like New_）清單需要已定義的條件。 | 更新必要資訊，並手動[將條件](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition)指派給清單。 |
| 無法指派至Amazon清單 | 此清單自動比對至您的目錄失敗。 如果找不到相符專案，AmazonSales Channel將無法管理該清單 | 更新必要資訊，並手動[將ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing)指派給目錄產品，以符合清單。 |
| 找到多個相符專案 | 此清單自動比對至您的目錄失敗。 如果找到多個可能的相符專案，您必須為您的產品選取正確的相符專案。 | 更新必要資訊，並手動[選擇產品及清單的產品相符專案](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found)。 |
| 具有變體 | 如果您的產品有變體，例如可用不同大小或顏色的T恤，您必須在目錄中選擇要正確指派並符合清單的變體 | 更新必要資訊，並手動[選擇正確的變體](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants)，以指派並符合此清單。 |

>[!NOTE]
>當不完整的清單正確符合您的目錄產品時，清單會從&#x200B;_[!UICONTROL Incomplete]_索引標籤移動，並根據您的[_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md)設定發佈到Amazon。

_[!UICONTROL Incomplete]_標籤上的可用動作包括：

在&#x200B;_[!UICONTROL Actions]_下：

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**：選擇以啟動自動處理程式，將您的Amazon清單資料與您的[!DNL Commerce]目錄比對。 如果產品未自動比對，請重新造訪清單授權中的[_[!UICONTROL Catalog Search]_](./catalog-search.md)選項。 如果清單在更新&#x200B;_[!UICONTROL Catalog Search]_選項後未自動相符，您可以在[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found)動作中手動比對產品。

在&#x200B;_[!UICONTROL Action]_欄的&#x200B;**[!UICONTROL Select]**下：

- **[!UICONTROL Update Required Info]**：當清單未自動符合您的目錄時選擇。 您可以手動[比對目錄產品與清單](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found)、手動[將ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing)指派給目錄相符專案，或[指派清單的遺漏條件](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition)。

- **[!UICONTROL View Details]**：選擇檢視清單詳細資料，包括[清單活動記錄](./product-listing-details.md#listing-activity-log)、[Buy Box競爭者定價](./product-listing-details.md#buy-box-competitor-pricing)和[最低競爭者定價](./product-listing-details.md#lowest-competitor-pricing)。 此動作僅供檢視。 清單詳細資料不可變更。 檢視[檢視詳細資料](./product-listing-details.md)。

>[!NOTE]
>
>如果您有處理中的清單，清單的數量會顯示在標籤上方的訊息中。

![不完整的Amazon清單](assets/amazon-incomplete-listings.png){width="600" zoomable="yes"}

Amazon sales channel首頁共用一些常見的[工作區控制項](./workspace-controls.md)，可讓您自訂顯示的資料。

| 欄 | 說明 |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Amazon指派給產品的SKU （庫存單位），用於識別產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 識別專案的10個字母和/或數字的唯一區塊。<br><br>ASIN代表[!DNL Amazon Standard Identification Number]。 ASIN是識別專案的10個字母和/或數字的唯一區塊。 對於書籍，ASIN與ISBN編號相同，但對於所有其他產品，當專案上傳到它們的目錄時會建立新的ASIN。 您可以在Amazon的產品詳細資料頁面上找到專案ASIN，以及與此專案相關的其他詳細資料。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Condition] | 產品的[狀況](./product-listing-condition.md)。 |
| [!UICONTROL Landed Price] | 產品的上市價格加上其送貨價格。 |
| [!UICONTROL Amazon Quantity] | 產品在Amazon上主動列出時的可用數量。 |
| [!UICONTROL Status] | 清單的狀態，由Amazon定義。 請參閱上方的「狀態」表格。 |
| [!UICONTROL Action] | 可套用至特定清單的可用動作清單。 若要套用動作，請按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Select]**並選取選項：<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

---
title: 未完成的清單
description: Amazon銷售管道提供 [!UICONTROL Incomplete] 標籤，幫助您識別並符合不完整Amazon清單的資格要求。
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 未完成的清單

此 _[!UICONTROL Incomplete]_索引標籤會列出 [!DNL Commerce] 符合Amazon資格要求的目錄產品(定義於 [清單規則](./listing-rules.md))，但缺少Amazon所需的資訊(例如Amazon ASIN或已定義的產品條件)。

清單不完整有四個可能的原因，每個原因都以其狀態識別。

| 狀態 | 原因 | 動作 |
|--- |--- |--- |
| 缺少條件 | Amazon接受不同條件的清單(例如 _新增_, _翻新_, _已使用：贊新_)清單需要定義的條件。 | 更新所需資訊並手動 [指派條件](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) 列名。 |
| 無法指派至Amazon清單 | 此清單與目錄的自動匹配失敗。 如果找不到相符項目，則無法由AmazonSales Channel管理清單 | 更新所需資訊並手動 [指派ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) 到目錄產品以符合清單。 |
| 找到多個匹配項 | 此清單與目錄的自動匹配失敗。 如果找到多個可能的匹配項，則必須為產品選擇正確的匹配項。 | 更新所需資訊並手動 [選擇產品匹配](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) 和清單。 |
| 有變體 | 如果您的產品有變體，例如T恤衫，其大小或顏色不同，您必須在目錄中選擇變體，才能正確指派並符合清單 | 更新所需資訊並手動 [選擇正確的變體](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) 來指派及比對此清單。 |

>[!NOTE]
>當未完成的清單與目錄產品匹配時，清單將從 _[!UICONTROL Incomplete]_標籤，並根據 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 設定。

上的可用動作 _[!UICONTROL Incomplete]_索引標籤包括：

在 _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**:選擇啟動自動流程，將Amazon清單資料與 [!DNL Commerce] 目錄。 如果產品不自動相符，請重新造訪 [_[!UICONTROL Catalog Search]_](./catalog-search.md) 選項。 如果清單在更新 _[!UICONTROL Catalog Search]_選項，您可以在 [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) 動作。

在 **[!UICONTROL Select]** 在 _[!UICONTROL Action]_欄：

- **[!UICONTROL Update Required Info]**:選擇清單何時不自動與目錄相符。 您可以手動 [將目錄產品與清單匹配](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found)，手動 [指派ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) 目錄比對，或 [指派遺漏的條件](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) 中。

- **[!UICONTROL View Details]**：選擇檢視清單詳細資訊，包括 [列出活動日誌](./product-listing-details.md#listing-activity-log), [Buy Box競爭者定價](./product-listing-details.md#buy-box-competitor-pricing)，和 [最低競爭者定價](./product-listing-details.md#lowest-competitor-pricing). 此動作僅供檢視。 清單詳細資訊中不能進行任何更改。 請參閱 [檢視詳細資料](./product-listing-details.md).

>[!NOTE]
>
>如果正在處理清單，則清單數將顯示在頁簽上方的消息中。

![不完整的Amazon清單](assets/amazon-incomplete-listings.png)

Amazon銷售管道首頁有一些共同之處 [工作區控制項](./workspace-controls.md) 可讓您自訂顯示的資料。

| 欄 | 說明 |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | 由Amazon指派給產品的SKU（庫存保管單位），用以識別產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 10個字母和/或數字的唯一區塊，用於識別項目。<br><br>ASIN代表 [!DNL Amazon Standard Identification Number]. ASIN是10個字母和/或數字的唯一塊，用於標識項目。 對於帳簿，ASIN與ISBN號相同，但是對於所有其他產品，當將項目上載到其目錄時將建立新的ASIN。 您可以在Amazon的產品詳細資訊頁面上找到項目ASIN，以及與項目相關的詳細資訊。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Condition] | 此 [條件](./product-listing-condition.md) 產品。 |
| [!UICONTROL Landed Price] | 產品的掛牌價加其運價。 |
| [!UICONTROL Amazon Quantity] | 產品主動列於Amazon時的可用數量。 |
| [!UICONTROL Status] | 清單的狀態，由Amazon定義。 請參閱上方的「狀態」表格。 |
| [!UICONTROL Action] | 可套用至特定清單的可用動作清單。 若要套用動作，請按一下 **[!UICONTROL Select]** 在 _[!UICONTROL Action]_欄，然後選取選項：<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

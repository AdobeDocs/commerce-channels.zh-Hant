---
title: 未完成清單
description: Amazon銷售渠道 [!UICONTROL Incomplete] 頁籤，幫助您確定並滿足未完成的Amazon清單的資格要求。
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 未完成清單

的 _[!UICONTROL Incomplete]_清單 [!DNL Commerce] 滿足您的Amazon資格要求的目錄產品(在您的 [上市規則](./listing-rules.md))，但缺少Amazon所需的資訊(例如AmazonASIN或已定義的產品條件)。

有四種可能的原因導致清單不完整，每種原因都由清單的狀態確定。

| 狀態 | 原因 | 操作 |
|--- |--- |--- |
| 缺少條件 | Amazon接受各種條件(如 _新建_。 _翻新_。 _已用：類似新_)清單需要定義的條件。 | 更新所需資訊並手動 [指定條件](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) 列名。 |
| 無法分配到Amazon清單 | 此清單與目錄的自動匹配失敗。 如果找不到匹配項，則無法由AmazonSales Channel管理清單 | 更新所需資訊並手動 [分配ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) 到目錄產品以匹配清單。 |
| 找到多個匹配項 | 此清單與目錄的自動匹配失敗。 如果找到多個可能的匹配項，則必須為產品選擇正確的匹配項。 | 更新所需資訊並手動 [選擇產品匹配項](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) 產品和清單。 |
| 具有變型 | 如果產品有變型，如T恤衫，該T恤衫的大小或顏色不同，則必須選擇目錄中的變型才能正確分配並與清單匹配 | 更新所需資訊並手動 [選擇正確的變型](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) 指定並匹配此清單。 |

>[!NOTE]
>當未完成清單與目錄產品正確匹配時，清單將從 _[!UICONTROL Incomplete]_頁籤，並根據您的 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 的子菜單。

上的可用操作 _[!UICONTROL Incomplete]_頁籤包括：

下 _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**:選擇啟動自動流程，將您的Amazon清單資料與您的 [!DNL Commerce] 目錄。 如果產品不自動匹配，請重新訪問 [_[!UICONTROL Catalog Search]_](./catalog-search.md) 選項。 如果清單在更新後不自動匹配 _[!UICONTROL Catalog Search]_選項，您可以在 [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) 操作。

下 **[!UICONTROL Select]** 的 _[!UICONTROL Action]_列：

- **[!UICONTROL Update Required Info]**:選擇清單與目錄不自動匹配的時間。 可以手動 [將目錄產品與清單匹配](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found)手動 [分配ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) 目錄匹配，或 [指定缺少的條件](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) 清單。

- **[!UICONTROL View Details]**：選擇查看清單詳細資訊，包括 [列出活動日誌](./product-listing-details.md#listing-activity-log)。 [Buy Box競爭對手定價](./product-listing-details.md#buy-box-competitor-pricing), [最低競爭對手定價](./product-listing-details.md#lowest-competitor-pricing)。 此操作僅用於查看。 無法在清單詳細資訊中進行更改。 請參閱 [查看詳細資訊](./product-listing-details.md)。

>[!NOTE]
>
>如果正在處理清單，則清單數將顯示在頁籤上方的消息中。

![未完成的Amazon清單](assets/amazon-incomplete-listings.png)

Amazon銷售渠道首頁共用一些共同的 [工作區控制項](./workspace-controls.md) 允許您自定義顯示的資料。

| 列 | 說明 |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | 由Amazon分配給產品的SKU（庫存單位），以標識產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 標識項的10個字母和/或數字的唯一塊。<br><br>ASIN代表 [!DNL Amazon Standard Identification Number]。 ASIN是由10個字母和/或數字組成的唯一塊，用於標識項目。 對於書籍，ASIN與ISBN號相同，但對於所有其他產品，在將項目上載到其目錄時會建立新的ASIN。 您可以在Amazon的產品詳細資訊頁面上找到項目ASIN，以及與項目相關的詳細資訊。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Condition] | 的 [條件](./product-listing-condition.md) 產品。 |
| [!UICONTROL Landed Price] | 產品的上市價格加其發運價格。 |
| [!UICONTROL Amazon Quantity] | 當產品在Amazon主動列出時可用的數量。 |
| [!UICONTROL Status] | 上市狀態，由Amazon定義。 請參閱上面的「狀態」(Status)表格。 |
| [!UICONTROL Action] | 可應用於特定清單的可用操作的清單。 要應用操作，請按一下 **[!UICONTROL Select]** 的 _[!UICONTROL Action]_列，然後選擇選項：<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

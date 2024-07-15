---
title: Amazon銷售管道 — [!UICONTROL Ready to List]
description: Amazon銷售管道提供準備好列出索引標籤，協助您檢閱符合資格但未自動列出的Commerce產品。
feature: Sales Channels, Products, Merchandising
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

_[!UICONTROL Ready to List]_索引標籤顯示您的[!DNL Commerce]目錄產品符合您的清單設定，並準備好以&#x200B;**新的**清單形式發佈到Amazon。 與其他清單索引標籤不同，此索引標籤不一定會顯示在[_[!UICONTROL Product Listings]_](./managing-product-listings.md)頁面上。

只有當清單設定中的[**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)設定為`Do Not Automatically List Eligible Products`時，_[!UICONTROL Ready to List]_索引標籤才會出現。 此設定可告知Amazon sales channel任何新的Amazon清單都必須手動發佈。

當[**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)設定為`Automatically List Eligible Products`時，Amazon銷售管道會自動發佈您合格目錄產品的新清單。 因為新清單會自動發佈，所以不會顯示&#x200B;_[!UICONTROL Ready to List]_索引標籤。

在&#x200B;_[!UICONTROL Actions]_下：

- **[!UICONTROL Publish Product to Amazon]**：選擇將清單重新發佈至[!DNL Amazon Marketplace]。 檢視[Publish與Amazon清單](./publish-listings-manually.md)

在&#x200B;_[!UICONTROL Action]_欄的&#x200B;**[!UICONTROL Select]**下：

- **[!UICONTROL Publish On Amazon]**：選擇將清單重新發佈至[!DNL Amazon Marketplace]。 請參閱[Publish與Amazon清單](./publish-listings-manually.md)。

- **[!UICONTROL View Details]**：選擇檢視清單詳細資料，包括[清單活動記錄](./product-listing-details.md#listing-activity-log)、[Buy Box競爭者定價](./product-listing-details.md#buy-box-competitor-pricing)和[最低競爭者定價](./product-listing-details.md#lowest-competitor-pricing)。 此動作僅供檢視。 清單詳細資料不可變更。 檢視[檢視詳細資料](./product-listing-details.md)。

您有幾個選項可手動[將新清單發佈到Amazon](./publish-listings-manually.md)。

>[!NOTE]
>如果您有處理中的清單，清單的數量會顯示在標籤上方的訊息中。

![準備列出](assets/amazon-ready-to-list.png){width="600" zoomable="yes"}

## 預設欄

| 欄 | 說明 |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Amazon指派給產品的SKU （庫存單位），用於識別產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 識別專案的10個字母和/或數字的唯一區塊。<br><br>ASIN代表[!DNL Amazon Standard Identification Number]。 ASIN是識別專案的10個字母和/或數字的唯一區塊。 對於書籍，ASIN與ISBN編號相同，但對於所有其他產品，當專案上傳到它們的目錄時會建立新的ASIN。 您可以在Amazon的產品詳細資料頁面上找到專案ASIN，以及與此專案相關的其他詳細資料。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Condition] | 產品的[狀況](./product-listing-condition.md)。 |
| [!UICONTROL Landed Price] | 產品的上市價格加上其送貨價格。 |
| [!UICONTROL Amazon Quantity] | 產品在Amazon上主動列出時的可用數量。 |
| [!UICONTROL Status] | 清單的狀態，由Amazon定義。 |
| [!UICONTROL Action] | 可套用至特定清單的可用動作清單。 若要套用動作，請按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Select]**並選擇選項：<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### 列出清單準備就緒的常見原因

- **[!UICONTROL Ready to List]** — 產品符合Amazon ASIN並已排定清單。 如果您的清單設定中的[**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)設定為`Do Not Automatically List Eligible Products`，則此狀態代表可以手動列出的產品。

- **[!UICONTROL List in Progress]** — 產品清單已提交至Amazon，並正在等待Amazon的接受確認。

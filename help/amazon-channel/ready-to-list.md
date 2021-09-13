---
title: 準備列出
description: Amazon銷售管道提供「準備列出」標籤，協助您檢閱符合資格但未自動列出的商務產品。
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

_[!UICONTROL Ready to List]_標籤會顯示符合清單設定且準備以&#x200B;**new**清單形式發佈至Amazon的[!DNL Commerce]目錄產品。 與其他清單頁簽不同，此頁簽不一定出現在[_[!UICONTROL Product Listings]_](./managing-product-listings.md)頁面上。

_[!UICONTROL Ready to List]_標籤僅在清單設定中的[**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)設定為`Do Not Automatically List Eligible Products`時顯示。 此設定會告訴Amazon銷售管道，任何新的Amazon清單都必須手動發佈。

當[**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)設為`Automatically List Eligible Products`時，Amazon銷售管道會自動發佈符合資格目錄產品的新清單。 由於新清單會自動發佈，因此不會顯示&#x200B;_[!UICONTROL Ready to List]_標籤。

在&#x200B;_[!UICONTROL Actions]_下：

- **[!UICONTROL Publish Product to Amazon]**:選擇將清單重新發佈到 [!DNL Amazon Marketplace]。請參閱[發佈Amazon清單](./publish-listings-manually.md)

在&#x200B;_[!UICONTROL Action]_欄的&#x200B;**[!UICONTROL Select]**下：

- **[!UICONTROL Publish On Amazon]**:選擇將清單重新發佈到 [!DNL Amazon Marketplace]。請參閱[發佈Amazon清單](./publish-listings-manually.md)。

- **[!UICONTROL View Details]**：選擇檢視清單詳細資訊，包括 [清單活動記錄](./product-listing-details.md#listing-activity-log)、 [Buy Box競爭者定價](./product-listing-details.md#buy-box-competitor-pricing)和最低 [競爭者定價](./product-listing-details.md#lowest-competitor-pricing)。此動作僅供檢視。 清單詳細資訊中不能進行任何更改。 請參閱[查看詳細資訊](./product-listing-details.md)。

您有幾個選項可手動[將新清單發佈至Amazon](./publish-listings-manually.md)。

>[!NOTE]
>如果正在處理清單，則清單數將顯示在頁簽上方的消息中。

![準備列出](assets/amazon-ready-to-list.png)

## 預設列

| 欄 | 說明 |
|---|---|
| [!UICONTROL Amazon Seller SKU] | 由Amazon指派給產品的SKU（庫存保管單位），用以識別產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 10個字母和/或數字的唯一區塊，用於識別項目。<br><br>ASIN代表 [!DNL Amazon Standard Identification Number]。ASIN是10個字母和/或數字的唯一塊，用於標識項目。 對於帳簿，ASIN與ISBN號相同，但是對於所有其他產品，當項目上載到其目錄時將建立新的ASIN。 您可以在Amazon的產品詳細資訊頁面上找到項目ASIN，以及與項目相關的詳細資訊。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Condition] | 產品的[條件](./product-listing-condition.md)。 |
| [!UICONTROL Landed Price] | 產品的掛牌價加其運價。 |
| [!UICONTROL Amazon Quantity] | 產品主動列於Amazon時的可用數量。 |
| [!UICONTROL Status] | 清單的狀態，由Amazon定義。 |
| [!UICONTROL Action] | 可套用至特定清單的可用動作清單。 若要套用動作，請按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Select]**，然後選擇一個選項：<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### 準備列出清單的常見原因

- **[!UICONTROL Ready to List]**  — 產品符合Amazon ASIN，且已排程列出。如果清單設定中的[**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)設為`Do Not Automatically List Eligible Products`，此狀態代表已準備好手動列出的產品。

- **[!UICONTROL List in Progress]**  — 產品清單已提交至Amazon，並等待Amazon確認接受。

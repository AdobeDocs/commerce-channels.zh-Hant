---
title: 『入門：建立清單規則'
description: 完成Amazon銷售管道入門程式時，請建立初始上市規則，為您的 [!DNL Commerce] 產品。
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 入門：建立清單規則

上市規則可在上線期間定義，但也可隨時修改。 上線後，您可以存取 [清單規則](./listing-rules.md) 在商店 [儀表板](./amazon-store-dashboard.md).

## 在上線期間建立清單規則

1. 連線商店後，按一下 **[!UICONTROL View Store]** ，以新增商店。

   商店 [儀表板](./amazon-store-dashboard.md) 隨 `No products listed to Amazon` 訊息。

1. 按一下 **[!UICONTROL Preview and List Eligible Products]**.

   此 _[!UICONTROL Listing Rules]_頁。

1. 為要在Amazon上列出的產品資格定義您想要的條件，然後按一下 **[!UICONTROL Preview changes]**，或按一下 **[!UICONTROL Preview changes]** 跳過此步驟。

   請參閱 [範例：定義條件](./ob-define-condition-example.md).

1. 在清單預覽中查看清單：

   ![清單預覽](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]**  — 根據您目前的清單規則設定，此標籤上列出的產品不符合Amazon清單的資格。

      不符合資格的產品不會發佈至Amazon。 如果Amazon上已列出不符合資格的產品，且您將Amazon清單與 [!DNL Commerce] 目錄產品，Amazon清單的數量變更為 `0` 防止產品銷售。 若要從Amazon手動移除清單，請參閱 [結束Amazon清單](./end-listings-manually.md). 不符合Amazon要求的產品不會列於此處。 這些產品列於 [[!UICONTROL Inactive Listings] 標籤](./inactive-listings.md).

      若要變更 `Ineligible` 清單至 `Eligible` 清單，重複此程式並修改您的清單規則。

   - **[!UICONTROL Eligible Listings]**  — 根據您目前的上市規則設定，此標籤上列出的產品符合Amazon上市資格，且符合Amazon要求。 此索引標籤包含已匯入的現有Amazon清單(若您有 **[!UICONTROL Import Third Party Listings]** 設為 `Import Listing` 在 [清單設定](./listing-settings.md))。

   - **[!UICONTROL New Listings]**  — 此標籤上列出的產品包括 [!DNL Commerce] 根據您目前的清單規則設定，目錄新符合Amazon清單資格的產品，並建立Amazon清單。

1. 完成後，按一下 **[!UICONTROL Save and Close]**.

   商店 [儀表板](./amazon-store-dashboard.md) 開啟。

上線商店完成後，資訊會同步於 [!DNL Commerce] 而Amazon已經開始。 您的Amazon清單會匯入 [!DNL Commerce] 並嘗試與 [!DNL Commerce] 目錄。

您可以在 _[!UICONTROL Recent Orders]_區段。 請參閱 [儲存控制面板](./amazon-store-dashboard.md) 或 [管理訂單](./managing-orders.md).

>[!IMPORTANT]
>
>某些重要商店設定（清單、定價、規則、履行等）具有新商店的預設值。 為確保您的商店已針對您的特定需求進行設定，請檢閱您的 [儲存設定](./default-store-settings.md) .

![下一個表徵圖](assets/btn-next.png) [**繼續使用預設儲存設定**](./default-store-settings.md)

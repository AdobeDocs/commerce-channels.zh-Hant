---
title: 建立Amazon清單規則
description: 完成Amazon銷售管道上線流程後，請建立初始清單規則，以便為產生Amazon清單 [!DNL Commerce] 產品。
role: Admin
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 建立Amazon清單規則

清單規則可在上線期間定義，但亦可隨時修改。 上線後，您可以存取 [清單規則](./listing-rules.md) 在存放區上 [儀表板](./amazon-store-dashboard.md).

## 上線期間建立清單規則

1. 在您的商店連線後，按一下 **[!UICONTROL View Store]** 用於新增的商店。

   商店 [儀表板](./amazon-store-dashboard.md) 出現時具有 `No products listed to Amazon` 訊息。

1. 按一下 **[!UICONTROL Preview and List Eligible Products]**.

   此 _[!UICONTROL Listing Rules]_頁面便會顯示。

1. 定義您想要的條件以符合在Amazon上列出的產品資格，然後按一下 **[!UICONTROL Preview changes]**，或按一下 **[!UICONTROL Preview changes]** 以略過此步驟。

   另請參閱 [範例：定義條件](./ob-define-condition-example.md).

1. 在「清單預覽」中檢閱您的清單：

   ![清單預覽](assets/amazon-ob-listing-preview.png){width="600" zoomable="yes"}

   - **[!UICONTROL Ineligible Listings]**  — 根據您目前的清單規則設定，此標籤上列出的產品不符合Amazon清單的資格。

     不符合資格的產品不會發佈至Amazon。 如果不符合資格的產品已列於Amazon上，且您將Amazon清單與 [!DNL Commerce] 目錄產品，Amazon清單的數量變更為 `0` 以防止產品銷售。 若要從Amazon手動移除清單，請參閱 [結束Amazon清單](./end-listings-manually.md). 不符合Amazon要求的產品在此不列出。 這些產品會列在 [[!UICONTROL Inactive Listings] 標籤](./inactive-listings.md).

     若要變更 `Ineligible` 列為 `Eligible` 列出、重複此程式，並修改您的清單規則。

   - **[!UICONTROL Eligible Listings]**  — 根據您目前的清單規則設定，此標籤上列出的產品符合Amazon清單的條件，並符合Amazon的要求。 此索引標籤包含已匯入的現有Amazon清單(如果已 **[!UICONTROL Import Third Party Listings]** 設為 `Import Listing` 在您的 [清單設定](./listing-settings.md))。

   - **[!UICONTROL New Listings]**  — 此標籤上列出的產品包含您的 [!DNL Commerce] 根據您目前的清單規則設定和建立Amazon清單，列出新符合Amazon清單資格的目錄產品。

1. 完成後，按一下 **[!UICONTROL Save and Close]**.

   商店 [儀表板](./amazon-store-dashboard.md) 隨即開啟。

上線商店完成之後，資訊會在 [!DNL Commerce] 和Amazon已啟動。 您的Amazon清單已匯入 [!DNL Commerce] 並嘗試比對您網站上的產品 [!DNL Commerce] 目錄。

您可以在以下位置檢視您的Amazon訂單資訊： _[!UICONTROL Recent Orders]_區段。 另請參閱 [存放區控制面板](./amazon-store-dashboard.md) 或 [管理訂單](./managing-orders.md).

>[!IMPORTANT]
>
>有些重要的商店設定（清單、定價、規則、履行等等）具有新商店的預設值。 為確保您的商店已設定符合您的特定需求，請檢閱您的 [商店設定](./default-store-settings.md) .

![「下一步」圖示](assets/btn-next.png) [**繼續使用預設商店設定**](./default-store-settings.md)

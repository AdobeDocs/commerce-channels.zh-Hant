---
title: 「登機：建立清單規則'
description: 在完成Amazon銷售渠道登陸流程時，建立初始上市規則，為您的 [!DNL Commerce] 產品。
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 登機：建立清單規則

上市規則可於入職期間定義，亦可隨時修訂。 登機後，您可以 [上市規則](./listing-rules.md) 店裡 [儀表板](./amazon-store-dashboard.md)。

## 在入職期間建立清單規則

1. 連接商店後，按一下 **[!UICONTROL View Store]** 添加的儲存。

   商店 [儀表板](./amazon-store-dashboard.md) 顯示 `No products listed to Amazon` 。

1. 按一下 **[!UICONTROL Preview and List Eligible Products]**。

   的 _[!UICONTROL Listing Rules]_的子菜單。

1. 為要在Amazon列出的產品的資格定義所需條件，然後按一下 **[!UICONTROL Preview changes]**，按一下 **[!UICONTROL Preview changes]** 跳過此步驟。

   請參閱 [示例：定義條件](./ob-define-condition-example.md)。

1. 在「清單預覽」中查看您的清單：

   ![列出預覽](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]**  — 根據您當前的清單規則設定，此標籤上列出的產品不符合Amazon清單條件。

      不合格產品不發佈給Amazon。 如果Amazon上已列出不合格產品，並且您將Amazon清單與 [!DNL Commerce] 目錄產品，Amazon清單的數量更改 `0` 防止產品銷售。 要手動從Amazon刪除清單，請參閱 [結束Amazon上市](./end-listings-manually.md)。 不符合Amazon要求的產品不在此列出。 這些產品列在 [[!UICONTROL Inactive Listings] 頁籤](./inactive-listings.md)。

      更改 `Ineligible` 列至 `Eligible` 列出，重複此過程並修改您的上市規則。

   - **[!UICONTROL Eligible Listings]**  — 此標籤上列出的產品根據您當前的上市規則設定有資格獲得Amazon上市，並符合Amazon要求。 此頁籤包括導入的現有Amazon清單(如果您 **[!UICONTROL Import Third Party Listings]** 設定為 `Import Listing` 在 [列出設定](./listing-settings.md))。

   - **[!UICONTROL New Listings]**  — 此標籤上列出的產品包括 [!DNL Commerce] 根據您當前的清單規則設定新建符合Amazon清單的目錄產品，並建立Amazon清單。

1. 完成後，按一下 **[!UICONTROL Save and Close]**。

   商店 [儀表板](./amazon-store-dashboard.md) 的上界。

登入儲存後，資訊在 [!DNL Commerce] 而Amazon是發起的。 您的Amazon清單已導入 [!DNL Commerce] 並嘗試與 [!DNL Commerce] 目錄。

您可以在以下位置查看您的Amazon訂單資訊： _[!UICONTROL Recent Orders]_的子菜單。 請參閱 [儲存儀表板](./amazon-store-dashboard.md) 或 [管理訂單](./managing-orders.md)。

>[!IMPORTANT]
>
>某些重要商店設定（清單、定價、規則、履行等）具有新商店的預設值。 要確保您的商店已根據您的特定需求設定，請查看 [儲存設定](./default-store-settings.md) 。

![下一個表徵圖](assets/btn-next.png) [**繼續預設儲存設定**](./default-store-settings.md)

---
title: 『入門：建立清單規則'
description: 在完成Amazon銷售管道入門程式時，建立初始清單規則，以產生您 [!DNL Commerce] 產品的Amazon清單。
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 入門：建立清單規則

上市規則可在上線期間定義，但也可隨時修改。 上線後，您可以存取[控制面板](./amazon-store-dashboard.md)上的[清單規則](./listing-rules.md)。

## 在上線期間建立清單規則

1. 連接商店後，按一下&#x200B;**[!UICONTROL View Store]**&#x200B;以獲取添加的商店。

   儲存區[儀表板](./amazon-store-dashboard.md)隨`No products listed to Amazon`訊息出現。

1. 按一下&#x200B;**[!UICONTROL Preview and List Eligible Products]**。

   此時將顯示&#x200B;_[!UICONTROL Listing Rules]_頁。

1. 為要在Amazon上列出的產品資格定義您所需的條件，然後按一下&#x200B;**[!UICONTROL Preview changes]**，或按一下&#x200B;**[!UICONTROL Preview changes]**&#x200B;以略過此步驟。

   請參閱[範例：定義條件](./ob-define-condition-example.md)。

1. 在清單預覽中查看清單：

   ![清單預覽](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]**  — 根據您目前的清單規則設定，此標籤上列出的產品不符合Amazon清單的資格。

      不符合資格的產品不會發佈至Amazon。 如果Amazon上已列出不合格產品，且您將Amazon清單與[!DNL Commerce]目錄產品相符，則Amazon清單的數量會變更為`0`，以防止產品銷售。 若要從Amazon手動移除清單，請參閱[結束Amazon清單](./end-listings-manually.md)。 不符合Amazon要求的產品不會列於此處。 這些產品會列在[[!UICONTROL Inactive Listings]標籤](./inactive-listings.md)上。

      若要將`Ineligible`清單變更為`Eligible`清單，請重複此程式並修改您的清單規則。

   - **[!UICONTROL Eligible Listings]**  — 根據您目前的上市規則設定，此標籤上列出的產品符合Amazon上市資格，且符合Amazon要求。此索引標籤包含已匯入的現有Amazon清單（若您在[清單設定](./listing-settings.md)中將&#x200B;**[!UICONTROL Import Third Party Listings]**&#x200B;設為`Import Listing`）。

   - **[!UICONTROL New Listings]**  — 此標籤上列出的產品包括 [!DNL Commerce] 根據您目前的清單規則設定，新符合Amazon清單資格的目錄產品，並建立Amazon清單。

1. 完成後，按一下&#x200B;**[!UICONTROL Save and Close]**。

   商店[儀表板](./amazon-store-dashboard.md)開啟。

上線商店完成後，[!DNL Commerce]和Amazon之間的資訊同步即會啟動。 您的Amazon清單會匯入[!DNL Commerce]，並嘗試與[!DNL Commerce]目錄中的產品相符。

您可以在存放區控制面板的&#x200B;_[!UICONTROL Recent Orders]_區段中檢視Amazon訂單資訊。 請參閱[儲存控制面板](./amazon-store-dashboard.md)或[管理訂單](./managing-orders.md)。

>[!IMPORTANT]
>
>某些重要商店設定（清單、定價、規則、履行等）具有新商店的預設值。 若要確保您的商店已針對您的特定需求進行設定，請檢閱您的[商店設定](./default-store-settings.md) 。

![下一](assets/btn-next.png) [**個圖示繼續預設商店設定**](./default-store-settings.md)

---
title: 建立和編輯屬性
description: AmazonSales Channel提供「屬性」檢視，協助您檢閱目前的Amazon屬性和連結的商務屬性。
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# 建立和編輯屬性

建立或更新 [!DNL Commerce] 屬性，以便透過Amazon銷售並更新商店。 檢閱目前的Amazon屬性並連結 [!DNL Commerce] 屬性 [_[!UICONTROL Attributes]_檢視](./attributes-view.md) Amazon銷售管道首頁。 此_[!UICONTROL Action]_ 欄顯示屬性的可用操作。 您可以建立並對應新 [!DNL Commerce] 屬性，或者您可以編輯現有的Amazon屬性 [!DNL Commerce] 屬性，及其對應至Amazon屬性。

建立和更新屬性時，您可能想驗證 [!DNL Commerce] 和Amazon產品。 如果您未從Amazon同步和匯入值，這些值可能會有所不同。 若要檢閱這些屬性的Amazon值，請參閱 [檢閱Amazon屬性對應](./amazon-matching-attributes-values.md). 如果您想要變更這些值，您可以 [編輯或建立對應](./amazon-manually-update-incomplete-listing.md) 在Amazon和 [!DNL Commerce].

## 建立屬性 {#create-an-attribute}

這些步驟會建立 [!DNL Commerce] 屬性，並將其對應至Amazon屬性。 視設定而定，值可能會開始在目錄之間同步。

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 按一下 **[!UICONTROL Attributes]** 在左側功能表中，找出Amazon屬性，然後按一下 **[!UICONTROL Create Attribute]** 在 _[!UICONTROL Action]_欄。

1. 啟用將Amazon值同步至連結的 [!DNL Commerce] 屬性，設定 **[!UICONTROL Is Active]** to `Yes`.

   設為時 `Yes`，則值會根據您的設定同步。

1. 選擇 `Create New Magento Attribute` for **[!UICONTROL Select Magento Product Attribute]**.

   屬性對應至所選的 **[!UICONTROL Amazon Attribute Name]**.

1. 輸入 **[!UICONTROL Magento Product Attribute Name]**.

1. 輸入 **[!UICONTROL Magento Product Attribute Code]**.

   此值必須全部為小寫，不含空格。

1. 針對 **[!UICONTROL Attribute Set Ids]**，選擇要分配的屬性集。

   通常，屬性是屬性集的一部分，如具有藍色、綠色、黃色和紅色屬性的顏色集。

1. 針對 **[!UICONTROL Type]**，選擇屬性值的類型，如文本和數字。

   此選項會影響屬性的允許值。

1. 針對 **[!UICONTROL Use for Promo Rule Conditions]**，設為 `Yes` 允許屬性可用於促銷條件中的參數。

1. 針對 **[!UICONTROL Used in Search]**，設為 `Yes` 如果屬性和值可用於產品搜尋。

1. 針對 **[!UICONTROL Comparable on Storefront]**，設為 `Yes` 如果屬性值可用於Amazon的「比較依據」功能。

1. 選擇 [!DNL Commerce] [範圍](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;}作為屬性，然後選取一或多個「儲存檢視」來將Amazon值匯入。

   如果範圍設定為 `Global`, _[!UICONTROL Store View]_建立屬性後無法變更。

   如果您選擇 `All Store Views (Global)`，它會同步並儲存值至所有Amazon商店檢視。 您可能只想將值同步至特定商店檢視。

1. 完成後，按一下 **[!UICONTROL Save Attribute Settings]**.

儲存後，您可能想要編輯屬性以檢閱設定及比對Amazon和 [!DNL Commerce] 值。 您也可以指出Amazon值是否應覆寫 [!DNL Commerce] 值。

![建立屬性設定](assets/amazon-attribute-settings-create.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Is Active] | 指出此屬性是否為即時，且在Amazon和 [!DNL Commerce]. 設為 `Yes` 以確保來自Amazon和 [!DNL Commerce] 針對所選屬性保持同步。 |
| 選擇Magento產品屬性 | 指示要連結到列出的Amazon屬性名稱的選定屬性。 建立屬性時，請選擇 `Create New Magento Attribute`. |
| [!UICONTROL Amazon Attribute Name] | 顯示您所選Amazon屬性的名稱。 所選屬性連結到此Amazon屬性。 您無法透過 [!DNL Commerce]. |
| [!UICONTROL Magento Product Attribute Name] | 指示屬性名稱或&quot;label&quot;。 |
| [!UICONTROL Magento Product Attribute Code] | 指示屬性代碼，全部以小寫字元表示，不含空格。 |
| [!UICONTROL Attribute Set Ids] | 指示要向其分配屬性的屬性集。 屬性往往是屬性集的一部分，如具有藍色、綠色、黃色和紅色屬性的顏色集。 |
| [!UICONTROL Type] | 指示屬性值的值類型，如文本和數字。 選擇會影響屬性的允許值。 |
| [!UICONTROL Use for Promo Rule Conditions] | 切換為 `Yes` 允許屬性可用於促銷條件中的參數。 |
| [!UICONTROL Used in Search] | 指出屬性和值是否可用於產品搜尋。 |
| [!UICONTROL Comparable on Storefront] | 指出屬性值是否可用於Amazon的「比較依據」功能。 |
| [!UICONTROL Magento Product Attribute Scope] | 指出 [範圍](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;}取得。 選項：全域/商店檢視<br>設為時 `Global`，則建立屬性後就無法編輯「商店檢視」。 |
| [!UICONTROL Store Views (to import values into to)] | 僅當作用域設定為 `Store View`. 選擇 [商店檢視](https://docs.magento.com/user-guide/stores/websites-stores-views.html)將Amazon屬性值同步到的{target=&quot;_blank&quot;}。 選擇 `All Store Views (Global)` 會更新所有 [!DNL Commerce] 儲存檢視。 |

## 編輯屬性 {#edit-an-attribute}

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 按一下 **[!UICONTROL Attributes]** 在左側功能表中，找出Amazon屬性，然後按一下 **[!UICONTROL Edit]** 在 _[!UICONTROL Action]_欄。

1. 啟用或停用將Amazon值同步至連結的 [!DNL Commerce] 屬性，設定 **活動** to `Yes` 或 `No`.

   設為時 `Yes`，則值會根據您的設定同步。

1. 針對 **[!UICONTROL Select Magento Product Attribute]**，驗證或更新屬性以對應至所選的 **[!UICONTROL Amazon Attribute Name]**.

1. 指出您是否希望傳入的Amazon屬性值覆寫現有屬性值。

   例如，您不想將價格從Amazon覆寫至 [!DNL Commerce].

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]**  — 保留值，保留您 [!DNL Commerce] 和Amazon店。

   - **[!UICONTROL Overwrite Existing Magento Values]**  — 覆寫 [!DNL Commerce] 包含傳入Amazon值的產品目錄。

1. 如果可供編輯，請選擇一或多個 **[!UICONTROL Store Views (to import Amazon values into)]**.

   如果屬性是以 `Global` 範圍， _商店檢視_ 建立屬性後無法變更。

   如果您選擇 `All Store Views (Global)`，它會同步並將值儲存至所有商店檢視。 您可能只想將值同步至特定商店檢視。

1. 完成後，按一下 **[!UICONTROL Save Attribute Settings]**.

![編輯屬性設定](assets/amazon-attribute-settings-edit.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Is Active] | 指出此屬性是否為即時，且在Amazon和 [!DNL Commerce]. 設為 `Yes` 以確保來自Amazon和 [!DNL Commerce] 針對所選屬性保持同步。 |
| [!UICONTROL Select Magento Product Attribute] | 指示所選 [!DNL Commerce] 屬性，以連結至列出的Amazon屬性名稱。 如果您想要變更連結的 [!DNL Commerce] 屬性，從下拉式清單中選擇其他屬性。 值會根據設定同步。 |
| [!UICONTROL Amazon Attribute Name] | 顯示Amazon屬性的名稱，如 [!DNL Amazon Seller Central]. 選取的 [!DNL Commerce] 屬性連結至此Amazon屬性。 您無法透過 [!DNL Commerce]. |
| [!UICONTROL Overwrite Existing Value] | 指出Amazon屬性值是否覆寫現有 [!DNL Commerce] 值，會影響所有具有此 [!DNL Commerce] 屬性。<ul><li>**請勿覆寫現有的Magento值**  — （預設）保留 [!DNL Commerce] 值，保留不同的值 [!DNL Commerce] 和Amazon店。</li><li>**覆寫現有Magento值**  — 將Amazon值儲存於 [!DNL Commerce] 值 [!DNL Commerce] 產品目錄。</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | 編輯屬性時，如果屬性是使用 `Global` 範圍。 指出 [!DNL Commerce] [範圍](https://docs.magento.com/user-guide/configuration/scope.html)已建立{target=&quot;_blank&quot;}，並將其設定為 `Store View`. |
| [!UICONTROL Store Views (to import values into to)] | 選擇您的 [!DNL Commerce] [商店檢視](https://docs.magento.com/user-guide/stores/websites-stores-views.html)將Amazon屬性值同步到的{target=&quot;_blank&quot;}。 選擇 `All Store Views (Global)` 會更新所有商店檢視的值。 |

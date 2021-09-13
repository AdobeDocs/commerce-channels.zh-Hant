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

透過Amazon銷售時建立或更新[!DNL Commerce]屬性，並更新您的商店。 透過Amazon銷售管道首頁的&#x200B;[_[!UICONTROL Attributes]_檢視](./attributes-view.md)，檢閱目前的Amazon屬性和連結的[!DNL Commerce]屬性。_[!UICONTROL Action]_&#x200B;欄顯示屬性的可用操作。 您可以為未連結的Amazon屬性建立並映射新的[!DNL Commerce]屬性，或編輯現有的[!DNL Commerce]屬性及其與Amazon屬性的對應。

當您建立和更新屬性時，可能需要驗證[!DNL Commerce]和Amazon產品的屬性值。 如果您未從Amazon同步和匯入值，這些值可能會有所不同。 若要查看這些屬性的Amazon值，請參閱[查看Amazon屬性對應](./amazon-matching-attributes-values.md)。 如果您想要變更這些值，可以[編輯或建立Amazon與[!DNL Commerce]之間的對應](./amazon-manually-update-incomplete-listing.md)。

## 建立屬性 {#create-an-attribute}

這些步驟會建立[!DNL Commerce]屬性，並將其對應至Amazon屬性。 視設定而定，值可能會開始在目錄之間同步。

1. 在&#x200B;_Admin_&#x200B;側欄中，前往&#x200B;**[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Attributes]**，找出Amazon屬性，然後按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Create Attribute]**。

1. 若要啟用將Amazon值同步至連結的[!DNL Commerce]屬性，請將&#x200B;**[!UICONTROL Is Active]**&#x200B;設為`Yes`。

   設為`Yes`時，值會根據您的設定同步。

1. 為&#x200B;**[!UICONTROL Select Magento Product Attribute]**&#x200B;選擇`Create New Magento Attribute`。

   該屬性映射到為&#x200B;**[!UICONTROL Amazon Attribute Name]**&#x200B;選擇的。

1. 輸入&#x200B;**[!UICONTROL Magento Product Attribute Name]**。

1. 輸入&#x200B;**[!UICONTROL Magento Product Attribute Code]**。

   此值必須全部為小寫，不含空格。

1. 對於&#x200B;**[!UICONTROL Attribute Set Ids]**，選擇要分配的屬性集。

   通常，屬性是屬性集的一部分，如具有藍色、綠色、黃色和紅色屬性的顏色集。

1. 對於&#x200B;**[!UICONTROL Type]**，選擇屬性值的類型，如文本和數字。

   此選項會影響屬性的允許值。

1. 對於&#x200B;**[!UICONTROL Use for Promo Rule Conditions]**，設為`Yes`以允許該屬性可用於促銷條件內的參數。

1. 對於&#x200B;**[!UICONTROL Used in Search]**，如果屬性和值可用於產品搜尋，則設為`Yes`。

1. 對於&#x200B;**[!UICONTROL Comparable on Storefront]**，如果屬性值可用於Amazon的「比較依據」功能，請設為`Yes`。

1. 為屬性選擇[!DNL Commerce] [scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;}，然後選擇一個或多個儲存視圖以將Amazon值導入。

   如果將範圍設定為`Global`，則在建立屬性後無法更改&#x200B;_[!UICONTROL Store View]_。

   如果您選擇`All Store Views (Global)`，它會同步並將值儲存至所有Amazon存放區檢視。 您可能只想將值同步至特定商店檢視。

1. 完成後，按一下&#x200B;**[!UICONTROL Save Attribute Settings]**。

儲存後，您可能想要編輯屬性以檢閱設定，並比對屬性的Amazon和[!DNL Commerce]值。 您也可以指出Amazon值是否應覆寫[!DNL Commerce]值。

![建立屬性設定](assets/amazon-attribute-settings-create.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Is Active] | 指出此屬性是否為即時，且在Amazon和[!DNL Commerce]之間主動同步。 設為`Yes` ，以確保來自Amazon和[!DNL Commerce]的屬性值在所選屬性中保持同步。 |
| 選擇Magento產品屬性 | 指示要連結到列出的Amazon屬性名稱的選定屬性。 建立屬性時，請選擇`Create New Magento Attribute`。 |
| [!UICONTROL Amazon Attribute Name] | 顯示您所選Amazon屬性的名稱。 所選屬性連結到此Amazon屬性。 無法通過[!DNL Commerce]編輯此值。 |
| [!UICONTROL Magento Product Attribute Name] | 指示屬性名稱或&quot;label&quot;。 |
| [!UICONTROL Magento Product Attribute Code] | 指示屬性代碼，全部以小寫字元表示，不含空格。 |
| [!UICONTROL Attribute Set Ids] | 指示要向其分配屬性的屬性集。 屬性往往是屬性集的一部分，如具有藍色、綠色、黃色和紅色屬性的顏色集。 |
| [!UICONTROL Type] | 指示屬性值的值類型，如文本和數字。 選擇會影響屬性的允許值。 |
| [!UICONTROL Use for Promo Rule Conditions] | 切換至`Yes`以允許屬性可用於促銷條件內的參數。 |
| [!UICONTROL Used in Search] | 指出屬性和值是否可用於產品搜尋。 |
| [!UICONTROL Comparable on Storefront] | 指出屬性值是否可用於Amazon的「比較依據」功能。 |
| [!UICONTROL Magento Product Attribute Scope] | 指示該屬性的[scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;}。 選項：全局/儲存視圖<br>設定為`Global`時，在建立屬性後無法編輯儲存視圖。 |
| [!UICONTROL Store Views (to import values into to)] | 僅當作用域設定為`Store View`時才顯示。 選擇要將Amazon屬性值同步到的[儲存視圖](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}。 選擇`All Store Views (Global)`會更新所有[!DNL Commerce]儲存檢視的值。 |

## 編輯屬性 {#edit-an-attribute}

1. 在&#x200B;_Admin_&#x200B;側欄中，前往&#x200B;**[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Attributes]**，找出Amazon屬性，然後按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Edit]**。

1. 若要啟用或停用將Amazon值同步至連結的[!DNL Commerce]屬性，請將&#x200B;**Is Active**&#x200B;設為`Yes`或`No`。

   設為`Yes`時，值會根據您的設定同步。

1. 對於&#x200B;**[!UICONTROL Select Magento Product Attribute]**，驗證或更新屬性以映射到所選&#x200B;**[!UICONTROL Amazon Attribute Name]**。

1. 指出您是否希望傳入的Amazon屬性值覆寫現有屬性值。

   例如，您不可將Amazon的價格覆寫為[!DNL Commerce]。

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]**  — 保留值，保留您和Amazon商店 [!DNL Commerce] 的不同值。

   - **[!UICONTROL Overwrite Existing Magento Values]**  — 使用傳入的Amazon值 [!DNL Commerce] 覆寫產品目錄中的值。

1. 如果可編輯，請選擇一個或多個&#x200B;**[!UICONTROL Store Views (to import Amazon values into)]**。

   如果屬性是使用`Global`範圍建立的，則在建立屬性後，無法更改&#x200B;_儲存視圖_。

   如果選擇`All Store Views (Global)`，它會同步並將值保存到所有儲存視圖。 您可能只想將值同步至特定商店檢視。

1. 完成後，按一下&#x200B;**[!UICONTROL Save Attribute Settings]**。

![編輯屬性設定](assets/amazon-attribute-settings-edit.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Is Active] | 指出此屬性是否為即時，且在Amazon和[!DNL Commerce]之間主動同步。 設為`Yes` ，以確保來自Amazon和[!DNL Commerce]的屬性值在所選屬性中保持同步。 |
| [!UICONTROL Select Magento Product Attribute] | 指示要連結到列出的Amazon屬性名稱的選定[!DNL Commerce]屬性。 如果要更改連結的[!DNL Commerce]屬性，請從下拉清單中選擇其他屬性。 值會根據設定同步。 |
| [!UICONTROL Amazon Attribute Name] | 顯示[!DNL Amazon Seller Central]中定義的Amazon屬性名稱。 所選[!DNL Commerce]屬性連結到此Amazon屬性。 無法通過[!DNL Commerce]編輯此值。 |
| [!UICONTROL Overwrite Existing Value] | 指出Amazon屬性值是否覆寫現有的[!DNL Commerce]值，進而影響具有此[!DNL Commerce]屬性的所有產品。<ul><li>**請勿覆寫現有的Magento值**  — （預設值）會保留 [!DNL Commerce] 值，保留和Amazon [!DNL Commerce] 存放區的不同值。</li><li>**覆寫現有Magento值**  — 儲存Amazon值而非 [!DNL Commerce] 產品目錄 [!DNL Commerce] 中的值。</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | 如果屬性是使用`Global`範圍建立，則在編輯屬性時不會顯示。 指示已建立[!DNL Commerce] [scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;}並將其設定為`Store View`。 |
| [!UICONTROL Store Views (to import values into to)] | 選擇要將Amazon屬性值同步到的[!DNL Commerce] [儲存視圖](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}。 選擇`All Store Views (Global)`會更新所有商店檢視的值。 |

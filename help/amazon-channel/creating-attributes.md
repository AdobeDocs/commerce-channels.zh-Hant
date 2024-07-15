---
title: 建立和編輯Amazon sales channel的屬性
description: AmazonSales Channel提供「屬性」檢視，協助您檢閱目前的Amazon屬性和連結的Commerce屬性。
feature: Sales Channels, Products, Configuration
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# 建立和編輯屬性

在您透過Amazon銷售時建立或更新[!DNL Commerce]屬性，並更新您的商店。 檢閱目前的Amazon屬性，並透過Amazon銷售管道首頁的&#x200B;[_[!UICONTROL Attributes]_檢視](./attributes-view.md)連結[!DNL Commerce]屬性。_[!UICONTROL Action]_&#x200B;欄顯示屬性的可用動作。 您可以為未連結的Amazon屬性建立和對應新的[!DNL Commerce]屬性，也可以編輯現有的[!DNL Commerce]屬性及其對Amazon屬性的對應。

當您建立和更新屬性時，您可能想要驗證[!DNL Commerce]和Amazon產品的屬性值。 如果您未從Amazon同步及匯入值，這些值可能會有所不同。 若要檢閱這些屬性的Amazon值，請參閱[檢閱Amazon屬性對應](./amazon-matching-attributes-values.md)。 若要變更這些值，您可以[編輯或建立Amazon與[!DNL Commerce]之間的對應](./amazon-manually-update-incomplete-listing.md)。

## 建立屬性 {#create-an-attribute}

這些步驟會建立[!DNL Commerce]屬性，並將其對應至Amazon屬性。 視設定而定，值可能會開始在目錄之間同步。

1. 在&#x200B;_管理員_&#x200B;側邊欄上，移至&#x200B;**[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Attributes]**，找到Amazon屬性，然後按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Create Attribute]**。

1. 若要啟用Amazon值與連結[!DNL Commerce]屬性的同步處理，請將&#x200B;**[!UICONTROL Is Active]**&#x200B;設為`Yes`。

   設定為`Yes`時，值會根據您的設定同步。

1. 為&#x200B;**[!UICONTROL Select Magento Product Attribute]**&#x200B;選擇`Create New Magento Attribute`。

   屬性對應到&#x200B;**[!UICONTROL Amazon Attribute Name]**&#x200B;選擇的屬性。

1. 輸入&#x200B;**[!UICONTROL Magento Product Attribute Name]**。

1. 輸入&#x200B;**[!UICONTROL Magento Product Attribute Code]**。

   此值必須全部小寫且不加空格。

1. 針對&#x200B;**[!UICONTROL Attribute Set Ids]**，選擇要指派的屬性集。

   通常，屬性是屬性集的一部分，例如具有藍色、綠色、黃色和紅色屬性的顏色集。

1. 針對&#x200B;**[!UICONTROL Type]**，選擇屬性值的型別，例如文字和數字。

   此選項會影響屬性允許的值。

1. 針對&#x200B;**[!UICONTROL Use for Promo Rule Conditions]**，設定為`Yes`以允許屬性可用於促銷條件內的引數。

1. 如果屬性和值可用於產品搜尋，請針對&#x200B;**[!UICONTROL Used in Search]**&#x200B;設為`Yes`。

1. 如果屬性值可用於Amazon的「比較對象」功能，請針對&#x200B;**[!UICONTROL Comparable on Storefront]**&#x200B;設為`Yes`。

1. 選擇屬性的[!DNL Commerce] [範圍](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings)，然後選取一或多個要將Amazon值匯入的存放區檢視。

   如果範圍設定為`Global`，則在屬性建立之後無法變更&#x200B;_[!UICONTROL Store View]_。

   如果選擇`All Store Views (Global)`，則會同步值並儲存至您所有的Amazon存放區檢視。 您可能只想將值同步至特定的存放區檢視。

1. 完成時，按一下&#x200B;**[!UICONTROL Save Attribute Settings]**。

儲存後，您可能會想要編輯屬性以檢閱設定，並比對屬性的Amazon和[!DNL Commerce]值。 您也可以指示Amazon值是否應該覆寫[!DNL Commerce]值。

![建立屬性設定](assets/amazon-attribute-settings-create.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|-----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | 表示此屬性是否為即時狀態，且會在Amazon和[!DNL Commerce]之間主動同步。 設定為`Yes`以確保來自Amazon的屬性值與[!DNL Commerce]保持所選屬性的同步。 |
| 選取Magento產品屬性 | 表示您要連結至所列「Amazon屬性名稱」的選取屬性。 建立屬性時，請選擇`Create New Magento Attribute`。 |
| [!UICONTROL Amazon Attribute Name] | 顯示您選擇的Amazon屬性名稱。 選取的屬性會連結至此Amazon屬性。 您無法透過[!DNL Commerce]編輯此值。 |
| [!UICONTROL Magento Product Attribute Name] | 表示屬性名稱或「標籤」。 |
| [!UICONTROL Magento Product Attribute Code] | 指示屬性代碼，全部以小寫字元表示，不含空格。 |
| [!UICONTROL Attribute Set Ids] | 指示要指派屬性的「屬性集」。 屬性往往是屬性集的一部分，例如具有藍色、綠色、黃色和紅色屬性的顏色集。 |
| [!UICONTROL Type] | 指示屬性值的值型別，例如文字和數字。 選取範圍會影響屬性的允許值。 |
| [!UICONTROL Use for Promo Rule Conditions] | 切換至`Yes`，讓屬性可用於促銷條件中的引數。 |
| [!UICONTROL Used in Search] | 表示屬性和值是否可用於產品搜尋。 |
| [!UICONTROL Comparable on Storefront] | 指出屬性值是否可用於Amazon的「比較依據」功能。 |
| [!UICONTROL Magento Product Attribute Scope] | 表示屬性的[範圍](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings)。 選項：全域/存放區檢視<br>當設為`Global`時，建立屬性後就無法編輯存放區檢視。 |
| [!UICONTROL Store Views (to import values into to)] | 僅當範圍設定為`Store View`時才會出現。 選擇Amazon屬性值同步至的[存放區檢視](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html)。 選擇`All Store Views (Global)`會更新所有[!DNL Commerce]存放區檢視中的值。 |

## 編輯屬性 {#edit-an-attribute}

1. 在&#x200B;_管理員_&#x200B;側邊欄上，移至&#x200B;**[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Attributes]**，找到Amazon屬性，然後按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Edit]**。

1. 若要啟用或停用將Amazon值同步至連結的[!DNL Commerce]屬性，請將&#x200B;**Is Active**&#x200B;設定為`Yes`或`No`。

   設定為`Yes`時，值會根據您的設定同步。

1. 針對&#x200B;**[!UICONTROL Select Magento Product Attribute]**，驗證或更新要對應至所選&#x200B;**[!UICONTROL Amazon Attribute Name]**&#x200B;的屬性。

1. 指示您是否希望傳入的Amazon屬性值覆寫現有的屬性值。

   例如，您可能不想將Amazon的價格覆寫為[!DNL Commerce]。

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** — 保留值，保留您的[!DNL Commerce]和Amazon存放區的不同值。

   - **[!UICONTROL Overwrite Existing Magento Values]** — 以傳入的Amazon值覆寫[!DNL Commerce]產品目錄中的值。

1. 如果可以編輯，請選擇一或多個&#x200B;**[!UICONTROL Store Views (to import Amazon values into)]**。

   如果屬性是以`Global`範圍建立的，則在屬性建立後就無法變更&#x200B;_存放區檢視_。

   如果選擇`All Store Views (Global)`，則會同步值並儲存至所有存放區檢視。 您可能只想將值同步至特定的存放區檢視。

1. 完成時，按一下&#x200B;**[!UICONTROL Save Attribute Settings]**。

![編輯屬性設定](assets/amazon-attribute-settings-edit.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | 表示此屬性是否為即時狀態，且會在Amazon和[!DNL Commerce]之間主動同步。 設定為`Yes`以確保來自Amazon的屬性值與[!DNL Commerce]保持所選屬性的同步。 |
| [!UICONTROL Select Magento Product Attribute] | 表示您想要連結至所列Amazon屬性名稱的已選取[!DNL Commerce]屬性。 如果您想要變更連結的[!DNL Commerce]屬性，請從下拉式清單中選擇不同的屬性。 值會根據設定同步。 |
| [!UICONTROL Amazon Attribute Name] | 顯示[!DNL Amazon Seller Central]中定義的Amazon屬性名稱。 選取的[!DNL Commerce]屬性連結至此Amazon屬性。 您無法透過[!DNL Commerce]編輯此值。 |
| [!UICONTROL Overwrite Existing Value] | 指出Amazon屬性值是否會覆寫現有的[!DNL Commerce]值，進而影響具有此[!DNL Commerce]屬性的所有產品。<ul><li>**不覆寫現有的Magento值** - （預設）保留[!DNL Commerce]值，保留[!DNL Commerce]和Amazon存放區的不同值。</li><li>**覆寫現有的Magento值** — 儲存Amazon值超過[!DNL Commerce]產品目錄中的[!DNL Commerce]值。</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | 如果屬性是以`Global`範圍建立的，編輯屬性時不會顯示。 表示[!DNL Commerce] [領域](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings)已建立並設定為`Store View`。 |
| [!UICONTROL Store Views (to import values into to)] | 選擇要將Amazon屬性值同步至您的[!DNL Commerce] [存放區檢視](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html)。 選擇`All Store Views (Global)`會更新所有存放區檢視中的值。 |

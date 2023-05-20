---
title: 建立和編輯屬性
description: AmazonSales Channel提供「屬性」視圖，幫助您查看當前Amazon屬性和連結的Commerce屬性。
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 0%

---

# 建立和編輯屬性

建立或更新 [!DNL Commerce] 在Amazon銷售和更新商店時的屬性。 查看當前Amazon屬性並連結 [!DNL Commerce] 屬性 [_[!UICONTROL Attributes]_視圖](./attributes-view.md) Amazon銷售渠道首頁。 的_[!UICONTROL Action]_ 列顯示屬性的可用操作。 可以建立和映射新 [!DNL Commerce] 未連結的Amazon屬性的屬性，或者可以編輯現有 [!DNL Commerce] 屬性及其到Amazon屬性的映射。

在建立和更新屬性時，您可能希望驗證 [!DNL Commerce] 和Amazon產品。 如果不從Amazon同步和導入值，則這些值可能不同。 要查看這些屬性的Amazon值，請參閱 [查看Amazon屬性映射](./amazon-matching-attributes-values.md)。 如果要更改這些值，您可以 [編輯或建立映射](./amazon-manually-update-incomplete-listing.md) 在Amazon和 [!DNL Commerce]。

## 建立屬性 {#create-an-attribute}

這些步驟建立 [!DNL Commerce] 將其映射到Amazon屬性。 根據配置的不同，這些值可能會開始在目錄之間同步。

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下 **[!UICONTROL Attributes]** 在左側菜單中，找到一個Amazon屬性，然後按一下 **[!UICONTROL Create Attribute]** 的 _[!UICONTROL Action]_的雙曲餘切值。

1. 啟用將Amazon值同步到連結的 [!DNL Commerce] 屬性，設定 **[!UICONTROL Is Active]** 至 `Yes`。

   設定為時 `Yes`，值根據您的配置同步。

1. 選擇 `Create New Magento Attribute` 為 **[!UICONTROL Select Magento Product Attribute]**。

   屬性映射到所選的 **[!UICONTROL Amazon Attribute Name]**。

1. 輸入 **[!UICONTROL Magento Product Attribute Name]**。

1. 輸入 **[!UICONTROL Magento Product Attribute Code]**。

   此值必須全部為小寫，不帶空格。

1. 對於 **[!UICONTROL Attribute Set Ids]**，選擇要分配的屬性集。

   通常，屬性是屬性集的一部分，如具有藍色、綠色、黃色和紅色屬性的顏色集。

1. 對於 **[!UICONTROL Type]**，選擇屬性值的類型，如文本和數字。

   此選項影響屬性的允許值。

1. 對於 **[!UICONTROL Use for Promo Rule Conditions]**，設定為 `Yes` 允許屬性在提升條件中可用於參數。

1. 對於 **[!UICONTROL Used in Search]**，設定為 `Yes` 屬性和值是否可用於產品搜索。

1. 對於 **[!UICONTROL Comparable on Storefront]**，設定為 `Yes` 如果該屬性值可用於Amazon的「比較依據」功能。

1. 選擇 [!DNL Commerce] [範圍](https://docs.magento.com/user-guide/configuration/scope.html){target="_blank"} ，然後選擇一個或多個儲存視圖以將Amazon值導入。

   如果範圍設定為 `Global`，也請參見Wiki頁。 _[!UICONTROL Store View]_在建立屬性後無法更改。

   如果您選擇 `All Store Views (Global)`，它將同步並保存值到所有Amazon商店視圖。 您可能只想將值同步到特定儲存視圖。

1. 完成後，按一下 **[!UICONTROL Save Attribute Settings]**。

保存後，您可能希望編輯屬性以查看設定和匹配Amazon和 [!DNL Commerce] 屬性的值。 您還可以指示Amazon值是否應覆蓋 [!DNL Commerce] 值。

![建立屬性設定](assets/amazon-attribute-settings-create.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Is Active] | 指示此屬性是否為Live且在Amazon和 [!DNL Commerce]。 設定為 `Yes` 確保來自Amazon和 [!DNL Commerce] 保持與所選屬性同步。 |
| 選擇Magento產品屬性 | 指示要連結到列出的Amazon屬性名稱的選定屬性。 建立屬性時，選擇 `Create New Magento Attribute`。 |
| [!UICONTROL Amazon Attribute Name] | 顯示您選擇的Amazon屬性的名稱。 所選屬性連結到此Amazon屬性。 無法通過 [!DNL Commerce]。 |
| [!UICONTROL Magento Product Attribute Name] | 指示屬性名稱或「標籤」。 |
| [!UICONTROL Magento Product Attribute Code] | 指示屬性代碼，所有字元都用小寫字元表示，不帶空格。 |
| [!UICONTROL Attribute Set Ids] | 指示要將屬性分配給的屬性集。 屬性往往是屬性集的一部分，例如具有藍色、綠色、黃色和紅色屬性的顏色集。 |
| [!UICONTROL Type] | 指示屬性值的值類型，如文本和數字。 所選內容會影響屬性的允許值。 |
| [!UICONTROL Use for Promo Rule Conditions] | 切換到 `Yes` 允許屬性在提升條件中可用於參數。 |
| [!UICONTROL Used in Search] | 指示屬性和值是否可以用於產品搜索。 |
| [!UICONTROL Comparable on Storefront] | 指示屬性值是否可用於Amazon的「比較依據」功能。 |
| [!UICONTROL Magento Product Attribute Scope] | 指示 [範圍](https://docs.magento.com/user-guide/configuration/scope.html){target="_blank"} 的子菜單。 選項：全局/儲存視圖<br>設定為時 `Global`，在建立屬性後無法編輯「儲存視圖」。 |
| [!UICONTROL Store Views (to import values into to)] | 僅在範圍設定為時顯示 `Store View`。 選擇 [商店視圖](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} 將Amazon屬性值同步到的。 選擇 `All Store Views (Global)` 更新所有 [!DNL Commerce] 儲存視圖。 |

## 編輯屬性 {#edit-an-attribute}

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下 **[!UICONTROL Attributes]** 在左側菜單中，找到一個Amazon屬性，然後按一下 **[!UICONTROL Edit]** 的 _[!UICONTROL Action]_的雙曲餘切值。

1. 啟用或禁用將Amazon值同步到連結的 [!DNL Commerce] 屬性，設定 **活動** 至 `Yes` 或 `No`。

   設定為時 `Yes`，值根據您的配置同步。

1. 對於 **[!UICONTROL Select Magento Product Attribute]**，驗證或更新要映射到所選屬性的屬性 **[!UICONTROL Amazon Attribute Name]**。

1. 指示是否希望傳入的Amazon屬性值覆蓋現有屬性值。

   例如，您可能不想將價格從Amazon改寫為 [!DNL Commerce]。

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]**  — 保留值，保留不同的值 [!DNL Commerce] 和Amazon店。

   - **[!UICONTROL Overwrite Existing Magento Values]**  — 覆蓋 [!DNL Commerce] 具有傳入Amazon值的產品目錄。

1. 如果可編輯，請選擇一個或多個 **[!UICONTROL Store Views (to import Amazon values into)]**。

   如果屬性是使用 `Global` 範圍， _儲存視圖_ 在建立屬性後無法更改。

   如果您選擇 `All Store Views (Global)`，它將同步並保存值到所有儲存視圖。 您可能只想將值同步到特定儲存視圖。

1. 完成後，按一下 **[!UICONTROL Save Attribute Settings]**。

![編輯屬性設定](assets/amazon-attribute-settings-edit.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Is Active] | 指示此屬性是否為Live且在Amazon和 [!DNL Commerce]。 設定為 `Yes` 確保來自Amazon和 [!DNL Commerce] 保持與所選屬性同步。 |
| [!UICONTROL Select Magento Product Attribute] | 指示選定的 [!DNL Commerce] 要連結到列出的Amazon屬性名稱的屬性。 如果要更改連結 [!DNL Commerce] 屬性，從下拉清單中選擇其他屬性。 值根據配置同步。 |
| [!UICONTROL Amazon Attribute Name] | 顯示在中定義的Amazon屬性的名稱 [!DNL Amazon Seller Central]。 所選 [!DNL Commerce] 屬性指向此Amazon屬性的連結。 無法通過 [!DNL Commerce]。 |
| [!UICONTROL Overwrite Existing Value] | 指示Amazon屬性值是否覆蓋現有 [!DNL Commerce] 值，影響所有具有此值的產品 [!DNL Commerce] 屬性。<ul><li>**不覆蓋現有Magento值**  — （預設）保留 [!DNL Commerce] 值，保留不同的值 [!DNL Commerce] 和Amazon店。</li><li>**覆蓋現有Magento值**  — 節省Amazon價值超過 [!DNL Commerce] 值 [!DNL Commerce] 產品目錄。</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | 如果使用 `Global` 範圍。 指示 [!DNL Commerce] [範圍](https://docs.magento.com/user-guide/configuration/scope.html){target="_blank"} 已建立並設定為 `Store View`。 |
| [!UICONTROL Store Views (to import values into to)] | 選擇 [!DNL Commerce] [商店視圖](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} 將Amazon屬性值同步到的。 選擇 `All Store Views (Global)` 更新所有儲存視圖的值。 |

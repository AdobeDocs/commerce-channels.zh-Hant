---
title: 建立並指派Amazon銷售管道的產品
description: AmazonSales Channel提供[!UICONTROL New Third Party]索引標籤，協助建立並指派符合Amazon清單的Commerce目錄產品。
feature: Sales Channels, Products, Configuration
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# 建立及指派產品

檢視&#x200B;_[!UICONTROL New Third Party]_索引標籤時，您可以將[!DNL Commerce]目錄產品與現有的Amazon清單比對。 這個相符專案有兩個選項。 您可以將清單指定給現有的目錄產品，也可以使用清單中的資訊來建立目錄產品。 當您的Amazon清單未自動符合您的[!DNL Commerce]目錄時，這些選項會很有幫助。

您必須比對（或指派）產品與Amazon清單，才能使用Amazon sales channel的完整功能集。

從Amazon清單建立目錄產品時：

- **ASIN**&#x200B;成為[!DNL Commerce] SKU
- **產品清單名稱**&#x200B;會變成目錄清單名稱
- 已從Amazon清單匯入&#x200B;**價格**&#x200B;和&#x200B;**數量**

其餘的必要設定由您在建立期間選取的[!DNL Commerce]產品設定決定。

建立並比對後，清單會從&#x200B;_[!UICONTROL New Third Party]_索引標籤中移除，並出現在_[!UICONTROL Active]_&#x200B;索引標籤上。

## 將單一目錄產品指派給Amazon清單

1. 在[_[!UICONTROL New Third Party]_](./new-third-party-listings.md)標籤上檢視您的產品清單。

1. 尋找您要在清單中指派的清單，按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Select]**，然後按一下&#x200B;**[!UICONTROL Assign Catalog Product]**。

   此動作會開啟&#x200B;_[!UICONTROL Assign Magento Catalog Product]_頁面。

1. 使用[工作區控制項](./workspace-controls.md)來瀏覽或篩選清單，並尋找符合清單的適當目錄產品。

1. 當正確的產品出現在清單中時，請按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Assign Catalog Product]**。

您的產品和清單現在已相符。 Amazon sales channel現在可以與Amazon共用產品和清單資料，並管理您的清單及其資訊，包括清單價格、送貨價格、庫存/數量、訂單資訊和狀態等。

## 使用Amazon清單資訊建立單一目錄產品

1. 在[_[!UICONTROL New Third Party]_](./new-third-party-listings.md)標籤上檢視您的產品清單。

1. 尋找您要在[!DNL Commerce]目錄中建立的清單，按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Select]**，然後按一下&#x200B;**[!UICONTROL Create New Catalog Product]**。

   此動作會開啟&#x200B;_[!UICONTROL Create Magento Catalog Product]_頁面。

1. 完成產品的目錄設定。

   - 設定&#x200B;**[!UICONTROL Enable Product(s)]**&#x200B;切換至`Yes`或`No` （必要）。

     |是|選擇讓產品符合您[!DNL Commerce]店面銷售的資格。|
|否|選擇讓產品不符合您[!DNL Commerce]店面銷售的資格。|

   - 針對&#x200B;**[!UICONTROL Categories]**，指派產品的類別（選擇性）。

     若要選取產品的類別，請按一下向下箭頭，然後選取類別核取方塊。 完成時，請按一下&#x200B;**[!UICONTROL Done]**。

   - 針對&#x200B;**[!UICONTROL Website Ids]**，選擇要與產品相關聯的網站（店面）。

     此清單中的選項取決於您的[!DNL Commerce] [存放區組態](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html)設定。

   - 針對&#x200B;**[!UICONTROL Attribute Set Id]** （必要），請選擇選項。

     `Default`為預設選取專案。 此清單中的選項取決於您已設定的[!DNL Commerce] [屬性集](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html)。

   - 針對&#x200B;**[!UICONTROL Visibility]**，選擇新產品的選項。

     |**[!UICONTROL Not Visible Individually]** （預設）|此產品未包含在您的店面清單中，雖然它可能作為其他產品的變體提供。|
|**[!UICONTROL Catalog]**|產品會出現在您的目錄清單中。|
|**[!UICONTROL Search]**|產品可用於搜尋作業。|
|**[!UICONTROL Catalog and Search]**|產品包含在目錄清單中，可用於搜尋作業。|

   - 針對&#x200B;**[!UICONTROL Assign Tax Class]**，選擇產品的選項。

     此清單中顯示的選項取決於您所設定的[稅捐類別](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html)。

   - 完成時，按一下&#x200B;**[!UICONTROL Create Catalog Products]**。

目錄產品是在您的[!DNL Commerce]目錄中建立，並指派給從中建立它的Amazon清單。 清單現在與現有的Amazon清單相符，清單會從「_[!UICONTROL New Third Party]_」標籤中移除，並出現在「_[!UICONTROL Active]_」標籤中。

## 使用其Amazon清單資訊建立多個目錄產品

1. 在[_[!UICONTROL New Third Party]_](./new-third-party-listings.md)標籤上檢視您的產品清單。

1. 選取要為其建立目錄產品的清單。

   您可以選取左側欄中的個別核取方塊，或按一下左上欄中的向下箭頭，然後選擇&#x200B;**[!UICONTROL Select All]**&#x200B;或&#x200B;**[!UICONTROL Select All on this Page]**。

1. 在&#x200B;_[!UICONTROL Actions]_底下，按一下&#x200B;**[!UICONTROL Create New Catalog Product(s)]**。

1. 若要接受確認訊息並開啟&#x200B;_[!UICONTROL Create Magento Catalog Product]_頁面，請按一下&#x200B;**[!UICONTROL OK]**。

1. 完成產品的目錄設定。

   >[!NOTE]
   >為多個選取的清單建立目錄產品時，輸入的產品設定會套用至所有清單。

   - 設定&#x200B;**[!UICONTROL Enable Product(s)]**&#x200B;切換至`Yes`或`No` （必要）。

     |是|選擇讓產品符合您[!DNL Commerce]店面銷售的資格。|
|否|選擇讓產品不符合您[!DNL Commerce]店面銷售的資格。|

   - 針對&#x200B;**[!UICONTROL Categories]**，指派產品的類別（選擇性）。

     若要選取產品的類別，請按一下向下箭頭，然後選取類別核取方塊。 完成時，按一下&#x200B;**完成**。

   - 針對&#x200B;**[!UICONTROL Website Ids]**，選擇要與產品相關聯的網站（店面）。

     此清單中的選項取決於您的[!DNL Commerce] [存放區組態](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html)設定。

   - 針對&#x200B;**[!UICONTROL Attribute Set Id]** （必要），請選擇選項。

     `Default`為預設選取專案。 此清單中的選項取決於您已設定的[!DNL Commerce] [屬性集](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html)。

   - 針對&#x200B;**[!UICONTROL Visibility]**，選擇新產品的選項。

     |**[!UICONTROL Not Visible Individually]** （預設）|此產品未包含在您的店面清單中，雖然它可能作為其他產品的變體提供。|
|**[!UICONTROL Catalog]**|產品會出現在您的目錄清單中。|
|**[!UICONTROL Search]**|產品可用於搜尋作業。|
|**[!UICONTROL Catalog and Search]**|產品包含在目錄清單中，可用於搜尋作業。|

   - 針對&#x200B;**[!UICONTROL Assign Tax Class]**，選擇產品的選項。

     此清單中顯示的選項取決於您所設定的[稅捐類別](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html)。

   - 完成時，按一下&#x200B;**[!UICONTROL Create Catalog Products]**。

目錄產品會在您的[!DNL Commerce]目錄中建立，並指派給從中建立該目錄的Amazon清單。 清單現在與其各自的Amazon清單相符，清單會從「[_[!UICONTROL New Third Party]_](./new-third-party-listings.md)」標籤中移除，並出現在「[_[!UICONTROL Active]_](./active-listings.md)」標籤中。

![建立Commerce目錄產品](assets/amazon-magento-catalog-product.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Product(s)] | （必要）如果啟用，產品會顯示在您的[!DNL Commerce]店面中。 如果停用，產品將不會顯示在您的[!DNL Commerce]店面中。 |
| [!UICONTROL Categories] | 您可以輸入新產品的類別名稱，或按一下向下箭頭以顯示選項來選取類別。 選項取決於您的[類別](https://experienceleague.adobe.com/docs/commerce-admin/catalog/categories/create/category-create.html)設定。 |
| [!UICONTROL Website Ids] | （必要）選擇要與產品相關聯的網站（店面）。 選項取決於您的[!DNL Commerce] [存放區組態](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html)設定 |
| 屬性集ID | 選擇屬性集。 選項取決於您設定的[!DNL Commerce] [屬性集](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html)。 |
| [!UICONTROL Visibility] | 選項：<ul><li>**[!UICONTROL Not Visible Individually]** — 該產品在您的[!DNL Commerce]店面中不可見（最常見於變體產品）。</li><li>**[!UICONTROL Catalog]** — 允許透過網站中與產品相關聯的類別存取產品。</li><li>**搜尋** — 僅允許透過搜尋工具找到產品。</li><li>**[!UICONTROL Catalog and Search]** — 允許透過類別結構和使用搜尋工具來存取產品。</li></ul> |
| [!UICONTROL Assign Tax Class] | 指定新產品的稅捐類別。 選項取決於您設定的[稅捐類別](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html)。 |

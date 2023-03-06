---
title: 建立並指派產品
description: AmazonSales Channel提供 [!UICONTROL New Third Party] 標籤，以協助建立及指派具有Amazon清單的相符商務目錄產品。
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---

# 建立並指派產品

檢視時 _[!UICONTROL New Third Party]_標籤，您可以 [!DNL Commerce] 將產品目錄至現有的Amazon清單。 此比對有兩個選項。 您可以將清單指派給現有目錄產品，或使用清單中的資訊建立目錄產品。 當Amazon清單未自動符合您的 [!DNL Commerce] 目錄。

若要使用Amazon銷售管道的完整功能集，您必須將產品與Amazon清單相符（或指派）。

從Amazon清單建立目錄產品時：

- 此 **ASIN** 變成 [!DNL Commerce] SKU
- 此 **產品清單名稱** 成為目錄清單名稱
- 此 **價格** 和 **數量** 會從Amazon清單匯入

其餘必要設定由 [!DNL Commerce] 建立期間選取的產品設定。

建立並比對後，清單會從 _[!UICONTROL New Third Party]_標籤上_[!UICONTROL Active]_ 標籤。

## 將單一目錄產品指派至Amazon清單

1. 在 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 標籤。

1. 在清單中查找要指派的清單，按一下 **[!UICONTROL Select]** 在 _[!UICONTROL Action]_欄，然後按一下&#x200B;**[!UICONTROL Assign Catalog Product]**.

   此動作會開啟 _[!UICONTROL Assign Magento Catalog Product]_頁面。

1. 瀏覽或篩選清單，使用 [工作區控制項](./workspace-controls.md) 並找到與清單相符的適當目錄產品。

1. 當清單中出現正確的產品時，按一下 **[!UICONTROL Assign Catalog Product]** 在 _[!UICONTROL Action]_欄。

您的產品和清單現在已相符。 Amazon銷售管道現在可以與Amazon共用產品和清單資料，並管理您的清單及其資訊，包括清單價格、運價、存貨/數量、訂單資訊和狀態等。

## 使用Amazon清單資訊建立單一目錄產品

1. 在 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 標籤。

1. 在 [!DNL Commerce] 目錄，按一下 **[!UICONTROL Select]** 在 _[!UICONTROL Action]_欄，然後按一下&#x200B;**[!UICONTROL Create New Catalog Product]**.

   此動作會開啟 _[!UICONTROL Create Magento Catalog Product]_頁面。

1. 完成產品的目錄設定。

   - 設定 **[!UICONTROL Enable Product(s)]** 切換為 `Yes` 或 `No` （必要）。

      |是|選擇讓產品符合您的 [!DNL Commerce] 店面銷售。| |否|選擇使產品不符合您的 [!DNL Commerce] 店面銷售。|

   - 針對 **[!UICONTROL Categories]**，指派產品的類別（選用）。

      若要選取產品的類別，請按一下向下箭頭並選取類別核取方塊。 按一下 **[!UICONTROL Done]** 完成時。

   - 針對 **[!UICONTROL Website Ids]**，選擇要關聯產品的網站(storefront)。

      此清單中的選項取決於您的 [!DNL Commerce] [儲存配置](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} 設定。

   - 針對 **[!UICONTROL Attribute Set Id]** （必要），選擇選項。

      `Default` 是預設選取項目。 此清單中的選項取決於您的 [!DNL Commerce] [屬性集](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"} 您已設定。

   - 針對 **[!UICONTROL Visibility]**，選擇新產品的選項。

      |**[!UICONTROL Not Visible Individually]** （預設）|產品不包含在店面清單中，但可能作為其他產品的變體提供。| |**[!UICONTROL Catalog]**|產品將出現在目錄清單中。| |**[!UICONTROL Search]**|產品可用於搜索操作。| |**[!UICONTROL Catalog and Search]**|產品包含在目錄清單中，可用於搜索操作。|

   - 針對 **[!UICONTROL Assign Tax Class]**，請為產品選擇選項。

      此清單中顯示的選項取決於 [稅種](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"} 您已設定。

   - 完成後，按一下 **[!UICONTROL Create Catalog Products]**.

目錄產品會建立在 [!DNL Commerce] 目錄，並指派給建立該目錄的Amazon清單。 由於清單現在符合現有的Amazon清單，因此會從 _[!UICONTROL New Third Party]_標籤中_[!UICONTROL Active]_ 標籤。

## 使用其Amazon清單資訊建立多個目錄產品

1. 在 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 標籤。

1. 選擇要為其建立目錄產品的清單。

   您可以選取左側欄中的個別核取方塊，或按一下左上角欄中的向下箭頭並選擇 **[!UICONTROL Select All]** 或 **[!UICONTROL Select All on this Page]**.

1. 在 _[!UICONTROL Actions]_，按一下&#x200B;**[!UICONTROL Create New Catalog Product(s)]**.

1. 要接受確認消息並開啟 _[!UICONTROL Create Magento Catalog Product]_頁面，按一下&#x200B;**[!UICONTROL OK]**.

1. 完成產品的目錄設定。

   >[!NOTE]
   >為多個選定清單建立目錄產品時，輸入的產品設定將應用於所有清單。

   - 設定 **[!UICONTROL Enable Product(s)]** 切換為 `Yes` 或 `No` （必要）。

      |是|選擇讓產品符合您的 [!DNL Commerce] 店面銷售。| |否|選擇使產品不符合您的 [!DNL Commerce] 店面銷售。|

   - 針對 **[!UICONTROL Categories]**，指派產品的類別（選用）。

      若要選取產品的類別，請按一下向下箭頭並選取類別核取方塊。 按一下 **完成** 完成時。

   - 針對 **[!UICONTROL Website Ids]**，選擇要關聯產品的網站(storefront)。

      此清單中的選項取決於您的 [!DNL Commerce] [儲存配置](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} 設定。

   - 針對 **[!UICONTROL Attribute Set Id]** （必要），選擇選項。

      `Default` 是預設選取項目。 此清單中的選項取決於您的 [!DNL Commerce] [屬性集](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"} 您已設定。

   - 針對 **[!UICONTROL Visibility]**，選擇新產品的選項。

      |**[!UICONTROL Not Visible Individually]** （預設）|產品不包含在店面清單中，但可能作為其他產品的變體提供。| |**[!UICONTROL Catalog]**|產品將出現在目錄清單中。| |**[!UICONTROL Search]**|產品可用於搜索操作。| |**[!UICONTROL Catalog and Search]**|產品包含在目錄清單中，可用於搜索操作。|

   - 針對 **[!UICONTROL Assign Tax Class]**，請為產品選擇選項。

      此清單中顯示的選項取決於 [稅種](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"} 您已設定。

   - 完成後，按一下 **[!UICONTROL Create Catalog Products]**.

目錄產品會在 [!DNL Commerce] 目錄，並指派給建立該目錄的Amazon清單。 由於清單現在符合其各自的Amazon清單，因此會從 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 標籤中 [_[!UICONTROL Active]_](./active-listings.md) 標籤。

![建立商務目錄產品](assets/amazon-magento-catalog-product.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Enable Product(s)] | （必要）如果已啟用，產品會顯示在 [!DNL Commerce] 店面。 如果已停用，產品不會顯示在 [!DNL Commerce] 店面。 |
| [!UICONTROL Categories] | 您可以輸入新產品的類別名稱，或按一下向下箭頭以顯示選項來選取類別。 選項視您的 [類別](https://docs.magento.com/user-guide/catalog/category-create.html){target="_blank"} 設定。 |
| [!UICONTROL Website Ids] | （必要）選擇要關聯產品的網站（店面）。 選項視您的 [!DNL Commerce] [儲存配置](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} 設定 |
| 屬性集Id | 選擇屬性集。 選項視您的設定而定 [!DNL Commerce] [屬性集](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"}. |
| [!UICONTROL Visibility] | 選項：<ul><li>**[!UICONTROL Not Visible Individually]**  — 產品不會顯示在 [!DNL Commerce] storefront（變型產品最常見）。</li><li>**[!UICONTROL Catalog]**  — 允許透過與網站內相關聯的類別來存取產品。</li><li>**搜尋**  — 僅允許通過搜索工具找到產品。</li><li>**[!UICONTROL Catalog and Search]**  — 允許通過類別結構和使用搜索工具訪問產品。</li></ul> |
| [!UICONTROL Assign Tax Class] | 為新產品分配稅類。 選項視您的設定而定 [稅種](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"}. |

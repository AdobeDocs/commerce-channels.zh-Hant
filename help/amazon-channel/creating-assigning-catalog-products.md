---
title: 建立並指派產品
description: AmazonSales Channel提供[!UICONTROL New Third Party]標籤，協助建立及指派具有Amazon清單的相符商務目錄產品。
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# 建立並指派產品

檢視&#x200B;_[!UICONTROL New Third Party]_標籤時，您可以將[!DNL Commerce]目錄產品與現有的Amazon清單相符。 此比對有兩個選項。 您可以將清單指派給現有目錄產品，或使用清單中的資訊建立目錄產品。 當您的Amazon清單未自動符合您的[!DNL Commerce]目錄時，這些選項很實用。

若要使用Amazon銷售管道的完整功能集，您必須將產品與Amazon清單相符（或指派）。

從Amazon清單建立目錄產品時：

- **ASIN**&#x200B;會變成[!DNL Commerce] SKU
- **產品清單名稱**&#x200B;變為目錄清單名稱
- **Price**&#x200B;和&#x200B;**Quantity**&#x200B;是從Amazon清單匯入

其餘的必要設定由您在建立期間選取的[!DNL Commerce]產品設定決定。

建立並匹配清單後，清單將從&#x200B;_[!UICONTROL New Third Party]_頁簽中刪除，並顯示在_[!UICONTROL Active]_&#x200B;頁簽上。

## 將單一目錄產品指派至Amazon清單

1. 在[_[!UICONTROL New Third Party]_](./new-third-party-listings.md)標籤上檢視您的產品清單。

1. 在清單中查找要分配的清單，按一下&#x200B;_[!UICONTROL Action]_列中的&#x200B;**[!UICONTROL Select]**，然後按一下&#x200B;**[!UICONTROL Assign Catalog Product]**。

   此動作會開啟&#x200B;_[!UICONTROL Assign Magento Catalog Product]_頁面。

1. 使用[workspace控制項](./workspace-controls.md)瀏覽或篩選清單，然後找到與清單相符的適當目錄產品。

1. 當清單中出現正確的產品時，按一下&#x200B;_[!UICONTROL Action]_列中的&#x200B;**[!UICONTROL Assign Catalog Product]**。

您的產品和清單現在已相符。 Amazon銷售管道現在可以與Amazon共用產品和清單資料，並管理您的清單及其資訊，包括清單價格、運價、存貨/數量、訂單資訊和狀態等。

## 使用Amazon清單資訊建立單一目錄產品

1. 在[_[!UICONTROL New Third Party]_](./new-third-party-listings.md)標籤上檢視您的產品清單。

1. 在[!DNL Commerce]目錄中查找要建立的清單，按一下&#x200B;_[!UICONTROL Action]_列中的&#x200B;**[!UICONTROL Select]**，然後按一下&#x200B;**[!UICONTROL Create New Catalog Product]**。

   此動作會開啟&#x200B;_[!UICONTROL Create Magento Catalog Product]_頁面。

1. 完成產品的目錄設定。

   - 將&#x200B;**[!UICONTROL Enable Product(s)]**&#x200B;切換為`Yes`或`No`（必要）。

      |是|選擇使產品符合[!DNL Commerce]店面銷售的條件。|
|否|選擇使產品不符合您的[!DNL Commerce]店面銷售。|

   - 對於&#x200B;**[!UICONTROL Categories]**，為產品指派類別（可選）。

      若要選取產品的類別，請按一下向下箭頭並選取類別核取方塊。 完成後，按一下&#x200B;**[!UICONTROL Done]**。

   - 對於&#x200B;**[!UICONTROL Website Ids]**，選擇要關聯產品的網站（店面）。

      此清單中的選項取決於您的[!DNL Commerce] [儲存配置](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}設定。

   - 對於&#x200B;**[!UICONTROL Attribute Set Id]**（必要），選擇一個選項。

      `Default` 是預設選取項目。此清單中的選項取決於您已配置的[!DNL Commerce] [屬性集](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;}。

   - 對於&#x200B;**[!UICONTROL Visibility]**，選擇新產品的選項。

      |**[!UICONTROL Not Visible Individually]**（預設值）|產品未包含在店面清單中，但可能作為其他產品的變體提供。|
|**[!UICONTROL Catalog]**|產品會出現在目錄清單中。|
|**[!UICONTROL Search]**|產品可用於搜索操作。|
|**[!UICONTROL Catalog and Search]**|產品包含在目錄清單中，可用於搜索操作。|

   - 對於&#x200B;**[!UICONTROL Assign Tax Class]**，選擇產品的選項。

      此清單中顯示的選項取決於您配置的[稅類](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;}。

   - 完成後，按一下&#x200B;**[!UICONTROL Create Catalog Products]**。

目錄產品會在您的[!DNL Commerce]目錄中建立，並指派給建立該產品的Amazon清單。 由於清單現在與現有的Amazon清單相符，該清單將從&#x200B;_[!UICONTROL New Third Party]_標籤中移除，並顯示在_[!UICONTROL Active]_&#x200B;標籤中。

## 使用其Amazon清單資訊建立多個目錄產品

1. 在[_[!UICONTROL New Third Party]_](./new-third-party-listings.md)標籤上檢視您的產品清單。

1. 選擇要為其建立目錄產品的清單。

   您可以選取左側欄中的個別核取方塊，或按一下左上角欄中的向下箭頭，然後選擇&#x200B;**[!UICONTROL Select All]**&#x200B;或&#x200B;**[!UICONTROL Select All on this Page]**。

1. 在&#x200B;_[!UICONTROL Actions]_下，按一下&#x200B;**[!UICONTROL Create New Catalog Product(s)]**。

1. 要接受確認消息並開啟&#x200B;_[!UICONTROL Create Magento Catalog Product]_頁，請按一下&#x200B;**[!UICONTROL OK]**。

1. 完成產品的目錄設定。

   >[!NOTE]
   >為多個選定清單建立目錄產品時，輸入的產品設定將應用於所有清單。

   - 將&#x200B;**[!UICONTROL Enable Product(s)]**&#x200B;切換為`Yes`或`No`（必要）。

      |是|選擇使產品符合[!DNL Commerce]店面銷售的條件。|
|否|選擇使產品不符合您的[!DNL Commerce]店面銷售。|

   - 對於&#x200B;**[!UICONTROL Categories]**，為產品指派類別（可選）。

      若要選取產品的類別，請按一下向下箭頭並選取類別核取方塊。 完成後，按一下&#x200B;**Done**。

   - 對於&#x200B;**[!UICONTROL Website Ids]**，選擇要關聯產品的網站（店面）。

      此清單中的選項取決於您的[!DNL Commerce] [儲存配置](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}設定。

   - 對於&#x200B;**[!UICONTROL Attribute Set Id]**（必要），選擇一個選項。

      `Default` 是預設選取項目。此清單中的選項取決於您已配置的[!DNL Commerce] [屬性集](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;}。

   - 對於&#x200B;**[!UICONTROL Visibility]**，選擇新產品的選項。

      |**[!UICONTROL Not Visible Individually]**（預設值）|產品未包含在店面清單中，但可能作為其他產品的變體提供。|
|**[!UICONTROL Catalog]**|產品會出現在目錄清單中。|
|**[!UICONTROL Search]**|產品可用於搜索操作。|
|**[!UICONTROL Catalog and Search]**|產品包含在目錄清單中，可用於搜索操作。|

   - 對於&#x200B;**[!UICONTROL Assign Tax Class]**，選擇產品的選項。

      此清單中顯示的選項取決於您配置的[稅類](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;}。

   - 完成後，按一下&#x200B;**[!UICONTROL Create Catalog Products]**。

目錄產品會在您的[!DNL Commerce]目錄中建立，並指派給建立該產品的Amazon清單。 如果清單現在符合其各自的Amazon清單，則會從[_[!UICONTROL New Third Party]_](./new-third-party-listings.md)標籤中移除清單，並顯示在[_[!UICONTROL Active]_](./active-listings.md)標籤中。

![建立商務目錄產品](assets/amazon-magento-catalog-product.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Enable Product(s)] | （必要）如果已啟用，產品會顯示在您的[!DNL Commerce]店面中。 如果禁用，[!DNL Commerce]店面中不會顯示產品。 |
| [!UICONTROL Categories] | 您可以輸入新產品的類別名稱，或按一下向下箭頭以顯示選項來選取類別。 選項取決於您的[categories](https://docs.magento.com/user-guide/catalog/category-create.html){target=&quot;_blank&quot;}配置。 |
| [!UICONTROL Website Ids] | （必要）選擇要關聯產品的網站（店面）。 選項取決於您的[!DNL Commerce] [儲存配置](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}設定 |
| 屬性集Id | 選擇屬性集。 選項取決於您配置的[!DNL Commerce] [屬性集](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;}。 |
| [!UICONTROL Visibility] | 選項：<ul><li>**[!UICONTROL Not Visible Individually]**  — 您的店面中看不到產 [!DNL Commerce] 品（變型產品最常見）。</li><li>**[!UICONTROL Catalog]**  — 允許透過與網站內相關聯的類別來存取產品。</li><li>**搜尋**  — 僅允許透過搜尋工具找到產品。</li><li>**[!UICONTROL Catalog and Search]**  — 允許通過類別結構和使用搜索工具訪問產品。</li></ul> |
| [!UICONTROL Assign Tax Class] | 為新產品分配稅類。 選項取決於您配置的[稅類](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;}。 |

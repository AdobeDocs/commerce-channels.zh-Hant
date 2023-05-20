---
title: 建立和分配產品
description: AmazonSales Channel提供 [!UICONTROL New Third Party] 頁籤，幫助建立和分配具有Amazon清單的匹配Commerce目錄產品。
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---

# 建立和分配產品

查看 _[!UICONTROL New Third Party]_頁籤 [!DNL Commerce] 將產品目錄列入Amazon現有清單。 此匹配有兩個選項。 您可以將清單分配給現有目錄產品，或者使用清單中的資訊建立目錄產品。 當您的Amazon清單與您的清單不自動匹配時，這些選項很有幫助 [!DNL Commerce] 目錄。

要使用Amazon銷售渠道的完整功能集，必須將您的產品與Amazon清單匹配（或分配）。

從Amazon清單建立目錄產品時：

- 的 **阿辛** 變成 [!DNL Commerce] SKU
- 的 **產品清單名稱** 成為目錄清單名稱
- 的 **價格** 和 **數量** 是從Amazon上市

其餘必要設定由 [!DNL Commerce] 在建立過程中選擇的產品設定。

建立和匹配時，清單將從 _[!UICONTROL New Third Party]_的子菜單。_[!UICONTROL Active]_ 頁籤。

## 將單個目錄產品分配給Amazon清單

1. 查看您的產品清單 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 頁籤。

1. 查找要在清單中分配的清單，按一下 **[!UICONTROL Select]** 的 _[!UICONTROL Action]_，然後按一下&#x200B;**[!UICONTROL Assign Catalog Product]**。

   此操作將開啟 _[!UICONTROL Assign Magento Catalog Product]_的子菜單。

1. 使用 [工作區控制項](./workspace-controls.md) 並找到與清單匹配的適當目錄產品。

1. 當清單中出現正確的產品時，按一下 **[!UICONTROL Assign Catalog Product]** 的 _[!UICONTROL Action]_的雙曲餘切值。

您的產品和清單現在已匹配。 Amazon銷售渠道現在可以與Amazon共用產品和上市資料，並管理您的上市及其資訊，包括上市價格、發運價格、庫存/數量、訂單資訊和狀態等。

## 使用Amazon清單資訊建立單個目錄產品

1. 查看您的產品清單 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 頁籤。

1. 查找要在中建立的清單 [!DNL Commerce] 目錄，按一下 **[!UICONTROL Select]** 的 _[!UICONTROL Action]_，然後按一下&#x200B;**[!UICONTROL Create New Catalog Product]**。

   此操作將開啟 _[!UICONTROL Create Magento Catalog Product]_的子菜單。

1. 完成產品的目錄設定。

   - 設定 **[!UICONTROL Enable Product(s)]** 切換至 `Yes` 或 `No` （必需）。

      |是|選擇使產品符合您的條件 [!DNL Commerce] 店面銷售。| |否|選擇使產品不適合您的 [!DNL Commerce] 店面銷售。|

   - 對於 **[!UICONTROL Categories]**，為產品分配類別（可選）。

      要選擇產品的類別，請按一下向下箭頭並選中類別複選框。 按一下 **[!UICONTROL Done]** 的子菜單。

   - 對於 **[!UICONTROL Website Ids]**，選擇要關聯產品的網站（商店）。

      此清單中的選項取決於 [!DNL Commerce] [儲存配置](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} 的子菜單。

   - 對於 **[!UICONTROL Attribute Set Id]** （必需），選擇選項。

      `Default` 選項。 此清單中的選項取決於 [!DNL Commerce] [屬性集](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"} 已配置。

   - 對於 **[!UICONTROL Visibility]**，則選擇新產品的選項。

      |**[!UICONTROL Not Visible Individually]** （預設）|該產品不包括在您的店面清單中，儘管它可能是其他產品的變體。| |**[!UICONTROL Catalog]**|產品將出現在目錄清單中。| |**[!UICONTROL Search]**|產品可用於搜索操作。| |**[!UICONTROL Catalog and Search]**|產品包含在目錄清單中，可用於搜索操作。|

   - 對於 **[!UICONTROL Assign Tax Class]**，請選擇

      此清單中顯示的選項取決於 [稅類](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"} 已配置。

   - 完成後，按一下 **[!UICONTROL Create Catalog Products]**。

目錄產品是在 [!DNL Commerce] 目錄，並分配給建立該目錄的Amazon清單。 由於該上市目前與Amazon現有上市相符，因此該上市將從 _[!UICONTROL New Third Party]_的子菜單。_[!UICONTROL Active]_ 頁籤。

## 使用其Amazon清單資訊建立多個目錄產品

1. 查看您的產品清單 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 頁籤。

1. 選擇要為其建立目錄產品的清單。

   可以在左側列中選擇單個複選框，或者按一下左上列中的向下箭頭，然後選擇 **[!UICONTROL Select All]** 或 **[!UICONTROL Select All on this Page]**。

1. 下 _[!UICONTROL Actions]_按一下&#x200B;**[!UICONTROL Create New Catalog Product(s)]**。

1. 接受確認消息並開啟 _[!UICONTROL Create Magento Catalog Product]_的&#x200B;**[!UICONTROL OK]**。

1. 完成產品的目錄設定。

   >[!NOTE]
   >為多個選定清單建立目錄產品時，輸入的產品設定將應用於所有清單。

   - 設定 **[!UICONTROL Enable Product(s)]** 切換至 `Yes` 或 `No` （必需）。

      |是|選擇使產品符合您的條件 [!DNL Commerce] 店面銷售。| |否|選擇使產品不適合您的 [!DNL Commerce] 店面銷售。|

   - 對於 **[!UICONTROL Categories]**，為產品分配類別（可選）。

      要選擇產品的類別，請按一下向下箭頭並選中類別複選框。 按一下 **完成** 的子菜單。

   - 對於 **[!UICONTROL Website Ids]**，選擇要關聯產品的網站（商店）。

      此清單中的選項取決於 [!DNL Commerce] [儲存配置](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} 的子菜單。

   - 對於 **[!UICONTROL Attribute Set Id]** （必需），選擇選項。

      `Default` 選項。 此清單中的選項取決於 [!DNL Commerce] [屬性集](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"} 已配置。

   - 對於 **[!UICONTROL Visibility]**，則選擇新產品的選項。

      |**[!UICONTROL Not Visible Individually]** （預設）|該產品不包括在您的店面清單中，儘管它可能是其他產品的變體。| |**[!UICONTROL Catalog]**|產品將出現在目錄清單中。| |**[!UICONTROL Search]**|產品可用於搜索操作。| |**[!UICONTROL Catalog and Search]**|產品包含在目錄清單中，可用於搜索操作。|

   - 對於 **[!UICONTROL Assign Tax Class]**，請選擇

      此清單中顯示的選項取決於 [稅類](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"} 已配置。

   - 完成後，按一下 **[!UICONTROL Create Catalog Products]**。

目錄產品是在 [!DNL Commerce] 目錄，並分配給建立該目錄的Amazon清單。 由於這些上市目前與它們各自的Amazon上市目錄相匹配，這些上市將從 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 的子菜單。 [_[!UICONTROL Active]_](./active-listings.md) 頁籤。

![建立Commerce目錄產品](assets/amazon-magento-catalog-product.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Enable Product(s)] | （必需）如果啟用，則產品在 [!DNL Commerce] 店面。 如果禁用，則產品不會顯示在 [!DNL Commerce] 店面。 |
| [!UICONTROL Categories] | 您可以輸入新產品的類別名稱，或通過按一下向下箭頭顯示選項來選擇類別。 選項取決於 [類別](https://docs.magento.com/user-guide/catalog/category-create.html){target="_blank"} 配置。 |
| [!UICONTROL Website Ids] | （必需）選擇要關聯產品的網站（店面）。 選項取決於 [!DNL Commerce] [儲存配置](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} 設定 |
| 屬性集ID | 選擇屬性集。 選項取決於您的配置 [!DNL Commerce] [屬性集](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"}。 |
| [!UICONTROL Visibility] | 選項：<ul><li>**[!UICONTROL Not Visible Individually]**  — 產品在您的 [!DNL Commerce] storefront（變型產品最常見）。</li><li>**[!UICONTROL Catalog]**  — 允許通過網站中與其關聯的類別訪問產品。</li><li>**搜索**  — 僅允許通過搜索工具找到產品。</li><li>**[!UICONTROL Catalog and Search]**  — 允許通過類別結構和使用搜索工具訪問產品。</li></ul> |
| [!UICONTROL Assign Tax Class] | 為新產品分配稅分類。 選項取決於您的配置 [稅類](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"}。 |

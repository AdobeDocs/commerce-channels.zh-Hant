---
title: 產品清單操作
description: 使用「產品清單操作」設定定義您的Commerce目錄如何與Amazon交互。
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# 產品清單操作

產品清單操作設定是您的商店清單設定的一部分。 從 [儲存儀表板](./amazon-store-dashboard.md)。

這些設定定義目錄與Amazon的交互方式。 這些設定：

- 指示 [!DNL Commerce] 符合Amazon資格要求的目錄產品自動發送到您 [!DNL Amazon Seller Central] 帳戶以建立清單。

- 設定訂單的預設處理時間。 此值定義處理和發運訂單所需的天數。 例如，如果某人選擇了2天發運，則在處理完成並將包交給承運人之前，不會開始發運中轉時間。 總交貨時間為（處理時間+過境時間+任何節假日）。

## 配置設定

1. 按一下 **[!UICONTROL Listing Settings]** 在商店儀表板上。

1. 展開 _[!UICONTROL Product Listing Actions]_的子菜單。

1. 對於 **[!UICONTROL Automatic List Action]** （必需），選擇選項：

   - `Automatically List Eligible Products`  — （預設）選擇您希望的時間 [!DNL Commerce] 目錄產品(符合Amazon的資格要求)自動發佈到Amazon並建立Amazon清單。

   - `Do Not Automatically List Eligible Products`  — 選擇要人工選擇符合條件的時間 [!DNL Commerce] 對產品進行編目並建立Amazon清單。 選擇時，符合清單條件並包含所有必需資訊的目錄產品將顯示在 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 頁籤，以手動發佈到Amazon。

1. 對於 **[!UICONTROL Default Handling Time]** （必需），輸入裝運前提前期所需的天數。

   預設值為 `2` 天。

   >[!NOTE]
   >
   >此預設交付時間值僅對通過Amazon銷售渠道建立的Amazon清單有效。 在您 [!DNL Amazon Seller Central] 帳戶使用在Amazon設定的預設處理時間。

1. 完成後，按一下 **[!UICONTROL Save listing settings]**。

![產品清單操作](assets/amazon-product-listing-actions.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Automatic List Action] | 選項：<ul><li>**[!UICONTROL Automatically List Eligible Products]**  — （推薦）選擇您希望的時間 [!DNL Commerce] 目錄產品(符合Amazon的資格要求)自動發佈到Amazon並建立Amazon清單。 選擇後， [_[!UICONTROL Ready to List]_](./ready-to-list.md) 頁籤。 </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]**  — 選擇要人工選擇合格的時間 [!DNL Commerce] 編錄產品並建立Amazon清單。 選擇時，符合清單條件並包含所有必需資訊的目錄產品將顯示在 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 頁籤。</li></ul> |
| [!UICONTROL Default Handling Time] | 通常表示處理和發運訂單所需天數的數值。 預設值為 `2`。 此值用於在中建立的Amazon清單 [!DNL Commerce] 出版給Amazon。 與整合前Amazon清單的預設處理時間 [!DNL Commerce] 不受此設定的影響。<br><br>在Amazon銷售渠道中定義的值不會替換現有Amazon清單中定義的預設處理時間。 當 **[!UICONTROL Handling Time Override]** 啟用並刪除，訂單的處理時間將恢復為此處定義的值。<br><br>如果您的產品具有不同的處理時間，則可以在特定於產品的層建立「處理時間改寫」。 您可以在 [_[!UICONTROL Overrides]_](./overrides.md) 頁籤，讓您能夠靈活地管理產品履行。 如果中沒有處理時間覆蓋 [!DNL Commerce] 對於產品，處理時間預設值是在Amazon清單中定義的值。<br><br>處理時間是區域屬性。 當更改清單的值時，該更改將影響共用 [!DNL Amazon Seller SKU] 在Amazon所有店鋪中 [儲存整合](./store-integration.md))。 但是，更改共用的值 [!DNL Amazon Seller SKU] 區域，不會影響在具有不同定義區域的商店中列出的相同產品。 建立日期最早的區域的儲存控制「預設處理時間」設定的優先順序。 |

**快速訪問** - [!UICONTROL Listing Settings] 節

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

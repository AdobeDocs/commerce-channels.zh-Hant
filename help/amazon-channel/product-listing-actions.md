---
title: Amazon sales channel — 產品清單動作
description: 使用產品清單動作設定來定義您的Commerce目錄與Amazon的互動方式。
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# 產品清單動作

產品清單動作設定是商店清單設定的一部分。 清單設定可從以下位置存取： [存放區儀表板](./amazon-store-dashboard.md).

這些設定會定義您的目錄與Amazon的互動方式。 這些設定：

- 顯示您的 [!DNL Commerce] 符合Amazon資格要求的目錄產品會自動傳送至您的 [!DNL Amazon Seller Central] 帳戶以建立清單。

- 設定訂單的預設處理時間。 此值會定義處理及出貨訂單所需的天數。 例如，若有人選取2天出貨，則在處理完成並將包裹遞送至承運商之前，該出貨運送時間不會開始。 總交貨時間為（處理時間+運輸時間+任何假日）。

## 設定設定

1. 按一下 **[!UICONTROL Listing Settings]** 在商店控制面板上。

1. 展開 _[!UICONTROL Product Listing Actions]_區段。

1. 的 **[!UICONTROL Automatic List Action]** （必要），選擇一個選項：

   - `Automatically List Eligible Products` - （預設）選擇您想要的 [!DNL Commerce] 目錄產品(符合Amazon的資格要求)以自動發佈至Amazon並建立Amazon清單。

   - `Do Not Automatically List Eligible Products`  — 選擇您要手動選取合適專案的時間 [!DNL Commerce] 將產品編目，並建立Amazon清單。 選擇後，符合清單條件並包含所有必要資訊的產品目錄會顯示在 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 以手動方式發佈至Amazon的標籤。

1. 的 **[!UICONTROL Default Handling Time]** （必要），輸入出貨前前置時間所需的天數。

   預設值為 `2` 天。

   >[!NOTE]
   >
   >此預設處理時間值僅適用於透過Amazon銷售管道建立的Amazon清單。 已在您的中建立的任何Amazon清單 [!DNL Amazon Seller Central] 帳戶使用Amazon中設定的預設處理時間。

1. 完成後，按一下 **[!UICONTROL Save listing settings]**.

![產品清單動作](assets/amazon-product-listing-actions.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Automatic List Action] | 選項：<ul><li>**[!UICONTROL Automatically List Eligible Products]** - （建議）選擇您想要的 [!DNL Commerce] 目錄產品(符合Amazon的資格要求)以自動發佈至Amazon並建立Amazon清單。 選擇後， [_[!UICONTROL Ready to List]_](./ready-to-list.md) 索引標籤未顯示。 </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]**  — 選擇您要手動選取合適專案的時間 [!DNL Commerce] 將產品編目並建立Amazon清單。 選擇後，符合清單條件並包含所有必要資訊的產品目錄會顯示在 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 標籤以供手動發佈。</li></ul> |
| [!UICONTROL Default Handling Time] | 通常代表處理及出貨訂單所需的天數。 預設值為 `2`. 此值用於在中建立的Amazon清單 [!DNL Commerce] 並發佈至Amazon。 與整合之前Amazon清單的預設處理時間 [!DNL Commerce] 不受此設定影響。<br><br>Amazon sales channel中定義的值不會取代現有Amazon清單中定義的預設處理時間。 當 **[!UICONTROL Handling Time Override]** 啟用後移除，訂單的處理時間會恢復為此處定義的值。<br><br>如果您的產品具有不同的處理時間，則可以在產品特定層級建立「處理時間覆寫」 。 您可在以下位置管理處理時間覆寫： [_[!UICONTROL Overrides]_](./overrides.md) 索引標籤，讓您能夠靈活地管理產品履行。 如果中沒有處理時間覆寫 [!DNL Commerce] 對於產品，處理時間預設為Amazon清單中定義的值。<br><br>處理時間是地區屬性。 當清單的值變更時，變更會影響所有共用清單的清單 [!DNL Amazon Seller SKU] 在相同區域的所有Amazon存放區中(定義於 [存放區整合](./store-integration.md))。 但是，變更共用的值 [!DNL Amazon Seller SKU] 在北美地區，對於列於不同地區商店的相同產品不會造成影響。 建立日期最早的區域存放區會控制「預設處理時間」設定的優先順序。 |

**快速存取** - [!UICONTROL Listing Settings] 區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

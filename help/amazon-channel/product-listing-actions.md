---
title: 產品清單動作
description: 使用產品清單動作設定來定義您的商務目錄與Amazon的互動方式。
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# 產品清單動作

產品清單動作設定是您商店清單設定的一部分。 清單設定可從 [儲存儀表板](./amazon-store-dashboard.md).

這些設定可定義目錄與Amazon的互動方式。 這些設定：

- 指出 [!DNL Commerce] 符合Amazon資格要求的目錄產品會自動傳送至您的 [!DNL Amazon Seller Central] 帳戶以建立清單。

- 設定訂單的預設處理時間。 此值定義了處理和發運訂單所需的天數。 例如，如果某人選擇2天發運，則在處理完成並將包交給承運人之前，發運過境時間不會開始。 總交貨時間為（處理時間+過境時間+任何假日）。

## 配置設定

1. 按一下 **[!UICONTROL Listing Settings]** 在商店控制面板上。

1. 展開 _[!UICONTROL Product Listing Actions]_區段。

1. 針對 **[!UICONTROL Automatic List Action]** （必要），選擇選項：

   - `Automatically List Eligible Products`  — （預設）選擇您想要的時間 [!DNL Commerce] 目錄產品(符合Amazon的資格要求)以自動發佈至Amazon並建立Amazon清單。

   - `Do Not Automatically List Eligible Products`  — 選擇您想要手動選取符合資格的 [!DNL Commerce] 編錄產品並建立Amazon清單。 選擇後，將符合清單條件且包含所有必要資訊的產品目錄顯示在 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 標籤，以手動發佈至Amazon。

1. 針對 **[!UICONTROL Default Handling Time]** （必要），輸入發運前提前期所需的天數。

   預設值為 `2` 天。

   >[!NOTE]
   >
   >此預設處理時間值僅對透過Amazon銷售管道建立的Amazon清單有效。 在 [!DNL Amazon Seller Central] 帳戶會使用Amazon中設定的預設處理時間。

1. 完成後，按一下 **[!UICONTROL Save listing settings]**.

![產品清單動作](assets/amazon-product-listing-actions.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Automatic List Action] | 選項：<ul><li>**[!UICONTROL Automatically List Eligible Products]**  — （建議）選擇您想要的時間 [!DNL Commerce] 目錄產品(符合Amazon的資格要求)以自動發佈至Amazon並建立Amazon清單。 選擇後， [_[!UICONTROL Ready to List]_](./ready-to-list.md) 標籤。 </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]**  — 選擇何時手動選擇合格 [!DNL Commerce] 編錄產品並建立Amazon清單。 選擇後，將符合清單條件且包含所有必要資訊的產品目錄顯示在 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 標籤進行手動發佈。</li></ul> |
| [!UICONTROL Default Handling Time] | 表示訂單處理和發運所需天數的數值。 預設值為 `2`. 此值適用於中建立的Amazon清單 [!DNL Commerce] 並發佈至Amazon。 Amazon清單的預設處理時間，再與整合 [!DNL Commerce] 不受此設定影響。<br><br>在Amazon銷售管道中定義的值不會取代現有Amazon清單中定義的預設處理時間。 當 **[!UICONTROL Handling Time Override]** 啟用後移除，訂單的處理時間會回復為此處定義的值。<br><br>如果您的產品具有不同的處理時間，則可以在產品特定層建立「處理時間覆蓋」。 您可以在 [_[!UICONTROL Overrides]_](./overrides.md) 頁簽，讓您有彈性管理產品履行。 如果中沒有處理時間覆蓋 [!DNL Commerce] 對於產品，處理時間預設值是Amazon清單中定義的值。<br><br>「處理時間」是區域屬性。 當清單的值變更時，此變更會影響共用 [!DNL Amazon Seller SKU] 位於存在於相同地區的所有Amazon商店(定義於 [商店整合](./store-integration.md))。 不過，會變更共用的值 [!DNL Amazon Seller SKU] 在北美地區，不會影響所列位於不同地區商店的相同產品。 建立日期最久的區域的儲存控制「預設處理時間」設定的優先順序。 |

**快速存取** - [!UICONTROL Listing Settings] 區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

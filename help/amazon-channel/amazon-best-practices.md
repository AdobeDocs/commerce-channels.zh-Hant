---
title: 的最佳實務和限制 [!DNL Amazon sales channel]
description: 檢閱針對Adobe Commerce和Magento Open Source使用Amazon銷售管道時的最佳實務和限制。
role: Leader, Admin, User
feature: Sales Channels, Best Practices
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 的最佳實務和限制 [!DNL Amazon sales channel]

最佳實務包括：

- Amazon sales channel可以透過提高或降低價格、同步化產品資訊（包括可用存貨），以及新增、更新和結束（刪除）清單來影響您的Amazon清單。 在設定期間依狀態檢閱您的清單，並調整您的設定([清單設定](./listing-settings.md)， [清單規則](./listing-rules.md)， [pricing rules （定價規則）](./pricing-products.md)， [覆寫](./overrides.md)、等等)之後再完成商店設定。 您也可以在設定後，視需要修改這些設定。

- Amazon sales channel可以設定您的定價規則，以自動調整您的掛牌價格。 自動化定價保障包括 [底價](./floor-price.md) 和 [選擇性最高價格](./optional-ceiling-price.md) 的功能 [智慧型重新訂價規則](./intelligent-repricing-rules.md). 使用這些保障措施，可確保您的上市價格不會低於成本或高於定義的價格。

- Amazon Sales Channel與Amazon之間的資料同步由您的控制 [[!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) 設定。 內建節流，介於 [!DNL Commerce] Amazon可協助確保順暢且有效率的資料傳輸，但在電子商務流量旺盛期間（例如黑色星期五），Amazon的系統更新時間可能會比平常更長。 設定您的 [!DNL Commerce] cron每五分鐘執行一次。

- Amazon sales channel會匯入您的Amazon訂單資訊。 若要在Amazon銷售管道中管理您的Amazon訂單，您必須確保 [訂單設定](./order-settings.md) 定義來匯入並建立對應的 [!DNL Commerce] 每個Amazon訂單的訂單。 如果未定義，則只能檢視您的Amazon訂單資訊。 所有透過Amazon的銷售稅捐，仍透過您的管理及匯出。 [!DNL Amazon Seller Central] 帳戶。 某些州會要求Amazon自動徵收及匯出稅金。 若為其他州，則賣方可選擇手動或自動計算稅捐。 另請參閱 [Amazon：稅務政策](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target="_blank"}. 您可能需要登入 [!DNL Amazon Seller Central] 用於檢視Amazon稅務政策檔案的帳戶。

- 針對英國地區，最佳作法是註冊 [Amazon VAT計算服務](https://sell.amazon.co.uk/learn/vat-resources/){target="_blank"} 上線Amazon sales channel之前。

  >[!NOTE]
  >
  >Amazon可能需要10到14天的時間來驗證及啟用您的VAT計算服務帳戶。

限制包括：

- 屬於您的套裝、禮品卡及分組產品型別 [!DNL Commerce] Amazon sales channel不支援將目錄列為Amazon。

- Amazon sales channel無法為沒有現有或先前Amazon清單的產品建立清單。 如果中不存在產品 [!DNL Amazon Seller Central] 若使用ASIN，則必須將其新增至 [!DNL Amazon Seller Central] 以便Amazon能夠將產品指派給ASIN。 在Amazon中新增產品並建立清單後，該清單即可與Amazon銷售管道中的目錄比對並同步。

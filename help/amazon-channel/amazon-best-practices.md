---
title: Amazon銷售管道的最佳作法和限制
description: 檢閱使用適用於Adobe Commerce和Magento Open Source的Amazon銷售管道時的最佳作法和限制。
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Amazon銷售管道的最佳作法和限制

最佳實務包括：

- Amazon銷售管道可能會因下列原因影響您的Amazon清單：提高或降低價格、同步產品資訊（包括可用庫存），以及新增、更新和結束（刪除）清單。 在設定期間依狀態檢閱清單，並調整設定([清單設定](./listing-settings.md), [清單規則](./listing-rules.md), [定價規則](./pricing-products.md), [覆寫](./overrides.md)等)，再完成商店設定。 您也可以視需要在設定後修改這些設定。

- Amazon銷售管道可設定您的定價規則，以自動調整您的上市價格。 自動定價保障包括 [底價](./floor-price.md) 和 [可選上限價格](./optional-ceiling-price.md) 功能 [智慧重新定價規則](./intelligent-repricing-rules.md). 使用這些保障措施有助於確保您的上市價格不會低於成本或高於定義的價格。

- Amazon銷售管道與Amazon之間的資料同步由 [[!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}設定。 內置節流 [!DNL Commerce] 而Amazon有助於確保資料傳輸順暢且高效，但在高電子商務流量時間（如黑色星期五）,Amazon的系統更新可能需要比平常更長的時間。 設定您的 [!DNL Commerce] cron每五分鐘運行一次。

- Amazon銷售管道會匯入您的Amazon訂單資訊。 若要在Amazon銷售管道中管理Amazon訂單，您必須確保 [順序設定](./order-settings.md) 定義來匯入和建立對應的 [!DNL Commerce] 每筆Amazon訂單的訂單。 如果未定義，則您只能檢視Amazon訂單資訊。 所有透過Amazon銷售的稅款仍透過 [!DNL Amazon Seller Central] 帳戶。 在一些州，Amazon需要自動收稅和繳稅。 對於其他州，賣方可以選擇手動或自動計算稅。 請參閱 [Amazon:稅收政策](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target=&quot;_blank&quot;}。 您可能需要登入 [!DNL Amazon Seller Central] 帳戶以檢視Amazon稅務政策檔案。

- 對於英國地區，最佳做法是註冊 [Amazon增值稅計算服務](https://sell.amazon.co.uk/learn/vat-resources/){target=&quot;_blank&quot;}，再開始使用Amazon銷售管道。


   >[!NOTE]
   >
   >Amazon可能需要10到14天的時間來驗證和啟用您的增值稅計算服務帳戶。

限制包括：

- 捆綁包、禮品卡和屬於您 [!DNL Commerce] Amazon銷售管道不支援目錄，因此無法列入Amazon。

- Amazon銷售管道無法為沒有現有或先前Amazon清單的產品建立清單。 如果產品不存在於 [!DNL Amazon Seller Central] 若使用ASIN，則必須將其新增至 [!DNL Amazon Seller Central] 以便Amazon能將產品指派一個ASIN。 在Amazon中新增產品並建立清單後，清單便可與Amazon銷售管道中的目錄相符並同步。

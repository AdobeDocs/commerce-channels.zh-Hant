---
title: Amazon銷售管道的最佳作法和限制
description: 針對Adobe商務和Magento Open Source使用Amazon銷售管道時，請檢閱最佳作法和限制。
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Amazon銷售管道的最佳作法和限制

最佳實務包括：

- Amazon銷售管道可能會因下列原因影響您的Amazon清單：提高或降低價格、同步產品資訊（包括可用庫存），以及新增、更新和結束（刪除）清單。 在完成商店設定之前，請依設定期間的狀態檢閱清單，並調整設定（[listing settings](./listing-settings.md)、[listing rules](./listing-rules.md)、[pricing rules](./pricing-products.md)、[overrides](./overrides.md)等）。 您也可以視需要在設定後修改這些設定。

- Amazon銷售管道可設定您的定價規則，以自動調整您的上市價格。 自動定價保障包括[智慧重定價規則](./intelligent-repricing-rules.md)的[底價](./floor-price.md)和[可選最高價](./optional-ceiling-price.md)功能。 使用這些保障措施有助於確保您的上市價格不會低於成本或高於定義的價格。

- Amazon銷售管道和Amazon之間的資料同步是由您的[[!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}設定控制。 [!DNL Commerce]和Amazon之間的內建限制有助於確保資料傳輸順暢且高效，但在高電子商務流量時間（如黑色星期五）,Amazon的系統更新所需時間可能比平常長。 將[!DNL Commerce] cron設定為每五分鐘執行一次。

- Amazon銷售管道會匯入您的Amazon訂單資訊。 若要在Amazon銷售管道中管理Amazon訂單，您必須確定已定義您的[訂單設定](./order-settings.md)，以匯入並建立每個Amazon訂單的對應[!DNL Commerce]訂單。 如果未定義，則您只能檢視Amazon訂單資訊。 通過Amazon銷售的所有稅仍通過您的[!DNL Amazon Seller Central]帳戶進行管理和匯出。 在一些州，Amazon需要自動收稅和繳稅。 對於其他州，賣方可以選擇手動或自動計算稅。 請參閱[Amazon:稅策略](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target=&quot;_blank&quot;}。 您可能需要登入[!DNL Amazon Seller Central]帳戶才能檢視Amazon稅務政策檔案。

- 對於英國地區，在登入Amazon銷售管道之前，最好先註冊[Amazon VAT計算服務](https://sell.amazon.co.uk/learn/vat-resources/){target=&quot;_blank&quot;}。


   >[!NOTE]
   >
   >Amazon可能需要10到14天的時間來驗證和啟用您的增值稅計算服務帳戶。

限制包括：

- Amazon銷售管道不支援將屬於[!DNL Commerce]目錄的套件組合、禮品卡和分組產品類型列入Amazon。

- Amazon銷售管道無法為沒有現有或先前Amazon清單的產品建立清單。 如果[!DNL Amazon Seller Central]中沒有具有ASIN的產品，則必須在[!DNL Amazon Seller Central]中添加該產品，以便Amazon可以為產品分配ASIN。 在Amazon中新增產品並建立清單後，清單便可與Amazon銷售管道中的目錄相符並同步。

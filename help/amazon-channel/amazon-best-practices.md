---
title: Amazon銷售渠道的最佳做法和限制
description: 在使用AmazonAdobe Commerce和Magento Open Source銷售渠道時，請回顧最佳做法和限制。
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# 最佳做法和AmazonSales Channel

最佳做法包括：

- Amazon銷售渠道可通過提高或降低價格、同步產品資訊（包括可用庫存）以及添加、更新和結束（刪除）清單來影響您的Amazon清單。 在設定期間按狀態查看清單並調整設定([清單設定](./listing-settings.md)。 [上市規則](./listing-rules.md)。 [定價規則](./pricing-products.md)。 [覆蓋](./overrides.md)等)之後完成儲存設定。 還可以根據需要在設定後修改這些設定。

- Amazon銷售渠道可以設定您的定價規則以自動調整您的上市價格。 自動定價保護包括 [底價](./floor-price.md) 和 [可選上限](./optional-ceiling-price.md) 特徵 [智慧重定價規則](./intelligent-repricing-rules.md)。 使用這些保護措施有助於確保您的上市價格不會低於成本或高於定義的價格。

- Amazon銷售渠道和Amazon之間的資料同步由您控制 [[!DNL Commerce] 克隆](https://docs.magento.com/user-guide/system/cron.html){target="_blank"} 的子菜單。 內置調節 [!DNL Commerce] 而Amazon則有助於確保資料傳輸的平穩和高效，但在高電子商務流量（如「黑色星期五」）期間，Amazon的系統更新可能比通常需要更長的時間。 設定 [!DNL Commerce] 克龍每五分鐘跑一次。

- Amazon銷售渠道導入您的Amazon訂單資訊。 要在Amazon銷售渠道管理您的Amazon訂單，您必須確保 [順序設定](./order-settings.md) 定義為導入和建立相應 [!DNL Commerce] 每份Amazon訂單。 如果未定義，則您只能查看您的Amazon訂單資訊。 所有通過Amazon銷售的稅款仍通過您的 [!DNL Amazon Seller Central] 帳戶。 在一些州，Amazon被要求自動徵稅和匯稅。 對於其他州，賣方可以選擇手動或自動計算稅款。 請參閱 [Amazon:稅收政策](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target="_blank"}。 可能需要您登錄 [!DNL Amazon Seller Central] 帳戶以查看Amazon稅收政策文檔。

- 對於英國地區而言，最佳做法是註冊 [Amazon增值稅計稅服務](https://sell.amazon.co.uk/learn/vat-resources/){target="_blank"} 在Amazon銷售頻道上。


   >[!NOTE]
   >
   >Amazon可能需要10至14天時間驗證並激活您的增值稅計算服務帳戶。

限制包括：

- 捆綁包、禮品卡和分組產品類型是您的 [!DNL Commerce] Amazon銷售渠道不支援將目錄列入Amazon。

- Amazon銷售渠道無法為沒有現有或先前Amazon清單的產品建立清單。 如果中不存在產品 [!DNL Amazon Seller Central] ASIN必須加入 [!DNL Amazon Seller Central] 讓Amazon給產品分配一個ASIN 在Amazon添加產品並建立清單後，清單可以與Amazon銷售渠道中的目錄匹配並同步。

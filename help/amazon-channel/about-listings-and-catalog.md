---
title: 關於Amazon和商業目錄
description: Amazon銷售渠道將您的Amazon清單導入您的Commerce後端，並持續與產品和銷售同步。
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 5d30a5282ede2db0d9619eb2263b733328d26426
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# 關於Amazon和 [!DNL Commerce] 目錄

您的Adobe Commerce或Magento Open Source後端包括包含所有產品和相關設定和資訊（映像、選項、價格等）以及訂單和發運配置的目錄。 您 [!DNL Amazon Seller Central] 帳戶還具有目錄和訂單配置，嚴格跟蹤您通過 [!DNL Amazon Marketplace]。

為了更好地管理和查看您的產品目錄和通過一個地點進行的銷售，Amazon銷售渠道將您的Amazon清單導入到您的 [!DNL Commerce] 後端，持續與產品和銷售同步，並報告問題和趨勢。 它支援與多個 [!DNL Amazon Seller Central] 通過單個介面跟蹤所有資料，用於多個店面。

## 產品屬性

Adobe Commerce和Magento Open Source使用產品管理目錄同步 [屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}以定義產品設定和資料。 Amazon也使用屬性，通過登陸來映射。 期間 [預設定任務](./amazon-pre-setup-tasks.md) 對於Amazon銷售渠道，您可以定義其他Amazon屬性（如果需要），以確保在將Amazon清單導入到您的 [!DNL Commerce] 目錄。 這些屬性包括UPC、EAN、ISBN和ASIN([!DNL Amazon Standard Identification Number])。 通過登陸，產品在Amazon和 [!DNL Commerce] 目錄。 正確映射 [!DNL Commerce] Amazon產品確保產品資訊，訂單和庫存的持續同步。

如果您沒有為目錄建立或配置這些屬性，則應添加 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}和產品值，然後再開始使用。 導入Amazon屬性時，可用於搜索、導航、價格規則等。 請參閱 [ASIN、UPC、EAN、ISBN、SKU和其他條形碼意味著什麼？](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target=&quot;_blank&quot;

登錄後，您可以隨時管理和更新產品屬性和Amazon映射。

## 產品清單

Amazon清單是您通過 [!DNL Amazon Marketplace]，顯示通過屬性映射的產品說明、價格、影像等。 登機期間，您可以配置 [!DNL Commerce] 產品可以自動發佈到Amazon的清單上。 您還可以通過將現有的Amazon清單映射到您的 [!DNL Commerce] 產品。

建立清單時 [!DNL Commerce] 產品，提交Amazon審批。 大多數成功的上市在幾小時內獲得批准。 如果您的清單已獲批准，則它將出現在 [!DNL Amazon Marketplace] 客戶即時訂購。 的 [!DNL Amazon Sales Channel] extension提供一組頁籤，用於查看Amazon清單。 根據問題或所需資料，您應查看 [!DNL Amazon Seller Central] 清單的特定詳細資訊。

- [活動](./active-listings.md):列出通過市場提供的已批准產品清單。

- [準備列出](./ready-to-list.md):列出符合上市規則要求並準備發佈到Amazon的產品。

- [非活動](./inactive-listings.md):列出由於特定原因（如品牌問題）、關閉和需要重新啟用等原因而無法在市場上使用的產品。

- [不合格](./ineligible-listings.md):由於上市規則，列出無法在市場上主動列出的產品(例如 `0` 數量或銷售日期)。

- [不完整](./incomplete-listings.md):列出缺少所需資訊的產品。 更新產品資料以供其他審閱。

- [結束](./ended-listings.md):列出符合清單條件但手動從Amazon刪除的產品清單。 您可以重新列出這些產品。

## 同步資料

Adobe Commerce和Magento Open Source在您的 [!DNL Amazon Seller Central] 帳戶和 [!DNL Commerce] 後端。 連續更新通過 [!DNL Commerce] 管理和維護庫存、履行訂單、跟蹤銷售，並減少開銷和工作重複。 Reporting可捕獲最新資料，用於跟蹤趨勢並解決兩個系統之間捕獲的通信問題。

所有同步都由 [克倫](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}，設定為每五分鐘更新一次 [預設定任務](./amazon-pre-setup-tasks.md)。

---
title: 關於Amazon和商務目錄
description: Amazon銷售管道會將您的Amazon清單匯入您的Commerce後端，並持續與產品和銷售同步。
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# 關於Amazon和 [!DNL Commerce] 目錄

您的Adobe Commerce或Magento Open Source後端包含目錄，其中包含所有產品和相關設定及資訊（影像、選項、價格等），以及訂購和運送設定。 您的 [!DNL Amazon Seller Central] 帳戶也有目錄和訂單設定，嚴格追蹤您的銷售，透過 [!DNL Amazon Marketplace].

為了透過一個位置更妥善地管理及檢閱您的產品目錄和銷售，Amazon銷售管道會將您的Amazon清單匯入您的 [!DNL Commerce] 後端會持續與產品和銷售同步，並回報問題和趨勢。 支援與多個 [!DNL Amazon Seller Central] 帳戶，透過單一介面追蹤多個商店的所有資料。

## 產品屬性

Adobe Commerce和Magento Open Source透過產品使用管理目錄同步 [屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} 以定義產品設定和資料。 Amazon也使用屬性，可透過入門進行對應。 期間 [預先設定任務](./amazon-pre-setup-tasks.md) 針對Amazon銷售管道，您需要定義其他Amazon屬性（如有需要），以確保將Amazon清單匯入您的 [!DNL Commerce] 目錄。 這些屬性包括UPC、EAN、ISBN和ASIN([!DNL Amazon Standard Identification Number])。 透過上線，產品可在Amazon和 [!DNL Commerce] 目錄。 正確對應 [!DNL Commerce] 而Amazon產品可確保產品資訊、訂單和庫存持續同步。

如果您尚未針對目錄建立或設定這些屬性，則應新增 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} and values to your products before onboarding. When an Amazon attribute is imported, it can be used for search, navigation, price rules, and much more. See [What Do ASIN, UPC, EAN, ISBN, SKU and Other Barcodes Mean?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

上線後，您可以隨時管理和更新產品屬性和Amazon對應。

## 產品清單

Amazon清單是您透過 [!DNL Amazon Marketplace]，顯示產品說明、價格、影像，以及透過屬性對應的更多項目。 在上線期間，您可以設定 [!DNL Commerce] 產品可自動發佈至Amazon清單。 您也可以將現有的Amazon清單對應至 [!DNL Commerce] 產品。

建立清單時 [!DNL Commerce] 產品，則會提交Amazon以供核准。 大多數成功的清單會在幾小時內獲得批准。 如果您的清單獲得批准，它會顯示在 [!DNL Amazon Marketplace] 客戶立即訂購。 此 [!DNL Amazon Sales Channel] 擴充功能提供一組標籤，供您檢閱Amazon清單。 您應根據問題或所需資料檢閱 [!DNL Amazon Seller Central] 帳戶取得這些清單的特定詳細資訊。

- [作用中](./active-listings.md):列出通過Marketplace提供的已批准產品清單。

- [準備列出](./ready-to-list.md):列出符合上市規則要求且可發佈至Amazon的產品。

- [非作用中](./inactive-listings.md):列出因特定原因（例如品牌問題）、關閉和需要重新啟用等原因而無法在市場上使用的產品。

- [不合格](./ineligible-listings.md):由於上市規則，列出未能於市場上積極上市之產品(例如 `0` 數量或銷售日期)。

- [不完整](./incomplete-listings.md):列出缺少所需資訊的產品。 更新產品資料以供其他審核。

- [已結束](./ended-listings.md):列出符合列出資格，但需從Amazon手動移除的產品清單。 您可以重新列出這些產品。

## 同步資料

Adobe Commerce和Magento Open Source可在您的 [!DNL Amazon Seller Central] 帳戶和 [!DNL Commerce] 後端。 持續更新可提供單一來源，透過 [!DNL Commerce] 管理和維護庫存、履行訂單、跟蹤銷售，以及減少開銷和工作重複。 報表會擷取最新資料，以追蹤趨勢並解決兩個系統之間所擷取的通訊問題。

所有同步均由 [cron job](https://docs.magento.com/user-guide/system/cron.html){target="_blank"}，請在 [預先設定任務](./amazon-pre-setup-tasks.md).

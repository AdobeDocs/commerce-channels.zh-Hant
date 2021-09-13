---
title: 關於Amazon和商務目錄
description: Amazon銷售管道會將您的Amazon清單匯入您的Commerce後端，並持續與產品和銷售同步。
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# 關於Amazon和[!DNL Commerce]目錄

您的Adobe商務或Magento Open Source後端包含目錄，其中包含所有產品和相關設定及資訊（影像、選項、價格等），以及訂購和運送設定。 您的[!DNL Amazon Seller Central]帳戶也有目錄和訂單設定，嚴格透過[!DNL Amazon Marketplace]追蹤您的銷售。

為了透過一個位置更妥善地管理及檢閱您的產品目錄和銷售，Amazon銷售管道會將您的Amazon清單匯入您的[!DNL Commerce]後端，與產品和銷售持續同步，並回報問題和趨勢。 它支援與多個[!DNL Amazon Seller Central]帳戶的整合，可透過單一介面追蹤多個店面的所有資料。

## 產品屬性

Adobe商務和Magento Open Source管理目錄同步，使用產品[attributes](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}來定義產品設定和資料。 Amazon也使用屬性，可透過入門進行對應。 在[預先設定工作](./amazon-pre-setup-tasks.md)期間，您需要為Amazon銷售管道定義其他Amazon屬性（如有需要），以確保將Amazon清單匯入[!DNL Commerce]目錄時有正確的產品對應。 這些屬性包括UPC、EAN、ISBN和ASIN([!DNL Amazon Standard Identification Number])。 透過上線，產品可使用您的屬性在Amazon和[!DNL Commerce]目錄之間同步。 正確對應[!DNL Commerce]和Amazon產品可確保產品資訊、訂單和庫存持續同步。

如果您尚未針對目錄建立或設定這些屬性，您應在上線前，先將[!DNL Commerce] [product屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}和值新增至產品。 匯入Amazon屬性時，可用於搜尋、導覽、價格規則等。 如需這些屬性的詳細資訊，請參閱[Amazon:什麼是UPC、EAN、ISBN和ASIN?](https://www.amazon.com/gp/seller/asin-upc-isbn-info.html){target=&quot;_blank&quot;}

上線後，您可以隨時管理和更新產品屬性和Amazon對應。

## 產品清單

Amazon清單是您透過[!DNL Amazon Marketplace]銷售之每項產品的產品頁面，顯示透過屬性對應的產品說明、價格、影像等。 在上線期間，您可以設定您的[!DNL Commerce]產品可自動發佈至Amazon清單。 您也可以將現有的Amazon清單對應至您的[!DNL Commerce]產品，以匯入這些清單。

當您建立清單[!DNL Commerce]產品時，這些產品會提交Amazon以供核准。 大多數成功的清單會在幾小時內獲得批准。 如果您的清單獲得批准，該清單將顯示在[!DNL Amazon Marketplace]中，供客戶立即訂購。 [!DNL Amazon Sales Channel]擴充功能提供一組索引標籤，供您檢閱Amazon清單。 根據問題或所需資料，您應查看[!DNL Amazon Seller Central]帳戶，以了解這些清單的特定詳細資訊。

- [作用中](./active-listings.md):列出通過Marketplace提供的已批准產品清單。

- [準備列出](./ready-to-list.md):列出符合上市規則要求且可發佈至Amazon的產品。

- [非作用中](./inactive-listings.md):列出因特定原因（例如品牌問題）、關閉和需要重新啟用等原因而無法在市場上使用的產品。

- [不合格](./ineligible-listings.md):由於上市規則，列出無法在市場上積極列出的產品(例如數 `0` 量或銷售日期)。

- [不完整](./incomplete-listings.md):列出缺少所需資訊的產品。更新產品資料以供其他審核。

- [已結束](./ended-listings.md):列出符合列出資格，但需從Amazon手動移除的產品清單。您可以重新列出這些產品。

## 同步資料

Adobe商務和Magento Open Source會在您的[!DNL Amazon Seller Central]帳戶和[!DNL Commerce]後端之間傳遞產品和訂單資料。 持續更新通過[!DNL Commerce]提供單個源，以管理和維護您的庫存、完成訂單、跟蹤銷售，並減少開銷和工作重複。 報表會擷取最新資料，以追蹤趨勢並解決兩個系統之間所擷取的通訊問題。

所有同步均由[cron job](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}管理，在[預設設定任務](./amazon-pre-setup-tasks.md)中設定為每五分鐘更新一次。

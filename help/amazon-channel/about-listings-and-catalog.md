---
title: Amazon與Commerce目錄
description: Amazon銷售管道會將您的Amazon清單匯入您的Commerce後端，並持續與產品和銷售同步。
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services, Merchandising, Catalog Management
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Amazon和[!DNL Commerce]目錄

您的Adobe Commerce或Magento Open Source後端包含目錄，內含所有產品及相關設定和資訊（影像、選項、價格等），以及訂單和送貨設定。 您的[!DNL Amazon Seller Central]帳戶也有目錄和訂單設定，透過[!DNL Amazon Marketplace]嚴格追蹤您的銷售。

為了透過單一位置更好地管理和檢閱您的產品目錄和銷售，Amazon銷售管道會將您的Amazon清單匯入您的[!DNL Commerce]後端，持續與產品和銷售同步，並報告問題和趨勢。 它支援與多個[!DNL Amazon Seller Central]帳戶整合，透過單一介面追蹤多個店面的所有資料。

## 產品屬性

Adobe Commerce和Magento Open Source使用產品[屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)來管理目錄同步，以定義產品設定和資料。 Amazon也使用屬性，透過上線進行對應。 在Amazon銷售管道的[預先設定工作](./amazon-pre-setup-tasks.md)期間，您可以定義其他Amazon屬性（如有需要），以確保將您的Amazon清單匯入您的[!DNL Commerce]目錄時，產品對應正確。 這些屬性包括UPC、EAN、ISBN和ASIN ([!DNL Amazon Standard Identification Number])。 透過上線，產品會使用您的屬性在Amazon和[!DNL Commerce]目錄之間同步。 適當對應您的[!DNL Commerce]與Amazon產品，確保產品資訊、訂單與存貨的持續同步。

如果您沒有為目錄建立或設定這些屬性，您應該在入門之前新增[!DNL Commerce] [產品屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)和值到您的產品。 匯入Amazon屬性時，該屬性可用於搜尋、導覽、價格規則等。 請參閱[ASIN、UPC、EAN、ISBN、SKU和其他條碼代表什麼？](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

上線後，您可以隨時管理和更新產品屬性和Amazon對應。

## 產品清單

Amazon清單是您透過[!DNL Amazon Marketplace]銷售之每個產品的產品頁面，可透過屬性顯示產品說明、價格、影像及其他對應專案。 上線期間，您可以設定可將您的[!DNL Commerce]產品自動發佈至Amazon清單。 您也可以將現有的Amazon清單對應至您的[!DNL Commerce]產品，以匯入這些清單。

當您建立清單[!DNL Commerce]產品時，這些產品會提交至Amazon進行核准。 大多數成功的清單都會在數小時內獲得核准。 如果您的清單已核准，則會在[!DNL Amazon Marketplace]中顯示客戶的即時訂單。 [!DNL Amazon Sales Channel]擴充功能提供一組標籤來檢閱Amazon清單。 根據問題或所需的資料，您應該檢閱您的[!DNL Amazon Seller Central]帳戶，以取得這些清單的特定詳細資料。

- [使用中](./active-listings.md)：列出可透過市集取得的已核准產品清單。

- [準備清單](./ready-to-list.md)：列出符合清單規則要求且可發佈至Amazon的產品。

- [非使用中](./inactive-listings.md)：列出由於特定原因（例如品牌問題）遭到封鎖、已關閉且需要重新刊登等而無法在市集上使用的產品。

- [不合格](./ineligible-listings.md)：由於清單規則，列出無法主動在市集上列出的產品（例如`0`數量或銷售日期）。

- [不完整](./incomplete-listings.md)：列出遺失必要資訊的產品。 更新產品資料以進行其他檢閱。

- [已結束](./ended-listings.md)：列出符合清單資格，但手動從Amazon移除的產品清單。 您可以重新列出這些產品。

## 正在同步資料

Adobe Commerce和Magento Open Source在您的[!DNL Amazon Seller Central]帳戶和[!DNL Commerce]後端之間通訊產品和訂單資料。 持續更新會透過[!DNL Commerce]提供單一來源，以管理和維護您的存貨、完成訂單、追蹤銷售，以及減少製造費用與重複工作。 報告會擷取最新資料，以追蹤趨勢並解決兩個系統之間所發生的通訊問題。

所有同步處理都由[cron工作](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html)管理，設定為每5分鐘更新一次[預先設定工作](./amazon-pre-setup-tasks.md)。

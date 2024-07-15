---
title: 「內建 [!DNL Amazon Sales Channel]」
description: 瞭解預先設定任務、上線步驟，以及Amazon如何在Adobe Commerce和Magento Open Source中搭配AmazonSales Channel使用。
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 6321f17c0e6f9e86bb3f5755dc7710fa68d68b0d
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# 上線[!DNL Amazon Sales Channel]

本節說明預先設定工作、入門步驟，以及Amazon如何在Adobe Commerce和Magento Open Source中與Amazon銷售管道搭配運作的一些重要概念。

[!DNL Amazon Sales Channel]擴充功能支援多個Amazon存放區。 針對在Amazon美國/加拿大/墨西哥地區營運的單一[!DNL Amazon Seller Central]帳戶，建立三個Amazon商店（分別為美國銷售、墨西哥銷售和加拿大銷售銷售）。 這三家商店的每一家在建立期間都會定義市場國家。 如果您擁有多個[!DNL Amazon Seller Central]帳戶，則每個[!DNL Amazon Seller Central]帳戶最多可以有三個Amazon商店。 如果您也在英國銷售，您將擁有第四家Amazon商店。

>[!TIP]
>
>北美或歐洲(UK)區域的[!DNL Amazon Seller Central]需要[專業賣家帳戶](https://sell.amazon.com/){target="_blank"}。 Amazon每月會收取訂閱及銷售費用。 檢視[Amazon：選擇您的銷售計畫](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>
>入門很簡單 — 建立您的商店，然後將其連線至您的[!DNL Amazon Seller Central]帳戶。
>當您的商店已連線時，Amazon管道會嘗試匯入您的Amazon清單，並根據您的[屬性對應](./attributes-view.md).<br><br>，將它們與您的目錄比對
>您的Amazon銷售管道設定會影響您的Amazon清單。 您的初始清單、定價和產品設定皆會為您預設。 在商店連線至您的[!DNL Amazon Seller Central]帳戶後，您可以修改您的[商店設定](./ob-store-review.md) （清單、定價、訂單和報告）。

| 步驟 | 發生什麼情況 |
|---------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [預先設定工作](./amazon-pre-setup-tasks.md) | 上線之前，您必須確定您擁有使用中且已核准的[!DNL Amazon Seller Central]帳戶。 上線前還有一些[!DNL Commerce]需求和建議需要完成。 |
| [驗證Amazon API金鑰](./amazon-verify-api-key.md) | 存取Amazon Sales Channel時，[!DNL Commerce]會自動檢查並驗證您新增至商店設定中的Amazon API金鑰。 如果您的API金鑰尚未新增或無效，系統會提示您[新增或更新您的Amazon API金鑰](./amazon-verify-api-key.md)。 |
| [存放區整合](./store-integration.md) | 此步驟包括建立Amazon銷售管道商店，然後將其連線至您的[!DNL Amazon Seller Central]帳戶。 您需要您的[!DNL Amazon Seller Central]帳戶（用來建立賣家帳戶的電子郵件或電話）的主要登入認證，才能完成此步驟。 |
| [建立清單規則](./ob-create-listing-rule.md) | 連線Amazon銷售管道商店後，系統會提示您建立清單規則。 我們建議您執行此步驟，但您也可以略過此步驟，以開始清單匯入程式。 您也可以在商店[儀表板](./amazon-store-dashboard.md)存取您的[商店及清單設定](./ob-store-review.md)。 |

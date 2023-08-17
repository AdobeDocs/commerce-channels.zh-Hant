---
title: 「上線 [!DNL Amazon Sales Channel]"
description: 瞭解預先設定任務、上線步驟，以及Amazon如何在Adobe Commerce和Magento Open Source中搭配AmazonSales Channel使用。
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 6321f17c0e6f9e86bb3f5755dc7710fa68d68b0d
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 上線 [!DNL Amazon Sales Channel]

本節說明預先設定工作、入門步驟，以及Amazon如何在Adobe Commerce和Magento Open Source中與Amazon銷售管道搭配運作的一些重要概念。

此 [!DNL Amazon Sales Channel] 擴充功能可支援多個Amazon存放區。 針對單一 [!DNL Amazon Seller Central] 在Amazon美國/加拿大/墨西哥地區營運的帳戶，可建立三家Amazon商店（美國銷售、墨西哥銷售和加拿大銷售各一家）。 這三家商店的每一家在建立期間都會定義市場國家。 如果您有多個 [!DNL Amazon Seller Central] 帳戶，您的每個帳戶最多可以有三個Amazon商店 [!DNL Amazon Seller Central] 帳戶。 如果您也在英國銷售，您將擁有第四家Amazon商店。

>[!TIP]
>
>A [專業賣家帳戶](https://sell.amazon.com/){target="_blank"} on [!DNL Amazon Seller Central] in the North America or European (UK) region is required. Amazon charges a monthly subscription and fees for selling. See [Amazon: Choose your selling plan](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>
>入門很簡單 — 建立您的商店，然後將其連線到您的 [!DNL Amazon Seller Central] 帳戶。
>當您的商店已連線時，Amazon管道會嘗試匯入您的Amazon清單，並根據您的 [屬性對應](./attributes-view.md).<br><br>
>您的Amazon銷售管道設定會影響您的Amazon清單。 您的初始清單、定價和產品設定皆會為您預設。 您可以修改您的 [商店設定](./ob-store-review.md) （清單、定價、訂購和報告）建立連線後 [!DNL Amazon Seller Central] 帳戶。

| 步驟 | 發生什麼情況 |
|---------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [預先設定任務](./amazon-pre-setup-tasks.md) | 上線之前，您必須確定您已擁有使用中且已核准許可權 [!DNL Amazon Seller Central] 帳戶。 此外還有一些 [!DNL Commerce] 上線前完成的要求和建議。 |
| [驗證Amazon API金鑰](./amazon-verify-api-key.md) | 存取Amazon銷售管道時， [!DNL Commerce] 自動檢查及驗證您新增至商店設定的Amazon API金鑰。 如果您的API金鑰尚未新增或無效，系統會提示您輸入 [新增或更新您的Amazon API金鑰](./amazon-verify-api-key.md). |
| [存放區整合](./store-integration.md) | 此步驟包括建立Amazon銷售管道商店，然後將其連線到您的 [!DNL Amazon Seller Central] 帳戶。 您需要的主要登入認證 [!DNL Amazon Seller Central] 此步驟的帳戶（用來建立賣家帳戶的電子郵件或電話）。 |
| [建立清單規則](./ob-create-listing-rule.md) | 連線Amazon銷售管道商店後，系統會提示您建立清單規則。 我們建議您執行此步驟，但您也可以略過此步驟，以開始清單匯入程式。 您也可以存取 [商店和清單設定](./ob-store-review.md) 在存放區上 [儀表板](./amazon-store-dashboard.md). |

---
title: 板載AmazonSales Channel
description: 了解預先設定工作、入門步驟，以及Amazon如何與Adobe Commerce和Magento Open Source中的AmazonSales Channel搭配使用。
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 板載AmazonSales Channel

本節說明預先設定工作、入門步驟，以及Amazon如何與Adobe Commerce和Magento Open Source中的Amazon銷售管道搭配運作的一些重要概念。

此 [!DNL Amazon Sales Channel] 擴充功能支援多個Amazon商店。 單一 [!DNL Amazon Seller Central] 在Amazon美國/加拿大/墨西哥地區運營的客戶，建立了三家Amazon商店（每家分別銷售美國、墨西哥和加拿大銷售）。 這三家商店在建立期間分別定義市集國家。 如果您有多個 [!DNL Amazon Seller Central] 帳戶中，您每個 [!DNL Amazon Seller Central] 帳戶。 如果你也在英國賣，你會有第四家Amazon店。

>[!TIP]
>
>A [專業賣家帳戶](https://sell.amazon.com/){target="_blank"} on [!DNL Amazon Seller Central] in the North America or European (UK) region is required. Amazon charges a monthly subscription and fees for selling. See [Amazon: Choose your selling plan](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>
>上線很簡單：建立商店，然後將其連結到您的 [!DNL Amazon Seller Central] 帳戶。
>連線您的商店時，Amazon管道會嘗試匯入您的Amazon清單，並根據您的 [屬性對應](./attributes-view.md).<br><br>
>您的Amazon銷售管道設定會影響您的Amazon清單。 您的初始清單、定價和產品設定是預設值。 您可以修改 [儲存設定](./ob-store-review.md) （清單、定價、訂單和報告） [!DNL Amazon Seller Central] 帳戶。

| 步驟 | 發生的情況 |
|--- |--- |
| [預先設定任務](./amazon-pre-setup-tasks.md) | 上線前，您必須確定您有已啟用且已核准 [!DNL Amazon Seller Central] 帳戶。 還有一些 [!DNL Commerce] 要求和建議，請在上線前完成。 |
| [驗證Amazon API金鑰](./amazon-verify-api-key.md) | 存取Amazon銷售管道時， [!DNL Commerce] 自動檢查並驗證您在商店設定中新增的Amazon API金鑰。 如果您的API金鑰尚未新增或無效，系統會提示您 [新增或更新您的Amazon API金鑰](./amazon-verify-api-key.md). |
| [商店整合](./store-integration.md) | 此步驟包括建立Amazon銷售管道商店，然後將其連結至您的 [!DNL Amazon Seller Central] 帳戶。 您需要的主要登入憑證 [!DNL Amazon Seller Central] 帳戶（用來建立賣家帳戶的電子郵件或電話）。 |
| [建立清單規則](./ob-create-listing-rule.md) | 連線Amazon銷售管道商店後，系統會提示您建立清單規則。 我們建議您執行此步驟，但您也可以略過此步驟，以開始清單匯入程式。 您也可以存取 [儲存和清單設定](./ob-store-review.md) 在商店 [儀表板](./amazon-store-dashboard.md). |

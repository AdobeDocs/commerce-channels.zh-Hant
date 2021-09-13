---
title: 板載AmazonSales Channel
description: 了解預先設定工作、入門步驟，以及Amazon如何與AmazonSales Channel搭配使用Adobe商務和Magento Open Source。
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html: 
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 0%

---

# 板載Amazon銷售渠道

本節說明預先設定工作、入門步驟，以及Amazon如何搭配Adobe商務和Magento Open Source中的Amazon銷售管道運作的一些重要概念。

[!DNL Amazon Sales Channel]擴充功能支援多個Amazon商店。 對於在Amazon美國/加拿大/墨西哥地區運作的單一[!DNL Amazon Seller Central]帳戶，建立三家Amazon商店（分別針對美國銷售額、墨西哥銷售額和加拿大銷售額）。 這三家商店在建立期間分別定義市集國家。 如果您有多個[!DNL Amazon Seller Central]帳戶，則每個[!DNL Amazon Seller Central]帳戶最多可能有三個Amazon商店。 如果你也在英國賣，你會有第四家Amazon店。

>[!TIP]
>
>在北美或歐洲（英國）地區的[!DNL Amazon Seller Central]上，需要[專業賣家帳戶](https://sell.amazon.com/){target=&quot;_blank&quot;}。 Amazon每月收取訂購費和銷售費。 請參閱[Amazon:選擇您的銷售計畫](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}。<br><br>
>上線很簡單：請建立您的商店，然後將其連接到您的[!DNL Amazon Seller Central]帳戶。
>連線您的商店時，Amazon管道會根據您的[屬性對應](./attributes-view.md).<br><br>，嘗試匯入您的Amazon清單，並將它們與目錄比對
>您的Amazon銷售管道設定會影響您的Amazon清單。 您的初始清單、定價和產品設定是預設值。 在您的商店連接到[!DNL Amazon Seller Central]帳戶後，您可以修改[商店設定](./ob-store-review.md)（清單、定價、訂單和報告）。

| 步驟 | 發生的情況 |
|--- |--- |
| [預先設定任務](./amazon-pre-setup-tasks.md) | 在上線之前，您必須確保擁有有效的已核准[!DNL Amazon Seller Central]帳戶。 上線前還需要完成某些[!DNL Commerce]需求和建議。 |
| [驗證Amazon API金鑰](./amazon-verify-api-key.md) | 存取Amazon銷售管道時， [!DNL Commerce]會自動檢查並驗證您在商店設定中新增的Amazon API金鑰。 如果您的API金鑰尚未新增或無效，系統會提示您新增或更新Amazon API金鑰](./amazon-verify-api-key.md)。[ |
| [商店整合](./store-integration.md) | 此步驟包括建立Amazon銷售管道商店，然後將其連結至您的[!DNL Amazon Seller Central]帳戶。 此步驟需要[!DNL Amazon Seller Central]帳戶（用於建立賣家帳戶的電子郵件或電話）的主要登入憑證。 |
| [建立清單規則](./ob-create-listing-rule.md) | 連線Amazon銷售管道商店後，系統會提示您建立清單規則。 我們建議您執行此步驟，但您也可以略過此步驟，以開始清單匯入程式。 您也可以存取[商店，並列出商店[控制面板](./amazon-store-dashboard.md)上的設定](./ob-store-review.md)。 |

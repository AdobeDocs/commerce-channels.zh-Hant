---
title: 機載AmazonSales Channel
description: 瞭解預先設定的任務、入門步驟以及Amazon如何與Adobe Commerce和Magento Open Source的AmazonSales Channel合作。
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 機載AmazonSales Channel

本節介紹預設定任務、入門步驟以及Amazon如何與Adobe Commerce和Magento Open Source的Amazon銷售渠道合作的一些關鍵概念。

的 [!DNL Amazon Sales Channel] 擴展支援多個Amazon商店。 對於單個 [!DNL Amazon Seller Central] 在Amazon美國/加拿大/墨西哥地區運營的客戶，建立了三家Amazon商店（分別針對美國銷售、墨西哥銷售和加拿大銷售）。 這三家商店中的每一家都在其建立過程中定義了市場國家。 如果你有多個 [!DNL Amazon Seller Central] 你每個人可能有3家Amazon店 [!DNL Amazon Seller Central] 帳戶。 如果你在英國也賣，你會有第四家Amazon店。

>[!TIP]
>
>A [專業賣家帳戶](https://sell.amazon.com/){target="_blank"} on [!DNL Amazon Seller Central] in the North America or European (UK) region is required. Amazon charges a monthly subscription and fees for selling. See [Amazon: Choose your selling plan](https://sell.amazon.com/pricing.html){target="_blank"}。<br><br>
>入門很簡單 — 建立您的商店，然後將其連接到您的 [!DNL Amazon Seller Central] 帳戶。
>當您的商店連接後，Amazon頻道會根據您的 [屬性映射](./attributes-view.md)。<br><br>
>您的Amazon銷售渠道設定會影響您的Amazon清單。 您的初始清單、定價和產品設定是預設的。 您可以修改 [儲存設定](./ob-store-review.md) （清單、定價、訂單和報告） [!DNL Amazon Seller Central] 帳戶。

| 步驟 | 發生什麼 |
|--- |--- |
| [預設定任務](./amazon-pre-setup-tasks.md) | 在上載之前，必須確保您具有活動且已批准 [!DNL Amazon Seller Central] 帳戶。 還有一些 [!DNL Commerce] 要求和建議，以在登機前完成。 |
| [驗證AmazonAPI密鑰](./amazon-verify-api-key.md) | 訪問Amazon銷售渠道時， [!DNL Commerce] 自動檢查並驗證您在儲存配置中添加的AmazonAPI密鑰。 如果API密鑰尚未添加或無效，系統將提示您 [添加或更新您的AmazonAPI密鑰](./amazon-verify-api-key.md)。 |
| [儲存整合](./store-integration.md) | 此步驟包括建立Amazon銷售渠道商店，然後將其連接到 [!DNL Amazon Seller Central] 帳戶。 您需要主登錄憑據 [!DNL Amazon Seller Central] 帳戶（用於建立賣家帳戶的電子郵件或電話）。 |
| [建立清單規則](./ob-create-listing-rule.md) | 連接Amazon銷售渠道商店後，系統將提示您建立清單規則。 鼓勵執行此步驟，但您也可以跳過此步驟以啟動清單導入過程。 您還可以訪問 [儲存和列出設定](./ob-store-review.md) 店裡 [儀表板](./amazon-store-dashboard.md)。 |

---
title: 「 [!DNL Amazon Sales Channel]簡介」
description: '[!DNL Amazon Sales Channel]可讓商家在 [!DNL Amazon Marketplace]中順暢地銷售產品。'
redirect_from: /sales-channels/amazon/amazon-sales-channel.html
role: Admin, User, Leader
exl-id: a4a6f446-7029-4c92-bce3-5b857cc33056
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel]簡介

身為Adobe Commerce或Magento Open Source商家，您可以使用[!DNL Amazon Sales Channel]擴充功能，將您的商店與世界上最大的全球網際網路購物目的地整合。 此擴充功能可讓Amazon銷售人員將[!DNL Commerce]連線至您的[!DNL Amazon Seller Central]帳戶，並提供目錄與訂單資料的自動化與同步處理。 透過單一[!DNL Commerce]儀表板，完整管理所有Amazon清單、實作簡易或智慧型訂價規則，以及維護您的訂單與存貨。

[上線](./amazon-onboarding-home.md)後，[!DNL Commerce]會成為「中央指揮中心」，以管理和控制您的Amazon清單、訂單和庫存以及您Amazon商店的定價。 [存放區整合](./store-integration.md)會連線您的[!DNL Commerce]執行個體和Amazon，以便在兩個平台之間同步資料。 Amazon sales channel可讓您：

- [上線](./amazon-onboarding-home.md)並將一或多個[!DNL Amazon Seller Central]帳戶與Adobe Commerce或Magento Open Source整合。

- 匯入並同步處理您現有的Amazon清單，並比對您[!DNL Commerce]目錄中的產品，以建立集中式產品目錄。

- 為您[!DNL Commerce]目錄中的產品建立和管理Amazon清單。

- 在[!DNL Commerce]與Amazon中檢視並履行（出貨）訂單，同步處理訂單狀態、付款及退款資訊。

- 檢視[競爭性價格](./competitive-price-analysis.md)、[清單變更](./listing-changes-log.md)和[通訊問題](./communication-errors-log.md)的分析記錄檔和錯誤。

存取您的Amazon商店，以在Amazon銷售管道[首頁](./amazon-sales-channel-home.md)上檢視及管理所有這些功能、帳戶資訊、清單、訂單等。

## 促銷與定價

使用[!DNL Amazon Sales Channel]副檔名，您可以：

- 將Amazon清單定價同步至[!DNL Commerce]目錄價格（或替代價格屬性）。

- 在您的Amazon清單中啟用MSRP [刪除線定價](./listing-price.md#configure-listing-price-settings)，以增加客戶價值主張。

- 啟用並管理您Amazon清單中的[最低廣告價格(MAP)](./listing-price.md#configure-listing-price-settings)。

- 在您的Amazon定價中設定額外的[VAT稅](./listing-price.md#configure-listing-price-settings)。

- 在您的[庫存/數量設定](./stock-quantity.md#configure-stock--quantity-settings)中設定「可用數量」的自訂值，以便與您的Amazon清單一起顯示，以增加購買者的急迫性。

## 定價規則

使用[!DNL Amazon Sales Channel]副檔名，您可以：

- 建立可棧疊、彈性且複雜的[定價規則](./pricing-products.md)，以管理日常銷售或季節性促銷的Amazon定價。

- 建立[下限](./floor-price.md)和[上限](./optional-ceiling-price.md)價格，以保護您的最低與最高價格。

- 建立並管理[智慧型重新訂價規則](./intelligent-repricing-rules.md)，此規則可自動調整您產品相對於其他Amazon競爭者的定價([最低競爭者](./lowest-competitor-pricing.md)和[Buy Box](./buy-box-competitor-pricing.md)價格)。

## 目錄摘要管理

使用[!DNL Amazon Sales Channel]副檔名，您可以：

- 匯入您現有的Amazon清單（產品），並與您的[!DNL Commerce]目錄中的現有或建立產品相符。

- 將您的[!DNL Commerce]產品Publish到Amazon以建立Amazon清單。

- 建立[覆寫](./creating-editing-overrides.md)以設定個別價格、處理時間、條件和賣家筆記訊息。

- 從您的Amazon清單匯入並對應產品[屬性](./attributes-view.md)，以自動比對您[!DNL Commerce]目錄中的產品。

- 設定多個搜尋引數以比對Amazon清單與您的[!DNL Commerce]目錄。

- 定義[清單規則](./listing-rules.md)，以決定您的[!DNL Commerce]個產品中哪些符合在Amazon上列出的資格。

- 為您新的Amazon清單設定預設[處理時間](./product-listing-actions.md)。

- 根據[!DNL Commerce]屬性符合清單條件。

- 為每種條件型別新增賣家備註（選擇性）。

- 將Amazon清單匯入您的[!DNL Commerce]目錄時，實作數量臨界值。

- 檢視建議的[清單改進](./listing-improvements.md)。

## 訂單管理與客戶服務

使用[!DNL Amazon Sales Channel]副檔名，您可以：

- 在Amazon和[!DNL Commerce]中支援及處理訂單。

- [將您的Amazon訂單](./order-settings.md#configure-order-settings)匯入[!DNL Commerce]或保留在Amazon中。

- 定義您的[!DNL Commerce]個網站商店中的哪些要與您的Amazon訂單產生關聯，以便匯入和管理訂單。

- 根據您的[履行設定](./fulfilled-by.md)，檢視、取消和出貨[!DNL Commerce]和/或Amazon的訂單。

- 將您的Amazon訂單狀態對應至[!DNL Commerce]內的自訂狀態（選擇性）。

- 檢視及管理訂單錯誤，以解決問題並與客戶聯絡。

- 傳送訂單追蹤資料至您的[!DNL Amazon Seller Central]帳戶。

- [取消訂單](./cancel-unshipped-order.md)並選取原因回應。

- 檢視您Amazon訂單的[最近訂單](./amazon-store-dashboard.md)資訊。

## 報告

使用[!DNL Amazon Sales Channel]擴充功能，您可以檢閱下列相關報表資訊：

- 依使用中、非使用中、符合資格及未完成狀態列出的清單。

- 等待出貨的訂單。

- 最近訂單。

- Amazon [清單變更記錄](./listing-changes-log.md)以檢閱產品/清單摘要變更（例如價格和數量）。

- 產品[Buy Box](./buy-box-competitor-pricing.md)競爭者定價資料。

- 產品[最低競爭者價格](./lowest-competitor-pricing.md)資料。

## 支援全球銷售

使用[!DNL Amazon Sales Channel]副檔名，您可以：

- 管理多個[!DNL Amazon Marketplace]地區（國家/地區）。

- 使用[Commerce貨幣設定工具](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html)支援多種貨幣。

- 管理您的產品地點與Amazon履行中心的出貨。

## 客戶管理

透過[匯入與您的Amazon訂單相關的客戶資料](./order-settings.md#configure-order-settings)，建置您的[!DNL Commerce]客戶資料庫。 透過您的[!DNL Amazon Marketplace]清單和[!DNL Commerce]店面，擴大客戶清單以增加您的行銷潛力。


快速入門很容易。 快速入門程式會引導您建立[!DNL Amazon Seller Central]帳戶，並與Amazon銷售管道存放區和[!DNL Commerce]目錄整合，以管理Amazon清單、訂單、存貨和履行。 中央儀表板會顯示所有Amazon銷售管道商店整合和Amazon清單的狀態更新。 透過簡化和自動化的流程，與全球[!DNL Amazon Marketplace]的新客戶接觸 — 幾乎不需要建立新系統的成本或人力。

整合您的[!DNL Amazon Seller Central]帳戶後，[!DNL Amazon Sales Channel]擴充功能可讓您管理您的帳戶，以及在[!DNL Commerce]和Amazon之間同步資料。 它可讓您直接透過[!DNL Commerce]管理員建立清單、管理促銷活動、設定價格，以及管理存貨與履行。 這些選項包括訂價規則，可監控相同專案的Amazon訂價，並自動調整您的價格以提高競爭力。


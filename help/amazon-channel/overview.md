---
title: 「簡介 [!DNL Amazon Sales Channel]"
description: '"[!DNL Amazon Sales Channel] 可讓商戶順暢地銷售產品， [!DNL Amazon Marketplace].」'
redirect_from: /sales-channels/amazon/amazon-sales-channel.html
role: Admin, User, Leader
exl-id: a4a6f446-7029-4c92-bce3-5b857cc33056
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---

# 簡介 [!DNL Amazon Sales Channel]

身為Adobe Commerce或Magento Open Source商人，您可以使用 [!DNL Amazon Sales Channel] 擴充功能，整合您的商店與全球最大的網際網路購物目的地。 此擴充功能可讓Amazon銷售人員透過連線 [!DNL Commerce] 與您的 [!DNL Amazon Seller Central] 帳戶，並提供目錄和訂單資料的自動化和同步化。 完整管理所有Amazon清單、實作簡易或智慧型訂價規則，並透過單一維護訂單與存貨 [!DNL Commerce] 儀表板。

晚於 [入門](./amazon-onboarding-home.md)， [!DNL Commerce] 會成為「中央指揮中心」，用於管理和控制您的Amazon清單、訂單和庫存，以及Amazon商店的定價。 [存放區整合](./store-integration.md) 連線您的 [!DNL Commerce] 執行個體和Amazon之間的資料同步。 Amazon sales channel可讓您：

- [上線](./amazon-onboarding-home.md) 並整合一或多個 [!DNL Amazon Seller Central] 具有Adobe Commerce或Magento Open Source的帳戶。

- 匯入並同步處理您現有的Amazon清單，並與您網站上的產品相符。 [!DNL Commerce] 目錄，建立集中式產品目錄。

- 建立並管理您產品的Amazon清單 [!DNL Commerce] 目錄。

- 檢視與履行（出貨）訂單，於 [!DNL Commerce] 和Amazon，同步處理訂單狀態、付款和退款資訊。

- 檢視分析記錄檔和錯誤 [具競爭力的價格](./competitive-price-analysis.md)， [清單變更](./listing-changes-log.md)、和 [通訊問題](./communication-errors-log.md).

存取您的Amazon商店，以檢視及管理Amazon銷售頻道上的所有功能、帳戶資訊、清單、訂單等 [首頁](./amazon-sales-channel-home.md).

## 促銷與定價

使用 [!DNL Amazon Sales Channel] 擴充功能上，您可以：

- 同步Amazon清單定價至 [!DNL Commerce] 型錄價格（或替代價格屬性）。

- 啟用MSRP [刪除式定價](./listing-price.md#configure-listing-price-settings) 在您的Amazon清單中增加客戶價值主張。

- 啟用和管理 [最低廣告價格(MAP)](./listing-price.md#configure-listing-price-settings) 在您的Amazon清單中。

- 設定其他 [VAT稅](./listing-price.md#configure-listing-price-settings) 在您的Amazon定價中。

- 設定自訂值，設定 [庫存/數量設定](./stock-quantity.md#configure-stock--quantity-settings) 與您的Amazon清單一起顯示，以增加購買者的急迫性。

## 定價規則

使用 [!DNL Amazon Sales Channel] 擴充功能上，您可以：

- 建立可棧疊、彈性且複雜的架構 [pricing rules （定價規則）](./pricing-products.md) 為日常銷售或季節性促銷活動管理Amazon定價。

- 建立 [floor](./floor-price.md) 和 [上限](./optional-ceiling-price.md) 價格可保護您的最低與最高價格。

- 建立和管理 [智慧型重新訂價規則](./intelligent-repricing-rules.md) 會自動調整與其他Amazon競爭者相關的產品定價([最低競爭者](./lowest-competitor-pricing.md) 和 [Buy Box](./buy-box-competitor-pricing.md) 價格)。

## 目錄摘要管理

使用 [!DNL Amazon Sales Channel] 擴充功能上，您可以：

- 匯入您現有的Amazon清單（產品），並與中的現有或建立產品相符 [!DNL Commerce] 目錄。

- 發佈您的 [!DNL Commerce] Amazon的產品以建立Amazon清單。

- 建立 [覆寫](./creating-editing-overrides.md) 設定個別價格、處理時間、條件和賣家備註訊息。

- 匯入及對應產品 [屬性](./attributes-view.md) 從您的Amazon清單，自動比對您產品中的 [!DNL Commerce] 目錄。

- 設定多個搜尋引數以比對Amazon清單與您的 [!DNL Commerce] 目錄。

- 定義 [清單規則](./listing-rules.md) 以判斷您的 [!DNL Commerce] 產品符合在Amazon上列出的資格。

- 設定預設 [處理時間](./product-listing-actions.md) 以取得您新的Amazon清單。

- 根據 [!DNL Commerce] 屬性。

- 為每種條件型別新增賣家備註（選擇性）。

- 將Amazon清單匯入您的清單時，實施數量臨界值 [!DNL Commerce] 目錄。

- 檢視建議 [清單改善](./listing-improvements.md).

## 訂單管理與客戶服務

使用 [!DNL Amazon Sales Channel] 擴充功能上，您可以：

- Amazon和中的支援與處理訂單 [!DNL Commerce].

- [匯入](./order-settings.md#configure-order-settings) 您的Amazon訂單 [!DNL Commerce] 或將它們留在Amazon中。

- 定義 [!DNL Commerce] 與您的Amazon訂單產生關聯的網站商店，用於匯入和管理訂單。

- 檢視、取消與出貨訂單 [!DNL Commerce] 和/或Amazon，視您的 [履行設定](./fulfilled-by.md).

- 將您的Amazon訂單狀態對應至內的自訂狀態 [!DNL Commerce] （選擇性）。

- 檢視及管理訂單錯誤，以解決問題並與客戶聯絡。

- 將訂單追蹤資料傳送至 [!DNL Amazon Seller Central] 帳戶。

- [取消訂單](./cancel-unshipped-order.md) 並選取原因回應。

- 檢視 [最近的訂單](./amazon-store-dashboard.md) Amazon訂單的相關資訊。

## 報告

使用 [!DNL Amazon Sales Channel] 擴充功能中，您可以檢閱以下專案的報表資訊：

- 依使用中、非使用中、符合資格及未完成狀態列出的清單。

- 等待出貨的訂單。

- 最近訂單。

- Amazon [列出變更記錄](./listing-changes-log.md) 複查產品/清單摘要變更（例如價格與數量）。

- 產品 [Buy Box](./buy-box-competitor-pricing.md) 競爭者定價資料。

- 產品 [最低競爭者定價](./lowest-competitor-pricing.md) 資料。

## 支援全球銷售

使用 [!DNL Amazon Sales Channel] 擴充功能上，您可以：

- 管理多個 [!DNL Amazon Marketplace] 地區（國家）。

- 使用支援多種貨幣 [Commerce貨幣設定工具](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html).

- 管理您的產品地點與Amazon履行中心的出貨。

## 客戶管理

建置您的 [!DNL Commerce] 客戶資料庫依據 [匯入客戶資料](./order-settings.md#configure-order-settings) 與您的Amazon訂單相關聯。 透過您擴充的客戶清單，提升您的行銷潛力 [!DNL Amazon Marketplace] 清單和 [!DNL Commerce] 店面。


快速入門很容易。 入門流程會引導您建立 [!DNL Amazon Seller Central] 帳戶並整合您的Amazon sales channel store和 [!DNL Commerce] 目錄，用於管理Amazon清單、訂單、存貨及履行。 中央儀表板會顯示所有Amazon銷售管道商店整合和Amazon清單的狀態更新。 接觸全球的新客戶 [!DNL Amazon Marketplace] 簡化並自動化流程，幾乎不需要安裝新系統的成本及人力。

整合您的 [!DNL Amazon Seller Central] 帳戶， [!DNL Amazon Sales Channel] 擴充功能可讓您管理帳戶，並在以下兩者之間同步資料： [!DNL Commerce] 和Amazon。 它可讓您直接透過建立清單、管理促銷、設定價格，以及管理存貨與履行 [!DNL Commerce] 管理員。 這些選項包括訂價規則，可監控相同專案的Amazon訂價，並自動調整您的價格以提高競爭力。


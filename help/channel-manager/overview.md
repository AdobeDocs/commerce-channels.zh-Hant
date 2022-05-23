---
title: 關於 [!DNL Channel Manager]
description: 瞭解如何安裝和使用 [!DNL Channel Manager] 將Adobe Commerce和Magento Open Source商店與第三方市場整合，並建立銷售渠道，從您的商務管理員無縫地管理市場清單、定價、庫存和銷售。
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 61d72e655a9f9eaefddd7561e0bc5fe36da69577
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---


# 關於 [!DNL Channel Manager]

[!DNL Channel Manager] 通過將您的Adobe Commerce或Magento Open Source產品目錄與 [!DNL Walmart US Marketplace]。

![[!DNL Channel Manager] 擴展管理員視圖](assets/channel-manager-home.png)

安裝和配置後 [!DNL Channel Manager]，也請參見Wiki頁。 [!DNL Commerce] 管理員已擴展，因此您可以管理 [!DNL Walmart Marketplace] 與您的Commerce環境無縫地進行銷售操作。

* **清單管理** — 通過將商品目錄中的產品與現有的沃爾瑪市場清單匹配，輕鬆發佈產品清單。

* **Inventory management** — 商戶市場銷售商帳戶中的物料將自動同步並從Commerce更新，以確保準確的庫存水準。

* **定價更新** — 使用自動價格同步為市場清單維護準確的定價。 當Adobe Commerce的價格發生變化時，這些變化將在10分鐘內反映在市場上。

* **訂單管理** — 當在市場中建立新訂單時，Channel Manager會將訂單與Adobe Commerce同步，並向市場發送訂單確認，以確保為每個訂單保留庫存。

* **發運管理** — 當訂單在Adobe Commerce標籤為已發運時，發運更新將發送到 [!DNL Walmart Marketplace]。 此通知確保銷售商滿足其履行SLA要求，並確保客戶收到其當前訂單的發運更新通知。

* **取消** — 當在Adobe Commerce取消訂單時，渠道經理會將更新的訂單資訊發送到市場，以複製相應市場訂單的操作。

[!DNL Channel Manager] 支援Adobe Commerce或Magento Open Source賣家 [!DNL Walmart Marketplace]。

## Channel Manager操作的預期延遲

資料同步過程 [!DNL Channel Manager] 和連結 [!DNL Walmart Marketplace] 商店需要一些時間才能完成。 查看的預期處理時間 [!DNL Channel Manager] 操作以幫助計畫銷售渠道運營工作。

**Channel Manager操作的估計延遲**

| **操作** | **說明** | **預期延遲** |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| 將產品添加到Channel Manager | 從Commerce產品目錄中選擇產品，然後將其導入Channel Manager。 | **最多5分鐘** — 如果您選擇了許多產品，例如，整個產品目錄，則導入過程需要更長時間。 |
| 在沃爾瑪市場上匹配產品 | 在渠道經理中選擇產品清單，然後發送到沃爾瑪進行匹配。 | **最多30分鐘** — 如果選擇了多個產品，則匹配過程將花費更長的時間，具體取決於選定的數量。 |
| 庫存更新 | 當Oracle Commerce中的庫存數量發生變化時， [!DNL Channel Manager] 將更新同步到沃爾瑪。 | **最多10分鐘** |
| 價格更新 | 當產品價格發生變化時，渠道經理會將更新同步到Walmart。 | **最多5分鐘** |
| 從Walmart到Commerce的訂單同步 | 客戶在沃爾瑪市場上訂購商務產品。 沃爾瑪將訂單發給渠道經理。 訂單按訂單儀表板顯示。 | **最多30分鐘** |
| 在Oracle Commerce Order Management中建立的訂單 | 渠道經理從Walmart訂單建立商務訂單，並更新訂單控制面板以包括商務訂單編號。 | **最多5分鐘** |

## 沃爾瑪先決條件

您需要從沃爾瑪獲得以下資訊才能將Commerce與Walmart Marketplace整合：

* 批准在沃爾瑪上銷售和登錄註冊的Marketplace Seller帳戶的憑據

* 將Adobe Commerce或Magento Open Source連接到Walmart Marketplace的API密鑰

   Walmart Marketplace API密鑰支援Adobe Commerce或Magento Open Source的渠道經理與Walmart Marketplace之間的整合。 在啟動Channel Manager登錄過程之前，在Seller Central中設定API密鑰。

### 設定Marketplace賣家帳戶

1. [提交您的沃爾瑪銷售商申請](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI)。
2. 在獲得沃爾瑪批准後， [設定沃爾瑪賣家帳戶](https://sellerhelp.walmart.com/seller/s/guide?article=000008219)。

### 生成Walmart Marketplace API密鑰

1. 轉到Walmart Marketplace以生成 [解決方案提供商生產API密鑰，用於Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey)。

1. 建立密鑰並配置權限：

   * 選擇「Adobe」作為解決方案提供商。

   * 如下表所示設定權限。 有關詳細資訊，請參閱 [API憑據](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) 的 *[!DNL Walmart Marketplace]賣家幫助*。

   **AdobeAPI鍵配置**

   | **權限** | **設定** |
   |----------------|-------------|
   | 內容 | 完全訪問 |
   | 獲取源 | 僅查看 |
   | 庫存 | 完全訪問 |
   | 項目 | 完全訪問 |
   | 延遲時間 | 完全訪問 |
   | 訂單 | 完全訪問 |
   | 價格 | 完全訪問 |
   | 報表 | 僅查看 |
   | 返回 | 完全訪問 |
   | 規則 | 完全訪問 |
   | 裝運 | 完全訪問 |

## Walmart Marketplace商店狀態

當您向沃爾瑪市場發佈產品時，列出產品的可用性取決於您的沃爾瑪市場商店的狀態：

* 對於即時商店，您的產品優惠將列出，並在匹配操作完成時可供銷售。

* 對於不即時的商店，您的產品優惠將被提供，而且客戶無法看到。 當商店開始上線時，分時段的清單會自動推送到現場商店。


![[!DNL Walmart Seller Central] 分段產品](assets/walmart-seller-central-staged.png)

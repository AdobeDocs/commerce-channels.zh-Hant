---
title: '"[!DNL Walmart] 要求"'
description: '"驗證您是否具有[!DNL Walmart Marketplace]與Channel Manager整合的資訊和資源。」'
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: fffbdac54443b7b9bed8854eba8341446e78cc80
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# [!DNL Walmart] 要求

[!DNL Channel Manager] 需要以下資源和資訊來配置 [!DNL Commerce] 銷售渠道 [!DNL Walmart Marketplace.]

* 批准銷售 [!DNL Walmart] 登錄註冊的Marketplace賣家帳戶的憑據

* 將Adobe Commerce或Magento Open Source連接到的API密鑰 [!DNL Walmart Marketplace]

   的 [!DNL Walmart Marketplace] API密鑰支援在 [!DNL Channel Manager] Adobe Commerce、Magento Open Source和沃爾瑪市場。 在啟動Channel Manager登錄過程之前，在Seller Central中設定API密鑰。

## 設定Marketplace賣家帳戶

1. [提交您的沃爾瑪銷售商申請](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI)。
1. 在獲得 [!DNL Walmart]。 [設定沃爾瑪賣家帳戶](https://sellerhelp.walmart.com/seller/s/guide?article=000008219)。

## 生成 [!DNL Walmart Marketplace] 生產API密鑰

1. 轉到 [!DNL Walmart Marketplace]生成 [解決方案提供商生產API密鑰，用於Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey)。

1. 建立密鑰並配置權限：

   * 選擇「Adobe」作為解決方案提供商。

   * 如下表所示設定權限。 有關詳細資訊，請參閱 [API憑據](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) 的 _沃爾瑪市場銷售商幫助_。

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

## [!DNL Walmart Marketplace] 儲存狀態

將產品發佈到市場時，列出可用性取決於您的 [!DNL Walmart Marketplace] 商店：

* 對於即時商店，您的產品優惠將列出，並在匹配操作完成時可供銷售。

* 對於不即時的商店，您的產品優惠將被提供，而且客戶無法看到。 當 [!DNL Walmart Marketplace] 商店開始上線，臨時清單被自動推送到現場商店。

![[!DNL Walmart Seller Central] 分段產品](assets/walmart-seller-central-staged.png)
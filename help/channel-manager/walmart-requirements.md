---
title: '[!DNL Walmart] 要求'
description: '''確認您擁有所需的 [!DNL Walmart Marketplace]與Channel Manager整合的資訊和資源。'
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 618bbd6d6c889d555f0ff74ade3dd84b412e1e59
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# [!DNL Walmart] 需求

[!DNL Channel Manager] 需要下列資源和資訊才能設定 [!DNL Commerce] 銷售管道 [!DNL Walmart Marketplace.]

* A [!DNL Walmart] 賣家帳戶

* 將Adobe Commerce或Magento Open Source連線至的API金鑰 [!DNL Walmart Marketplace]

   此 [!DNL Walmart Marketplace] API金鑰可讓您整合 [!DNL Channel Manager] Adobe [!DNL Commerce] 或是Magento Open Source和沃爾瑪市場。 在開始Channel Manager上線程式之前，請在Seller Central中設定API金鑰。

## 設定 [!DNL Walmart Seller] 帳戶

前往 [!DNL Walmart Seller Center] 設定 [沃爾瑪賣家賬戶](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

## 產生 [!DNL Walmart Marketplace] 生產API金鑰

1. 前往 [!DNL Walmart Marketplace] 生成 [解決方案提供者生產API金鑰(用於Adobe)](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. 建立金鑰並設定權限：

   * 選擇Adobe作為解決方案提供者。

   * 如下表所示設定權限。 如需詳細資訊，請參閱 [API憑證](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) 在 _沃爾瑪Marketplace賣家幫助_.

   **Walmart的AdobeAPI密鑰配置**

   | **權限** | **設定** |
   |----------------|-------------|
   | 內容 | 完全存取 |
   | 取得摘要 | 僅查看 |
   | 庫存 | 完全存取 |
   | 項目 | 完全存取 |
   | 延遲時間 | 完全存取 |
   | 順序 | 完全存取 |
   | 價格 | 完全存取 |
   | 報表 | 僅查看 |
   | 傳回 | 完全存取 |
   | 規則 | 完全存取 |
   | 裝運 | 完全存取 |

## [!DNL Walmart Marketplace] 儲存狀態

將產品連接到市場時，清單的可用性取決於您 [!DNL Walmart Marketplace] 商店：

* 若為即時商店，您的產品選件會列出並在符合操作完成時可供銷售。

* 對於未上線的商店，您的產品選件會分階段，且不會顯示給客戶。 當 [!DNL Walmart Marketplace] 商店上線，分段清單會自動推送至即時商店。

![[!DNL Walmart Seller Central] 分段產品](assets/walmart-seller-central-staged.png)

>[!IMPORTANT]
>
>之後 [!DNL Channel Manager] 已安裝並配置，所有庫存、價格和訂單更新都會自動同步。 不連接 [!DNL Channel Manager] 直到您禁用任何其他更新產品和訂單資料的整合。 如果您已設定其他整合，請確認項目數量和價格 [!DNL Commerce] 符合 [!DNL Walmart Marketplace] 之後才能連接到現場商店。


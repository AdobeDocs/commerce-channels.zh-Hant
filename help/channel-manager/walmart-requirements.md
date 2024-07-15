---
title: '[!DNL Walmart]需求'
description: '確認您擁有必要的 [!DNL Walmart Marketplace]資訊和資源，以便與管道管理員整合。'
role: Leader, Admin, Developer
feature: Sales Channels, Install, User Account, Tools and External Services
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# [!DNL Walmart]需求

[!DNL Channel Manager]需要下列資源與資訊才能為[!DNL Walmart Marketplace.]設定[!DNL Commerce]銷售管道

* [!DNL Walmart]賣家帳戶

* 連線Adobe Commerce或Magento Open Source至[!DNL Walmart Marketplace]的API金鑰

  [!DNL Walmart Marketplace] API金鑰可為Adobe[!DNL Commerce]或Magento Open Source與Walmart Marketplace啟用[!DNL Channel Manager]整合。 開始管道管理員上線流程之前，請先在賣方中心設定API金鑰。

## 設定[!DNL Walmart Seller]帳戶

移至[!DNL Walmart Seller Center]設定您的[沃爾瑪賣家帳戶](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp)。

## 產生[!DNL Walmart Marketplace]生產API金鑰

1. 移至[!DNL Walmart Marketplace]以產生Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey)的[方案提供者生產API金鑰。

1. 建立金鑰並設定許可權：

   * 選取Adobe作為解決方案提供者。

   * 設定許可權，如下表所示。 如需詳細資訊，請參閱&#x200B;_Walmart Marketplace賣家說明_&#x200B;中的[API認證](https://sellerhelp.walmart.com/seller/s/guide?article=000006422)。

   Walmart的&#x200B;**AdobeAPI金鑰組態**

   | **許可權** | **設定** |
   |----------------|-------------|
   | 內容 | 完全存取 |
   | 取得摘要 | 僅供檢視 |
   | 詳細目錄 | 完全存取 |
   | 專案 | 完全存取 |
   | 延遲時間 | 完全存取 |
   | 訂購 | 完全存取 |
   | 價格 | 完全存取 |
   | 報表 | 僅供檢視 |
   | 傳回 | 完全存取 |
   | 規則 | 完全存取 |
   | 送貨 | 完全存取 |

## [!DNL Walmart Marketplace]存放區狀態

將產品連線至市集時，清單可用性會視您[!DNL Walmart Marketplace]商店的狀態而定：

* 若為已上線的商店，您的產品選件會列出，並可在比對作業完成後出售。

* 對於未上線的商店，您的產品選件會進行預備，且客戶不會看到。 當[!DNL Walmart Marketplace]存放區上線時，分階段清單會自動推送至上線存放區。

![[!DNL Walmart Seller Central]個分階段產品](assets/walmart-seller-central-staged.png){width="600" zoomable="yes"}

>[!IMPORTANT]
>
>在安裝及設定[!DNL Channel Manager]之後，所有存貨、價格及訂單更新都會自動同步化。 在您停用任何更新產品與訂單資料的其他整合功能之前，請勿將[!DNL Channel Manager]連線至沃爾瑪市集線上商店。 如果您已設定其他整合，請先確認[!DNL Commerce]中的專案數量與價格符合[!DNL Walmart Marketplace]中的數量，然後再連線到線上商店。


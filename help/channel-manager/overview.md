---
title: '''簡介 [!DNL Channel Manager]"'
description: '''瞭解如何安裝和使用 [!DNL Channel Manager] 將Adobe Commerce和Magento Open Source店與沃爾瑪市場整合，並建立銷售渠道，從您的商務管理員處無縫管理市場清單、定價、庫存和銷售。'
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---


# 簡介 [!DNL Channel Manager]

[!DNL Channel Manager] 通過將Adobe Commerce或Magento Open Source產品目錄與之整合，幫助商家增加銷售、接觸新客戶、簡化銷售操作並節省時間 [!DNL Walmart Marketplace]。

![[!DNL Channel Manager] 擴展管理員視圖](assets/channel-manager-home.png)

[!DNL Channel Manager] 支援Adobe Commerce或想賣東西的Magento Open Source商 [!DNL Walmart Marketplace] 通過 [!DNL Commerce] 管理員。 與 [!DNL Channel Manager] 安裝、儲存管理員和操作人員可以管理 [!DNL Walmart Marketplace] 銷售、庫存和產品定價與商務環境無縫對接。

擴展的管理員簡化了操作，因為商家可以使用相同的工作流和流程來管理兩者的銷售 [!DNL Commerce] 店面和沃爾瑪市場。

安裝和配置後 [!DNL Channel Manager]，您可以使用以下功能管理Walmart Marketplace銷售訂單：

* **清單管理** — 通過匹配您的產品，輕鬆連接產品清單 [!DNL Commerce] 目錄到現有 [!DNL Walmart Marketplace] 清單。

* **Inventory management** — 商家市場銷售商帳戶中的項目將自動同步和更新，從 [!DNL Commerce] 以確保準確的庫存水準。

* **定價更新** — 使用自動價格同步為市場清單維護準確的定價。 當Adobe Commerce的價格發生變化時，這些變化將反映在市場上。

* **訂單管理** — 在市場上建立新訂單時， [!DNL Channel Manager] 將訂單與Adobe Commerce同步，並向市場發送訂單確認。 此確認可確保為每個訂單預留庫存。 最後一步是在 [!DNL Commerce] 訂單管理系統，用於處理。

* **裝運管理** — 當訂單在Adobe Commerce標籤為已發運時，發運更新將發送到 [!DNL Walmart Marketplace]。 此通知確保銷售商滿足其履行SLA要求，並確保客戶收到其當前訂單的發運更新通知。

* **取消** — 在Adobe Commerce, [!DNL Channel Manager] 將更新的訂單資訊發送到市場以複製相應市場訂單的操作。 訂單取消完成後， [!DNL Commerce] 庫存數量更新以反映退回的物料和庫存更新自動同步到 [!DNL Walmart Marketplace]。

* **退貨和退款** — 當Walmart Marketplace要求退回通過Adobe Commerce或Magento Open Source銷售渠道訂購的產品時， [!DNL Channel Manager] 將返回請求資訊發送到Commerce銷售渠道商店以複製返回請求。 然後，可以使用 [!DNL Commerce] [退款工作流](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow)，離線方法。 退款完成後， [!DNL Channel Manager] 將更新與沃爾瑪同步，以便市場銷售商帳戶中的退貨狀態可以更新以反映退款。

## 預期延遲 [!DNL Channel Manager] 操作

資料同步過程 [!DNL Channel Manager] 和連結 [!DNL Walmart Marketplace] 商店需要一些時間才能完成。 查看的預期處理時間 [!DNL Channel Manager] 操作以幫助計畫銷售渠道運營工作。

**估計延遲 [!DNL Channel Manager] 操作**

| **操作** | **說明** | **預期延遲** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 將產品添加到 [!DNL Channel Manager] | 從 [!DNL Commerce] 產品目錄和導入 [!DNL Channel Manager]。 | **最多五分鐘** — 如果您選擇了許多產品，例如，整個產品目錄，則導入過程需要更長時間。 |
| 匹配上的產品 [!DNL Walmart Marketplace] | 在中選擇產品清單 [!DNL Channel Manager] 送沃爾瑪去匹配。 | **最多30分鐘** — 如果選擇了多個產品，則匹配過程將花費更長的時間，具體取決於選定的數量。 |
| 庫存更新 | 當Oracle Commerce中的庫存數量發生變化時， [!DNL Channel Manager] 將更新同步到沃爾瑪。 | **最多10分鐘** |
| 價格更新 | 當產品價格變化時， [!DNL Channel Manager] 將更新同步到沃爾瑪。 | **最多五分鐘** |
| 從Walmart到 [!DNL Commerce] | 客戶訂單a [!DNL Commerce] 在沃爾瑪市場上銷售。 沃爾瑪將訂單 [!DNL Channel Manager]。 訂單按訂單儀表板顯示。 | **最多30分鐘** |
| 建立的訂單 [!DNL Commerce] 訂單管理 | [!DNL Channel Manager] 建立 [!DNL Commerce] 訂單，並更新訂單控制板以包括 [!DNL Commerce] 訂單編號。 | **最多五分鐘** |
| 裝運狀態更新 [!DNL Commerce] 訂單管理 | 從Commerce發運訂單時， [!DNL Channel Manager] 在訂單控制板中更新「發運」狀態，並將更新發送到沃爾瑪市場，以便通知客戶。 | **最多五分鐘** |
| Oracle Commerce Order Management中的訂單取消更新 | 當從Commerce取消訂單時， [!DNL Channel Manager] 更新訂單控制板中的訂單狀態，並將更新發送到沃爾瑪市場，以便通知客戶。 訂單取消完成後， [!DNL Commerce] 庫存數量更新以反映退回的物料。 然後， [!DNL Channel Manager] 將更新同步到 [!DNL Walmart Marketplace]。 | **最多五分鐘** |



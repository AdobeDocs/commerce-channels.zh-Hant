---
title: '簡介 [!DNL Channel Manager]'
description: '''了解如何安裝和使用 [!DNL Channel Manager] 將Adobe Commerce和Magento Open Source店與沃爾瑪市場整合，並建立銷售渠道，從您的商務管理員無縫地管理市場清單、定價、庫存和銷售。'
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 2e3f8e51b765cda0559d8624d61e1ae9dc1c9667
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---


# 簡介 [!DNL Channel Manager]

[!DNL Channel Manager] 將Adobe Commerce或Magento Open Source產品目錄與整合，可協助商戶增加銷售、觸及新客戶、簡化銷售作業並節省時間 [!DNL Walmart Marketplace].

![[!DNL Channel Manager] 擴充功能管理檢視](assets/channel-manager-home.png)

[!DNL Channel Manager] 支援Adobe Commerce或Magento Open Source商 [!DNL Walmart Marketplace] 將 [!DNL Commerce] 管理員。 使用 [!DNL Channel Manager] 安裝、儲存管理員和操作人員可以管理 [!DNL Walmart Marketplace] 銷售、庫存和產品定價可從商務環境中無縫實現。

擴充的管理員可簡化操作，因為商家可以使用相同的工作流程和程式來管理來自這兩種工具的銷售 [!DNL Commerce] 店面和沃爾瑪超市。

安裝和配置後 [!DNL Channel Manager]，您可以使用以下功能管理Walmart Marketplace銷售訂單：

* **清單管理** — 通過匹配 [!DNL Commerce] 目錄至現有 [!DNL Walmart Marketplace] 清單。

* **Inventory management** — 自動同步和更新商家市場銷售商帳戶中的項目，從 [!DNL Commerce] 以確保準確的庫存水準。

* **定價更新** — 使用自動價格同步功能維護市場清單的準確定價。 當Adobe Commerce中的價格變更時，這些變更會反映在市集中。

* **訂單管理** — 在Marketplace中建立新訂單時， [!DNL Channel Manager] 與Adobe Commerce同步訂單，並傳送訂單確認給Marketplace。 此確認可確保為每筆訂單保留庫存。 最後一步是在 [!DNL Commerce] 訂單管理系統。

* **運費管理** — 在Adobe Commerce中將訂單標籤為已發運時，系統會將發運更新傳送至 [!DNL Walmart Marketplace]. 此通知可確保銷售商符合其履行SLA要求，並確保客戶收到其當前訂單的發運更新通知。

* **取消** — 在Adobe Commerce中取消訂單時， [!DNL Channel Manager] 將更新的訂單資訊發送到marketplace ，以複製相應的marketplace訂單的操作。 訂單取消完成後， [!DNL Commerce] 庫存數量更新以反映退回的物料和庫存更新自動同步到 [!DNL Walmart Marketplace].

* **退貨與退款** — 當Walmart Marketplace要求退回通過Adobe Commerce或Magento Open Source銷售渠道訂購的商品時， [!DNL Channel Manager] 將退貨請求資訊發送到商務銷售渠道商店以複製退貨請求。 然後，您可以使用 [!DNL Commerce] [退款工作流](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow)，離線方法。 退款完成後， [!DNL Channel Manager] 將更新同步到沃爾瑪，以便更新市場銷售商賬戶中的退貨狀態，以反映退款。

## 的預期延遲 [!DNL Channel Manager] 作業

資料同步處理 [!DNL Channel Manager] 和連結 [!DNL Walmart Marketplace] 儲存需要一些時間才能完成。 查看 [!DNL Channel Manager] 操作，幫助規劃銷售渠道操作。

**預計延遲 [!DNL Channel Manager] 作業**

| **操作** | **說明** | **預期延遲** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 將產品新增至 [!DNL Channel Manager] | 從 [!DNL Commerce] 產品目錄，並匯入 [!DNL Channel Manager]. | **最多五分鐘** — 如果選擇多種產品，例如整個產品目錄，則導入過程需要更長時間。 |
| 在上匹配產品 [!DNL Walmart Marketplace] | 在中選取產品清單 [!DNL Channel Manager] 然後送到沃爾瑪進行配對。 | **最多30分鐘** — 如果選擇了多個產品，則匹配過程所需時間會根據選擇的數量而延長。 |
| 庫存更新 | 當商務中的庫存數量更改時， [!DNL Channel Manager] 將更新同步到沃爾瑪。 | **最多10分鐘** |
| 價格更新 | 當產品價格改變時， [!DNL Channel Manager] 將更新同步到沃爾瑪。 | **最多五分鐘** |
| 從沃爾瑪到 [!DNL Commerce] | 客戶訂購a [!DNL Commerce] 在沃爾瑪市場上。 沃爾瑪下訂單 [!DNL Channel Manager]. 訂單顯示在訂單控制面板中。 | **最多30分鐘** |
| 在中建立的順序 [!DNL Commerce] Order Management | [!DNL Channel Manager] 會建立 [!DNL Commerce] 從沃爾瑪訂單中下單，並更新訂單控制面板以包括 [!DNL Commerce] 訂單編號。 | **最多五分鐘** |
| 發運狀態更新於 [!DNL Commerce] Order Management | 從Commerce發運訂單時， [!DNL Channel Manager] 更新訂單控制面板中的「運送」狀態，並將更新傳送至Walmart marketplace，以便通知客戶。 | **最多五分鐘** |
| Oracle Commerce Order Management中的訂單取消更新 | 從商務取消訂單時， [!DNL Channel Manager] 更新訂單控制面板中的訂單狀態，並將更新發送至Walmart marketplace，以便通知客戶。 訂單取消完成後， [!DNL Commerce] 庫存數量更新以反映退貨。 然後， [!DNL Channel Manager] 將更新同步至 [!DNL Walmart Marketplace]. | **最多五分鐘** |



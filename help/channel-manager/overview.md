---
title: '簡介 [!DNL Channel Manager]'
description: 「瞭解如何安裝並使用 [!DNL Channel Manager] 將Adobe Commerce和Magento Open Source商店與Walmart Marketplace整合，並建立銷售管道，以順暢地從Commerce管理員管理市集清單、定價、存貨和銷售。」
role: Leader, Admin, User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 850aece134084e108b324a964d7d834042c7ddfd
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---


# [!DNL Channel Manager]簡介

[!DNL Channel Manager]透過整合Adobe Commerce或Magento Open Source產品目錄與[!DNL Walmart Marketplace]，協助商戶增加銷售、接觸新客戶、簡化銷售作業，以及節省時間。

![[!DNL Channel Manager]延伸模組管理員檢視](assets/channel-manager-home.png){width="700" zoomable="yes"}

[!DNL Channel Manager]透過擴充[!DNL Commerce] Admin來支援想要在[!DNL Walmart Marketplace]上銷售的Adobe Commerce或Magento Open Source商家。 安裝[!DNL Channel Manager]後，商店管理員和營運人員可以從Commerce環境中順暢管理[!DNL Walmart Marketplace]銷售、詳細目錄和產品定價。

擴充的「管理員」可簡化營運，因為商家可使用相同的工作流程與程式，來管理[!DNL Commerce]店面與Walmart Marketplace的銷售。

安裝及設定[!DNL Channel Manager]之後，您可以使用下列功能來管理Walmart Marketplace的銷售訂單：

* **清單管理** — 透過將您的[!DNL Commerce]目錄中的產品與現有的[!DNL Walmart Marketplace]清單比對，輕鬆連線產品清單。

* **Inventory management** — 商家市集賣家帳戶中的專案會自動同步處理並從[!DNL Commerce]更新，以確保庫存量準確。

* **訂價更新** — 透過自動價格同步處理，維持市集清單的精確訂價。 當Adobe Commerce中的價格變更時，這些變更會反映在Marketplace中。

* **訂單管理** — 在市集中建立新訂單時，[!DNL Channel Manager]會與Adobe Commerce同步訂單，並將訂單確認傳送至市集。 此確認會確保為每筆訂單預留存貨。 最後一個步驟是在[!DNL Commerce] Order Management系統中建立對應的訂單以進行處理。

* **出貨管理** — 當訂單在Adobe Commerce中標示為出貨時，出貨更新會傳送至[!DNL Walmart Marketplace]。 此通知可確保賣方符合其履行SLA要求，並且客戶會收到其目前訂單的送貨更新通知。

* **取消** — 在Adobe Commerce中取消訂單時，[!DNL Channel Manager]會將更新的訂單資訊傳送至市集，以復寫對應市集訂單的動作。 訂單取消完成後，[!DNL Commerce]庫存數量更新以反映傳回的料號，存貨更新會自動同步處理至[!DNL Walmart Marketplace]。

* **退貨與退款** — 當沃爾瑪市集要求透過Adobe Commerce或Magento Open Source銷售管道訂購的商品退貨時，[!DNL Channel Manager]會將退貨要求資訊傳送至Commerce銷售管道商店，以複製退貨要求。 然後，可以使用[!DNL Commerce] [退款工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html#refund-workflow)離線方法處理退款。 退款完成之後，[!DNL Channel Manager]會同步化更新至Walmart，以便可以更新市集賣家帳戶中的退貨狀態以反映退款。

## [!DNL Channel Manager]個作業的預期延遲

[!DNL Channel Manager]與連結[!DNL Walmart Marketplace]存放區之間的資料同步處理需要一些時間才能完成。 檢閱[!DNL Channel Manager]作業的預期處理時間，以協助規劃銷售管道作業工作。

**預估的[!DNL Channel Manager]作業延遲**

| **作業** | **描述** | **預期延遲** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 將產品新增至[!DNL Channel Manager] | 從[!DNL Commerce]產品目錄中選取產品並將其匯入[!DNL Channel Manager]。 | **最多5分鐘** — 如果您選取許多產品（例如，整個產品目錄），則匯入程式需要更長的時間。 |
| 符合[!DNL Walmart Marketplace]上的產品 | 在[!DNL Channel Manager]中選取產品清單，並傳送至Walmart進行比對。 | **最多30分鐘** — 如果您選取許多產品，則相符程式會花費較長的時間（視選取的數量而定）。 |
| 詳細目錄更新 | 當Commerce中的存貨數量變更時，[!DNL Channel Manager]會將更新同步到Walmart。 | **最多10分鐘** |
| 價格更新 | 當產品價格變更時，[!DNL Channel Manager]會將更新同步到Walmart。 | **最多5分鐘** |
| 從Walmart向[!DNL Commerce]訂購同步處理 | 客戶在Walmart Marketplace訂購[!DNL Commerce]產品。 Walmart傳送訂單給[!DNL Channel Manager]。 訂單會顯示在訂單儀表板中。 | **最多30分鐘** |
| 在[!DNL Commerce] Order Management中建立的訂單 | [!DNL Channel Manager]從沃爾瑪訂單建立[!DNL Commerce]訂單，並更新訂單儀表板，以包含[!DNL Commerce]訂單編號。 | **最多5分鐘** |
| [!DNL Commerce] Order Management中的運送狀態更新 | 當訂單從Commerce出貨時，[!DNL Channel Manager]會更新訂單儀表板中的出貨狀態，並將更新傳送至Walmart Marketplace，以便通知客戶。 | **最多5分鐘** |
| Commerce Order Management中的訂單取消更新 | 取消來自Commerce的訂單時，[!DNL Channel Manager]會更新訂單儀表板中的訂單狀態，並將更新傳送至Walmart Marketplace，以便通知客戶。 訂單取消完成後，[!DNL Commerce]庫存數量會更新以反映傳回的專案。 然後，[!DNL Channel Manager]將更新同步到[!DNL Walmart Marketplace]。 | **最多5分鐘** |



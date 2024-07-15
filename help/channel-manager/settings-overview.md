---
title: 設定概述
description: 「瞭解如何設定 [!DNL Channel Manager settings] 驗證，以及對應產品目錄屬性與運送公司，以協調 [!DNL Commerce] 與 [!DNL Walmart Marketplace]之間的銷售作業。」
role: Admin
feature: Sales Channels, Configuration, Merchandising, Shipping/Delivery
exl-id: 305b3580-bfe2-4fc2-9dc8-fb41f5eaf959
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# 設定概述

銷售管道設定可啟用[!DNL Commerce]與[!DNL Walmart Marketplace]之間的通訊與資料同步處理，因此您可以從[!DNL Commerce]管理員管理[!DNL Walmart Marketplace]銷售作業。

在[!DNL Channel Manager]中，您會在上線流程中設定一些銷售管道設定。 上線後，您可以從[!UICONTROL Listings]和[!UICONTROL Orders]儀表板中選取&#x200B;**[!UICONTROL Channel Settings]**，以檢視和管理設定。

* **[Walmart連線](manage-wmt-connection.md)** — 在[!DNL Channel Manager]上線程式期間，您提供[!DNL Walmart Marketplace]賣家帳戶中的[API認證](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key)，以將[!DNL Commerce]連線至[!DNL Walmart Marketplace]以進行通訊和資料同步處理。 如有需要，您可以從&#x200B;*頻道設定*&#x200B;頁面更新這些認證。

* **[對應唯一識別碼](map-catalog-attributes.md)** — 將清單從[!DNL Commerce]連線到[!DNL Walmart Marketplace]之前，請將[!DNL Commerce]目錄中的至少一個唯一識別碼對應到Walmart中的對應識別碼。 必須執行此步驟才能比對[!DNL Commerce]產品與現有[!DNL Walmart]清單，以及同步處理[!DNL Commerce]與[!DNL Walmart]之間的產品資料。

* **[對應運送公司](map-shipping-carriers.md)** — 處理來自[!DNL Commerce]的[!DNL Walmart Marketplace]訂單之前，請確定您將來自[!DNL Commerce]執行個體的運送公司對應至[!DNL Walmart Marketplace]上對應的運送公司。

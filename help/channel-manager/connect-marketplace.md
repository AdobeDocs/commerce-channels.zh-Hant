---
title: '連線 [!DNL Channel Manager] 至 [!DNL Walmart Marketplace]'
description: 「將Commerce商店檢視連結至 [!DNL Walmart Marketplace] 以建立銷售管道，管理Commerce產品清單、存貨、價格以及沃爾瑪市集銷售的訂單。」
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
role: Admin, Developer
feature: Sales Channels, Install, Integration
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 將[!DNL Channel Manager]連線至[!DNL Walmart Marketplace]

在您的[!DNL Commerce]執行個體上安裝管道管理員後，在管道管理員中建立銷售管道，並設定認證以連線[!DNL Channel Manager]到[!DNL Walmart Marketplace]。

1. [選取產品清單的[!DNL Commerce]商店，以建立銷售管道](#create-the-sales-channel)。

1. [透過新增[!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace)將頻道連線到 [!DNL Walmart Marketplace] 。

1. [完成銷售管道設定](#complete-sales-channel-store-setup)，以管理您[!DNL Walmart Marketplace]產品分類的清單、存貨、定價和訂單。

>[!NOTE]
>
>「管道管理員」需要在Walmart帳戶和[!DNL Commerce]商店檢視之間建立一對一連線。 您無法將相同的商店檢視連線到多個Walmart帳戶。

## 建立銷售管道

1. 從「管理員」中，選取&#x200B;**[!UICONTROL Marketing** > _管道&#x200B;_> **管道管理員]**，以開啟[!DNL Channel Manager]。

1. 在&#x200B;**[!UICONTROL Marketplaces available to connect]**&#x200B;區段中，選取&#x200B;**[!UICONTROL Get Started]**。

   ![將新[!DNL Walmart]存放區連線至[!DNL Channel Manager]](assets/channel-manager-home.png){width="700" zoomable="yes"}

1. 如有需要，請設定您的[!DNL Walmart Marketplace Seller]帳戶。

1. 設定存放區和連線：

   - 選取&#x200B;**[!UICONTROL Add Credentials]**。

   - 選取[!DNL Commerce]商店檢視，該檢視提供您要在市集上銷售的產品。

     ![從[!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png){width="500" zoomable="yes"}設定[!DNL Commerce]與[!DNL Walmart Marketplace]之間的連線

   - 輸入唯一的&#x200B;**[!UICONTROL store name]**。

   - 選取產品清單與訂單處理的&#x200B;**[!UICONTROL Adobe [!DNL Commerce] site]**。

   - 若要接收與[!DNL Channel Manager]相關的通知，請新增&#x200B;**[!UICONTROL email address]**。

1. 將頻道連線到[!DNL Walmart Marketplace]。

   - 從您的[!DNL Walmart Marketplace Seller]帳戶新增[[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key)的認證。

   - 如果您沒有認證，請選取&#x200B;**[!UICONTROL Get API credentials]**，從[!DNL Walmart Marketplace Developer Portal]取得認證。

     在開發人員入口網站上，選取您所在的地區（美國和加拿大），然後登入。

     ![[!DNL Walmart Marketplace]帳戶登入](assets/walmart-marketplace-login-page.png){width="600"}

   - 在API金鑰表單上，將[!UICONTROL Adobe Inc Production API key]的&#x200B;**[!UICONTROL Client ID]**&#x200B;和&#x200B;**[!UICONTROL Client Secret]**&#x200B;值複製並儲存到安全位置。

     ![[!DNL Walmart Marketplace API key]設定頁面](assets/walmart-api-key-management-form.png){width="600" zoomable="yes"}

     >[!NOTE]
     >
     >如果[!DNL Adobe Inc]金鑰未列在開發人員入口網站中，請選取&#x200B;**[!UICONTROL Add New Key for a Solution Provider]**&#x200B;以設定許可權並產生金鑰。 如需組態詳細資訊，請參閱[產生a [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key)。

   - 返回[!DNL Channel Manager]以新增認證至&#x200B;**[!UICONTROL Walmart Connection]**&#x200B;資訊。

     當您新增認證時，Adobe會隱藏使用者端密碼，並將值儲存在安全的儲存庫中。

1. 選取&#x200B;**[!UICONTROL Save Store]**&#x200B;以套用組態並連線至[!DNL Walmart marketplace]。

1. 成功連線後，從&#x200B;**[!UICONTROL Channel Manager]**&#x200B;商店頁面[完成商店設定](complete-sales-channel-store-setup.md)。

![安裝第一個存放區](assets/channel-manager-setup-first-store.png){width="500" zoomable="yes"}

### 疑難排解連線問題

如果與[!DNL Walmart]的連線失敗，請參閱[Walmart Marketplace常見問題集](https://developer.walmart.com/faq/us/faq-auth/){target="_blank"}以取得疑難排解提示。

- 從[!DNL Walmart Developer Portal]，確認您已為[!UICONTROL Adobe Inc.]複製生產API金鑰的正確認證

- 驗證[!UICONTROL Walmart Adobe API key]的存取設定是否具有正確的許可權。 請參閱[[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key)。

- 確認可從[Walmart API狀態頁面](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target="_blank"}取得[!DNL Walmart API]服務。

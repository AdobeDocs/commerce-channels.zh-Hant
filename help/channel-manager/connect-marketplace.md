---
title: 'Connect [!DNL Channel Manager] to [!DNL Walmart Marketplace]'
description: '"將Commerce商店視圖連接到 [!DNL Walmart Marketplace] 建立銷售渠道，以管理Walmart Marketplace銷售的Commerce產品清單、庫存、價格和訂單。」'
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 3f6039ad78ff500c31129bee12d65e291e226567
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Connect [!DNL Channel Manager] to [!DNL Walmart Marketplace]

在您的 [!DNL Commerce] 例項，在Channel Manager中建立銷售管道並設定憑證以連線 [!DNL Channel Manager] to [!DNL Walmart Marketplace].

1. [建立銷售渠道](#create-the-sales-channel) 選取 [!DNL Commerce] 儲存以取得產品清單。

1. [將通道連接至 [!DNL Walmart Marketplace] 添加 [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [完成銷售渠道設定](#complete-sales-channel-store-setup) 管理清單、庫存、定價和訂單 [!DNL Walmart Marketplace] 產品分類。

>[!NOTE]
>
>渠道經理要求在沃爾瑪帳戶和 [!DNL Commerce] 儲存檢視。 您不能將同一商店視圖連接到多個Walmart帳戶。

## 建立銷售渠道

1. 從管理員開啟 [!DNL Channel Manager] 選取 **[!UICONTROL Marketing** > _管道&#x200B;_> **渠道管理員]**.

1. 在 **[!UICONTROL Marketplaces available to connect]** 部分，選擇 **[!UICONTROL Get Started]**.

   ![連接新 [!DNL Walmart] 儲存至 [!DNL Channel Manager]](assets/channel-manager-home.png)

1. 如有需要，請設定 [!DNL Walmart Marketplace Seller] 帳戶。

1. 配置儲存和連接：

   - 選擇 **[!UICONTROL Add Credentials]**.

   - 選取 [!DNL Commerce] 提供您要在市場上銷售之產品的商店檢視。

      ![配置之間的連接 [!DNL Commerce] 和 [!DNL Walmart Marketplace] 從 [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - 輸入唯一 **[!UICONTROL store name]**.

   - 選取 **[!UICONTROL Adobe [!DNL Commerce] site]** 用於產品清單和訂單處理。

   - 接收與 [!DNL Channel Manager]，新增 **[!UICONTROL email address]**.

1. 將通道連接至 [!DNL Walmart Marketplace].

   - 新增 [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) 從 [!DNL Walmart Marketplace Seller] 帳戶。

   - 如果您沒有認證，請從 [!DNL Walmart Marketplace Developer Portal] 選取 **[!UICONTROL Get API credentials]**.

      在開發人員入口網站上，選取您的地區（美國和加拿大），然後登入。

      ![[!DNL Walmart Marketplace] 帳戶登入](assets/walmart-marketplace-login-page.png)

   - 在API金鑰表單中，複製並儲存 **[!UICONTROL Client ID]** 和 **[!UICONTROL Client Secret]** 值 [!UICONTROL Adobe Inc Production API key] 到安全的地方。

      ![[!DNL Walmart Marketplace API key] 設定頁面](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >若 [!DNL Adobe Inc] 代碼未列在開發人員入口網站中，請選取 **[!UICONTROL Add New Key for a Solution Provider]** 設定權限和產生金鑰。 如需設定詳細資訊，請參閱 [產生 [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key).

   - 返回 [!DNL Channel Manager] 將憑證新增至 **[!UICONTROL Walmart Connection]** 資訊。

      添加憑據時，Adobe會隱藏客戶端密碼並將值儲存在安全保管庫中。

1. 選擇 **[!UICONTROL Save Store]** 以套用設定並連線至 [!DNL Walmart marketplace].

1. 成功連接後， [完整商店設定](complete-sales-channel-store-setup.md) 從 **[!UICONTROL Channel Manager]** 儲存頁面。

![設定第一個商店](assets/channel-manager-setup-first-store.png)

### 疑難排解連線問題

如果連線至 [!DNL Walmart] 失敗，請參閱 [Walmart Marketplace常見問題集](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;}以取得疑難排解提示。

- 從 [!DNL Walmart Developer Portal]，確認您已複製的生產API金鑰憑證正確無誤 [!UICONTROL Adobe Inc.]

- 驗證 [!UICONTROL Walmart Adobe API key] 具有正確的權限。 請參閱 [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key).

- 確認 [!DNL Walmart API] 服務可從 [Walmart API狀態頁](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}。

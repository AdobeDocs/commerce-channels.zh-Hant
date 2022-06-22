---
title: '''連接 [!DNL Channel Manager] 至 [!DNL Walmart Marketplace]"'
description: '"將Commerce商店視圖連接到 [!DNL Walmart Marketplace] 建立銷售渠道，管理Commerce產品清單、庫存、價格和Walmart Marketplace銷售訂單。」'
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 8146be1c94ffb1c8abd0d28e53d3476fd78f2c62
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# 連接 [!DNL Channel Manager] 至 [!DNL Walmart Marketplace]

在您的 [!DNL Commerce] 實例，在Channel Manager中建立銷售渠道並配置憑據以連接 [!DNL Channel Manager] 至 [!DNL Walmart Marketplace]。

1. [建立銷售渠道](#create-the-sales-channel) 選擇 [!DNL Commerce] 產品清單的儲存。

1. [將通道連接到 [!DNL Walmart Marketplace] 通過 [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace)。

1. [完成銷售渠道設定](#complete-store-setup) 管理清單、庫存、定價和訂單 [!DNL Walmart Marketplace] 產品分類。

>[!NOTE]
>
>渠道經理要求在Walmart帳戶和Walmart帳戶之間建立一對一的連接 [!DNL Commerce] 儲存視圖。 無法將同一商店視圖連接到多個沃爾瑪帳戶。

## 建立銷售渠道

1. 從管理員開啟 [!DNL Channel Manager] 通過 **[!UICONTROL Marketing** > _頻道&#x200B;_> **渠道管理器]**。

1. 在 **[!UICONTROL Marketplaces available to connect]** 選擇 **[!UICONTROL Get Started]**。

   ![連接新 [!DNL Walmart] 儲存 [!DNL Channel Manager]](assets/channel-manager-home.png)

1. 如果需要，請設定 [!DNL Walmart Marketplace Seller] 帳戶。

1. 配置儲存和連接：

   - 選擇 **[!UICONTROL Add Credentials]**。

   - 選擇 [!DNL Commerce] 提供要在市場上銷售的產品的商店視圖。

      ![配置之間的連接 [!DNL Commerce] 和 [!DNL Walmart Marketplace] 從 [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - 輸入唯一 **[!UICONTROL store name]**。

   - 選擇 **[!UICONTROL Adobe [!DNL Commerce] site]** 用於產品清單和訂單處理。

   - 接收與 [!DNL Channel Manager]，添加 **[!UICONTROL email address]**。

1. 將通道連接到 [!DNL Walmart Marketplace]。

   - 添加憑據 [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) 從 [!DNL Walmart Marketplace Seller] 帳戶。

   - 如果您沒有憑據，請從 [!DNL Walmart Marketplace Developer Portal] 通過 **[!UICONTROL Get API credentials]**。

      在開發人員門戶上，選擇您的區域（美國和加拿大），然後登錄。

      ![[!DNL Walmart Marketplace] 帳戶登錄](assets/walmart-marketplace-login-page.png)

   - 在API密鑰窗體上，複製並保存 **[!UICONTROL Client ID]** 和 **[!UICONTROL Client Secret]** 值 [!UICONTROL Adobe Inc Production API key] 到安全的地方。

      ![[!DNL Walmart Marketplace API key] 配置頁](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >如果 [!DNL Adobe Inc] 未在開發人員門戶中列出鍵，請選擇 **[!UICONTROL Add New Key for a Solution Provider]** 配置權限並生成密鑰。 有關配置詳細資訊，請參閱 [生成 [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key)。

   - 返回到 [!DNL Channel Manager] 將憑據添加到 **[!UICONTROL Walmart Connection]** 的下界。

      添加憑據時，Adobe會隱藏客戶端機密並將值儲存在安全保管庫中。

1. 選擇 **[!UICONTROL Save Store]** 應用配置並連接到 [!DNL Walmart marketplace]。

1. 成功連接後， [完整商店設定](complete-store-setup.md) 從 **[!UICONTROL Channel Manager]** 儲存頁面。

![設定第一個儲存](assets/channel-manager-setup-first-store.png)

### 排除連接問題

如果與 [!DNL Walmart] 失敗，查看 [Walmart Marketplace常見問題](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;}以獲取疑難解答提示。

- 從 [!DNL Walmart Developer Portal]，驗證您是否複製了生產API密鑰的正確憑據 [!UICONTROL Adobe Inc.]

- 驗證的訪問配置 [!UICONTROL Walmart Adobe API key] 具有正確的權限。 請參閱 [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key)。

- 確認 [!DNL Walmart API] 服務可從 [Walmart API狀態頁](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}。

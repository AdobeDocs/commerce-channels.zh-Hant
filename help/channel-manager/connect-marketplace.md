---
title: 將銷售渠道連接到 [!DNL Walmart Marketplace]
description: 配置銷售渠道並連接到Walmart Marketplace。
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 7349dd92c2166ff6ae83b705416993e48aa5f954
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 將銷售渠道連接到 [!DNL Walmart Marketplace]

在您的 [!DNL Commerce] 例如，將Commerce商店連接到Walmart Marketplace。

1. [建立銷售渠道](#create-the-sales-channel) 通過為產品清單選擇Commerce商店。

1. [將通道連接到 [!DNL Walmart Marketplace] 通過添加Walmart API憑據](#connect-the-channel-to-walmart-marketplace)。

1. [完成銷售渠道設定](#complete-store-setup) 管理您的Walmart Marketplace產品分類的清單、庫存、定價和訂單。

## 建立銷售渠道

1. 從管理員開啟 [!DNL Channel Manager] 通過 **[!UICONTROL Marketing** > _頻道&#x200B;_> **渠道管理器]**。

1. 在 **[!UICONTROL Marketplaces available to connect]** 選擇 **[!UICONTROL Get Started]**。

   ![將新的Walmart商店連接到 [!DNL Channel Manager]](assets/channel-manager-home.png)

1. 如果需要，請設定您的Walmart Marketplace賣家帳戶。

1. 配置儲存和連接：

   - 選擇 **[!UICONTROL Add Credentials]**。

   - 選擇 [!DNL Commerce] 儲存視圖以連接到市場。

      ![配置Commerce和 [!DNL Walmart Marketplace] 從 [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - 輸入唯一 **[!UICONTROL store name]**。

   - 選擇 **[!UICONTROL Adobe Commerce site]** 清單。

   - 添加 **[!UICONTROL email address]** 接收與服務通知相關的 [!DNL Channel Manager]。

1. 將通道連接到 [!DNL Walmart Marketplace]。

   - 添加憑據 [[!DNL Walmart Marketplace Adobe Production API key]](walmart-prerequisites.md#generate-a-walmart-marketplace-production-api-key) 從 [!DNL Walmart Marketplace Seller] 帳戶。

   - 如果您沒有憑據，請從 [!DNL Walmart Marketplace Developer Portal] 通過 **[!UICONTROL Get API credentials]**。

      在開發人員門戶上，選擇您的區域（美國和加拿大），然後登錄。

      ![[!DNL Walmart Marketplace] 帳戶登錄](assets/walmart-marketplace-login-page.png)

   - 在API密鑰窗體上，複製並保存 **[!UICONTROL Client ID]** 和 **[!UICONTROL Client Secret]** 值 [!UICONTROL Adobe Inc Production API key] 到安全的地方。

      ![[!DNL Walmart Marketplace API key] 配置頁](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >如果 [!DNL Adobe Inc] 未在開發人員門戶中列出鍵，請選擇 **[!UICONTROL Add New Key for a Solution Provider]** 配置權限並生成密鑰。 有關配置詳細資訊，請參閱 [生成 [!DNL Walmart Marketplace API Key]](walmart-prerequisites.md#generate-a-walmart-marketplace-api-key)。

   - 返回到 [!DNL Channel Manager] 將憑據添加到 **[!UICONTROL Walmart Connection]** 的下界。

      添加憑據時，Adobe會隱藏客戶端機密並將值儲存在安全保管庫中。

1. 選擇 **[!UICONTROL Save Store]** 應用配置並連接到 [!DNL Walmart marketplace]。

1. 成功連接後， [完整商店設定](complete-store-setup.md) 從 **[!UICONTROL Channel Manager]** 儲存頁面。

![設定第一個儲存](assets/channel-manager-setup-first-store.png)

### 排除連接問題

如果與沃爾瑪的聯繫失敗，請參閱 [Walmart Marketplace常見問題](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;}以獲取疑難解答提示。

- 從 [!DNL Walmart Developer Portal]，驗證您是否複製了生產API密鑰的正確憑據 [!UICONTROL Adobe Inc.]

- 驗證WalmartAdobeAPI鍵的訪問配置是否具有正確的權限。 請參閱 [沃爾瑪先決條件](walmart-prerequisites.md##generate-a-walmart-marketplace-api-key)。

- 確認 [!DNL Walmart API] 服務可從 [Walmart API狀態頁](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}。

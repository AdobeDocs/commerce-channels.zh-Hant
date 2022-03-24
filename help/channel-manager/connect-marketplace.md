---
title: 將Sales Channel連接到 [!DNL Walmart Marketplace]
description: 配置銷售渠道並連接到Walmart Marketplace。
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 8f07b215c20cc28aa9a6862bcb2b00da30a1ed84
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 連接到 [!DNL Walmart Marketplace]

在您的 [!DNL Commerce] 例如，將Commerce商店連接到Walmart Marketplace。

1. 通過 [為產品清單選擇Commerce商店](#select-the-commerce-store-for-the-sales-channel)。

1. [將通道連接到 [!DNL Walmart Marketplace] 通過添加Walmart API憑據](#connect-the-channel-to-walmart-marketplace)。

1. [完成銷售渠道設定](#complete-store-setup) 因此，您可以從Channel Manger管理清單、庫存、定價和銷售。

## 建立銷售渠道

1. 開啟Channel Manager。

   - 在管理員中，選擇 **[!UICONTROL Marketing** > _頻道&#x200B;_> **渠道管理器]**。

   - 選擇 **[!UICONTROL Connect New Store]**。

      ![將Commerce儲存連接到 [!DNL Walmart Marketplace] 從 [!DNL Channel Manager]](assets/connect-commerce-store-to-marketplace.png)


1. 配置儲存和連接：

   - 輸入唯一 **[!UICONTROL store name]**。

   - 選擇 **[!UICONTROL Adobe Commerce site]** 清單。

   - 添加 **[!UICONTROL email address]** 接收與服務通知相關的 [!DNL Channel Manager]。

      ![配置Commerce和 [!DNL Walmart Marketplace] 從 [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)


## 將渠道連接到Walmart Marketplace

1. 添加憑據 [!DNL Walmart Marketplace Adobe Production API key] 從 [!DNL Walmart Marketplace Seller] 帳戶。

   - 如果您沒有憑據，請選擇 **[!UICONTROL Get API credentials]** 讓他們 [!DNL Walmart Marketplace Developer Portal]。

      如果出現提示，請選擇您所在的區域（美國和加拿大），然後登錄。

      ![[!DNL Walmart Marketplace] 帳戶登錄](assets/walmart-marketplace-login-page.png)

   - 在API密鑰窗體上，複製並保存 **[!UICONTROL Client ID]** 和 **[!UICONTROL Client Secret]** 值 [!UICONTROL Adobe Inc Production API key] 到安全的地方。

      ![[!DNL Walmart Marketplace API key] 配置頁](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >如果 [!DNL Adobe Inc] 未在開發人員門戶中列出鍵，請選擇 **[!UICONTROL Add New Key for a Solution Provider]** 配置權限並生成密鑰。 有關配置詳細資訊，請參閱 [生成 [!DNL Walmart Marketplace API Key]](walmart-prerequisites.md#generate-a-walmart-marketplace-api-key)。

   - 返回到 [!DNL Channel Manager] 將憑據添加到 **[!UICONTROL Walmart Connection]** 的下界。

      將憑據添加到 [!DNL Channel Manager],Adobe隱藏客戶機密碼，並將值儲存在安全保管庫中。

1. [!UICONTROL Save] 用於建立連接的配置。

   成功連接後，從 **[!UICONTROL Channel Manager > Marketplace Stores]**。

   ![[!DNL Walmart Marketplace API key] 配置頁](assets/manage-connected-stores.png)


### 排除連接問題

如果與沃爾瑪的聯繫失敗，請參閱 [Walmart Marketplace常見問題](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;}以獲取疑難解答提示。

- 從 [!DNL Walmart Developer Portal]，驗證您是否複製了生產API密鑰的正確憑據 [!UICONTROL Adobe Inc.]

- 驗證WalmartAdobeAPI鍵的訪問配置是否具有正確的權限。 請參閱 [沃爾瑪先決條件](walmart-prerequisites.md##generate-a-walmart-marketplace-api-key)。

- 確認Walmart API服務可從 [Walmart API狀態頁](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}。

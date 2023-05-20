---
title: 添加或驗證AmazonAPI密鑰
description: 在您的Commerce配置中，經驗證的AmazonAPI密鑰允許您將您的商店與您的Amazon賣家帳戶整合。
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 添加或驗證AmazonAPI密鑰

訪問Amazon銷售渠道時， [!DNL Commerce] 自動檢查並驗證您在儲存配置中添加的AmazonAPI密鑰。 如果已驗證，則可以轉到下一步， [儲存整合](./store-integration.md)。

如果AmazonAPI密鑰缺失、無效或已過期，則必須更新密鑰。 出現一條消息，提示您獲取API密鑰並將其添加到您的Amazon銷售渠道配置中。

## 根據提示獲取並添加AmazonAPI密鑰

每次訪問您的Amazon銷售渠道時，都會驗證API密鑰。

1. 登錄 [!DNL Commerce] 管理員。

1. 在 _[!UICONTROL Admin]_邊欄，轉到&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**。

   如果您是首次訪問Amazon銷售渠道，或API密鑰需要更新，系統會提示您完成該過程。

   ![獲取並添加AmazonAPI密鑰提示](assets/amazon-api-verification-prompt.png)

1. 按一下 **[!UICONTROL Sign in]** 訪問 [!DNL Commerce] Web帳戶。

   「商業帳戶」頁面將在新瀏覽器頁籤中開啟。

   - 如果您已登錄 [!DNL Commerce] 帳戶， _[!UICONTROL API Portal]_的下界_[!UICONTROL My Account]_ 的子菜單。

   - 如果您未登錄，系統將提示您輸入 [!DNL Commerce] 帳戶用戶名和密碼 _[!UICONTROL API Portal]_按鈕

   - 如果您沒有帳戶，請訪問 [這樣 [!DNL Commerce] 帳戶頁](https://account.magento.com/customer/account/login/){target="_blank"} 註冊。 此帳戶應是您公司或業務的一部分。

1. 如果需要，可以在 _[!UICONTROL API Portal]_頁籤 [!DNL Commerce] 帳戶。

   要建立API密鑰，請輸入描述，如 `Amazon Sales Channel` 按一下 **[!UICONTROL Add New]**。 將生成新密鑰，並以您輸入的名稱顯示。 按一下 **[!UICONTROL Copy]** 鍵。

   ![生成或複製API密鑰](assets/amazon-add-api-key.png)

1. 生成並複製新密鑰後，返回到 _[!UICONTROL Amazon Sales Channel]_的子菜單。

1. 在 _[!UICONTROL Welcome to Amazon Sales Channel]_的&#x200B;**[!UICONTROL Add the key]**。

   瀏覽器退出Amazon銷售渠道，商店配置頁開啟 _[!UICONTROL Api Keys]_的 [!DNL Commerce] 管理員。 您可以在轉到&#x200B;**[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**&#x200B;展開 **[!UICONTROL Services]** ，然後選擇 **[!UICONTROL Magento Services]**。

1. 貼上複製的密鑰 **[!UICONTROL Production Api key]**。

1. 按一下 **[!UICONTROL Save Config]**。 現在您可以返回Amazon銷售渠道。

   ![在儲存配置中添加API密鑰](assets/config-magento-services-api-screen.png)

1. 在 _[!UICONTROL Admin]_邊欄，轉到&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**。

   重新訪問Amazon銷售渠道觸發器 [!DNL Commerce] 驗證和驗證您的API密鑰，並允許您繼續。

   如果系統提示您再次驗證密鑰，請重複此操作 _添加和驗證_ 處理。

![下一個表徵圖](assets/btn-next.png) [**繼續儲存整合**](./store-integration.md)

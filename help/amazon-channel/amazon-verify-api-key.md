---
title: 新增或驗證Amazon API金鑰
description: 在您的商務設定中，經過驗證的Amazon API金鑰可讓您將您的商店與Amazon賣家帳戶整合。
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 新增或驗證Amazon API金鑰

存取Amazon銷售管道時， [!DNL Commerce] 自動檢查並驗證您在商店設定中新增的Amazon API金鑰。 如果已驗證，則您可以繼續執行下一個步驟， [商店整合](./store-integration.md).

如果Amazon API金鑰遺失、無效或過期，您必須更新金鑰。 系統會顯示訊息，提示您取得API金鑰，並將其新增至您的Amazon銷售管道設定。

## 依提示取得並新增Amazon API金鑰

每次您存取Amazon銷售管道時，都會驗證API金鑰。

1. 登入 [!DNL Commerce] 管理員。

1. 在 _[!UICONTROL Admin]_邊欄，轉到&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   如果您是第一次存取Amazon銷售管道，或您的API金鑰需要更新，系統會提示您完成此程式。

   ![取得並新增Amazon API金鑰提示](assets/amazon-api-verification-prompt.png)

1. 按一下 **[!UICONTROL Sign in]** 訪問 [!DNL Commerce] 網站帳戶。

   「商務」帳戶頁面會在新的瀏覽器標籤中開啟。

   - 如果您已登入 [!DNL Commerce] 帳戶、 _[!UICONTROL API Portal]_區段_[!UICONTROL My Account]_ 頁面自動顯示。

   - 如果您未登入，系統會提示您輸入 [!DNL Commerce] 帳戶使用者名稱和密碼 _[!UICONTROL API Portal]_頁簽。

   - 如果您沒有帳戶，請造訪 [the [!DNL Commerce] 帳戶頁面](https://account.magento.com/customer/account/login/){target=&quot;_blank&quot;}並註冊。 此帳戶應是您公司或業務的一部分。

1. 如有需要，您可以在 _[!UICONTROL API Portal]_標籤 [!DNL Commerce] 帳戶。

   若要建立API金鑰，請輸入說明，如 `Amazon Sales Channel` 按一下 **[!UICONTROL Add New]**. 系統會產生新金鑰，並以您輸入的名稱顯示。 按一下 **[!UICONTROL Copy]** 來複製新金鑰。

   ![產生或複製API金鑰](assets/amazon-add-api-key.png)

1. 產生並複製新金鑰後，會傳回至 _[!UICONTROL Amazon Sales Channel]_標籤。

1. 在 _[!UICONTROL Welcome to Amazon Sales Channel]_頁面，按一下&#x200B;**[!UICONTROL Add the key]**.

   瀏覽器會退出Amazon銷售管道，商店設定頁面會開啟 _[!UICONTROL Api Keys]_頁面 [!DNL Commerce] 管理員。 您可以在前往&#x200B;**[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**，展開 **[!UICONTROL Services]** ，然後選擇 **[!UICONTROL Magento Services]**.

1. 貼上複製的金鑰 **[!UICONTROL Production Api key]**.

1. 按一下 **[!UICONTROL Save Config]**. 您現在可以返回Amazon銷售管道。

   ![在儲存配置中新增API金鑰](assets/config-magento-services-api-screen.png)

1. 在 _[!UICONTROL Admin]_邊欄，轉到&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   重新存取Amazon銷售管道觸發器 [!DNL Commerce] 驗證及驗證您的API金鑰，並允許您繼續。

   如果系統提示您再次驗證密鑰，請重複此操作 _添加和驗證_ 程式。

![下一個表徵圖](assets/btn-next.png) [**繼續儲存整合**](./store-integration.md)

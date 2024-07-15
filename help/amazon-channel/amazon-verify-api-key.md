---
title: 新增或驗證Amazon API金鑰
description: 在您的Commerce設定中，驗證的Amazon API金鑰可讓您將商店與Amazon賣家帳戶整合。
role: Admin, Developer
feature: Sales Channels, Integration, Tools and External Services
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 新增或驗證Amazon API金鑰

存取Amazon Sales Channel時，[!DNL Commerce]會自動檢查並驗證您新增至商店設定中的Amazon API金鑰。 如果已驗證，則您可以繼續進行下一個步驟，[存放區整合](./store-integration.md)。

如果Amazon API金鑰遺失、無效或過期，您必須更新金鑰。 系統會顯示訊息，提示您取得API金鑰，並將其新增至您的Amazon銷售管道設定。

## 取得提示並新增Amazon API金鑰

每次存取您的Amazon銷售管道時，都會驗證API金鑰。

1. 登入[!DNL Commerce]管理員。

1. 在&#x200B;_[!UICONTROL Admin]_側邊欄上，前往&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**。

   如果您是第一次存取Amazon銷售管道，或您的API金鑰需要更新，系統會提示您完成此程式。

   ![取得並新增Amazon API金鑰提示](assets/amazon-api-verification-prompt.png){width="500"}

1. 按一下&#x200B;**[!UICONTROL Sign in]**&#x200B;以存取您的[!DNL Commerce]網頁帳戶。

   Commerce帳戶頁面會在新的瀏覽器標籤中開啟。

   - 如果您已登入您的[!DNL Commerce]帳戶，_[!UICONTROL My Account]_頁面的_[!UICONTROL API Portal]_&#x200B;區段會自動顯示。

   - 如果您未登入，系統會提示您輸入[!DNL Commerce]帳戶使用者名稱與密碼，然後才會顯示&#x200B;_[!UICONTROL API Portal]_索引標籤。

   - 如果您沒有帳戶，請造訪[ [!DNL Commerce] 帳戶頁面](https://account.magento.com/customer/account/login/){target="_blank"}並註冊。 此帳戶應該是您公司或企業的一部分。

1. 如有需要，您可以在[!DNL Commerce]帳戶的&#x200B;_[!UICONTROL API Portal]_標籤上檢視並產生API金鑰。

   若要建立API金鑰，請輸入`Amazon Sales Channel`之類的說明，然後按一下&#x200B;**[!UICONTROL Add New]**。 隨即產生新金鑰，並顯示您輸入的名稱。 按一下&#x200B;**[!UICONTROL Copy]**&#x200B;以複製新金鑰。

   ![產生或複製API金鑰](assets/amazon-add-api-key.png){width="500" zoomable="yes"}

1. 產生並複製新金鑰後，返回瀏覽器中的&#x200B;_[!UICONTROL Amazon Sales Channel]_標籤。

1. 在&#x200B;_[!UICONTROL Welcome to Amazon Sales Channel]_頁面上，按一下&#x200B;**[!UICONTROL Add the key]**。

   瀏覽器會退出Amazon銷售管道，而商店設定頁面會在[!DNL Commerce]管理員中開啟&#x200B;_[!UICONTROL Api Keys]_頁面。 當您前往「**[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**」，展開左側面板中的「**[!UICONTROL Services]**」，然後選擇「**[!UICONTROL Magento Services]**」時，可以手動開啟此頁面。

1. 貼上&#x200B;**[!UICONTROL Production Api key]**&#x200B;的複製金鑰。

1. 按一下&#x200B;**[!UICONTROL Save Config]**。 您現在可以返回Amazon銷售管道。

   ![正在將您的API金鑰加入您的商店設定中](assets/config-magento-services-api-screen.png){width="600" zoomable="yes"}

1. 在&#x200B;_[!UICONTROL Admin]_側邊欄上，前往&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**。

   重新存取Amazon sales channel觸發程式[!DNL Commerce]驗證及驗證您的API金鑰，並允許您繼續。

   如果系統提示您再次驗證金鑰，請重複此&#x200B;_新增並驗證_&#x200B;程式。

![下一個圖示](assets/btn-next.png) [**繼續儲存整合**](./store-integration.md)

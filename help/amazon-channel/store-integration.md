---
title: 與 [!DNL Amazon Seller Account]的存放區整合
description: 在開始入門流程之前，您必須建立（新增） AmazonSales Channel商店，並將其連線到您的Amazon賣家帳戶。
role: Admin, Developer
feature: Sales Channels, Configuration, Integration, Tools and External Services
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 與[!DNL Amazon Seller Account]的存放區整合

若要開始使用Amazon銷售管道，您必須建立（新增） Amazon銷售管道商店，並將其連結至您的[!DNL Amazon Seller Account]。 這兩個步驟整合您的[!DNL Commerce]和Amazon帳戶以共用資料、同步產品等。

_您需要您[!DNL Amazon Seller Central]帳戶（用來建立賣家帳戶的電子郵件或電話）的主要登入認證，才能連線您的商店。_

>[!NOTE]
>
>第一次整合商店後，系統每年會提示您再次授予存取權，以續約Amazon銷售管道與Amazon的連線。 您可以在Seller Central帳戶的&#x200B;**設定** > **使用者許可權**&#x200B;頁面的&#x200B;_Amazon MWS開發人員許可權_&#x200B;區段的&#x200B;_目前授權_&#x200B;表格中，更新或撤銷此授權。

## 新增Amazon存放區

1. 在&#x200B;_管理員_&#x200B;側邊欄上，前往&#x200B;**行銷** > _管道_ > **AmazonSales Channel**。

   新增您的第一個Amazon Sales Channel商店時，_預先設定工作_&#x200B;強制回應視窗會出現。 新增第一個商店後，您可在左側功能表的「_學習與準備_」底下的「[Amazon銷售管道首頁](./amazon-sales-channel-home.md)」存取預先設定工作。

1. 按一下&#x200B;**[!UICONTROL Add Amazon Store]**。

   _[!UICONTROL Add Amazon sales channel]_頁面隨即開啟。

   ![新增Amazon銷售管道商店](assets/amazon-store-integration.png){width="500" zoomable="yes"}

1. 針對&#x200B;**[!UICONTROL Magento Website to use for Amazon Listing]**，選擇要為這個Amazon銷售通路商店連線的[!DNL Commerce]網站。

   此設定也會定義[匯入Amazon訂單](./order-settings.md)的預設[!DNL Commerce]存放區。

1. 針對&#x200B;**[!UICONTROL Email Address]**，輸入您偏好的連絡人電子郵件地址。

1. 針對&#x200B;**[!UICONTROL New Store Name]**，為您新的Amazon銷售管道商店輸入描述性名稱。

   >[!NOTE]
   >
   >此名稱僅用作[!DNL Commerce]參考，可識別[Amazon銷售管道首頁](./amazon-sales-channel-home.md)頁面上的商店。 您希望讓您的團隊能夠輕鬆識別它。 例如，您在美國地區銷售的Amazon商店可能名為`Amazon Store USA`。

1. 針對&#x200B;**[!UICONTROL Amazon Marketplace Country]**，選擇此Amazon銷售管道商店銷售產品的地區/國家。 選項：

   - 美國
   - 加拿大
   - 墨西哥
   - 英國

1. 在&#x200B;_[!UICONTROL Map your Magento attributes to Amazon]_區段中，執行下列動作：

   - 針對&#x200B;**[!UICONTROL Product ID on the Amazon market]**，選擇要對應至下列所選[!DNL Commerce]屬性的Amazon屬性。

     此ID有助於正確比對[!DNL Commerce]目錄中的對應產品。

   - 針對&#x200B;**[!UICONTROL Map a Magento attribute]**，選擇要對應至上述所選Amazon屬性的[!DNL Commerce]產品屬性。

     [對應屬性](./ob-creating-magento-attributes.md)有助於確保您的Amazon清單正確符合[!DNL Commerce]目錄中的對應產品。

1. 按一下&#x200B;**[!UICONTROL Connect]**。

   對話方塊會關閉，新商店會顯示在[Amazon銷售管道首頁](./amazon-sales-channel-home.md)頁面，並附上確認訊息。

## 將存放區連線至[!DNL Amazon Seller Central]

1. 在商店儀表板上，按一下商店卡片上的&#x200B;**[!UICONTROL Connect store]**，在新索引標籤中啟動[!DNL Amazon Seller Central]。

1. 輸入您的[!DNL Amazon Seller Central]帳戶認證，然後按一下&#x200B;**[!UICONTROL Sign in]**。

   若要完成此連線，您必須使用主要使用者的登入認證（用來建立賣家帳戶的電子郵件或電話）登入您的[!DNL Amazon Seller Central]帳戶。

1. 如果出現提示，請輸入您從Amazon收到的程式碼，然後按一下「**[!UICONTROL Sign in]**」，以完成Amazon雙因素授權(2FA)。

1. 在&#x200B;_[!UICONTROL Amazon Marketplace Web Service]_確認頁面上，選取「[!UICONTROL I understand...]」核取方塊並按一下&#x200B;**[!UICONTROL Next]**。

1. 在&#x200B;_[!UICONTROL You are almost done]_訊息上，按一下&#x200B;**[!UICONTROL Continue]**。

   您已授予Amazon Sales Channel許可權來存取及與您的[!DNL Amazon Seller Central]帳戶共用資料。 Amazon頁面會關閉，並顯示確認訊息。

   [Amazon銷售管道首頁](./amazon-sales-channel-home.md)頁面隨即開啟，顯示您的Amazon商店卡片。

   若要檢視商店儀表板，請按一下商店卡片上的&#x200B;**[!UICONTROL View Store]**。

![Amazon銷售管道首頁（含新商店卡）](assets/asc-dashboard-after-2fa.png){width="600" zoomable="yes"}

您新的Amazon銷售管道商店現在已連線至您的[!DNL Amazon Seller Central]帳戶。

![下一個圖示](assets/btn-next.png) [**繼續建立清單規則**](./ob-create-listing-rule.md)

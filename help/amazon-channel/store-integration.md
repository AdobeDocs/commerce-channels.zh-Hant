---
title: 商店整合
description: 開始上線程式之前，您必須建立（新增）AmazonSales Channel商店，並將其連線至您的Amazon賣家帳戶。
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# 商店整合

若要開始使用Amazon銷售管道，您必須建立（新增）Amazon銷售管道商店，並將其連線至您的Amazon銷售者帳戶。 這兩個步驟整合您的[!DNL Commerce]和Amazon帳戶，以共用資料、同步產品等。

_您需要帳戶的主要登入憑證( [!DNL Amazon Seller Central] 用來建立賣家帳戶的電子郵件或電話)，才能連線您的商店。_

>[!NOTE]
>
>首次商店整合後，系統會每年提示您重新授與存取權，以續約Amazon銷售管道與Amazon的連線。 您可以在賣家中央帳戶的&#x200B;**Settings** > **User Permissions**&#x200B;頁的&#x200B;_Amazon MWS Developer Permissions_&#x200B;部分的&#x200B;_Current Authorizations_&#x200B;表中續訂或撤銷此授權。

## 新增Amazon商店

1. 在&#x200B;_Admin_&#x200B;側欄上，前往&#x200B;**行銷** > _頻道_ > **AmazonSales Channel**。

   新增第一個Amazon銷售管道商店時，會出現&#x200B;_預先設定工作_&#x200B;強制回應。 新增第一個商店後，您可以在左側功能表&#x200B;_學習與準備_&#x200B;下的[Amazon銷售管道首頁](./amazon-sales-channel-home.md)頁面存取預先設定工作。

1. 按一下&#x200B;**[!UICONTROL Add Amazon Store]**。

   _[!UICONTROL Add Amazon sales channel]_頁面隨即開啟。

   ![新增Amazon銷售管道商店](assets/amazon-store-integration.png)

1. 若為&#x200B;**[!UICONTROL Magento Website to use for Amazon Listing]**，選擇要連線至此Amazon銷售管道商店的[!DNL Commerce]網站。

   此設定也定義了[匯入Amazon訂單](./order-settings.md)的預設[!DNL Commerce]存放區。

1. 對於&#x200B;**[!UICONTROL Email Address]**，輸入首選聯繫人電子郵件地址。

1. 對於&#x200B;**[!UICONTROL New Store Name]**，輸入新Amazon銷售渠道商店的描述性名稱。

   >[!NOTE]
   >
   >此名稱僅用作[!DNL Commerce]參考，並標識[Amazon銷售渠道首頁](./amazon-sales-channel-home.md)頁面上的商店。 您希望讓團隊能夠輕鬆識別。 例如，您在美國地區銷售的Amazon商店可能命名為`Amazon Store USA`。

1. 對於&#x200B;**[!UICONTROL Amazon Marketplace Country]**，選擇此Amazon銷售渠道商店銷售產品的地區/國家/地區。 選項：

   - 美國
   - 加拿大
   - 墨西哥
   - 英國

1. 在&#x200B;_[!UICONTROL Map your Magento attributes to Amazon]_區段中，執行下列動作：

   - 對於&#x200B;**[!UICONTROL Product ID on the Amazon market]**，選擇要映射到下面選擇的[!DNL Commerce]屬性的Amazon屬性。

      此ID有助於正確匹配[!DNL Commerce]目錄中的對應產品。

   - 對於&#x200B;**[!UICONTROL Map a Magento attribute]**，選擇[!DNL Commerce]產品屬性以對應至上方選取的Amazon屬性。

      [對應](./ob-creating-magento-attributes.md) 屬性會擱置，確保您的Amazon清單正確符合目錄中的對應 [!DNL Commerce] 產品。

1. 按一下&#x200B;**[!UICONTROL Connect]**。

   對話框將關閉，新商店將顯示在[Amazon銷售渠道首頁](./amazon-sales-channel-home.md)頁面上，並帶有確認消息。

## 將儲存連接到[!DNL Amazon Seller Central]

1. 在商店控制面板上，按一下商店卡上的&#x200B;**[!UICONTROL Connect store]**&#x200B;以在新索引標籤中啟動[!DNL Amazon Seller Central]。

1. 輸入您的[!DNL Amazon Seller Central]帳戶憑證，然後按一下&#x200B;**[!UICONTROL Sign in]**。

   要完成此連接，您必須使用主要用戶（用於建立賣家帳戶的電子郵件或電話）的登錄憑據登錄[!DNL Amazon Seller Central]帳戶。

1. 如果出現提示，請輸入您從Amazon收到的代碼並按一下&#x200B;**[!UICONTROL Sign in]**&#x200B;以完成Amazon雙因素授權(2FA)。

1. 在&#x200B;_[!UICONTROL Amazon Marketplace Web Service]_確認頁面上，選中「[!UICONTROL I understand...]」複選框，然後按一下&#x200B;**[!UICONTROL Next]**。

1. 在&#x200B;_[!UICONTROL You are almost done]_訊息上，按一下&#x200B;**[!UICONTROL Continue]**。

   您已授予Amazon銷售管道存取權，並與您的[!DNL Amazon Seller Central]帳戶共用資料。 Amazon頁面關閉，並顯示確認訊息。

   [Amazon銷售管道首頁](./amazon-sales-channel-home.md)頁面隨即開啟，顯示您的Amazon商店卡片。

   若要檢視存放區控制面板，請按一下存放區卡片上的&#x200B;**[!UICONTROL View Store]**。

![Amazon銷售渠道首頁，帶有新商店卡](assets/asc-dashboard-after-2fa.png)

您的新Amazon銷售渠道商店現在已連接至您的[!DNL Amazon Seller Central]帳戶。

![下一](assets/btn-next.png) [**個圖示繼續建立清單規則**](./ob-create-listing-rule.md)

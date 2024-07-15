---
title: 安裝 [!DNL Amazon Sales Channel] 擴充功能
description: 若要將您的 [!DNL Commerce] 目錄與 [!DNL Amazon Seller Accounts] 整合，並透過 [!DNL Amazon Marketplace]銷售，請下載並安裝AmazonSales Channel擴充功能。
role: Admin, Developer
feature: Sales Channels, Install, Integration, Tools and External Services
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 010a95d7be29354515cf4dcbf5d557eebaa40ed6
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# 安裝[!DNL Amazon Sales Channel]擴充功能

>[!IMPORTANT]
>
>Adobe Commerce和Magento Open Source 2.4.x版本僅支援[!DNL Amazon Sales Channel]擴充功能4.0+版本。 如果您執行2.3.x版，請參閱有關[相容的Amazon sales channel版本](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html)的檔案。 如需版本相容性的詳細資訊，請參閱開發人員檔案中的[可用性](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html)頁面。

[!UICONTROL Amazon Sales Channel]擴充功能會安裝並新增功能，以將您的Commerce目錄與[!DNL Amazon Seller Accounts]整合，以透過[!DNL Amazon Marketplace]銷售。 若要檢閱其他資訊，請參閱[!DNL Commerce Marketplace]中的[AmazonSales Channel](https://marketplace.magento.com/magento-module-amazon.html)頁面和[發行說明](release-notes.md)。

## 需求

- **Commerce執行個體**： [!DNL Amazon Sales Channel]擴充功能可安裝在雲端基礎結構版本2.3.x或更新版本上具有Magento Open Source、Adobe Commerce和Adobe Commerce的執行個體上。 2.1、2.2或1.x版不再支援。
- **Commerce網頁帳戶**：您應該有一個Commerce網頁帳戶，用來建立和追蹤API金鑰。
- **API金鑰**：透過您的Amazon網路帳戶建立Commerce銷售管道API金鑰。 下列指示包含這些步驟。

## 安裝

如需有關在此程式中使用Composer的詳細資訊，請參閱開發人員檔案中的[擴充功能安裝](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html)指示。

1. 登入[Commerce Marketplace](https://marketplace.magento.com/customer/account/)。

1. 按一下&#x200B;**[!UICONTROL Marketplace]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL My Purchases]**。

1. 找到並選取&#x200B;**[!UICONTROL Amazon Sales Channel]**。

1. 在擴充功能頁面上，選取版本。

1. 如需元件名稱和版本，請按一下&#x200B;**[!UICONTROL Technical Details]**。

1. 使用名稱和版本資訊來更新`composer.json`檔案中的服務聯結器專案。

   - 新增擴充功能名稱和版本至您的`composer.json`檔案。

   - 導覽至您的[!DNL Commerce]專案目錄並更新您的`composer.json`檔案。

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - 輸入您的[驗證金鑰](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html)。 您的公開金鑰是您的使用者名稱；您的私密金鑰是您的密碼。

   - 請等待Composer完成更新您的專案相依性，並確保沒有錯誤。

1. [驗證擴充功能](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html)。

## 新增Amazon sales channel API金鑰

安裝之後，請輸入[API金鑰](./amazon-verify-api-key.md)以完成設定。

## 設定Amazon通道設定選項

您有以下選項可設定Amazon銷售管道。 您不需要修改這些設定，即可開始在Amazon上線和銷售。 建議進階管理員考慮這些選項。

1. 登入Admin。

1. 在&#x200B;_管理員_&#x200B;側邊欄上，移至&#x200B;**商店** > _設定_ > **設定**。

1. 按一下&#x200B;**Sales Channel**，然後按一下&#x200B;**全域設定**。

1. 針對&#x200B;**清除記錄歷史記錄**，定義清除收集記錄的時間間隔。

   選項包括`Once Daily`、`Once Weekly`和`Once Monthly` （預設）。

1. （選用）若為&#x200B;**背景工作(CRON) Source**，請將設定變更為`Command Line (CLI) CRON`。

   建議將此設定用於&#x200B;**_進階使用者/管理員_**。

1. 按一下&#x200B;**[!UICONTROL Save Config]**。

## 更新擴充功能

1. 登入[Commerce Marketplace](https://marketplace.magento.com/customer/account/)。

1. 按一下&#x200B;**[!UICONTROL Marketplace]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL My Purchases]**。

1. 找到並選取&#x200B;**[!UICONTROL Amazon Sales Channel]**。

1. 在擴充功能頁面上，選取版本。

1. 如需元件名稱和版本，請按一下&#x200B;**[!UICONTROL Technical Details]**。

1. 完成&#x200B;_安裝指南_&#x200B;中的[擴充功能升級指示](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html)。

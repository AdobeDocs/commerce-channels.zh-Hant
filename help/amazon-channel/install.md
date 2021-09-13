---
title: 安裝擴充功能
description: 若要整合您的 [!DNL Commerce] catalog with [!DNL Amazon Seller Accounts] 並透過 [!DNL Amazon Marketplace]銷售，請下載並安裝AmazonSales Channel擴充功能。
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 8d12a839bbdf77f27c732507b5b776729e252a9f
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 安裝擴充功能

>[!IMPORTANT]
>
>Adobe商務和Magento Open Source2.4.x版僅支援[!DNL Amazon Sales Channel]擴充功能4.0+版。 如果您執行的是2.3.x版，請參閱[相容Amazon銷售管道版本](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target=&quot;_blank&quot;}的檔案。 如需版本相容性的詳細資訊，請參閱開發人員檔案中的[可用性](https://devdocs.magento.com/release/availability.html){target=&quot;_blank&quot;}頁面。

[!UICONTROL Amazon Sales Channel]擴充功能會安裝並新增功能，以整合您的商務目錄與[!DNL Amazon Seller Accounts]，以透過[!DNL Amazon Marketplace]銷售。 若要查看其他資訊，請參閱[!DNL Commerce Marketplace]中的[AmazonSales Channel](https://marketplace.magento.com/magento-module-amazon.html)頁面，以及開發人員檔案中的[發行說明](https://devdocs.magento.com/extensions/amazon-sales/release-notes/)。

## 需求

- **商務例項**:此擴 [!DNL Amazon Sales Channel] 充功能可安裝在雲端基礎架構2.3.x版或更新版本上，具有Magento Open Source、Adobe商務和Adobe商務的執行個體上。2.1、2.2或1.x版不再支援此功能。
- **商務Web帳戶**:您應有Commerce Web帳戶，可用來建立及追蹤API金鑰。
- **API密鑰**:透過您的Commerce網站帳戶建立Amazon銷售管道API金鑰。下列指示包括這些步驟。

## 安裝

如需有關使用此程式使用撰寫器的詳細資訊，請參閱開發人員檔案中的[擴充功能安裝](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;}指示。

1. 登入[Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}。

1. 按一下&#x200B;**[!UICONTROL Marketplace]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL My Purchases]**。

1. 找到並選擇&#x200B;**[!UICONTROL Amazon Sales Channel]**。

1. 在擴充功能頁面上，選取版本。

1. 對於元件名稱和版本，按一下&#x200B;**[!UICONTROL Technical Details]**。

1. 使用名稱和版本資訊更新`composer.json`檔案中的服務連接器條目。

   - 將副檔名的名稱和版本新增至您的`composer.json`檔案。

   - 導覽至您的[!DNL Commerce]專案目錄，並更新您的`composer.json`檔案。

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - 輸入您的[驗證密鑰](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}。 您的公開金鑰是您的使用者名稱；您的私密金鑰是您的密碼。

   - 等待撰寫器完成專案相依性的更新，並確保沒有錯誤。


1. [驗證擴充功能](https://devdocs.magento.com/extensions/install/#verify-the-extension){target=&quot;_blank&quot;}。

## 新增Amazon銷售管道API金鑰

安裝後，輸入[API密鑰](./amazon-verify-api-key.md)以完成配置。

## 設定Amazon通道設定選項

您有下列選項可設定Amazon銷售管道。 您不需要修改這些設定即可開始在Amazon上上線和銷售。 建議進階管理員考慮這些選項。

1. 登入管理員。

1. 在&#x200B;_Admin_&#x200B;側欄上，轉至&#x200B;**儲存** > _設定_ > **配置**。

1. 按一下「**Sales Channel**」，然後按一下「**全域設定**」。

1. 對於&#x200B;**清除日誌歷史記錄**，定義清除收集日誌的間隔。

   選項包括`Once Daily`、`Once Weekly`和`Once Monthly`（預設）。

1. （可選）對於&#x200B;**背景任務(CRON)源**，將設定更改為`Command Line (CLI) CRON`。

   建議對&#x200B;**_進階使用者/管理員_**&#x200B;使用此設定。

1. 按一下&#x200B;**[!UICONTROL Save Config]**。

## 更新擴充功能

1. 登入[Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}。

1. 按一下&#x200B;**[!UICONTROL Marketplace]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL My Purchases]**。

1. 找到並選擇&#x200B;**[!UICONTROL Amazon Sales Channel]**。

1. 在擴充功能頁面上，選取版本。

1. 對於元件名稱和版本，按一下&#x200B;**[!UICONTROL Technical Details]**。

1. 在開發人員檔案中，完成[擴充功能升級指示](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target=&quot;_blank&quot;}。

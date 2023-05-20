---
title: 安裝擴展
description: 整合 [!DNL Commerce] 目錄 [!DNL Amazon Seller Accounts] 通過 [!DNL Amazon Marketplace]，下載並安裝AmazonSales Channel擴展。
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 安裝擴展

>[!IMPORTANT]
>
>僅 [!DNL Amazon Sales Channel] Adobe Commerce和Magento Open Source2.4.x版支援擴展4.0+版。 如果運行的是2.3.x版本，請參閱 [相容Amazon銷售渠道發佈](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target="_blank"}. For more information about version compatibility, see the [Availability](https://devdocs.magento.com/release/availability.html){target="_blank"} 頁。

的 [!UICONTROL Amazon Sales Channel] 擴展安裝並添加功能以將您的Commerce目錄與 [!DNL Amazon Seller Accounts] 通過 [!DNL Amazon Marketplace]。 要查看其他資訊，請參閱 [AmazonSales Channel](https://marketplace.magento.com/magento-module-amazon.html) 頁面 [!DNL Commerce Marketplace] 和 [發行說明](release-notes.md)。

## 要求

- **商業實例**:的 [!DNL Amazon Sales Channel] 擴展可安裝在雲基礎架構2.3.x版或更高版本上具有Magento Open Source、Adobe Commerce和Adobe Commerce的實例上。 在2.1、2.2或1.x版本上不再支援它。
- **Commerce Web帳戶**:您應該有一個Commerce Web帳戶，用於建立和跟蹤API密鑰。
- **API密鑰**:通過您的Commerce Web帳戶建立Amazon銷售渠道API密鑰。 以下說明包括這些步驟。

## 安裝

有關使用Composer進行此過程的詳細資訊，請參見 [擴展安裝](https://devdocs.magento.com/extensions/install/){target="_blank"} 開發人員文檔中的說明。

1. 登錄到 [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}。

1. 按一下 **[!UICONTROL Marketplace]** ，然後按一下 **[!UICONTROL My Purchases]**。

1. 查找並選擇 **[!UICONTROL Amazon Sales Channel]**。

1. 在擴展頁上，選擇版本。

1. 對於元件名稱和版本，按一下 **[!UICONTROL Technical Details]**。

1. 使用名稱和版本資訊更新您的服務連接器條目 `composer.json` 的子菜單。

   - 將副檔名的名稱和版本添加到 `composer.json` 的子菜單。

   - 導航到 [!DNL Commerce] 項目目錄和更新 `composer.json` 的子菜單。

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - 輸入 [身份驗證密鑰](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target="_blank"}。 您的公鑰是您的用戶名；你的私鑰是你的密碼。

   - 等待Composer完成對項目依賴項的更新並確保沒有錯誤。


1. [驗證擴展](https://devdocs.magento.com/extensions/install/#verify-the-extension){target="_blank"}。

## 添加Amazon銷售渠道API密鑰

安裝後，輸入 [API密鑰](./amazon-verify-api-key.md) 完成配置。

## 設定Amazon通道配置選項

您有以下選項來配置Amazon銷售渠道。 您無需修改這些設定即可開始在Amazon上登機和銷售。 建議高級管理員考慮這些選項。

1. 登錄管理員。

1. 在 _管理_ 邊欄，轉到 **商店** > _設定_ > **配置**。

1. 按一下 **Sales Channel**，則 **全局設定**。

1. 對於 **清除日誌歷史記錄**，定義清除收集的日誌的間隔。

   選項包括 `Once Daily`。 `Once Weekly`, `Once Monthly` （預設）。

1. （可選） **後台任務(CRON)源**，將設定更改為 `Command Line (CLI) CRON`。

   建議使用 **_高級用戶/管理員_**。

1. 按一下 **[!UICONTROL Save Config]**。

## 更新擴展

1. 登錄到 [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}。

1. 按一下 **[!UICONTROL Marketplace]** ，然後按一下 **[!UICONTROL My Purchases]**。

1. 查找並選擇 **[!UICONTROL Amazon Sales Channel]**。

1. 在擴展頁上，選擇版本。

1. 對於元件名稱和版本，按一下 **[!UICONTROL Technical Details]**。

1. 完成 [擴展升級說明](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target="_blank"} 在開發人員文檔中。

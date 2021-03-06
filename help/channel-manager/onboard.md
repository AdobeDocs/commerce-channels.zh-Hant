---
title: 板載 [!DNL Channel Manager]
description: '''將實例連接到 [!DNL Channel Manager] 完成幾個登機步驟。'
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 638ba8c595652e66aa5f15f5207855c6d2b872d7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---


# 板載 [!DNL Channel Manager]

完成登錄後，請通過 [!UICONTROL Channel Manager] 的上界 [!UICONTROL Commerce Admin Marketing] 的子菜單。

![[!DNL Channel Manager] 管理視圖中的選項](assets/channel-manager-admin-view.png)

## 登機概述

1. [安裝 [!DNL Channel Manager] 擴展](install.md)。

1. [配置 [!DNL Commerce Services Connector]](connect.md) 將Channel Manager與Commerce實例和其他支援服務整合。

1. [連接 [!DNL Commerce] 儲存 [!DNL Walmart Marketplace]](connect.md)。

1. [完成商店設定](complete-store-setup.md)。

## 要求

- 驗證您是否遇到 [沃爾瑪市場要求](walmart-requirements.md) 與Channel Manager整合。

- **商業帳戶資訊** — 下載和安裝 [!DNL Channel Manager] 需要 [商業帳戶](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;}。 您需要具有「所有者」或「管理員」訪問權限的帳戶ID和憑據 [!DNL Adobe Commerce] 或 [!DNL Magento Open Source] 實例。

   - **影像ID**-[登錄](https://account.magento.com/customer/account/login/) 到 [!DNL Commerce] 要獲取ID的帳戶 **[!UICONTROL My Account - Magento settings]**。

      ![[!DNL MAGEID] 上 [!DNL Commerce] 帳戶設定](assets/mageid-my-commerce-account.png)

   - **訪問密鑰 —** 獲取要下載的驗證密鑰 [!DNL Commerce] 擴展 [!DNL Commerce] 合成器儲存庫 `([!DNL repo.magento.com]`)。

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      在Adobe Commerce和Magento Open Source項目上，所有者可以 [共用訪問](https://docs.magento.com/user-guide/magento/magento-account-share.html) 允許受信任的員工和服務提供商使用所有者或許可證持有者帳戶的憑據下載擴展。

      對於 [!DNL Adobe Commerce] 在雲基礎架構項目上，軟體安裝程式必須具有以下訪問權限 [!DNL Commerce] 實例：

      - 超級用戶對雲項目的訪問
      - 管理員對特定環境的訪問
      - 一個 [!DNL Adobe Commerce] 或 [!DNL Magento Open Source] 具有訪問Composer儲存庫權限的帳戶

      請參閱 [管理用戶訪問](https://devdocs.magento.com/cloud/project/user-admin.html)。


- **使用Composer和[!DNL Commerce CLI]**  — 請參閱 [常規CLI安裝](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;，瞭解有關使用這些工具在上安裝和配置擴展的資訊 [!DNL Adobe Commerce] 或 [!DNL Magento Open Source] 平台。

- [[!DNL Amazon Sales Channel] 4.4.2版或更高版本](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html) — 如果已激活 [!DNL Amazon Sales Channel] 為 [!DNL Commerce] 站點，驗證 [!DNL Commerce] 安裝前已安裝4.4.2版平台 [!DNL Channel Manager]。

- [!DNL Inventory Management] Adobe Commerce和Magento Open Source

   如果您計畫使用渠道經理進行庫存和訂單管理，則必須在Adobe Commerce和Magento Open Source實例上安裝並啟用Inventory management擴展。 通常，此擴展在Adobe Commerce和Magento Open Source2.3.x及更高版本上預設安裝並啟用。

   如果您已從2.2.x升級了Commerce，或者您已禁用了Inventory management，則必須更新安裝以包括所需的模組。 有關詳細資訊，請參見 [安裝Inventory management](https://devdocs.magento.com/extensions/inventory-management/) 在Adobe Commerce開發人員文檔中。

### 系統要求

- [Adobe Commerce2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [7.3菲律賓比索/7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [作曲家1.x或更高版本](https://devdocs.magento.com/cloud/reference/cloud-composer.html)
- [[!DNL Amazon Sales Channel] 4.4.2版或更高版本](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html) — 如果已激活 [!DNL Amazon Sales Channel] 為 [!DNL Commerce] 站點，驗證 [!DNL Commerce] 安裝前已安裝4.4.2版平台 [!DNL Channel Manager]。
- [[!DNL Inventory Management]](https://devdocs.magento.com/extensions/inventory-management/)

### 支援的平台

- Adobe Commerce雲(ECE):2.4.x
- Adobe Commerce駐地：2.4.x
- Magento Open Source2.4.x

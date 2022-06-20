---
title: 映射目錄屬性
description: 映射匹配的屬性[DNL! Commerce]產品到現有 [!DNL Walmart Marketplace] 清單和同步資料 [!DNL Channel Manager] 和 [!DNL Walmart]。
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 97128dcf45d7672e958c771f88389aba40c6e39e
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# 映射目錄屬性

在連接清單之前， [!DNL Commerce] 至 [!DNL Walmart Marketplace]，必須從 [!DNL Commerce] 從Walmart獲取相應標識符。

需要此步驟才能匹配 [!DNL Commerce] 現有產品 [!DNL Walmart] 清單和同步產品資料 [!DNL Commerce] 和 [!DNL Walmart]。 的 [!DNL Commerce] product必須至少有一個與以下產品標識符（產品ID）匹配的產品屬性 [!DNL Walmart]。

**必需 [!DNL Walmart] 產品ID**

| **接受類型** | **名稱** | **目的** | **可接受數字** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| 格丁 | 全球貿易項目 | 一般用途，全球使用 | 14位 |
| ISBN | 國際標準書號 | 平裝書、精裝書和電子書 | 10或13位 |
| ISSN | 國際標準序列號 | 8位序列號，用於識別所有媒體印刷和電子出版物上的各類雜誌、期刊、報紙和期刊 | 8位 |
| UPC | 通用產品代碼 | 標準零售跟蹤代碼 | 12位 |

如果目錄沒有匹配的屬性， [添加或轉換現有目錄屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html)。

## 映射唯一標識符

1. 從 **[!UICONTROL Listings]** 或 **[!UICONTROL Orders]** 頁，選擇 **[!UICONTROL Channel Settings]**。

1. 開 **[!UICONTROL Channel Settings]**&#x200B;選中 **[!UICONTROL Shipping Carriers]**。

   - 查找 [!DNL Walmart Marketplace] 屬性。

   - 從 [!DNL Commerce] 儲存目錄。

      以下示例映射 [!UICONTROL Walmart Marketplace UPC] 屬性。
   ![映射產品匹配條件的屬性](assets/products-map-attributes-for-match.png)

   - 選擇 **[!UICONTROL Save]**。



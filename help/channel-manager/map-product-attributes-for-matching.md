---
title: 配置產品匹配
description: 將Commerce產品與現有Walmart Marketplace清單匹配的映射屬性
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: e6368d30e16ccffcb1dfc64bdd56561116934b54
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# 配置產品匹配

在將清單發佈到Walmart Marketplace之前，請將至少一個產品目錄屬性的唯一標識符映射到所需的Walmart Marketplace產品標識符之一。 此步驟是在沃爾瑪市場上匹配產品所必需的。

對於產品匹配，Commerce產品在目錄屬性中必須至少具有以下產品標識符（產品ID）之一。

**需要的Walmart產品ID**

| **接受類型** | **名稱** | **目的** | **可接受數字** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| 格丁 | 全球貿易項目 | 一般用途，全球使用 | 14位 |
| ISBN | 國際標準書號 | 平裝書、精裝書和電子書 | 10或13位 |
| ISSN | 國際標準序列號 | 8位序列號，用於識別所有媒體印刷和電子出版物上的各類雜誌、期刊、報紙和期刊 | 8位 |
| ISBN | 國際標準書號 | 平裝本、硬封面和電子 | 12位 |

如果目錄中有其他類型的「產品ID」屬性，請將其轉換為所需類型之一。 然後，將其映射到Channel Manager商店的「清單」配置中相應的Walmart Marketplace屬性。

## 配置產品屬性設定

1. 在 [!UICONTROL Listings] 頁面，在 *草稿* 狀態。

1. 選擇 **[!UICONTROL Settings]**。

   - 查找要映射的Walmart Marketplace屬性。

   - 從儲存目錄中選擇相應的屬性。

      以下示例將Walmart Marketplace UPC屬性映射到產品目錄中的UPC屬性。
   ![映射產品匹配條件的屬性](assets/products-map-attributes-for--match.png)

   - 選擇 **[!UICONTROL Save]**。


## 更新映射的屬性配置

通過更新映射的屬性設定來更改匹配產品的Commerce產品標識符。

例如，您可以根據SKU進行匹配，而不是基於Commerce UPC產品屬性代碼進行匹配。 或者，映射其他屬性以改進匹配。

1. 從 **[!UICONTROL Listings]**&#x200B;選中 **[!UICONTROL Settings]**。

1. 在「映射」屬性窗體中，根據需要更改映射的屬性配置。

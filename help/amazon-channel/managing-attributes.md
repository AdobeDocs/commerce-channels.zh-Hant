---
title: 管理屬性
description: 您可以管理Commerce產品屬性對應至Amazon屬性，以確保系統之間的產品資訊準確。
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 管理屬性

Amazon和 [!DNL Commerce] 兩者都使用產品屬性系統（稱為屬性）來定義產品。 屬性可定義產品的說明、內容、影像、價格和各種資料。

商務與Amazon之間的成功通訊需要 [!DNL Commerce] 屬性可正確對應（或符合）至對應的Amazon屬性。 與Amazon整合時，您會將這些屬性對應至Amazon屬性。 完成後， [!DNL Commerce] 可以同步及維護您的Amazon清單，與 [!DNL Commerce] 產品目錄。

例如，假設您的 [!DNL Commerce] 目錄和Amazon清單。 產品的一個屬性可能是項目的上市價格。 此 [!DNL Commerce] 可能已命名 `Price`，而Amazon的上市價格可能已命名 `ListingPrice`. 您必須指示 [!DNL Commerce] 在與Amazon通訊時 [!DNL Commerce] 名為 `Price` 與名為的Amazon屬性相同 `ListingPrice`. 此程式稱為 _管理屬性_，包括建立新屬性和編輯現有屬性。 確保屬性匹配得當，可確保正確通信 [!DNL Commerce] 和Amazon。

設定屬性對應時， [!DNL Commerce] 可以與Amazon來回傳遞產品資訊。 如果您有Amazon產品清單， [!DNL Commerce] 可將您的Amazon產品和詳細資訊匯入 [!DNL Commerce] 目錄，可讓您從單一、集中的產品目錄管理Amazon清單。

Amazon銷售管道可讓您視需要存取、檢閱、建立及管理 [_[!UICONTROL Attributes]_檢視](./attributes-view.md) 在Amazon銷售管道首頁。 如果您新增屬性至 [!DNL Commerce] 目錄，則可能需要更新所有產品中的這些值。

如需 [!DNL Commerce] 和Amazon屬性集和值，請參閱：

- [管理屬性基本知識](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}
- [建立屬性](./creating-attributes.md#create-an-attribute)
- [編輯現有屬性](./creating-attributes.md#edit-an-attribute)
- [檢視屬性對應](./amazon-matching-attributes-values.md)
- [編輯或建立屬性對應](./amazon-manually-update-incomplete-listing.md)

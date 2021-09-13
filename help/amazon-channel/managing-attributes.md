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

Amazon和[!DNL Commerce]都使用產品屬性系統（稱為屬性）來定義產品。 屬性可定義產品的說明、內容、影像、價格和各種資料。

商務與Amazon之間的成功通訊需要將[!DNL Commerce]屬性正確對應（或符合）至對應的Amazon屬性。 與Amazon整合時，您會將這些屬性對應至Amazon屬性。 完成後，[!DNL Commerce]可以使用您的[!DNL Commerce]產品目錄來同步和維護您的Amazon清單。

例如，假設您的[!DNL Commerce]目錄和Amazon清單中有相同的項目。 產品的一個屬性可能是項目的上市價格。 [!DNL Commerce]中的掛牌價格名稱可能命名為`Price`，而Amazon的掛牌價格可能命名為`ListingPrice`。 您必須指示[!DNL Commerce]，在與Amazon通訊時，名為`Price`的[!DNL Commerce]屬性與名為`ListingPrice`的Amazon屬性相同。 此過程稱為&#x200B;_管理屬性_，包括建立新屬性和編輯現有屬性。 請確定屬性已正確匹配，以確保[!DNL Commerce]和Amazon之間有正確的通訊。

設定屬性對應時，[!DNL Commerce]可以與Amazon來回傳遞產品資訊。 如果您有Amazon產品清單，[!DNL Commerce]可將您的Amazon產品和詳細資訊匯入[!DNL Commerce]目錄，讓您從單一集中的產品目錄管理Amazon清單。

Amazon銷售管道可讓您視需要，在Amazon銷售管道首頁的&#x200B;[_[!UICONTROL Attributes]_檢視](./attributes-view.md)中存取、檢閱、建立及管理屬性。 如果您將屬性新增至[!DNL Commerce]目錄，則可能需要更新所有產品中的這些值。

有關[!DNL Commerce]和Amazon屬性集和值的詳細資訊，請參閱：

- [管理屬性基本知識](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}
- [建立屬性](./creating-attributes.md#create-an-attribute)
- [編輯現有屬性](./creating-attributes.md#edit-an-attribute)
- [檢視屬性對應](./amazon-matching-attributes-values.md)
- [編輯或建立屬性對應](./amazon-manually-update-incomplete-listing.md)

---
title: 管理屬性
description: 您可以管理Commerce產品屬性到Amazon屬性的映射，以確保系統之間的產品資訊準確。
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# 管理屬性

Amazon [!DNL Commerce] 兩者都使用產品屬性系統（稱為屬性）來定義產品。 屬性定義產品的說明、內容、影像、價格和各種資料。

Commerce和Amazon之間的成功溝通需要 [!DNL Commerce] 屬性被正確映射（或匹配）到相應的Amazon屬性。 與Amazon整合時，將這些屬性映射到Amazon屬性。 完成後， [!DNL Commerce] 可以同步和維護您的Amazon清單 [!DNL Commerce] 產品目錄。

例如，假設您在 [!DNL Commerce] 目錄和Amazon的清單。 產品的一個屬性可能是項目的列價。 中的上市價格的名稱 [!DNL Commerce] 可能已命名 `Price`，而Amazon的上市價格則可能 `ListingPrice`。 您必須指示 [!DNL Commerce] 在和Amazon通訊時， [!DNL Commerce] 屬性 `Price` 與名為「C」的Amazon屬性 `ListingPrice`。 此進程稱為 _管理屬性_，包括建立新屬性和編輯現有屬性。 確保屬性正確匹配可確保在以下位置之間正確通信 [!DNL Commerce] 和Amazon。

設定屬性映射時， [!DNL Commerce] 可以與Amazon來回傳遞產品資訊。 如果你有Amazon產品清單， [!DNL Commerce] 可以將你的Amazon產品和細節 [!DNL Commerce] 目錄，允許您從單個中央產品目錄管理您的Amazon清單。

Amazon銷售渠道允許您根據需要訪問、查看、建立和管理屬性 [_[!UICONTROL Attributes]_視圖](./attributes-view.md) 在Amazon銷售渠道首頁上。 如果向 [!DNL Commerce] 目錄，它可能需要更新所有產品中的這些值。

有關 [!DNL Commerce] 和Amazon屬性集和值，請參閱：

- [管理屬性基礎知識](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"}
- [建立屬性](./creating-attributes.md#create-an-attribute)
- [編輯現有屬性](./creating-attributes.md#edit-an-attribute)
- [查看屬性映射](./amazon-matching-attributes-values.md)
- [編輯或建立屬性映射](./amazon-manually-update-incomplete-listing.md)

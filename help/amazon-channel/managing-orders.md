---
title: 管理訂單
description: 您可以在「訂單設定」中啟用訂單導入，以便更輕鬆地從商務管理員管理您的Amazon訂單。
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 管理訂單

您可以查看從Amazon收到的Amazon訂單資訊， _[!UICONTROL Recent Orders]_的下界 [儲存儀表板](./amazon-store-dashboard.md) 或_[!UICONTROL Amazon orders]_ 頁(也稱為 _[!UICONTROL All Orders]_)。

如何管理您的Amazon訂單取決於您的訂單導入是啟用還是禁用 [訂單設定](./order-settings.md#configure-order-settings)。

## 啟用訂單導入

之後 [儲存整合](./store-integration.md)，也請參見Wiki頁。 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 設定 `Enabled` 預設值。 使用此設定時， [!DNL Commerce] 為您的Amazon訂單建立訂單，可在 [[!DNL Commerce] 訂單](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 工作流。

>[!NOTE]
>
>無論您的訂單導入設定如何，您的訂單中存在的Amazon訂單 [!DNL Amazon Seller Central] 帳戶 [儲存整合](./store-integration.md) 未導入。

導入的Amazon訂單在 [[!DNL Commerce] 訂單](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} workflow, just like your other [!DNL Commerce] stores. Click the Amazon order number in the *[!UICONTROL Order Number]* column to open the order in the [[!DNL Commerce] order process](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target="_blank"}。 請參閱 [查看Amazon訂單](./amazon-orders-all.md)。

### 訂單導入流程

當對Amazon和 [訂單導入](./order-settings.md) 啟用後，將開始以下進程。

| 更改 | 操作 |
|---|---|
| 命令Amazon。 | <ul><li>Amazon將訂單狀態設定為 `Pending`。</li><li>訂單資訊已發送到 [!DNL Commerce]。</li><li>訂單已添加到 [_Amazon訂單_ 表](./amazon-orders-all.md) 帶 `Pending` 狀態。</li></ul> |
| Amazon將訂單狀態更改為 `Unshipped`。 | <ul><li>狀態更改已發送到 [!DNL Commerce]。</li><li>在 [_Amazon訂單_ 表](./amazon-orders-all.md)，訂單狀態更改為 `Unshipped`。</li><li>在 [[!DNL Commerce] 訂單工作流](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}，對應 [!DNL Commerce] 使用 `Processing` 狀態。</li></ul> |
| 在 [[!DNL Commerce] 訂單工作流](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}，也請參見Wiki頁。 [!DNL Commerce] 訂單已處理，狀態更改為 `Shipped`。 | <ul><li>在 [_Amazon訂單_ 表](./amazon-orders-all.md)，訂單狀態更改為 `Shipped`。</li><li>在下一個cron作業上，訂單狀態將更改為 `Complete` 的 [[!DNL Commerce] 訂單工作流](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}。</li></ul> |

### 訂單建立阻止程式

有幾種情況可阻止建立相應的 [!DNL Commerce] 命令。 [!DNL Commerce] 不會為在出現以下任何問題時收到的訂單建立訂單。

| 方案 | 解決方案 |
|---|---|
| 中不存在該項 [!DNL Commerce] 目錄。 | [建立產品](./creating-assigning-catalog-products.md) 在 [!DNL Commerce] 目錄和 [手動匹配](./creating-assigning-catalog-products.md) 就是產品。 |
| 目錄中的項已禁用。 | 確保 [產品狀態](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target="_blank"} 的子菜單。 |
| 訂購的物料缺貨。 | 更新或配置 [產品選項](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target="_blank"} 數量和來源。 |

當無法導入訂單時，螢幕頂部將顯示類似以下的系統消息：

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

問題解決後， [!DNL Commerce] 將在下次同步時建立訂單。

## 禁用訂單導入

如果您不想導入和管理您的Amazon訂單 [!DNL Commerce]，您可以更改 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 設定 `Disabled`。 此設定表示當從Amazon收到新訂單時， [!DNL Commerce] 未建立訂單。

禁用後，從Amazon接收的訂單資訊將顯示在 _[!UICONTROL Recent Orders]_的_[!UICONTROL All Orders]_ 的子菜單。 此訂單資訊僅查看，您必須在 [!DNL Amazon Seller Central]。 要在中開啟訂單詳細資訊，請執行以下操作： [!DNL Amazon Seller Central]，按一下 _[!UICONTROL Order Number]_的雙曲餘切值。

另請參閱 [查看Amazon訂單](./amazon-orders-all.md)。 [查看Amazon訂單詳細資訊](./amazon-order-details.md), [普通訂單處理任務](./common-order-processing.md)。

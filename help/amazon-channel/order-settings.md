---
title: 訂單設定
description: 使用「訂單」設定確定如何將Amazon訂單導入您的Commerce商店並在其中處理。
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# 訂單設定

訂單設定定義是否以及如何將Amazon訂單導入和處理 [!DNL Commerce] 可以在 [儲存儀表板](./amazon-store-dashboard.md)。

訂單導入設定設定為 `Enabled` 預設情況下，這意味著您的Amazon訂單將出現在商店儀表板上並建立相應的 [!DNL Commerce] 命令。 可以在 [!DNL Commerce] [訂單](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 工作流。

>[!NOTE]
>
>無論您的訂單設定如何，在您的商店整合之前存在的Amazon訂單都不會被導入。

之後 [儲存整合](./store-integration.md) 完成，您可以更改訂單設定。 如果將訂單設定設定為 `Disabled`,Amazon訂單顯示在商店儀表板上，但必須在您的 [!DNL Amazon Seller Central] 帳戶。

在Amazon上建立訂單時，不會立即導入 [!DNL Commerce]。 Amazon `Pending` 新建立訂單的狀態。 在Amazon驗證訂單和付款方式後，訂單的狀態將更改為 `Unshipped`。 此狀態更改觸發訂單導入， [!DNL Commerce] 建立匹配的對應順序。

從Amazon導入的訂單可在 [!DNL Commerce] [訂單工作流](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}。 另請參閱 [管理訂單](./managing-orders.md)。

## 配置訂單設定 {#configure-order-settings}

1. 按一下 **[!UICONTROL Order Settings]** 在商店儀表板上。

1. 對於 **[!UICONTROL Import Amazon Orders]** （必需），選擇選項：

   - `Disabled`  — 選擇您不想在 [!DNL Commerce] 從Amazon收到新訂單。 選中後，此頁上的所有其他欄位都將被禁用。

   - `Enabled`  — （預設）選擇建立相應的 [!DNL Commerce] 從Amazon接到新訂單。 [!DNL Commerce] 訂單根據Amazon狀態和庫存水準建立。

      >[!NOTE]
      >
      >導入Amazon訂單必須設定為 `Enabled` 管理Amazon的訂單 [!DNL Commerce] [訂單](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 工作流。 設定為時 `Disabled`你的Amazon訂單沒有 [!DNL Commerce] 訂單號，無法管理 [!DNL Commerce]。 您可以管理您的 [!DNL Amazon Seller Central] 帳戶。

1. 對於 **[!UICONTROL Import Amazon Orders Into Magento Store]**，選擇 [!DNL Commerce] 儲存當在中建立相應訂單時與關聯的Amazon訂單 [!DNL Commerce]。

   此設定預設為在您 [添加了Amazon店](./store-integration.md)。 如果要更改此設定，則選項清單取決於 [!DNL Commerce] 在配置中設定的儲存。 請參閱 [商店](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){target="_blank"}。

1. 對於 **[!UICONTROL Customer Creation]**，選擇選項：

   - `No Customer Creation (guest)`  — （預設）選擇您不想在中建立客戶帳戶的時間 [!DNL Commerce] 使用從Amazon訂單導入的客戶資料。 選擇後， [!DNL Commerce] 處理導入的Amazon訂單，其處理來賓簽出的方式與 [!DNL Commerce]。

   - `Build New Customer Account`  — 選擇要在中建立新客戶帳戶的時間 [!DNL Commerce] 使用隨Amazon訂單導入的客戶資料。 此選項有助於根據您的Amazon訂單構建客戶資料庫。

1. 對於 **[!UICONTROL Order Number Source]**，選擇選項：

   - `Build Using Magento Order Number`  — （預設）選擇要建立唯一 [!DNL Commerce] 相應Amazon訂單的訂單編號 [!DNL Commerce] 增量分配的訂單ID。

   - `Build Using Amazon Order Number`  — 選擇建立時間 [!DNL Commerce] 訂單編號，使用相應的Amazon分配的訂單編號。
   >[!NOTE]
   >
   >導入訂單後，Amazon訂單編號將顯示在 _[!UICONTROL Recent Orders]_清單中。 的 [!DNL Commerce] 訂單編號在查看訂單詳細資訊時顯示 [!DNL Commerce] [訂單](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 工作區。

1. 對於 **[!UICONTROL Order Status]** （必需），選擇選項：

   - `Default Order Status`  — （預設）選擇何時要將從Amazon導入的新建立訂單分配給新訂單的定義預設訂單狀態。 新訂單的預設狀態（除非您已為新訂單建立自定義訂單狀態）為 `Pending`。 請參閱 [處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}。

   - `Custom Order Status`  — 選擇何時將從Amazon導入的新建立訂單分配為預設狀態以外的狀態。

   - `Processing Order Status`  — 啟用時間 **[!UICONTROL Order Status]** 設定為 `Custom Order Status`。 選擇要用於從Amazon導入的新建立訂單的狀態。 此欄位中的選項基於中的預設狀態選項 [!DNL Commerce]。 請參閱 [訂單狀態](https://docs.magento.com/user-guide/sales/order-status.html)。 您還可以建立自定義訂單狀態，以在此顯示供選擇。 要建立自定義訂單狀態，請參閱 [自定義訂單狀態](https://docs.magento.com/user-guide/sales/order-status-custom.html){target="_blank"}。

1. 完成後，按一下 **[!UICONTROL Save order settings]**。

![訂單設定](assets/amazon-order-settings.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Import Amazon Orders] | 選項：<ul><li>**[!UICONTROL Disabled]**  — 選擇您不想在 [!DNL Commerce] 從Amazon收到新訂單。 選中後，此頁上的所有其他欄位都將被禁用。</li><li>**[!UICONTROL Enabled]**  — （預設）選擇建立相應的 [!DNL Commerce] 從Amazon接到新訂單。 [!DNL Commerce] 訂單根據Amazon狀態和庫存水準建立。</li></ul><br><br>`Enabled` 必須選擇在Amazon [!DNL Commerce]。 當 `Disabled` 已選擇，您的Amazon訂單將顯示在商店控制面板上，但訂單必須在您的 [!DNL Amazon Seller Central] 帳戶。 |
| [!UICONTROL Import Amazon Orders Into Magento Store] | 選擇 [!DNL Commerce] 儲存當在中建立Amazon訂單時，與 [!DNL Commerce] [訂單](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} workspace. This setting defaults to the Store View for the [!DNL Commerce] website selected when you [added the Amazon store](./store-integration.md). If you want to change this setting, the list of options depends on the [!DNL Commerce] stores you have set up in your configuration. See [Stores](https://docs.magento.com/user-guide/stores/stores-all-stores.html){target="_blank"}。 |
| [!UICONTROL Customer Creation] | 選項：<ul><li>**[!UICONTROL No Customer Creation (guest)]**  — （預設）選擇您不想在中建立客戶帳戶的時間 [!DNL Commerce] 使用從Amazon訂單導入的客戶資料。 當選中時，此選項將指示 [!DNL Commerce] 處理導入的Amazon訂單與處理來賓結帳的方式相同。</li><li>**[!UICONTROL Build New Customer Account]**  — 選擇在您的 [!DNL Commerce] 使用隨Amazon訂單導入的客戶資料的客戶資料庫。 此選項可幫助您 [!DNL Commerce] 客戶資料庫。</li></ul> |
| 訂單編號來源 | 選項：<ul><li>**[!UICONTROL Build Using Magento Order Number]**  — （預設）選擇要建立唯一 [!DNL Commerce] 相應Amazon訂單的訂單編號 [!DNL Commerce] 增量分配的訂單ID。 </li><li>**使用Amazon訂單號生成**  — 選擇建立時間 [!DNL Commerce] 訂單編號，使用相應的Amazon分配的訂單編號。</li></ul> |
| 待定訂單 | 選項：<ul><li>**[!UICONTROL Do Not Reserve Quantity]**  — 選擇不希望 [!DNL Commerce] 受您的Amazon訂單影響的庫存數量。 選擇是否將Amazon用於履行流程(FBA)。 選擇後，您收到了Amazon訂單，訂購的數量不會影響您的 [!DNL Commerce] 庫存數量。</li><li>**[!UICONTROL Reserve Quantity]**  — 選擇您希望Amazon訂單中的訂單數量在您的 [!DNL Commerce] 庫存數量。 當您選擇並收到Amazon訂單時，訂購的數量將「保留」 [!DNL Commerce] 庫存數量，防止 [!DNL Commerce] &quot;過度拋售&quot;的股票。 「保留」數量無法通過您的 [!DNL Commerce] 店面。</li></ul> |
| [!UICONTROL Order Status] | 選項：<ul><li>**[!UICONTROL Default Order Status]**  — （預設）選擇希望將從Amazon導入的新建立訂單分配給新訂單的預設訂單狀態的時間。 新訂單的預設狀態（除非您已為新訂單建立自定義訂單狀態）為 `Pending`。 請參閱 [處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html)。</li><li>>**[!UICONTROL Custom Order Status]**  — 選擇何時將從Amazon導入的新建立訂單分配為預設狀態以外的狀態。 選擇後， **[!UICONTROL Processing Order Status]** 允許您選擇要用於從Amazon導入的新建立訂單的狀態。</li></ul> |
| [!UICONTROL Processing Orders Status] | 啟用時間 _[!UICONTROL Order Status]_設定為 `Custom Order Status`。 選擇要分配給新訂單的訂單狀態。 此欄位中的選項取決於中的預設狀態選項 [!DNL Commerce]。 請參閱 [訂單狀態](https://docs.magento.com/user-guide/sales/order-status.html){target="_blank"}. You can also create a custom order status to show here. To create a custom order status, see [Custom Order Status](https://docs.magento.com/user-guide/sales/order-status-custom.html){target="_blank"}。 |

## [!DNL Commerce] 訂單建立

[!DNL Commerce] 根據以下狀態和庫存條件為Amazon訂單建立訂單。

### 與Inventory management

>[!NOTE]
>
>僅在Adobe Commerce和Magento Open Source2.3.x整合中支援。

| 履行渠道 | [!DNL Commerce] 庫存狀態 | Amazon訂單狀態 | [!UICONTROL Create Magento Order] 設定 | 庫存已保留 |
|---|---|---|---|---|
| FBA | 庫存<br>缺貨<br>不管理 | 待定 | 否 | 否 |
| FBA | 庫存<br>缺貨<br>不管理 | 掛起可用性 | 否 | 否 |
| FBA | 庫存<br>缺貨<br>不管理 | 已取消 | 否 | 否 |
| FBA | 庫存<br>缺貨<br>不管理 | 錯誤 | 否 | 否 |
| FBA | 庫存<br>缺貨<br>不管理 | 未發運 | 否 | 否 |
| FBA | 庫存<br>缺貨<br>不管理 | 部分發運 | 否 | 否 |
| FBA | 庫存<br>不管理 | 已發運 | 是 | 否 |
| FBA | 缺貨 | 已發運 | 否 | 否 |
| FBM | 庫存<br>缺貨<br>不管理 | 待定 | 否 | 否 |
| FBM | 庫存<br>缺貨<br>不管理 | 掛起可用性 | 否 | 否 |
| FBM | 庫存<br>缺貨<br>不管理 | 已取消 | 否 | 否 |
| FBM | 庫存<br>缺貨<br>不管理 | 錯誤 | 否 | 否 |
| FBM | 庫存<br>不管理 | 未發運 | 是 | 是 |
| FBM | 缺貨 | 未發運 | 否 | 否 |
| FBM | 庫存<br>不管理 | 部分發運 | 是 | 是 |
| FBM | 缺貨 | 部分發運 | 否 | 否 |
| FBM | 庫存<br>不管理 | 已發運 | 是 | 是 |
| FBM | 缺貨 | 已發運 | 否 | 否 |

>[!NOTE]
>如果Amazon訂單導入 `Partially Shipped` 或 `Shipped` 狀態，建立的庫存保留適用於訂單中的所有物料。 Amazon銷售渠道不會補償以前發運的產品。
>
>如果訂單由Amazon(FBA)履行，但物料在 `out of stock` 狀態， [!DNL Commerce] 無法建立相應的訂單。 這是Inventory management整合的局限。

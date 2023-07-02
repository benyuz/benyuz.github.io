# GooglePlayBilling

版本:5.0
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=GooglePlayBilling)

# BillingClient
完整类名：anywheresoftware.b4a.objects.BillingClientWrapper
> 所有者：process

?> 说明：Google Play计费库包装。
> 事件：
>
> Connected (Result As BillingResult)
>
> SkuQueryCompleted (Result As BillingResult, SkuDetails As List)
>
> PurchasesQueryCompleted (Result As BillingResult, Purchases As List)
>
> PurchasesUpdated (Result As BillingResult, Purchases As List)
>
> ConsumeCompleted (Result As BillingResult)
>
> AcknowledgeCompleted (Result As BillingResult)

> 所需权限：
com.android.vending.BILLING
## VerifyPurchase方法
**VerifyPurchase(Purchase,Base64Key)**

?> 说明：测试购买的签名是否正确。
>
> 参数：Purchase，类型：anywheresoftware.b4a.objects.BillingClientWrapper.PurchaseWrapper
>
> 参数：Base64Key，类型：java.lang.String
>
> 返回值：boolean
## InitializeWithBuilder方法
**InitializeWithBuilder(ba,EventName,Builder)**

?> 说明：接受自定义客户端生成器的可选初始化方法。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Builder，类型：com.android.billingclient.api.BillingClient.Builder
>
> 返回值：void
## Consume方法
**Consume(ba,PurchaseToken,Unused)**

?> 说明：消费产品。此调用之后，它将不会被“拥有”。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：PurchaseToken，类型：java.lang.String
>
> 参数：Unused，类型：java.lang.String
>
> 返回值：java.lang.Object
## AcknowledgePurchase方法
**AcknowledgePurchase(ba,PurchaseToken,Unused)**

?> 说明：所有购买必须在3天内确认或消费。调用此方法以确认购买。
```vbnet
Wait For (Billing.AcknowledgePurchase(p.PurchaseToken, "")) Billing_AcknowledgeCompleted (Result As BillingResult)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：PurchaseToken，类型：java.lang.String
>
> 参数：Unused，类型：java.lang.String
>
> 返回值：java.lang.Object
## QueryPurchases方法
**QueryPurchases(ba,SkuType)**

?> 说明：获取所有自有产品的购买详细信息。检查采购状态，因为还将列出待处理的采购。
```vbnet

Wait For (Starter.Billing.ConnectIfNeeded) Billing_Connected (Result As BillingResult)
If Result.IsSuccess Then
	Wait For (Starter.Billing.QueryPurchases("inapp")) Billing_PurchasesQueryCompleted (Result As BillingResult, Purchases As List)
	If Result.IsSuccess Then
		For Each Purchase As Purchase In Purchases
			
		Next
	End If
End If
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：SkuType，类型：java.lang.String
>
> 返回值：java.lang.Object
## LaunchBillingFlow方法
**LaunchBillingFlow(ba,Sku)**

?> 说明：启动计费流程。返回BillingResult。如果购买已完成（成功或未成功），将引发PurchasesUpdated事件。
```vbnet

Result = Starter.Billing.LaunchBillingFlow(SkuDetails.Get(0))
Log("LaunchBillingFlow: " & Result.IsSuccess)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Sku，类型：anywheresoftware.b4a.objects.BillingClientWrapper.SkuDetailsWrapper
>
> 返回值：anywheresoftware.b4a.objects.BillingClientWrapper.BillingResultWrapper
## QuerySkuDetails方法
**QuerySkuDetails(ba,SkuType,SKUs)**

?> 说明：获取指定SKU的详细信息。
```vbnet

Dim sf As Object = Starter.Billing.QuerySkuDetails("inapp", Array("android.test.purchased"))
Wait For (sf) Billing_SkuQueryCompleted (Result As BillingResult, SkuDetails As List)
If Result.IsSuccess And SkuDetails.Size = 1 Then
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：SkuType，类型：java.lang.String
>
> 参数：SKUs，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：java.lang.Object
## ConnectIfNeeded方法
**ConnectIfNeeded(ba)**

?> 说明：如果尚未连接，则连接到存储服务。在提出其他请求之前应始终调用。
```vbnet
Wait For (Billing.ConnectIfNeeded) Billing_Connected (Result As BillingResult)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：java.lang.Object
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化计费客户端。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SubscriptionsSupported属性

?> 说明：测试是否支持订阅。
>
> 返回值：boolean

# SkuDetails
完整类名：anywheresoftware.b4a.objects.BillingClientWrapper.SkuDetailsWrapper
> 所有者：process

> 包装器：com.android.billingclient.api.ProductDetails

?> 说明：产品详细信息。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Description属性

?> 说明：返回产品说明。
>
> 返回值：java.lang.String
## Price属性

?> 说明：返回一次性购买优惠的带货币符号的格式化价格。
>
> 返回值：java.lang.String
## Title属性

?> 说明：返回产品标题。
>
> 返回值：java.lang.String
## Sku属性

?> 说明：返回产品id。
>
> 返回值：java.lang.String

# BillingResult
完整类名：anywheresoftware.b4a.objects.BillingClientWrapper.BillingResultWrapper
> 所有者：process

> 包装器：com.android.billingclient.api.BillingResult

?> 说明：有关操作结果的信息。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## IsSuccess属性

?> 说明：测试结果是否成功。当结果不成功时，以调试模式记录响应代码和调试字符串。
>
> 返回值：boolean
## ResponseCode属性

?> 说明：返回响应代码。CODE常量之一。
>
> 返回值：int
## ResponseCodeString属性

?> 说明：以字符串形式返回响应代码。
>
> 返回值：java.lang.String
## DebugMessage属性

?> 说明：返回调试消息。
>
> 返回值：java.lang.String
## CODE_OK字段
>
> 返回值：int
## CODE_BILLING_UNAVAILABLE字段
>
> 返回值：int
## CODE_ITEM_UNAVAILABLE字段
>
> 返回值：int
## CODE_SERVICE_DISCONNECTED字段
>
> 返回值：int
## CODE_FEATURE_NOT_SUPPORTED字段
>
> 返回值：int
## CODE_SERVICE_TIMEOUT字段
>
> 返回值：int
## CODE_ITEM_ALREADY_OWNED字段
>
> 返回值：int
## CODE_SERVICE_UNAVAILABLE字段
>
> 返回值：int
## CODE_ERROR字段
>
> 返回值：int
## CODE_USER_CANCELED字段
>
> 返回值：int
## CODE_DEVELOPER_ERROR字段
>
> 返回值：int
## CODE_ITEM_NOT_OWNED字段
>
> 返回值：int

# Purchase
完整类名：anywheresoftware.b4a.objects.BillingClientWrapper.PurchaseWrapper
> 所有者：process

> 包装器：com.android.billingclient.api.Purchase
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## IsAcknowledged属性

?> 说明：测试是否确认购买。所有购买应在3天内确认或消费。
>
> 返回值：boolean
## PurchaseTime属性

?> 说明：返回购买产品的时间。
>
> 返回值：long
## PurchaseToken属性

?> 说明：返回一个令牌，该令牌唯一标识给定时间和用户对的购买。
>
> 返回值：java.lang.String
## DeveloperPayload属性

?> 说明：已弃用。
>
> 返回值：java.lang.String
## Signature属性

?> 说明：获取购买数据签名。
>
> 返回值：java.lang.String
## OrderId属性

?> 说明：返回事务的唯一订单标识符。
>
> 返回值：java.lang.String
## Sku属性

?> 说明：返回产品id
>
> 返回值：java.lang.String
## OriginalJson属性

?> 说明：获取包含购买信息的json字符串。
>
> 返回值：java.lang.String
## PurchaseState属性

?> 说明：返回购买状态。STATE常量之一。
>
> 返回值：int
## IsAutoRenewing属性

?> 说明：测试订阅是否自动续订。
>
> 返回值：boolean
## STATE_PENDING字段
>
> 返回值：int
## STATE_UNSPECIFIED字段
>
> 返回值：int
## STATE_PURCHASED字段
>
> 返回值：int

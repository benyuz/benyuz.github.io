# FirebaseNotifications

版本:3.1
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=FirebaseNotifications)

# FirebaseMessaging
完整类名：anywheresoftware.b4a.objects.FirebaseNotificationsService.FirebaseMessageWrapper
> 所有者：process

> 包装器：com.google.firebase.messaging.FirebaseMessaging

> 依赖：com.google.firebase:firebase-messaging | com.google.firebase:firebase-core
> 事件：
>
> TokenRefresh (Token As String)
>
> MessageArrived (Message As RemoteMessage)
## HandleIntent方法
**HandleIntent(Intent)**

?> 说明：应从Service_Start调用。如果意图已处理，则返回true。
>
> 参数：Intent，类型：android.content.Intent
>
> 返回值：boolean
## SubscribeToTopic方法
**SubscribeToTopic(Topic)**

?> 说明：订阅指定的主题。
```vbnet

fm.SubscribeToTopic("general")
```

>
> 参数：Topic，类型：java.lang.String
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## UnsubscribeFromTopic方法
**UnsubscribeFromTopic(Topic)**

?> 说明：取消订阅某个主题。
>
> 参数：Topic，类型：java.lang.String
>
> 返回值：void
## Token属性

?> 说明：返回设备令牌。令牌可以随时更改。令牌更改时会引发TokenRefresh事件。
>
> 返回值：java.lang.String

# RemoteMessage
完整类名：anywheresoftware.b4a.objects.FirebaseNotificationsService.RemoteMessageWrapper
> 所有者：process

> 包装器：com.google.firebase.messaging.RemoteMessage

> 依赖：com.google.firebase:firebase-messaging | com.google.firebase:firebase-core

?> 说明：保存推送消息数据。
## GetData方法
**GetData()**

?> 说明：返回一个Map，其中键/值设置为消息数据。
>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## SentTime属性

?> 说明：返回消息的发送时间。
>
> 返回值：long
## From属性

?> 说明：返回发件人id或主题名称。在后一种情况下，值将以/topics开头/
>
> 返回值：java.lang.String
## CollapseKey属性

?> 说明：获取折叠键（如果已设置）。
>
> 返回值：java.lang.String
## MessageId属性

?> 说明：获取消息id。
>
> 返回值：java.lang.String

# BLE2

版本:1.39
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=BLE2)

# BleManager2
完整类名：anywheresoftware.b4a.objects.BleManager2
> 所有者：process

?> 说明：此库将取代BLE库。它允许您搜索并连接到BLE设备。
> 事件：
>
> StateChanged (State As Int)
>
> DeviceFound (Name As String, DeviceId As String, AdvertisingData As Map, RSSI As Double)
>
> Disconnected
>
> Connected (Services As List)
>
> DataAvailable (ServiceId As String, Characteristics As Map)
>
> WriteComplete (Characteristic As String, Status As Int)
>
> RssiAvailable (Success As Boolean, RSSI As Double)
>
> MtuChanged (Success As Boolean, MTU As Int)

> 所需权限：
android.permission.BLUETOOTH
android.permission.BLUETOOTH_ADMIN
## Connect方法
**Connect(DeviceId)**

?> 说明：连接到具有给定id的设备。您只能连接到以前发现的设备。
>
> 参数：DeviceId，类型：java.lang.String
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象。StateChanged事件将在具有当前BLE状态的此方法之后引发。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetNotify方法
**SetNotify(Service,Characteristic,Notify)**

?> 说明：添加或删除用于监视值更改的通知侦听器。
>
> 参数：Service，类型：java.lang.String
>
> 参数：Characteristic，类型：java.lang.String
>
> 参数：Notify，类型：boolean
>
> 返回值：boolean
## GetCharacteristicProperties方法
**GetCharacteristicProperties(Service,Characteristic)**

?> 说明：返回一个数值，您可以从中查找指定特征的属性。
>
> 参数：Service，类型：java.lang.String
>
> 参数：Characteristic，类型：java.lang.String
>
> 返回值：int
## ReadRemoteRssi方法
**ReadRemoteRssi()**

?> 说明：读取连接设备的RSSI值。当值可用时，将引发RssiAvailable事件。
>
> 返回值：void
## StopScan方法
**StopScan()**

?> 说明：停止扫描新设备。
>
> 返回值：void
## SetIndication方法
**SetIndication(Service,Characteristic,Notify)**

?> 说明：类似于SetNotify。将描述符值设置为2（指示），而不是1（通知）。
>
> 参数：Service，类型：java.lang.String
>
> 参数：Characteristic，类型：java.lang.String
>
> 参数：Notify，类型：boolean
>
> 返回值：boolean
## Disconnect方法
**Disconnect()**
>
> 返回值：void
## Scan2方法
**Scan2(ServiceUUIDs,AllowDuplicates)**

?> 说明：类似于扫描。如果AllowDuplicates为true，则每当接收到数据包时都会引发DeviceFound事件。
>
> 参数：ServiceUUIDs，类型：anywheresoftware.b4a.objects.collections.List
>
> 参数：AllowDuplicates，类型：boolean
>
> 返回值：void
## GetRecordsFromAdvertisingData方法
**GetRecordsFromAdvertisingData(AdvertisingData,Key)**

?> 说明：返回一个包含指定类型的所有记录的列表。
>
> 参数：AdvertisingData，类型：anywheresoftware.b4a.objects.collections.Map
>
> 参数：Key，类型：int
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## RequestMtu方法
**RequestMtu(MTU)**

?> 说明：请求更改MTU大小（数据包大小）。将引发MtuChanged事件。
>
> 参数：MTU，类型：int
>
> 返回值：boolean
## Scan方法
**Scan(ServiceUUIDs)**

?> 说明：开始扫描设备。当找到设备时，将引发DeviceFound事件。
>
> 参数：ServiceUUIDs，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## Connect2方法
**Connect2(DeviceId,AutoConnect)**

?> 说明：类似于Connect。允许您禁用自动连接。
>
> 参数：DeviceId，类型：java.lang.String
>
> 参数：AutoConnect，类型：boolean
>
> 返回值：void
## ReadData方法
**ReadData(Service)**

?> 说明：异步读取给定服务的所有特征。当数据可用时，将引发DataAvailable。
>
> 参数：Service，类型：java.lang.String
>
> 返回值：void
## ReadData2方法
**ReadData2(Service,Characteristic)**

?> 说明：异步读取指定特征的值。
>
> 参数：Service，类型：java.lang.String
>
> 参数：Characteristic，类型：java.lang.String
>
> 返回值：void
## WriteData方法
**WriteData(Service,Characteristic,Data)**

?> 说明：将数据写入指定的特性。
>
> 参数：Service，类型：java.lang.String
>
> 参数：Characteristic，类型：java.lang.String
>
> 参数：Data，类型：byte[]
>
> 返回值：void
## State属性

?> 说明：返回当前蓝牙适配器状态。
>
> 返回值：int
## STATE_POWERED_OFF字段
>
> 返回值：int
## STATE_UNSUPPORTED字段
>
> 返回值：int
## STATE_POWERED_ON字段
>
> 返回值：int

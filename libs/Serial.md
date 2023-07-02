# Serial

版本:1.31
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Serial)

# Serial
完整类名：anywheresoftware.b4a.objects.Serial
> 所有者：process

?> 说明：串行库允许您使用RFCOMM（也称为虚拟串行端口）连接其他蓝牙设备。
> 事件：
>
> Connected (Success As Boolean)

> 所需权限：
android.permission.BLUETOOTH
android.permission.BLUETOOTH_ADMIN
## GetPairedDevices方法
**GetPairedDevices()**

?> 说明：返回一个映射，其中成对设备的友好名称作为键，地址作为值。
```vbnet

Dim PairedDevices As Map
PairedDevices = Serial1.GetPairedDevices
Dim l As List
l.Initialize
For i = 0 To PairedDevices.Size - 1
	l.Add(PairedDevices.GetKeyAt(i))
Next
Dim res As Int
res = InputList(l, "Choose device", -1) 'show list with paired devices
If res <> DialogResponse.CANCEL Then
	Serial1.Connect(PairedDevices.Get(l.Get(res))) 'convert the name to mac address and connect
End If
```

>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## ListenInsecure方法
**ListenInsecure(ba,Admin,Port)**

?> 说明：开始侦听传入的未加密连接。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Admin，类型：anywheresoftware.b4a.objects.Serial.BluetoothAdmin
>
> 参数：Port，类型：int
>
> 返回值：void
## IsEnabled方法
**IsEnabled()**

?> 说明：测试蓝牙是否已启用。
>
> 返回值：boolean
## Connect方法
**Connect(ba,MacAddress)**

?> 说明：尝试连接到具有给定地址的设备。连接是在后台完成的。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：MacAddress，类型：java.lang.String
>
> 返回值：void
## StopListening方法
**StopListening()**

?> 说明：停止侦听传入连接。
>
> 返回值：void
## Listen方法
**Listen(ba)**

?> 说明：使用默认UUID开始侦听传入连接。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(EventName)**

?> 说明：已初始化对象。在尝试使用该对象之前，您可能需要调用IsEnabled。
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Disconnect方法
**Disconnect()**

?> 说明：断开连接（如果存在）并停止侦听新连接。
>
> 返回值：void
## Listen2方法
**Listen2(Name,UUID,ba)**

?> 说明：开始侦听传入连接。
>
> 参数：Name，类型：java.lang.String
>
> 参数：UUID，类型：java.lang.String
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Connect3方法
**Connect3(ba,MacAddress,Port)**

?> 说明：此方法是不使用connect或Connect2连接的硬件设备的解决方法。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：MacAddress，类型：java.lang.String
>
> 参数：Port，类型：int
>
> 返回值：void
## ConnectInsecure方法
**ConnectInsecure(ba,Admin,MacAddress,Port)**

?> 说明：尝试通过未加密的连接连接到设备。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Admin，类型：anywheresoftware.b4a.objects.Serial.BluetoothAdmin
>
> 参数：MacAddress，类型：java.lang.String
>
> 参数：Port，类型：int
>
> 返回值：void
## Connect2方法
**Connect2(ba,MacAddress,UUID)**

?> 说明：尝试连接到具有给定地址和UUID的设备。连接是在后台完成的。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：MacAddress，类型：java.lang.String
>
> 参数：UUID，类型：java.lang.String
>
> 返回值：void
## Address属性

?> 说明：返回当前设备的MAC地址。
>
> 返回值：java.lang.String
## InputStream属性

?> 说明：返回用于从其他设备读取数据的InputStream。
>
> 返回值：java.io.InputStream
## OutputStream属性

?> 说明：返回用于向其他设备写入数据的OutputStream。
>
> 返回值：java.io.OutputStream
## Name属性

?> 说明：返回当前设备的友好名称。
>
> 返回值：java.lang.String

# BluetoothAdmin
完整类名：anywheresoftware.b4a.objects.Serial.BluetoothAdmin
> 所有者：process

?> 说明：蓝牙管理允许您管理蓝牙适配器。
> 事件：
>
> StateChanged (NewState As Int, OldState As Int)
>
> DiscoveryStarted
>
> DiscoveryFinished
>
> DeviceFound (Name As String, MacAddress As String)

> 所需权限：
android.permission.BLUETOOTH
android.permission.BLUETOOTH_ADMIN
android.permission.ACCESS_COARSE_LOCATION
## StartDiscovery方法
**StartDiscovery()**

?> 说明：启动发现过程。您应该处理DiscoveryStarted、DiscoveryFinished和DeviceFound事件以获取有关进程的详细信息。
>
> 返回值：boolean
## CancelDiscovery方法
**CancelDiscovery()**

?> 说明：取消发现过程。
>
> 返回值：boolean
## IsEnabled方法
**IsEnabled()**

?> 说明：测试蓝牙适配器是否已启用。
>
> 返回值：boolean
## Enable方法
**Enable()**

?> 说明：打开蓝牙适配器。适配器不会立即准备好。您应该使用StateChanged事件来查找它何时被启用。
>
> 返回值：boolean
## IsInitialized方法
**IsInitialized()**

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象并设置将处理事件的子对象。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Disable方法
**Disable()**

?> 说明：关闭蓝牙适配器。适配器不会立即被禁用。您应该使用StateChanged事件来监视适配器。
>
> 返回值：boolean
## LastFoundIntent属性

?> 说明：可在DeviceFound事件内部使用，以从接收到的意图中提取更多数据。如果未收到任何意向，则返回未初始化的对象。
>
> 返回值：anywheresoftware.b4a.objects.IntentWrapper
## STATE_TURNING_OFF字段
>
> 返回值：int
## STATE_ON字段
>
> 返回值：int
## STATE_OFF字段
>
> 返回值：int
## STATE_TURNING_ON字段
>
> 返回值：int

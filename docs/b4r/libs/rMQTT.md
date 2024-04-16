# rMQTT

版本:1.4
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rMQTT)

# MqttConnectOptions
完整类名：B4R::MqttConnectOptions
## Initialize方法
**Initialize(UserName,Password)**

?> 说明：设置用户名和密码。传递空字符串以省略值。
>
> 参数：UserName，类型：B4R::B4RString*
>
> 参数：Password，类型：B4R::B4RString*
>
> 返回值：B4R::void
## SetLastWill方法
**SetLastWill(Topic,Message,QOS,Retained)**

?> 说明：设置最后一条遗嘱信息。如果客户端突然断开连接，则会发送此消息。
>
> 参数：Topic，类型：B4R::B4RString*
>
> 参数：Message，类型：B4R::B4RString*
>
> 参数：QOS，类型：Byte
>
> 参数：Retained，类型：bool
>
> 返回值：B4R::void
## Password字段
>
> 返回值：B4R::B4RString*
## UserName字段
>
> 返回值：B4R::B4RString*

# MqttClient
完整类名：B4R::MqttClient
> 事件：
>
> MessageArrived (Topic As String, Payload() As Byte)
>
> Disconnected
## Initialize方法
**Initialize(Stream,Ip,Port,ClientId,MessageArrivedSub,DisconnectedSub)**

?> 说明：初始化客户端。
>
> 参数：Stream，类型：B4R::B4RStream*
>
> 参数：Ip，类型：Byte[]
>
> 参数：Port，类型：UInt
>
> 参数：ClientId，类型：B4R::B4RString*
>
> 参数：MessageArrivedSub，类型：SubVoidStringByteArray
>
> 参数：DisconnectedSub，类型：SubVoidVoid
>
> 返回值：B4R::void
## Initialize2方法
**Initialize2(Stream,HostName,Port,ClientId,MessageArrivedSub,DisconnectedSub)**

?> 说明：类似于初始化。接受服务器主机名而不是ip地址。
>
> 参数：Stream，类型：B4R::B4RStream*
>
> 参数：HostName，类型：B4R::B4RString*
>
> 参数：Port，类型：UInt
>
> 参数：ClientId，类型：B4R::B4RString*
>
> 参数：MessageArrivedSub，类型：SubVoidStringByteArray
>
> 参数：DisconnectedSub，类型：SubVoidVoid
>
> 返回值：B4R::void
## Connect方法
**Connect()**

?> 说明：尝试连接到服务器。如果连接成功，则返回true。
>
> 返回值：bool
## Connect2方法
**Connect2(Options)**

?> 说明：类似于Connect。允许通过MqttConnectOptions对象传递连接选项。
>
> 参数：Options，类型：B4R::MqttConnectOptions*
>
> 返回值：bool
## Subscribe方法
**Subscribe(Topic,QOS)**

?> 说明：订阅给定的主题。QOS应为0或1。如果操作成功，则返回true。
>
> 参数：Topic，类型：B4R::B4RString*
>
> 参数：QOS，类型：Byte
>
> 返回值：bool
## Unsubscribe方法
**Unsubscribe(Topic)**

?> 说明：取消订阅给定主题。如果操作成功，则返回true。
>
> 参数：Topic，类型：B4R::B4RString*
>
> 返回值：bool
## Publish方法
**Publish(Topic,Payload)**

?> 说明：发布针对给定主题的消息。QOS设置为0。
>
> 参数：Topic，类型：B4R::B4RString*
>
> 参数：Payload，类型：Byte[]
>
> 返回值：bool
## Publish2方法
**Publish2(Topic,Payload,Retained)**

?> 说明：类似于发布。允许设置保留标志。
>
> 参数：Topic，类型：B4R::B4RString*
>
> 参数：Payload，类型：Byte[]
>
> 参数：Retained，类型：bool
>
> 返回值：bool
## Close方法
**Close()**

?> 说明：关闭客户端。
>
> 返回值：B4R::void
## BeginPublish方法
**BeginPublish(Topic,TotalLength,Retained)**

?> 说明：启动基于区块的发布。这允许发送大型邮件。
```vbnet

mqtt.BeginPublish("last", 100, False)
Dim buffer(5) As Byte
For i = 1 To 100 Step 5
	buffer(0) = i
	buffer(1) = i + 1
	buffer(2) = i + 2
	buffer(3) = i + 3
	buffer(4) = i + 4
	mqtt.WriteChunk(buffer)
Next
mqtt.EndPublish
```

>
> 参数：Topic，类型：B4R::B4RString*
>
> 参数：TotalLength，类型：UInt
>
> 参数：Retained，类型：bool
>
> 返回值：bool
## WriteChunk方法
**WriteChunk(Payload)**

?> 说明：写入一块数据。必须在调用BeginPublish和调用EndPublish之间调用。
>
> 参数：Payload，类型：Byte[]
>
> 返回值：bool
## EndPublish方法
**EndPublish()**

?> 说明：结束基于区块的发布。
>
> 返回值：bool

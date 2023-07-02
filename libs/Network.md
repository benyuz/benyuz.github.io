# Network

版本:1.53
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Network)

# Socket
完整类名：anywheresoftware.b4a.objects.SocketWrapper
> 所有者：process

?> 说明：Socket对象是网络通信的端点。
```vbnet
InputStream
```

> 事件：
>
> Connected (Successful As Boolean)

> 所需权限：
android.permission.INTERNET
## InitializeSSL方法
**InitializeSSL(EventName,KeyStoreStream,Password)**

?> 说明：初始化新的SSL套接字。
>
> 参数：EventName，类型：java.lang.String
>
> 参数：KeyStoreStream，类型：java.io.InputStream
>
> 参数：Password，类型：java.lang.String
>
> 返回值：void
## Connect方法
**Connect(ba,Host,Port,TimeOut)**

?> 说明：尝试连接到给定的地址。连接是在后台完成的。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Host，类型：java.lang.String
>
> 参数：Port，类型：int
>
> 参数：TimeOut，类型：int
>
> 返回值：void
## Close方法
**Close()**

?> 说明：关闭套接字和流。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Initialize方法
**Initialize(EventName)**

?> 说明：初始化新套接字。
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## ResolveHost方法
**ResolveHost(Host)**

?> 说明：解析主机名并返回IP地址。
>
> 参数：Host，类型：java.lang.String
>
> 返回值：java.lang.String
## InitializeSSLAcceptAll方法
**InitializeSSLAcceptAll(EventName)**

?> 说明：初始化自动接受所有证书的新SSL套接字。由于未测试服务器证书，因此此方法的安全性较差。
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Connected属性

?> 说明：测试插座是否已连接。
>
> 返回值：boolean
## TimeOut属性

?> 说明：获取或设置套接字的InputStream的超时。值是以毫秒为单位指定的。
>
> 参数：value，类型：int
>
> 返回值：int
## InputStream属性

?> 说明：返回用于读取数据的套接字的InputStream。
>
> 返回值：java.io.InputStream
## OutputStream属性

?> 说明：返回用于写入数据的套接字的OutputStream。
>
> 返回值：java.io.OutputStream

# ServerSocket
完整类名：anywheresoftware.b4a.objects.SocketWrapper.ServerSocketWrapper
> 所有者：process

?> 说明：ServerSocket对象允许其他计算机连接到此计算机。
> 事件：
>
> NewConnection (Successful As Boolean, NewSocket As Socket)

> 所需权限：
android.permission.INTERNET
android.permission.ACCESS_WIFI_STATE
android.permission.ACCESS_NETWORK_STATE
## GetMyIP方法
**GetMyIP()**

?> 说明：返回服务器的IP。如果找不到其他IP，将返回“127.0.0.1”（localhost）。
>
> 返回值：java.lang.String
## Listen方法
**Listen()**

?> 说明：开始在后台侦听传入连接。
>
> 返回值：void
## Close方法
**Close()**

?> 说明：关闭ServerSocket。这不会关闭任何其他插座。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,Port,EventName)**

?> 说明：初始化ServerSocket。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Port，类型：int
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## GetMyWifiIP方法
**GetMyWifiIP()**

?> 说明：返回wifi网络的IP地址。
>
> 返回值：java.lang.String

# UDPSocket
完整类名：anywheresoftware.b4a.objects.SocketWrapper.UDPSocket
> 所有者：process

?> 说明：UDPSocket支持发送和接收UDP数据包。发送数据包是通过调用Send方法完成的。
```vbnet

Sub process_globals
	Dim UDPSocket1 As UDPSocket
End Sub

Sub Globals

End Sub
Sub Activity_Create(FirstTime As Boolean)
	If FirstTime Then
		UDPSocket1.Initialize("UDP", 0, 8000)
	End If
	Dim Packet As UDPPacket
	Dim data() As Byte
	data = "Hello from Android".GetBytes("UTF8")
	Packet.Initialize(data, "10.0.0.1", 5000)
	UDPSocket1.Send(Packet)
End Sub
Sub UDP_PacketArrived (Packet As UDPPacket)
	Dim msg As String
	msg = BytesToString(Packet.Data, Packet.Offset, Packet.Length, "UTF8")
	Msgbox("Message received: " & msg, "")
End Sub
```

> 事件：
>
> PacketArrived (Packet As UDPPacket)

> 所需权限：
android.permission.INTERNET
## GetBroadcastAddress方法
**GetBroadcastAddress()**

?> 说明：返回网络广播地址。
>
> 返回值：java.lang.String
## Close方法
**Close()**

?> 说明：关闭套接字。
>
> 返回值：void
## toString方法
**toString()**
>
> 返回值：java.lang.String
## IsInitialized方法
**IsInitialized()**

?> 说明：测试此对象是否已初始化。
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName,Port,ReceiveBufferSize)**

?> 说明：初始化套接字并开始侦听数据包。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Port，类型：int
>
> 参数：ReceiveBufferSize，类型：int
>
> 返回值：void
## Send方法
**Send(Packet)**

?> 说明：发送数据包。数据包将在后台（异步）发送。
>
> 参数：Packet，类型：anywheresoftware.b4a.objects.SocketWrapper.UDPSocket.UDPPacket
>
> 返回值：void
## Port属性

?> 说明：获取此套接字侦听的本地端口。
>
> 返回值：int

# UDPPacket
完整类名：anywheresoftware.b4a.objects.SocketWrapper.UDPSocket.UDPPacket
> 所有者：process

> 包装器：anywheresoftware.b4a.objects.SocketWrapper.UDPSocket.MyDatagramPacket

?> 说明：正在发送或接收的数据包。
## Initialize2方法
**Initialize2(Data,Offset,Length,Host,Port)**

?> 说明：类似于初始化。发送的数据基于“偏移”和“长度”值。
>
> 参数：Data，类型：byte[]
>
> 参数：Offset，类型：int
>
> 参数：Length，类型：int
>
> 参数：Host，类型：java.lang.String
>
> 参数：Port，类型：int
>
> 返回值：void
## toString方法
**toString()**
>
> 返回值：java.lang.String
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Data,Host,Port)**

?> 说明：初始化数据包并使其准备好发送。
>
> 参数：Data，类型：byte[]
>
> 参数：Host，类型：java.lang.String
>
> 参数：Port，类型：int
>
> 返回值：void
## Length属性

?> 说明：获取数据中可用字节的长度。这可以比数组长度短。
>
> 返回值：int
## Port属性

?> 说明：获取发送计算机的端口。
>
> 返回值：int
## Data属性

?> 说明：获取接收到的数据数组。
>
> 返回值：byte[]
## Host属性

?> 说明：<b>此方法已被弃用，在Android 4+设备上无法正常工作</b>
>
> 返回值：java.lang.String
## HostAddress属性

?> 说明：获取发送计算机的IP地址。
>
> 返回值：java.lang.String
## Offset属性

?> 说明：获取数据数组中可用数据开始的偏移量。
>
> 返回值：int

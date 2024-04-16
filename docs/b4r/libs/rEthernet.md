# rEthernet

版本:1.11
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rEthernet)

# Ethernet
完整类名：B4R::B4REthernet

> 依赖：<SPI.h> | <Ethernet.h>
## InitializeDHCP方法
**InitializeDHCP(MacAddress)**

?> 说明：初始化以太网连接。
```vbnet

eth.InitializeDHCP(Array As Byte(0xDE, 0xAD, 0xBE, 0xEF, 0xFE, 0xED))
```

>
> 参数：MacAddress，类型：Byte[]
>
> 返回值：bool
## Initialize方法
**Initialize(MacAddress,LocalIp)**

?> 说明：使用静态ip地址初始化屏蔽。
>
> 参数：MacAddress，类型：Byte[]
>
> 参数：LocalIp，类型：Byte[]
>
> 返回值：B4R::void
## MaintainDHCP方法
**MaintainDHCP()**

?> 说明：允许续订DHCP租约。应该近似调用此方法
>
> 返回值：Byte
## LocalIp属性

?> 说明：以字符串形式返回本地ip地址。
>
> 返回值：B4R::B4RString*

# EthernetSocket
完整类名：B4R::EthernetSocket

> 依赖：<SPI.h> | <Ethernet.h>

?> 说明：客户端套接字实现。
## ConnectIP方法
**ConnectIP(IP,Port)**

?> 说明：尝试连接到服务器。如果连接成功，则返回true。
>
> 参数：IP，类型：Byte[]
>
> 参数：Port，类型：UInt
>
> 返回值：bool
## ConnectHost方法
**ConnectHost(Host,Port)**

?> 说明：尝试连接到服务器。如果连接成功，则返回true。
>
> 参数：Host，类型：B4R::B4RString*
>
> 参数：Port，类型：UInt
>
> 返回值：bool
## Close方法
**Close()**

?> 说明：关闭连接。
>
> 返回值：B4R::void
## Stream属性

?> 说明：获取网络流。可以与AsyncStreams一起使用。
>
> 返回值：B4R::B4RStream*
## Connected属性

?> 说明：测试客户端是否已连接。
>
> 返回值：bool

# EthernetServerSocket
完整类名：B4R::EthernetServerSocket

> 依赖：<SPI.h> | <Ethernet.h>

?> 说明：服务器套接字实现。
> 事件：
>
> NewConnection (NewSocket As EthernetSocket)
## Initialize方法
**Initialize(Port,NewConnectionSub)**

?> 说明：初始化服务器。
>
> 参数：Port，类型：UInt
>
> 参数：NewConnectionSub，类型：SubVoidEthernetSocket
>
> 返回值：B4R::void
## Listen方法
**Listen()**

?> 说明：开始侦听连接。
>
> 返回值：B4R::void
## Socket属性

?> 说明：返回最后连接的套接字。
>
> 返回值：B4R::EthernetSocket*

# EthernetUDP
完整类名：B4R::B4REthernetUDP

> 依赖：<SPI.h> | <Ethernet.h>

?> 说明：允许接收和发送UDP数据包。
> 事件：
>
> PacketArrived (Data() As Byte, IP() As Byte, Port As UInt)
## Initialize方法
**Initialize(Port,PacketArrivedSub)**

?> 说明：初始化对象。如果成功，则返回True。
>
> 参数：Port，类型：UInt
>
> 参数：PacketArrivedSub，类型：SubPacketArrived
>
> 返回值：bool
## BeginPacket方法
**BeginPacket(IP,Port)**

?> 说明：开始发送数据包。数据包将在调用SendPacket时发送。
>
> 参数：IP，类型：Byte[]
>
> 参数：Port，类型：UInt
>
> 返回值：bool
## Write方法
**Write(Data)**

?> 说明：将数据写入数据包。返回成功写入的字节数。
>
> 参数：Data，类型：Byte[]
>
> 返回值：Int
## SendPacket方法
**SendPacket()**

?> 说明：发送数据包。
>
> 返回值：bool
## Close方法
**Close()**

?> 说明：关闭套接字。
>
> 返回值：B4R::void

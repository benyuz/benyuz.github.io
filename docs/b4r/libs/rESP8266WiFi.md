# rESP8266WiFi

版本:1.59
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rESP8266WiFi)

# ESP8266WiFi
完整类名：B4R::B4RESPWiFi
> 事件：
>
> Connected (Success As Boolean)
## Scan方法
**Scan()**

?> 说明：扫描无线网络。返回找到的网络数。
>
> 返回值：Byte
## ScannedSSID方法
**ScannedSSID(Index)**

?> 说明：返回网络的SSID。请确保在调用此方法之前先调用Scan。
>
> 参数：Index，类型：Byte
>
> 返回值：B4R::B4RString*
## ScannedBSSID方法
**ScannedBSSID(Index)**

?> 说明：返回网络的BSSID（MAC地址）。请确保在调用此方法之前先调用Scan。
>
> 参数：Index，类型：Byte
>
> 返回值：Byte[]
## ScannedRSSI方法
**ScannedRSSI(Index)**

?> 说明：返回网络的RSSI。请确保在调用此方法之前先调用Scan。
>
> 参数：Index，类型：Byte
>
> 返回值：Long
## Connect方法
**Connect(SSID)**

?> 说明：尝试连接到打开的网络。如果成功，则返回True。
>
> 参数：SSID，类型：B4R::B4RString*
>
> 返回值：bool
## Connect2方法
**Connect2(SSID,Password)**

?> 说明：尝试连接到安全网络。如果成功，则返回True。
>
> 参数：SSID，类型：B4R::B4RString*
>
> 参数：Password，类型：B4R::B4RString*
>
> 返回值：bool
## Connect3方法
**Connect3(SSID,Password,Channel,BSSID)**

?> 说明：尝试连接到网络。如果成功，则返回True。
>
> 参数：SSID，类型：B4R::B4RString*
>
> 参数：Password，类型：B4R::B4RString*
>
> 参数：Channel，类型：Long
>
> 参数：BSSID，类型：Byte[]
>
> 返回值：bool
## ConnectAsync方法
**ConnectAsync(SSID,Password,Channel,BSSID,ConnectedSub)**

?> 说明：尝试连接到网络。引发Connected事件。
>
> 参数：SSID，类型：B4R::B4RString*
>
> 参数：Password，类型：B4R::B4RString*
>
> 参数：Channel，类型：Long
>
> 参数：BSSID，类型：Byte[]
>
> 参数：ConnectedSub，类型：SubVoidBool
>
> 返回值：B4R::void
## StartAccessPoint方法
**StartAccessPoint(SSID)**

?> 说明：启动软接入点。
>
> 参数：SSID，类型：B4R::B4RString*
>
> 返回值：bool
## StartAccessPoint2方法
**StartAccessPoint2(SSID,Password)**

?> 说明：启动软接入点。
>
> 参数：SSID，类型：B4R::B4RString*
>
> 参数：Password，类型：B4R::B4RString*
>
> 返回值：bool
## Disconnect方法
**Disconnect()**
>
> 返回值：B4R::void
## LocalIp属性

?> 说明：以字符串形式返回本地ip地址。
>
> 返回值：B4R::B4RString*
## AccessPointIp属性

?> 说明：当板充当接入点时，返回板ip。
>
> 返回值：B4R::B4RString*
## IsConnected属性

?> 说明：如果已连接WiFi，则返回true。
>
> 返回值：bool

# WiFiSocket
完整类名：B4R::WiFiSocket

?> 说明：客户端套接字实现。用法与EthernetSocket的用法相同。
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
## RemoteIp属性

?> 说明：以字符串形式返回远程客户端ip地址。
>
> 返回值：B4R::B4RString*
## RemotePort属性

?> 说明：返回远程客户端端口。
>
> 返回值：UInt

# WiFiSSLSocket
完整类名：B4R::WiFiSSLSocket

?> 说明：客户端SSL套接字实现。类似于WiFiSocket。只能进行SSL连接。
## ConnectIP方法
**ConnectIP(IP,Port)**

?> 说明：尝试连接到服务器。如果连接成功，则返回true。
>
> 参数：IP，类型：Byte[]
>
> 参数：Port，类型：UInt
>
> 返回值：bool
## VerifyCertificate方法
**VerifyCertificate(FingerPrint,Host)**

?> 说明：什么都不做。
>
> 参数：FingerPrint，类型：B4R::B4RString*
>
> 参数：Host，类型：B4R::B4RString*
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

# WiFiServerSocket
完整类名：B4R::WiFiServerSocket

?> 说明：服务器套接字实现。用法与EthernetServerSocket的用法相同。
> 事件：
>
> NewConnection (NewSocket As WiFiSocket)
## Initialize方法
**Initialize(Port,NewConnectionSub)**

?> 说明：初始化服务器。
>
> 参数：Port，类型：UInt
>
> 参数：NewConnectionSub，类型：SubVoidWiFiSocket
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
> 返回值：B4R::WiFiSocket*

# WiFiUDP
完整类名：B4R::B4RWiFiUDP

?> 说明：允许接收和发送UDP数据包。用法与EthernetUDP的用法相同。
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

# rWebSocketClient

版本:1.2
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rWebSocketClient)

# WebSocketClient
完整类名：B4R::B4RWebSocketClient

?> 说明：WebSocket客户端实现。它旨在与B4J WebSocket服务器一起工作。
> 事件：
>
> Disconnected
>
> NewMessage (FunctionName As String, Params() As String)
## Initialize方法
**Initialize(NewMessageSub,DisconnectedSub)**

?> 说明：初始化对象并设置NewMessage和Disconnected子节点。
>
> 参数：NewMessageSub，类型：SubVoidStringArray
>
> 参数：DisconnectedSub，类型：SubVoidVoid
>
> 返回值：B4R::void
## ConnectHost方法
**ConnectHost(Stream,Host,Port,Path)**

?> 说明：尝试连接到服务器。如果连接成功，则返回true。
>
> 参数：Stream，类型：B4R::B4RStream*
>
> 参数：Host，类型：B4R::B4RString*
>
> 参数：Port，类型：UInt
>
> 参数：Path，类型：B4R::B4RString*
>
> 返回值：bool
## ConnectIP方法
**ConnectIP(Stream,IP,Port,Path)**

?> 说明：尝试连接到服务器。如果连接成功，则返回true。
>
> 参数：Stream，类型：B4R::B4RStream*
>
> 参数：IP，类型：Byte[]
>
> 参数：Port，类型：UInt
>
> 参数：Path，类型：B4R::B4RString*
>
> 返回值：bool
## SendEventToServer方法
**SendEventToServer(Event,DataMap)**

?> 说明：在服务器上引发事件。
>
> 参数：Event，类型：B4R::B4RString*
>
> 参数：DataMap，类型：String[]
>
> 返回值：B4R::void

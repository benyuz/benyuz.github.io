# rSoftwareSerial

版本:1
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rSoftwareSerial)

# SoftwareSerial
完整类名：B4R::B4RSoftwareSerial
## Initialize方法
**Initialize(BaudRate,ReceivePin,TransmitPin)**

?> 说明：初始化对象。
>
> 参数：BaudRate，类型：ULong
>
> 参数：ReceivePin，类型：Byte
>
> 参数：TransmitPin，类型：Byte
>
> 返回值：B4R::void
## Close方法
**Close()**

?> 说明：关闭串行端口。
>
> 返回值：B4R::void
## Stream属性

?> 说明：返回内部流。这可以与AsyncStreams一起用于从串行中读取或写入。
>
> 返回值：B4R::B4RStream*
## Listening属性

?> 说明：获取或设置此对象当前是否为“正在侦听”的序列号。
>
> 参数：b，类型：bool
>
> 返回值：bool

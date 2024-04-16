# rWire

版本:1.1
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rWire)

# WireMaster
完整类名：B4R::WireMaster
## Initialize方法
**Initialize()**

?> 说明：初始化WireMaster对象。
>
> 返回值：B4R::void
## RequestFrom方法
**RequestFrom(Address,Length)**

?> 说明：从从属服务器请求数据，并将其作为字节数组返回。
>
> 参数：Address，类型：Byte
>
> 参数：Length，类型：Byte
>
> 返回值：Byte[]
## WriteTo方法
**WriteTo(Address,Data)**

?> 说明：将给定的数组发送到从属数组。
>
> 参数：Address，类型：Byte
>
> 参数：Data，类型：Byte[]
>
> 返回值：Byte
## WriteTo2方法
**WriteTo2(Address,SendStop,Data)**

?> 说明：类似于WriteTo。
>
> 参数：Address，类型：Byte
>
> 参数：SendStop，类型：bool
>
> 参数：Data，类型：Byte[]
>
> 返回值：Byte

# WireSlave
完整类名：B4R::WireSlave
> 事件：
>
> NewData (Data() As Byte)
## Initialize方法
**Initialize(Address,NewDataSub)**

?> 说明：初始化WireSlave对象。
>
> 参数：Address，类型：Byte
>
> 参数：NewDataSub，类型：SubVoidArray
>
> 返回值：B4R::void
## SetDataForMaster方法
**SetDataForMaster(Data)**

?> 说明：设置当主机调用RequestFrom时将发送到主机的数据。
>
> 参数：Data，类型：Byte[]
>
> 返回值：B4R::void

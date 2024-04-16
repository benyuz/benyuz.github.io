# rEEPROM

版本:1.2
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rEEPROM)

# EEPROM
完整类名：B4R::B4REEPROM
## WriteBytes方法
**WriteBytes(Src,Position)**

?> 说明：将字节数组写入EEPROM。
>
> 参数：Src，类型：Byte[]
>
> 参数：Position，类型：UInt
>
> 返回值：B4R::void
## ReadBytes方法
**ReadBytes(Position,Count)**

?> 说明：从EEPROM读取数据，并将其作为新阵列返回。
>
> 参数：Position，类型：UInt
>
> 参数：Count，类型：UInt
>
> 返回值：Byte[]
## ReadBytes2方法
**ReadBytes2(Position,Count,Dest)**

?> 说明：类似于ReadBytes。数据被复制到传递的数组中。
>
> 参数：Position，类型：UInt
>
> 参数：Count，类型：UInt
>
> 参数：Dest，类型：Byte[]
>
> 返回值：B4R::void
## Size属性

?> 说明：返回EEPROM的大小。
>
> 返回值：UInt

# ByteConverter

版本:1.1
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=ByteConverter)

# ByteConverter
完整类名：anywheresoftware.b4a.agraham.byteconverter.ByteConverter
> 所有者：process

?> 说明：此ByteConverter对象可以将基元类型的数组转换为数组或从数组转换为基元类型
## CharsFromBytes方法
**CharsFromBytes(bytes)**

?> 说明：获取一个Bytes数组，并返回从该数组转换而来的Chars数组。
>
> 参数：bytes，类型：byte[]
>
> 返回值：char[]
## ShortsToBytes方法
**ShortsToBytes(vals)**

?> 说明：获取一个Shorts数组，并返回从该数组转换而来的Bytes数组。
>
> 参数：vals，类型：short[]
>
> 返回值：byte[]
## IntsToBytes方法
**IntsToBytes(vals)**

?> 说明：获取Ints数组，并返回从该数组转换的Bytes数组。
>
> 参数：vals，类型：int[]
>
> 返回值：byte[]
## DoublesFromBytes方法
**DoublesFromBytes(bytes)**

?> 说明：获取一个Bytes数组，并返回从该数组转换而来的Doubles数组。
>
> 参数：bytes，类型：byte[]
>
> 返回值：double[]
## StringToBytes方法
**StringToBytes(str,encoding)**

?> 说明：返回一个字节数组，其中包含根据编码转换为字节的str中的字符。
>
> 参数：str，类型：java.lang.String
>
> 参数：encoding，类型：java.lang.String
>
> 返回值：byte[]
## HexToBytes方法
**HexToBytes(hex)**

?> 说明：返回一个包含由十六进制字符串表示的数据的字节数组。字符串可以是大写或小写。
>
> 参数：hex，类型：java.lang.String
>
> 返回值：byte[]
## FloatsToBytes方法
**FloatsToBytes(vals)**

?> 说明：获取一个浮点数组，并返回从该数组转换而来的字节数组。
>
> 参数：vals，类型：float[]
>
> 返回值：byte[]
## FromChars方法
**FromChars(chars)**

?> 说明：返回从指定的字符数组转换而来的字符串。
>
> 参数：chars，类型：char[]
>
> 返回值：java.lang.String
## StringFromBytes方法
**StringFromBytes(bytes,encoding)**

?> 说明：返回一个字符串，该字符串包含数组中根据编码解释为字符的字节。
>
> 参数：bytes，类型：byte[]
>
> 参数：encoding，类型：java.lang.String
>
> 返回值：java.lang.String
## ArrayCopy方法
**ArrayCopy(src,srcOffset,dest,destOffset,count)**

?> 说明：将计数元素从src数组中的srcoffset复制到dest数组中的destoffset。
>
> 参数：src，类型：java.lang.Object
>
> 参数：srcOffset，类型：int
>
> 参数：dest，类型：java.lang.Object
>
> 参数：destOffset，类型：int
>
> 参数：count，类型：int
>
> 返回值：void
## ToChars方法
**ToChars(str)**

?> 说明：返回由指定字符串的字符组成的字符数组
>
> 参数：str，类型：java.lang.String
>
> 返回值：char[]
## DoublesToBytes方法
**DoublesToBytes(vals)**

?> 说明：获取一个Doubles数组，并返回从该数组转换而来的Bytes数组。
>
> 参数：vals，类型：double[]
>
> 返回值：byte[]
## SupportedEncodings方法
**SupportedEncodings()**

?> 说明：返回一个字符串数组，该数组包含此系统支持的编码的所有值。
>
> 返回值：java.lang.String[]
## ShortsFromBytes方法
**ShortsFromBytes(bytes)**

?> 说明：获取一个Bytes数组，并返回从该数组转换而来的Shorts数组。
>
> 参数：bytes，类型：byte[]
>
> 返回值：short[]
## IntsFromBytes方法
**IntsFromBytes(bytes)**

?> 说明：获取一个Bytes数组，并返回从该数组转换而来的Ints数组。
>
> 参数：bytes，类型：byte[]
>
> 返回值：int[]
## CharsToBytes方法
**CharsToBytes(vals)**

?> 说明：获取一个Chars数组，并返回从该数组转换而来的Bytes数组。
>
> 参数：vals，类型：char[]
>
> 返回值：byte[]
## FloatsFromBytes方法
**FloatsFromBytes(bytes)**

?> 说明：获取一个字节数组，并返回从该数组转换而来的浮点数组。
>
> 参数：bytes，类型：byte[]
>
> 返回值：float[]
## LongsToBytes方法
**LongsToBytes(vals)**

?> 说明：获取一个Longs数组，并返回从该数组转换而来的Bytes数组。
>
> 参数：vals，类型：long[]
>
> 返回值：byte[]
## LongsFromBytes方法
**LongsFromBytes(bytes)**

?> 说明：获取一个Bytes数组，并返回从该数组转换而来的Longs数组。
>
> 参数：bytes，类型：byte[]
>
> 返回值：long[]
## HexFromBytes方法
**HexFromBytes(bytes)**

?> 说明：返回一个字符串，该字符串包含字节数组中字节的十六进制表示形式。
>
> 参数：bytes，类型：byte[]
>
> 返回值：java.lang.String
## Version属性

?> 说明：返回此库的版本号。
>
> 返回值：double
## LittleEndian属性

?> 说明：获取或设置与其他基元值之间的字节转换的端序。
>
> 参数：littleEndian，类型：boolean
>
> 返回值：boolean

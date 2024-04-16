# rRandomAccessFile

版本:1.91
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rRandomAccessFile)

# ByteConverter
完整类名：B4R::ByteConverter

?> 说明：提供允许在不同类型的数组之间转换为字节数组的方法。
## Split方法
**Split(Src,Separator)**

?> 说明：根据Separator数组拆分字节数组并返回迭代器。
```vbnet

Dim bc As ByteConverter
For Each s() As Byte In bc.Split("abc,def,ghf", ",")
	Log(s)
Next
```

>
> 参数：Src，类型：Byte[]
>
> 参数：Separator，类型：Byte[]
>
> 返回值：B4R::SplitIterator*
## SubString方法
**SubString(Src,BeginIndex)**

?> 说明：创建一个与给定数组共享相同内存的新数组。
```vbnet

Dim bc As ByteConverter
Log(bc.SubString("012345", 2)) '2345
```

>
> 参数：Src，类型：Byte[]
>
> 参数：BeginIndex，类型：UInt
>
> 返回值：Byte[]
## SubString2方法
**SubString2(Src,BeginIndex,EndIndex)**

?> 说明：创建一个与给定数组共享相同内存的新数组。
```vbnet

Dim bc As ByteConverter
Log(bc.SubString2("012345", 2, 4)) '23
```

>
> 参数：Src，类型：Byte[]
>
> 参数：BeginIndex，类型：UInt
>
> 参数：EndIndex，类型：UInt
>
> 返回值：Byte[]
## IndexOf方法
**IndexOf(Src,SearchFor)**

?> 说明：返回Src数组中第一次出现SearchFor数组的索引。
>
> 参数：Src，类型：Byte[]
>
> 参数：SearchFor，类型：Byte[]
>
> 返回值：Int
## IndexOf2方法
**IndexOf2(Src,SearchFor,StartIndex)**

?> 说明：返回Src数组中第一次出现SearchFor数组的索引。
>
> 参数：Src，类型：Byte[]
>
> 参数：SearchFor，类型：Byte[]
>
> 参数：StartIndex，类型：UInt
>
> 返回值：Int
## LastIndexOf方法
**LastIndexOf(Src,SearchFor)**

?> 说明：返回Src数组中第一次出现SearchFor数组的索引。
>
> 参数：Src，类型：Byte[]
>
> 参数：SearchFor，类型：Byte[]
>
> 返回值：Int
## LastIndexOf2方法
**LastIndexOf2(Src,SearchFor,StartIndex)**

?> 说明：返回Src数组中第一次出现SearchFor数组的索引。
>
> 参数：Src，类型：Byte[]
>
> 参数：SearchFor，类型：Byte[]
>
> 参数：StartIndex，类型：UInt
>
> 返回值：Int
## Trim方法
**Trim(Src)**

?> 说明：创建一个新数组，该数组与给定数组共享相同的内存，不包含前导和尾部空白字符。
>
> 参数：Src，类型：Byte[]
>
> 返回值：Byte[]
## StartsWith方法
**StartsWith(Src,Prefix)**

?> 说明：如果Src数组以Prefix数组开头，则返回true。
>
> 参数：Src，类型：Byte[]
>
> 参数：Prefix，类型：Byte[]
>
> 返回值：bool
## EndsWith方法
**EndsWith(Src,Suffix)**

?> 说明：如果Src数组以Suffix数组结束，则返回true。
>
> 参数：Src，类型：Byte[]
>
> 参数：Suffix，类型：Byte[]
>
> 返回值：bool
## ArrayCompare方法
**ArrayCompare(Arr1,Arr2)**

?> 说明：比较这两个数组。
>
> 参数：Arr1，类型：Byte[]
>
> 参数：Arr2，类型：Byte[]
>
> 返回值：Int
## HexFromBytes方法
**HexFromBytes(Bytes)**

?> 说明：将字节数组转换为十六进制字符串。
>
> 参数：Bytes，类型：Byte[]
>
> 返回值：B4R::B4RString*
## HexToBytes方法
**HexToBytes(Hex)**

?> 说明：将十六进制字符串转换为字节数组。
>
> 参数：Hex，类型：B4R::B4RString*
>
> 返回值：Byte[]
## ObjectToBytes方法
**ObjectToBytes(Object,ObjectSize)**

?> 说明：将对象（非基元）转换为字节数组。请注意，数组和对象共享相同的内存。
>
> 参数：Object，类型：B4R::Object*
>
> 参数：ObjectSize，类型：UInt
>
> 返回值：Byte[]
## ObjectFromBytes方法
**ObjectFromBytes(Bytes)**

?> 说明：将字节数组转换为对象。请注意，数组和对象共享相同的内存。
>
> 参数：Bytes，类型：Byte[]
>
> 返回值：B4R::Object*
## ObjectCopy方法
**ObjectCopy(Src,Dest,ObjectSize)**

?> 说明：将源对象复制到目标对象。此方法对源对象的内存进行浅层复制。
```vbnet

bc.ObjectCopy(LocalType, GlobalType, SizeOf(LocalType))
```

>
> 参数：Src，类型：B4R::Object*
>
> 参数：Dest，类型：B4R::Object*
>
> 参数：ObjectSize，类型：UInt
>
> 返回值：B4R::void
## ObjectSet方法
**ObjectSet(Src,Dest)**

?> 说明：设置现有对象实例的值。此方法可用于设置
>
> 参数：Src，类型：B4R::Object*
>
> 参数：Dest，类型：B4R::Object*
>
> 返回值：B4R::void
## ArrayCopy方法
**ArrayCopy(Src,Dest)**

?> 说明：将Src阵列复制到Dest阵列。将设置目标数组长度
>
> 参数：Src，类型：Byte[]
>
> 参数：Dest，类型：Byte[]
>
> 返回值：B4R::void
## ArrayCopy2方法
**ArrayCopy2(Src,SrcOffset,Dest,DestOffset,Count)**

?> 说明：将字节从源阵列复制到目标阵列。
>
> 参数：Src，类型：Byte[]
>
> 参数：SrcOffset，类型：UInt
>
> 参数：Dest，类型：Byte[]
>
> 参数：DestOffset，类型：UInt
>
> 参数：Count，类型：UInt
>
> 返回值：B4R::void
## StringToBytes方法
**StringToBytes(Str)**

?> 说明：将字符串转换为字节数组。这与调用Str.GetBytes相同。
>
> 参数：Str，类型：B4R::B4RString*
>
> 返回值：Byte[]
## StringFromBytes方法
**StringFromBytes(Src)**

?> 说明：基于字节数组创建新字符串。
>
> 参数：Src，类型：Byte[]
>
> 返回值：B4R::B4RString*
## ByteConverter_IntsFromBytes方法
**ByteConverter_IntsFromBytes(Bytes)**

?> 说明：将字节数组转换为16位int的数组。请注意，两个阵列共享相同的内存。
>
> 参数：Bytes，类型：Byte[]
>
> 返回值：Int[]
## ByteConverter_IntsToBytes方法
**ByteConverter_IntsToBytes(Ints)**

?> 说明：将16位int数组转换为字节数组。请注意，两个阵列共享相同的内存。
>
> 参数：Ints，类型：Int[]
>
> 返回值：Byte[]
## ByteConverter_UIntsFromBytes方法
**ByteConverter_UIntsFromBytes(Bytes)**

?> 说明：将字节数组转换为16位无符号整数的数组。请注意，两个阵列共享相同的内存。
>
> 参数：Bytes，类型：Byte[]
>
> 返回值：UInt[]
## ByteConverter_UIntsToBytes方法
**ByteConverter_UIntsToBytes(UInts)**

?> 说明：将16位无符号int数组转换为字节数组。请注意，两个阵列共享相同的内存。
>
> 参数：UInts，类型：UInt[]
>
> 返回值：Byte[]
## ByteConverter_ULongsFromBytes方法
**ByteConverter_ULongsFromBytes(Bytes)**

?> 说明：将字节数组转换为32位无符号长字符的数组。请注意，两个阵列共享相同的内存。
>
> 参数：Bytes，类型：Byte[]
>
> 返回值：ULong[]
## ByteConverter_ULongsToBytes方法
**ByteConverter_ULongsToBytes(ArrayULong)**

?> 说明：将32位无符号长数组转换为字节数组。请注意，两个阵列共享相同的内存。
>
> 参数：ArrayULong，类型：ULong[]
>
> 返回值：Byte[]
## ByteConverter_LongsFromBytes方法
**ByteConverter_LongsFromBytes(Bytes)**

?> 说明：将字节数组转换为32位带符号长的数组。请注意，两个阵列共享相同的内存。
>
> 参数：Bytes，类型：Byte[]
>
> 返回值：Long[]
## ByteConverter_LongsToBytes方法
**ByteConverter_LongsToBytes(UInts)**

?> 说明：将32位带符号的长数组转换为字节数组。请注意，两个阵列共享相同的内存。
>
> 参数：UInts，类型：Long[]
>
> 返回值：Byte[]
## ByteConverter_DoublesFromBytes方法
**ByteConverter_DoublesFromBytes(Bytes)**

?> 说明：将字节数组转换为32位浮点数组。请注意，两个阵列共享相同的内存。
>
> 参数：Bytes，类型：Byte[]
>
> 返回值：Double[]
## ByteConverter_DoublesToBytes方法
**ByteConverter_DoublesToBytes(UInts)**

?> 说明：将32位浮点数组转换为字节数组。请注意，两个阵列共享相同的内存。
>
> 参数：UInts，类型：Double[]
>
> 返回值：Byte[]

# AsyncStreams
完整类名：B4R::AsyncStreams
> 事件：
>
> NewData (Buffer() As Byte)
>
> Error
## Initialize方法
**Initialize(Stream,NewDataSub,ErrorSub)**

?> 说明：初始化对象并设置将处理事件的子对象。
>
> 参数：Stream，类型：B4R::B4RStream*
>
> 参数：NewDataSub，类型：SubVoidArray
>
> 参数：ErrorSub，类型：SubVoidVoid
>
> 返回值：B4R::void
## InitializePrefix方法
**InitializePrefix(Stream,BigEndian,NewDataSub,ErrorSub)**

?> 说明：以前缀模式初始化对象。连接的两侧都必须遵守“前缀”协议。
>
> 参数：Stream，类型：B4R::B4RStream*
>
> 参数：BigEndian，类型：bool
>
> 参数：NewDataSub，类型：SubVoidArray
>
> 参数：ErrorSub，类型：SubVoidVoid
>
> 返回值：B4R::void
## Write方法
**Write(Data)**

?> 说明：将数组写入流。
>
> 参数：Data，类型：Byte[]
>
> 返回值：B4R::AsyncStreams*
## Write2方法
**Write2(Data,Start,Length)**

?> 说明：将数组写入流。
>
> 参数：Data，类型：Byte[]
>
> 参数：Start，类型：UInt
>
> 参数：Length，类型：UInt
>
> 返回值：B4R::AsyncStreams*
## MaxBufferSize字段

?> 说明：内部缓冲区限制。当缓冲区达到此大小或没有更多数据可用时，将引发NewData事件。
>
> 返回值：UInt
## WaitForMoreDataDelay字段

?> 说明：等待新数据的毫秒数（当至少有一个字节可用时）。
>
> 返回值：UInt

# RandomAccessFile
完整类名：B4R::RandomAccessFile
## Initialize方法
**Initialize(Buffer,LittleEndian)**

?> 说明：使用后端数组初始化对象。
>
> 参数：Buffer，类型：Byte[]
>
> 参数：LittleEndian，类型：bool
>
> 返回值：B4R::void
## WriteByte方法
**WriteByte(Value,Position)**

?> 说明：写入单个字节。
>
> 参数：Value，类型：Byte
>
> 参数：Position，类型：UInt
>
> 返回值：B4R::void
## ReadByte方法
**ReadByte(Position)**

?> 说明：读取单个字节。
>
> 参数：Position，类型：UInt
>
> 返回值：Byte
## WriteInt16方法
**WriteInt16(Value,Position)**

?> 说明：写入一个2字节的Int（相当于B4X Short）。
>
> 参数：Value，类型：Int
>
> 参数：Position，类型：UInt
>
> 返回值：B4R::void
## ReadInt16方法
**ReadInt16(Position)**

?> 说明：读取一个2字节的Int（相当于B4X Short）。
>
> 参数：Position，类型：UInt
>
> 返回值：Int
## WriteUInt16方法
**WriteUInt16(Value,Position)**

?> 说明：写一个2字节的无符号Int。
>
> 参数：Value，类型：UInt
>
> 参数：Position，类型：UInt
>
> 返回值：B4R::void
## ReadUInt16方法
**ReadUInt16(Position)**

?> 说明：读取一个2字节的无符号Int。
>
> 参数：Position，类型：UInt
>
> 返回值：UInt
## WriteLong32方法
**WriteLong32(Value,Position)**

?> 说明：写入一个4字节长（相当于B4X Int）。
>
> 参数：Value，类型：Long
>
> 参数：Position，类型：UInt
>
> 返回值：B4R::void
## ReadLong32方法
**ReadLong32(Position)**

?> 说明：读取4字节长（相当于B4X Int）。
>
> 参数：Position，类型：UInt
>
> 返回值：Long
## WriteULong32方法
**WriteULong32(Value,Position)**

?> 说明：写入一个4字节的无符号长。
>
> 参数：Value，类型：ULong
>
> 参数：Position，类型：UInt
>
> 返回值：B4R::void
## ReadULong32方法
**ReadULong32(Position)**

?> 说明：读取一个4字节的无符号长。
>
> 参数：Position，类型：UInt
>
> 返回值：ULong
## WriteDouble32方法
**WriteDouble32(Value,Position)**

?> 说明：写入一个4字节的双精度（相当于B4X浮点）。
>
> 参数：Value，类型：Double
>
> 参数：Position，类型：UInt
>
> 返回值：B4R::void
## ReadDouble32方法
**ReadDouble32(Position)**

?> 说明：读取一个4字节的双精度（相当于B4X浮点）。
>
> 参数：Position，类型：UInt
>
> 返回值：Double
## ReadBytes方法
**ReadBytes(Dest,StartOffset,Length,Position)**

?> 说明：将字节从后端阵列复制到Dest阵列。不检查边界。
>
> 参数：Dest，类型：Byte[]
>
> 参数：StartOffset，类型：int
>
> 参数：Length，类型：int
>
> 参数：Position，类型：UInt
>
> 返回值：B4R::void
## ReadBytes2方法
**ReadBytes2(Length,Position)**

?> 说明：与ReadBytes类似，但数据不会被复制。
>
> 参数：Length，类型：int
>
> 参数：Position，类型：UInt
>
> 返回值：Byte[]
## WriteBytes方法
**WriteBytes(Src,StartOffset,Length,Position)**

?> 说明：将字节复制到后端阵列。不检查边界。
>
> 参数：Src，类型：Byte[]
>
> 参数：StartOffset，类型：int
>
> 参数：Length，类型：int
>
> 参数：Position，类型：UInt
>
> 返回值：B4R::void
## CurrentPosition字段

?> 说明：获取或设置当前位置。
>
> 返回值：UInt

# B4RSerializator
完整类名：B4R::B4RSerializator

?> 说明：将对象数组转换为字节，反之亦然。
## ConvertArrayToBytes方法
**ConvertArrayToBytes(Objects)**

?> 说明：将对象数组转换为字节数组。
>
> 参数：Objects，类型：Object[]
>
> 返回值：Byte[]
## ConvertArrayToBytes2方法
**ConvertArrayToBytes2(Objects,Buffer)**

?> 说明：类似于ConvertArrayToBytes。返回的数组将与Buffer数组共享内存，而不是使用堆栈缓冲区。
>
> 参数：Objects，类型：Object[]
>
> 参数：Buffer，类型：Byte[]
>
> 返回值：Byte[]
## ConvertBytesToArray方法
**ConvertBytesToArray(Bytes,ObjectsBuffer)**

?> 说明：将以前序列化的字节数组转换为对象数组。
>
> 参数：Bytes，类型：Byte[]
>
> 参数：ObjectsBuffer，类型：Object[]
>
> 返回值：Object[]

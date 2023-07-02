# RandomAccessFile

版本:2.33
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=RandomAccessFile)

# RandomAccessFile
完整类名：anywheresoftware.b4a.randomaccessfile.RandomAccessFile
> 所有者：process

?> 说明：此对象允许您按非顺序访问文件和字节数组。
## WriteLong方法
**WriteLong(Value,Position)**

?> 说明：将长值写入指定位置。
>
> 参数：Value，类型：long
>
> 参数：Position，类型：long
>
> 返回值：void
## ReadShort方法
**ReadShort(Position)**

?> 说明：读取存储在指定位置的短值。
>
> 参数：Position，类型：long
>
> 返回值：short
## ReadInt方法
**ReadInt(Position)**

?> 说明：读取存储在指定位置的Int值。
>
> 参数：Position，类型：long
>
> 返回值：int
## ReadDouble方法
**ReadDouble(Position)**

?> 说明：读取存储在指定位置的Double值。
>
> 参数：Position，类型：long
>
> 返回值：double
## WriteShort方法
**WriteShort(Value,Position)**

?> 说明：将Short值写入指定位置。
>
> 参数：Value，类型：short
>
> 参数：Position，类型：long
>
> 返回值：void
## WriteDouble方法
**WriteDouble(Value,Position)**

?> 说明：将Double值写入指定位置。
>
> 参数：Value，类型：double
>
> 参数：Position，类型：long
>
> 返回值：void
## Initialize方法
**Initialize(Dir,File,ReadOnly)**

?> 说明：打开指定的文件。
```vbnet

Dim raf As RandomAccessFile
raf.Initialize(File.DirInternal, "1.dat", false)
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：File，类型：java.lang.String
>
> 参数：ReadOnly，类型：boolean
>
> 返回值：void
## ReadEncryptedObject方法
**ReadEncryptedObject(Password,Position)**

?> 说明：从流中读取加密的对象。
>
> 参数：Password，类型：java.lang.String
>
> 参数：Position，类型：long
>
> 返回值：java.lang.Object
## ReadSignedByte方法
**ReadSignedByte(Position)**

?> 说明：读取存储在指定位置的带符号字节（-128-127）。
>
> 参数：Position，类型：long
>
> 返回值：byte
## WriteFloat方法
**WriteFloat(Value,Position)**

?> 说明：将浮点值写入指定位置。
>
> 参数：Value，类型：float
>
> 参数：Position，类型：long
>
> 返回值：void
## ReadB4XObject方法
**ReadB4XObject(Position)**

?> 说明：读取以前使用WriteB4XObject写入的对象。
>
> 参数：Position，类型：long
>
> 返回值：java.lang.Object
## WriteObject方法
**WriteObject(Object,Compress,Position)**

?> 说明：将给定的对象写入流。
>
> 参数：Object，类型：java.lang.Object
>
> 参数：Compress，类型：boolean
>
> 参数：Position，类型：long
>
> 返回值：void
## ReadUnsignedByte方法
**ReadUnsignedByte(Position)**

?> 说明：读取存储在指定位置的无符号字节（0-255）。
>
> 参数：Position，类型：long
>
> 返回值：int
## Flush方法
**Flush()**

?> 说明：刷新所有缓存的数据。
>
> 返回值：void
## ReadBytes方法
**ReadBytes(Buffer,StartOffset,Length,Position)**

?> 说明：从流中读取字节，并将其读入给定的数组。
>
> 参数：Buffer，类型：byte[]
>
> 参数：StartOffset，类型：int
>
> 参数：Length，类型：int
>
> 参数：Position，类型：long
>
> 返回值：int
## WriteByte方法
**WriteByte(Byte,Position)**

?> 说明：将字节值写入指定位置。
>
> 参数：Byte，类型：byte
>
> 参数：Position，类型：long
>
> 返回值：void
## ReadLong方法
**ReadLong(Position)**

?> 说明：读取存储在指定位置的长值。
>
> 参数：Position，类型：long
>
> 返回值：long
## Initialize3方法
**Initialize3(Buffer,LittleEndian)**

?> 说明：将给定的缓冲区视为大小不变的随机访问文件。
>
> 参数：Buffer，类型：byte[]
>
> 参数：LittleEndian，类型：boolean
>
> 返回值：void
## Initialize2方法
**Initialize2(Dir,File,ReadOnly,LittleEndian)**

?> 说明：与Initialize相同，具有将字节顺序设置为little-endian而不是
>
> 参数：Dir，类型：java.lang.String
>
> 参数：File，类型：java.lang.String
>
> 参数：ReadOnly，类型：boolean
>
> 参数：LittleEndian，类型：boolean
>
> 返回值：void
## ReadFloat方法
**ReadFloat(Position)**

?> 说明：读取存储在指定位置的浮点值。
>
> 参数：Position，类型：long
>
> 返回值：float
## ReadObject方法
**ReadObject(Position)**

?> 说明：从流中读取对象。
>
> 参数：Position，类型：long
>
> 返回值：java.lang.Object
## Close方法
**Close()**

?> 说明：关闭流。
>
> 返回值：void
## WriteInt方法
**WriteInt(Value,Position)**

?> 说明：将Int值写入指定位置。
>
> 参数：Value，类型：int
>
> 参数：Position，类型：long
>
> 返回值：void
## WriteBytes方法
**WriteBytes(Buffer,StartOffset,Length,Position)**

?> 说明：将给定的缓冲区写入流。写入的第一个字节是Buffer（StartOffset）
>
> 参数：Buffer，类型：byte[]
>
> 参数：StartOffset，类型：int
>
> 参数：Length，类型：int
>
> 参数：Position，类型：long
>
> 返回值：int
## WriteB4XObject方法
**WriteB4XObject(Object,Position)**

?> 说明：类似于WriteObject。此方法以B4i、B4A和B4J支持的格式写入对象。
>
> 参数：Object，类型：java.lang.Object
>
> 参数：Position，类型：long
>
> 返回值：void
## WriteEncryptedObject方法
**WriteEncryptedObject(Object,Password,Position)**

?> 说明：类似于WriteObject。该对象使用AES-256进行加密，然后写入流中。
>
> 参数：Object，类型：java.lang.Object
>
> 参数：Password，类型：java.lang.String
>
> 参数：Position，类型：long
>
> 返回值：void
## Size属性

?> 说明：返回文件大小。
>
> 返回值：long
## CurrentPosition字段

?> 说明：保持当前文件位置。
>
> 返回值：long

# CountingInputStream
完整类名：anywheresoftware.b4a.randomaccessfile.CountingStreams.CountingInput
> 所有者：process

> 包装器：java.io.InputStream

?> 说明：CountingInputStream和CountingOutputStream允许您监控读取或写入进度。
```vbnet

Sub Process_Globals
	Dim hc As HttpClient
	Dim cout As CountingOutputStream
	Dim length As Int
	Dim timer1 As Timer
End Sub
Sub Globals

End Sub
Sub Activity_Create(FirstTime As Boolean)
	If FirstTime Then
		hc.Initialize("hc")
		timer1.Initialize("Timer1", 500)
	End If
	Dim req As HttpRequest
	req.InitializeGet("http://www.basic4ppc.com/android/files/b4a-trial.zip")
	hc.Execute(req, 1)
End Sub

Sub hc_ResponseSuccess (Response As HttpResponse, TaskId As Int)
	cout.Initialize(File.OpenOutput(File.DirRootExternal, "1.zip", False))
	Timer1.Enabled = True
	length = Response.ContentLength
	Response.GetAsynchronously("response", cOut, True, TaskId)
End Sub

Sub hc_ResponseError (Response As HttpResponse, Reason As String, StatusCode As Int, TaskId As Int)
	Log("Error: " & Reason)
	If Response <> Null Then
		Log(Response.GetString("UTF8"))
		Response.Release
	End If
End Sub

Sub Response_StreamFinish (Success As Boolean, TaskId As Int)
	timer1.Enabled = False
	If Success Then
		Timer1_Tick 'Show the current counter status
		Log("Success!")
	Else
		Log("Error: " & LastException.Message)
	End If
End Sub

Sub Timer1_Tick
	Log(cout.Count & " out of " & length)
End Sub
```

## BytesAvailable方法
**BytesAvailable()**
>
> 返回值：int
## Close方法
**Close()**
>
> 返回值：void
## ReadBytes方法
**ReadBytes(arg0,arg1,arg2)**
>
> 参数：arg0，类型：byte[]
>
> 参数：arg1，类型：int
>
> 参数：arg2，类型：int
>
> 返回值：int
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(InputStream)**

?> 说明：通过包装给定的输入流来初始化计数流。
>
> 参数：InputStream，类型：java.io.InputStream
>
> 返回值：void
## Count属性

?> 说明：获取或设置读取的字节数。
>
> 参数：v，类型：long
>
> 返回值：long

# CountingOutputStream
完整类名：anywheresoftware.b4a.randomaccessfile.CountingStreams.CountingOutput
> 所有者：process

> 包装器：java.io.OutputStream

?> 说明：有关详细信息，请参阅CountingInputStream。
## Flush方法
**Flush()**
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(OutputStream)**

?> 说明：通过包装给定的输出流来初始化计数流。
>
> 参数：OutputStream，类型：java.io.OutputStream
>
> 返回值：void
## ToBytesArray方法
**ToBytesArray()**
>
> 返回值：byte[]
## Close方法
**Close()**
>
> 返回值：void
## WriteBytes方法
**WriteBytes(arg0,arg1,arg2)**
>
> 参数：arg0，类型：byte[]
>
> 参数：arg1，类型：int
>
> 参数：arg2，类型：int
>
> 返回值：void
## Count属性

?> 说明：获取或设置写入的字节数。
>
> 参数：v，类型：long
>
> 返回值：long

# CompressedStreams
完整类名：anywheresoftware.b4a.randomaccessfile.CompressedStreams
> 所有者：process

?> 说明：CompressedStreams对象允许您使用gzip或zlib压缩方法压缩和解压缩数据。
```vbnet

Sub Globals

End Sub

Sub Activity_Create(FirstTime As Boolean)
	Dim sb As StringBuilder
	sb.Initialize
	'Concatenation operations are much faster with StringBuilder than with String.
	For i = 1 To 10000
		sb.Append("Playing with compressed streams.").Append(CRLF)
	Next
	Dim out As OutputStream
	Dim s As String
	Dim compress As CompressedStreams
	s = sb.ToString
	'Write the string without compressing it (we could have used File.WriteString instead).
	out = File.OpenOutput(File.DirRootExternal, "test.txt", False)
	WriteStringToStream(out, s)
	
	'Write the string with gzip compression.
	out = File.OpenOutput(File.DirRootExternal, "test.gz", False)
	out = compress.WrapOutputStream(out, "gzip")
	WriteStringToStream(out, s)
	
	'Write the string with zlib compression
	out = File.OpenOutput(File.DirRootExternal, "test.zlib", False)
	out = compress.WrapOutputStream(out, "zlib")
	WriteStringToStream(out, s)
	
	'Show the files sizes
	Msgbox("No compression: " & File.Size(File.DirRootExternal, "test.txt") & CRLF _
		& "Gzip: " & File.Size(File.DirRootExternal, "test.gz") & CRLF _
		& "zlib: " & File.Size(File.DirRootExternal, "test.zlib"), "Files sizes")

	'Read data from a compressed file
	Dim in As InputStream
	in = File.OpenInput(File.DirRootExternal, "test.zlib")
	in = compress.WrapInputStream(in, "zlib")
	Dim reader As TextReader
	reader.Initialize(in)
	Dim line As String
	line = reader.ReadLine
	Msgbox(line, "First line")
	reader.Close
	
	'In memory compression / decompression
	Dim data() As Byte
	data = "Playing with in-memory compression.".GetBytes("UTF8")
	Dim compressed(), decompressed() As Byte
	compressed = compress.CompressBytes(data, "gzip")
	decompressed = compress.DecompressBytes(compressed, "gzip")
	'In this case the compressed data is longer than the decompressed data.
	'The data is too short for the compression to be useful.
	Log("Compressed: " & compressed.Length) 
	Log("Decompressed: " & decompressed.Length)
	Msgbox(BytesToString(decompressed,0, decompressed.Length, "UTF8"), "")
End Sub
Sub WriteStringToStream(Out As OutputStream, s As String)
	Dim t As TextWriter
	t.Initialize(Out)
	t.Write(s)
	t.Close 'Closes the internal stream as well
End Sub
```

## WrapOutputStream方法
**WrapOutputStream(Out,CompressMethod)**

?> 说明：包装输出流并返回一个输出流，该输出流在数据写入流时自动压缩数据。
>
> 参数：Out，类型：java.io.OutputStream
>
> 参数：CompressMethod，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.streams.File.OutputStreamWrapper
## DecompressBytes方法
**DecompressBytes(CompressedData,CompressMethod)**

?> 说明：返回包含解压缩数据的字节数组。
>
> 参数：CompressedData，类型：byte[]
>
> 参数：CompressMethod，类型：java.lang.String
>
> 返回值：byte[]
## CompressBytes方法
**CompressBytes(Data,CompressMethod)**

?> 说明：返回包含压缩数据的字节数组。
>
> 参数：Data，类型：byte[]
>
> 参数：CompressMethod，类型：java.lang.String
>
> 返回值：byte[]
## WrapInputStream方法
**WrapInputStream(In,CompressMethod)**

?> 说明：包装输入流并返回一个输入流，该输入流在读取时自动解压缩该流。
>
> 参数：In，类型：java.io.InputStream
>
> 参数：CompressMethod，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.streams.File.InputStreamWrapper

# B4XSerializator
完整类名：anywheresoftware.b4a.randomaccessfile.B4XSerializator
> 所有者：process
> 事件：
>
> ObjectToBytes (Success As Boolean, Bytes() As Byte)
>
> BytesToObject (Success As Boolean, NewObject As Object)
## ConvertBytesToObjectAsync方法
**ConvertBytesToObjectAsync(ba,Bytes,EventName)**

?> 说明：异步地将字节转换为对象。当对象准备就绪时，将引发BytesToObject事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Bytes，类型：byte[]
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## ConvertObjectToBytesAsync方法
**ConvertObjectToBytesAsync(ba,Object,EventName)**

?> 说明：异步地将对象转换为字节。ObjectToBytes事件将使用序列化的字节引发。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Object，类型：java.lang.Object
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## ConvertBytesToObject方法
**ConvertBytesToObject(Bytes)**

?> 说明：RandomAccessFile.ReadB4XObject的内存版本。
>
> 参数：Bytes，类型：byte[]
>
> 返回值：java.lang.Object
## ConvertObjectToBytes方法
**ConvertObjectToBytes(Object)**

?> 说明：RandomAccessFile.WriteB4X对象的内存版本。
>
> 参数：Object，类型：java.lang.Object
>
> 返回值：byte[]
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object

# AsyncStreams
完整类名：anywheresoftware.b4a.randomaccessfile.AsyncStreams
> 所有者：process

?> 说明：AsyncStreams对象允许您在后台读取InputStream并写入OutputStream，而不会阻塞主线程。
> 事件：
>
> NewData (Buffer() As Byte)
>
> Error
>
> Terminated
>
> NewStream (Dir As String, FileName As String)
## Write方法
**Write(Buffer)**

?> 说明：将给定的字节数组添加到输出流队列中。
>
> 参数：Buffer，类型：byte[]
>
> 返回值：boolean
## InitializePrefix方法
**InitializePrefix(ba,In,BigEndian,Out,EventName)**

?> 说明：初始化对象并将其设置为“前缀”模式。在此模式下，传入数据应遵守以下协议：
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：In，类型：java.io.InputStream
>
> 参数：BigEndian，类型：boolean
>
> 参数：Out，类型：java.io.OutputStream
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SendAllAndClose方法
**SendAllAndClose()**

?> 说明：向内部队列发送消息。AsyncStreams将在处理消息时关闭。
>
> 返回值：boolean
## WriteStream方法
**WriteStream(In,Size)**

?> 说明：写入给定的流。此方法仅在前缀模式下受支持。
>
> 参数：In，类型：java.io.InputStream
>
> 参数：Size，类型：java.lang.Long
>
> 返回值：boolean
## Close方法
**Close()**

?> 说明：关闭关联的流。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**

?> 说明：测试此对象是否已初始化。
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,In,Out,EventName)**

?> 说明：初始化对象。与前缀模式不同，NewData事件将在新数据可用时立即引发。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：In，类型：java.io.InputStream
>
> 参数：Out，类型：java.io.OutputStream
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Write2方法
**Write2(Buffer,Start,Length)**

?> 说明：将给定的字节数组添加到输出流队列中。
>
> 参数：Buffer，类型：byte[]
>
> 参数：Start，类型：int
>
> 参数：Length，类型：int
>
> 返回值：boolean
## StreamTotal属性

?> 说明：返回当前接收的文件的总字节数。仅在前缀模式下有效。
>
> 返回值：long
## StreamReceived属性

?> 说明：返回当前接收的文件的字节数。仅在前缀模式下有效。
>
> 返回值：long
## OutputQueueSize属性

?> 说明：返回在输出队列中等待的消息数。
>
> 返回值：int
## StreamFolder字段

?> 说明：收到的流将保存在此文件夹中。
>
> 返回值：java.lang.String

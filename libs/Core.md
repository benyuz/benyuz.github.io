# Core

版本:12.5
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Core)

# 
完整类名：anywheresoftware.b4a.objects.streams.File
> 所有者：process

?> 说明：File是一个预定义的对象，其中包含用于处理文件的方法。
## Delete方法
**Delete(Dir,FileName)**

?> 说明：删除指定的文件。如果文件名是目录，则必须为空才能删除。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：boolean
## IsDirectory方法
**IsDirectory(Dir,FileName)**

?> 说明：测试指定的文件是否为目录。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：boolean
## Size方法
**Size(Dir,FileName)**

?> 说明：返回指定文件的大小（以字节为单位）。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：long
## Combine方法
**Combine(Dir,FileName)**

?> 说明：返回给定文件的完整路径。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：java.lang.String
## MakeDir方法
**MakeDir(Parent,Dir)**

?> 说明：创建给定的文件夹（根据需要创建所有文件夹）。
```vbnet

File.MakeDir(File.DirInternal, "music/90")
```

>
> 参数：Parent，类型：java.lang.String
>
> 参数：Dir，类型：java.lang.String
>
> 返回值：void
## ReadMap2方法
**ReadMap2(Dir,FileName,Map)**

?> 说明：类似于ReadMap。ReadMap2将项目添加到给定的Map中。
```vbnet

Dim m As Map
m.Initialize
m.Put("Item #1", "")
m.Put("Item #2", "")
m = File.ReadMap2(File.DirInternal, "settings.txt", m)
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：Map，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## ListFiles方法
**ListFiles(Dir)**

?> 说明：返回一个只读列表，其中包含存储在指定路径中的所有文件和目录。
>
> 参数：Dir，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## LastModified方法
**LastModified(Dir,FileName)**

?> 说明：返回指定文件的最后修改日期。
```vbnet

Dim d As Long
d = File.LastModified(File.DirRootExternal, "1.txt")
Msgbox(DateTime.Date(d), "Last modified")
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：long
## ReadList方法
**ReadList(Dir,FileName)**

?> 说明：读取整个文件并返回一个包含所有行的列表（作为字符串）。
```vbnet

Dim List1 As List
List1 = File.ReadList(File.DirInternal, "1.txt")
For i = 0 to List1.Size - 1
	Log(List1.Get(i))
Next 
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## WriteMap方法
**WriteMap(Dir,FileName,Map)**

?> 说明：创建一个新文件并写入给定的映射。每个键值对都被写成一行。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：Map，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## Copy2方法
**Copy2(In,Out)**

?> 说明：将输入流中的所有可用数据复制到输出流中。
>
> 参数：In，类型：java.io.InputStream
>
> 参数：Out，类型：java.io.OutputStream
>
> 返回值：void
## ReadMap方法
**ReadMap(Dir,FileName)**

?> 说明：读取文件并将每一行解析为（字符串的）键值对。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## OpenOutput方法
**OpenOutput(Dir,FileName,Append)**

?> 说明：打开（或创建）位于Dir文件夹中的指定文件以进行写入。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：Append，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.streams.File.OutputStreamWrapper
## OpenInput方法
**OpenInput(Dir,FileName)**

?> 说明：打开位于Dir文件夹中的指定文件名进行读取。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.streams.File.InputStreamWrapper
## WriteList方法
**WriteList(Dir,FileName,List)**

?> 说明：将列表中的每个项目作为一行写入。
```vbnet

File.WriteList (File.DirInternal, "mylist.txt", List1)
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：List，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## WriteString方法
**WriteString(Dir,FileName,Text)**

?> 说明：将给定的文本写入新文件。
```vbnet

File.WriteString(File.DirInternal, "1.txt", "Some text")
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：Text，类型：java.lang.String
>
> 返回值：void
## ReadString方法
**ReadString(Dir,FileName)**

?> 说明：读取文件并将其内容作为字符串返回。
```vbnet

Dim text As String
text = File.ReadString(File.DirInternal, "1.txt")
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：java.lang.String
## ListFilesAsync方法
**ListFilesAsync(ba,Dir)**

?> 说明：ListFiles的异步版本。应与“等待”一起使用。
```vbnet

Wait For (File.ListFilesAsync(Dir)) Complete (Success As Boolean, Files As List)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Dir，类型：java.lang.String
>
> 返回值：java.lang.Object
## Copy2Async方法
**Copy2Async(ba,In,Out)**

?> 说明：将输入流中的所有可用数据异步复制到输出流中。
```vbnet

Wait For (File.Copy2Async(in, out)) Complete (Success As Boolean)
Log("Success: " & Success)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：In，类型：java.io.InputStream
>
> 参数：Out，类型：java.io.OutputStream
>
> 返回值：java.lang.Object
## ReadBytes方法
**ReadBytes(Dir,FileName)**

?> 说明：从给定文件中读取数据。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：byte[]
## CopyAsync方法
**CopyAsync(ba,DirSource,FileSource,DirTarget,FileTarget)**

?> 说明：将源文件异步复制到目标路径。
```vbnet

Wait For (File.CopyAsync(File.DirAssets, "1.txt", File.DirInternal, "1.txt")) Complete (Success As Boolean)
Log("Success: " & Success)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：DirSource，类型：java.lang.String
>
> 参数：FileSource，类型：java.lang.String
>
> 参数：DirTarget，类型：java.lang.String
>
> 参数：FileTarget，类型：java.lang.String
>
> 返回值：java.lang.Object
## Copy方法
**Copy(DirSource,FileSource,DirTarget,FileTarget)**

?> 说明：将指定的源文件复制到目标文件名。
>
> 参数：DirSource，类型：java.lang.String
>
> 参数：FileSource，类型：java.lang.String
>
> 参数：DirTarget，类型：java.lang.String
>
> 参数：FileTarget，类型：java.lang.String
>
> 返回值：void
## Exists方法
**Exists(Dir,FileName)**

?> 说明：如果指定的目录中存在指定的FileName，则返回true。
```vbnet

If File.Exists(File.DirInternal, "MyFile.txt") Then ...
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：boolean
## GetText方法
**GetText(Dir,FileName)**

?> 说明：读取整个文件并返回其文本。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：java.lang.String
## WriteBytes方法
**WriteBytes(Dir,FileName,Data)**

?> 说明：将数据写入给定的文件。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：Data，类型：byte[]
>
> 返回值：void
## ExternalReadable属性

?> 说明：测试是否可以读取外部存储介质。
>
> 返回值：boolean
## ExternalWritable属性

?> 说明：测试外部存储介质是否可以写入（也可以从中读取）。
>
> 返回值：boolean
## DirAssets属性

?> 说明：返回对添加到“文件”选项卡的文件的引用。这些文件是只读的。
>
> 返回值：java.lang.String
## DirInternalCache属性

?> 说明：返回设备内部存储中用于保存应用程序缓存数据的文件夹。
>
> 返回值：java.lang.String
## DirInternal属性

?> 说明：返回设备内部存储中用于保存应用程序专用数据的文件夹。
>
> 返回值：java.lang.String
## DirDefaultExternal属性

?> 说明：返回基于包名称的应用程序默认外部文件夹。
>
> 返回值：java.lang.String
## DirRootExternal属性

?> 说明：返回外部存储介质的根文件夹。
>
> 返回值：java.lang.String

# InputStream
完整类名：anywheresoftware.b4a.objects.streams.File.InputStreamWrapper
> 所有者：process

> 包装器：java.io.InputStream

?> 说明：你可以从中阅读的流。通常，您会将流传递给一个“更高级别”的对象，如处理读取的TextReader。
## BytesAvailable方法
**BytesAvailable()**

?> 说明：返回无阻塞可用字节数的估计值。
>
> 返回值：int
## Close方法
**Close()**

?> 说明：关闭流。
>
> 返回值：void
## ReadBytes方法
**ReadBytes(Buffer,StartOffset,MaxCount)**

?> 说明：从流中读取最多MaxCount个字节，并将其写入给定的缓冲区。
```vbnet

Dim buffer(1024) As byte
count = InputStream1.ReadBytes(buffer, 0, buffer.length)
```

>
> 参数：Buffer，类型：byte[]
>
> 参数：StartOffset，类型：int
>
> 参数：MaxCount，类型：int
>
> 返回值：int
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## InitializeFromBytesArray方法
**InitializeFromBytesArray(Buffer,StartOffset,MaxCount)**

?> 说明：使用File.OpenInput获取文件输入流。
>
> 参数：Buffer，类型：byte[]
>
> 参数：StartOffset，类型：int
>
> 参数：MaxCount，类型：int
>
> 返回值：void

# OutputStream
完整类名：anywheresoftware.b4a.objects.streams.File.OutputStreamWrapper
> 所有者：process

> 包装器：java.io.OutputStream

?> 说明：一个你可以写入的流。通常你会把流传递给一个“更高级别”的对象，比如TextWriter，它将处理写入。
## InitializeToBytesArray方法
**InitializeToBytesArray(StartSize)**

?> 说明：使用File.OpenOutput获取文件输出流。
>
> 参数：StartSize，类型：int
>
> 返回值：void
## ToBytesArray方法
**ToBytesArray()**

?> 说明：返回内部字节数组的副本。只能在使用InitializeToBytesArray初始化输出流时使用。
>
> 返回值：byte[]
## Flush方法
**Flush()**

?> 说明：刷新所有缓冲的数据。
>
> 返回值：void
## Close方法
**Close()**

?> 说明：关闭流。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## WriteBytes方法
**WriteBytes(Buffer,StartOffset,Length)**

?> 说明：将缓冲区写入流。要写入的第一个字节是Buffer（StartOffset），
>
> 参数：Buffer，类型：byte[]
>
> 参数：StartOffset，类型：int
>
> 参数：Length，类型：int
>
> 返回值：void

# TextWriter
完整类名：anywheresoftware.b4a.objects.streams.File.TextWriterWrapper
> 所有者：process

> 包装器：java.io.BufferedWriter

?> 说明：将文本写入基础流<br/>
```vbnet

Dim Writer As TextWriter
Writer.Initialize(File.OpenOutput(File.DirDefaultExternal, "1.txt", False))
Writer.WriteLine("This is the first line.")
Writer.WriteLine("This is the second line.")
Writer.Close
```

## Write方法
**Write(Text)**

?> 说明：将给定的文本写入流。
>
> 参数：Text，类型：java.lang.String
>
> 返回值：void
## WriteList方法
**WriteList(List)**

?> 说明：将列表中的每个项目作为一行写入。
>
> 参数：List，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## WriteLine方法
**WriteLine(Text)**

?> 说明：将给定的Text写入流，后跟一个换行符。
```vbnet

 	Dim Writer As TextWriter
	Writer.Initialize(File.OpenOutput(File.DirDefaultExternal, "1.txt", False))
	Writer.WriteLine("This is the first line.")
	Writer.WriteLine("This is the second line.")
	Writer.Close 
```

>
> 参数：Text，类型：java.lang.String
>
> 返回值：void
## Flush方法
**Flush()**

?> 说明：刷新所有缓冲的数据。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(OutputStream)**

?> 说明：通过使用UTF8编码包装给定的OutputStream来初始化此对象。
>
> 参数：OutputStream，类型：java.io.OutputStream
>
> 返回值：void
## Initialize2方法
**Initialize2(OutputStream,Encoding)**

?> 说明：通过使用指定的编码包装给定的OutputStream来初始化此对象。
>
> 参数：OutputStream，类型：java.io.OutputStream
>
> 参数：Encoding，类型：java.lang.String
>
> 返回值：void
## Close方法
**Close()**

?> 说明：关闭流。
>
> 返回值：void

# TextReader
完整类名：anywheresoftware.b4a.objects.streams.File.TextReaderWrapper
> 所有者：process

> 包装器：java.io.BufferedReader

?> 说明：从基础流中读取文本。在大多数情况下，您应该避免使用TextReader，而是使用File.ReadString或File.ReadList读取文本。
## ReadLine方法
**ReadLine()**

?> 说明：从流中读取下一行。不会返回换行符。
```vbnet

	Dim Reader As TextReader
	Reader.Initialize(File.OpenInput(File.DirInternal, "1.txt"))
	Dim line As String
 	line = Reader.ReadLine
 	Do While line <> Null
		Log(line)
		line = Reader.ReadLine
	Loop
	Reader.Close
```

>
> 返回值：java.lang.String
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(InputStream)**

?> 说明：通过使用UTF8编码包装给定的InputStream来初始化此对象。
>
> 参数：InputStream，类型：java.io.InputStream
>
> 返回值：void
## Read方法
**Read(Buffer,StartOffset,Length)**

?> 说明：从流中读取字符并将其写入缓冲区。
>
> 参数：Buffer，类型：char[]
>
> 参数：StartOffset，类型：int
>
> 参数：Length，类型：int
>
> 返回值：int
## Ready方法
**Ready()**

?> 说明：测试是否至少有一个字符可以在不阻塞的情况下读取。
>
> 返回值：boolean
## Initialize2方法
**Initialize2(InputStream,Encoding)**

?> 说明：通过使用指定的编码包装给定的InputStream来初始化此对象。
>
> 参数：InputStream，类型：java.io.InputStream
>
> 参数：Encoding，类型：java.lang.String
>
> 返回值：void
## ReadList方法
**ReadList()**

?> 说明：读取剩余的文本并返回一个用行填充的List对象。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## ReadAll方法
**ReadAll()**

?> 说明：读取所有剩余的文本并关闭流。
>
> 返回值：java.lang.String
## Skip方法
**Skip(NumberOfCharaceters)**

?> 说明：跳过指定的字符数。
>
> 参数：NumberOfCharaceters，类型：int
>
> 返回值：int
## Close方法
**Close()**

?> 说明：关闭流。
>
> 返回值：void

# Map
完整类名：anywheresoftware.b4a.objects.collections.Map
> 所有者：process

> 包装器：java.util.Map

?> 说明：包含成对键和值的集合。钥匙是独一无二的。这意味着，如果您添加一个键/值对（条目）和
```vbnet

For Each Key As String In Map.Keys
 Dim Value As Object = Map.Get(Key)
Next
```

## GetValueAt方法
**GetValueAt(Index)**

?> 说明：<b>此方法已弃用。使用For Each迭代值或使用B4XOrderedMap</b>
```vbnet

For i = 0 to Map.Size - 1
	Log("Key: " & Map.GetKeyAt(i))
	Log("Value: " & Map.GetValueAt(i))
Next
```

>
> 参数：Index，类型：int
>
> 返回值：java.lang.Object
## Values方法
**Values()**

?> 说明：返回一个对象，该对象可用于使用For Each块迭代所有值。
```vbnet

For Each v As Int In map1.Values
	Log(v)
Next
```

>
> 返回值：anywheresoftware.b4a.BA.IterableList
## Remove方法
**Remove(Key)**

?> 说明：删除具有给定键的项（如果存在）。
>
> 参数：Key，类型：java.lang.Object
>
> 返回值：java.lang.Object
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize()**

?> 说明：初始化对象。
```vbnet

Dim Map1 As Map
Map1.Initialize
```

>
> 返回值：void
## Put方法
**Put(Key,Value)**

?> 说明：在映射中放入一个键/值对，用这个键覆盖上一个项（如果存在的话）。
```vbnet

Map1.Put("Key", "Value")
```

>
> 参数：Key，类型：java.lang.Object
>
> 参数：Value，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Clear方法
**Clear()**

?> 说明：清除地图中的所有项目。
>
> 返回值：void
## ContainsKey方法
**ContainsKey(Key)**

?> 说明：测试是否存在具有给定密钥的项。
```vbnet

If Map.ContainsKey("some key") Then ... 
```

>
> 参数：Key，类型：java.lang.Object
>
> 返回值：boolean
## Get方法
**Get(Key)**

?> 说明：返回具有给定键的项的值。
>
> 参数：Key，类型：java.lang.Object
>
> 返回值：java.lang.Object
## GetKeyAt方法
**GetKeyAt(Index)**

?> 说明：<b>此方法已弃用。使用For Each迭代键或使用B4XOrderedMap</b>
```vbnet

For i = 0 to Map.Size - 1
	Log("Key: " & Map.GetKeyAt(i))
	Log("Value: " & Map.GetValueAt(i))
Next
```

>
> 参数：Index，类型：int
>
> 返回值：java.lang.Object
## Keys方法
**Keys()**

?> 说明：返回一个对象，该对象可用于使用For Each块迭代所有键。
```vbnet

For Each k As String In map1.Keys
	Log(k)
Next
```

>
> 返回值：anywheresoftware.b4a.BA.IterableList
## GetDefault方法
**GetDefault(Key,Default)**

?> 说明：返回具有给定键的项的值。如果不存在此类项，则返回指定的默认值。
>
> 参数：Key，类型：java.lang.Object
>
> 参数：Default，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Size属性

?> 说明：返回存储在映射中的项目数。
>
> 返回值：int

# List
完整类名：anywheresoftware.b4a.objects.collections.List
> 所有者：process

> 包装器：java.util.List

?> 说明：列表类似于动态数组。您可以在列表中添加和删除项目，列表将相应地更改其大小。
```vbnet

Dim List1 As List
List1.Initialize
List1.AddAll(Array As Int(1, 2, 3, 4, 5))
```

## Add方法
**Add(item)**

?> 说明：在列表末尾添加一个项目。
>
> 参数：item，类型：java.lang.Object
>
> 返回值：void
## Set方法
**Set(Index,Item)**

?> 说明：用新项替换指定索引中的当前项。
>
> 参数：Index，类型：int
>
> 参数：Item，类型：java.lang.Object
>
> 返回值：void
## SortCaseInsensitive方法
**SortCaseInsensitive(Ascending)**

?> 说明：从词法角度对列表进行排序，忽略字符大小写。
>
> 参数：Ascending，类型：boolean
>
> 返回值：void
## IndexOf方法
**IndexOf(Item)**

?> 说明：返回指定项的索引，如果未找到，则返回-1。
>
> 参数：Item，类型：java.lang.Object
>
> 返回值：int
## InsertAt方法
**InsertAt(Index,Item)**

?> 说明：将指定索引中的指定元素插入该索引的当前项之前。
>
> 参数：Index，类型：int
>
> 参数：Item，类型：java.lang.Object
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize()**

?> 说明：初始化一个空列表。
>
> 返回值：void
## SortTypeCaseInsensitive方法
**SortTypeCaseInsensitive(FieldName,Ascending)**

?> 说明：类似于排序类型。从词法角度对列表进行排序，忽略字符大小写。
>
> 参数：FieldName，类型：java.lang.String
>
> 参数：Ascending，类型：boolean
>
> 返回值：void
## Clear方法
**Clear()**

?> 说明：从列表中删除所有项目。
>
> 返回值：void
## SortType方法
**SortType(FieldName,Ascending)**

?> 说明：使用用户定义类型的项对列表进行排序。列表根据指定的字段进行排序。
```vbnet

Sub Process_Globals
	Type Person(Name As String, Age As Int)
End Sub

Sub Activity_Create(FirstTime As Boolean)
	Dim Persons As List
	Persons.Initialize
	For i = 1 To 50
		Dim p As Person
		p.Name = "Person" & i
		p.Age = Rnd(0, 121)
		Persons.Add(p)
	Next
	Persons.SortType("Age", True) 'Sort the list based on the Age field.
	For i = 0 To Persons.Size - 1
		Dim p As Person
		p = Persons.Get(i)
		Log(p)
	Next
End Sub
```

>
> 参数：FieldName，类型：java.lang.String
>
> 参数：Ascending，类型：boolean
>
> 返回值：void
## Initialize2方法
**Initialize2(Array)**

?> 说明：使用给定的值初始化列表。此方法应用于将数组转换为列表。
```vbnet

Dim List1 As List
List1.Initialize2(Array As Int(1,2,3,4,5))
```

>
> 参数：Array，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## AddAllAt方法
**AddAllAt(Index,List)**

?> 说明：从指定索引开始添加指定集合中的所有元素。
>
> 参数：Index，类型：int
>
> 参数：List，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## Get方法
**Get(Index)**

?> 说明：获取指定索引中的项。该项目不会从列表中删除。
>
> 参数：Index，类型：int
>
> 返回值：java.lang.Object
## Sort方法
**Sort(Ascending)**

?> 说明：对列表进行排序。
>
> 参数：Ascending，类型：boolean
>
> 返回值：void
## AddAll方法
**AddAll(List)**

?> 说明：将指定集合中的所有元素添加到列表的末尾。
```vbnet

List.AddAll(Array As String("value1", "value2"))
```

>
> 参数：List，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## RemoveAt方法
**RemoveAt(Index)**

?> 说明：删除指定索引处的项。
>
> 参数：Index，类型：int
>
> 返回值：void
## Size属性

?> 说明：返回列表中的项数。
>
> 返回值：int

# Typeface
完整类名：anywheresoftware.b4a.keywords.constants.TypefaceWrapper
> 所有者：process

> 包装器：android.graphics.Typeface

?> 说明：Typeface是一个预定义的对象，用于保存字体样式和默认安装的字体。
```vbnet

EditText1.Typeface = Typeface.DEFAULT_BOLD
```

## CreateNew方法
**CreateNew(Typeface1,Style)**

?> 说明：返回具有指定样式的字体。
```vbnet

Typeface.CreateNew(Typeface.MONOSPACE, Typeface.STYLE_ITALIC)
```

>
> 参数：Typeface1，类型：android.graphics.Typeface
>
> 参数：Style，类型：int
>
> 返回值：android.graphics.Typeface
## LoadFromAssets方法
**LoadFromAssets(FileName)**

?> 说明：加载使用文件管理器添加的字体文件。
```vbnet

Dim MyFont As Typeface
MyFont = Typeface.LoadFromAssets("MyFont.ttf")
EditText1.Typeface = MyFont
```

>
> 参数：FileName，类型：java.lang.String
>
> 返回值：android.graphics.Typeface
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## MATERIALICONS属性
>
> 返回值：android.graphics.Typeface
## FONTAWESOME属性
>
> 返回值：android.graphics.Typeface
## STYLE_BOLD_ITALIC字段
>
> 返回值：int
## STYLE_NORMAL字段
>
> 返回值：int
## STYLE_ITALIC字段
>
> 返回值：int
## DEFAULT_BOLD字段
>
> 返回值：android.graphics.Typeface
## MONOSPACE字段
>
> 返回值：android.graphics.Typeface
## STYLE_BOLD字段
>
> 返回值：int
## DEFAULT字段
>
> 返回值：android.graphics.Typeface
## SANS_SERIF字段
>
> 返回值：android.graphics.Typeface
## SERIF字段
>
> 返回值：android.graphics.Typeface

# 
完整类名：anywheresoftware.b4a.keywords.constants.KeyCodes
> 所有者：process

?> 说明：具有键代码常量的预定义对象。例如，这些常量会传递给“活动键按下”事件。
## KEYCODE_ALT_RIGHT字段
>
> 返回值：int
## KEYCODE_MEDIA_REWIND字段
>
> 返回值：int
## KEYCODE_SYM字段
>
> 返回值：int
## KEYCODE_AT字段
>
> 返回值：int
## KEYCODE_DPAD_UP字段
>
> 返回值：int
## KEYCODE_MINUS字段
>
> 返回值：int
## KEYCODE_ENVELOPE字段
>
> 返回值：int
## KEYCODE_DPAD_DOWN字段
>
> 返回值：int
## KEYCODE_COMMA字段
>
> 返回值：int
## KEYCODE_EQUALS字段
>
> 返回值：int
## KEYCODE_Y字段
>
> 返回值：int
## KEYCODE_DPAD_LEFT字段
>
> 返回值：int
## KEYCODE_Z字段
>
> 返回值：int
## KEYCODE_W字段
>
> 返回值：int
## KEYCODE_X字段
>
> 返回值：int
## KEYCODE_UNKNOWN字段
>
> 返回值：int
## KEYCODE_U字段
>
> 返回值：int
## KEYCODE_V字段
>
> 返回值：int
## KEYCODE_MEDIA_FAST_FORWARD字段
>
> 返回值：int
## KEYCODE_S字段
>
> 返回值：int
## KEYCODE_T字段
>
> 返回值：int
## KEYCODE_SHIFT_LEFT字段
>
> 返回值：int
## KEYCODE_VOLUME_UP字段
>
> 返回值：int
## KEYCODE_LEFT_BRACKET字段
>
> 返回值：int
## KEYCODE_PLUS字段
>
> 返回值：int
## KEYCODE_BACKSLASH字段
>
> 返回值：int
## KEYCODE_MUTE字段
>
> 返回值：int
## KEYCODE_ENDCALL字段
>
> 返回值：int
## KEYCODE_CLEAR字段
>
> 返回值：int
## KEYCODE_GRAVE字段
>
> 返回值：int
## KEYCODE_HEADSETHOOK字段
>
> 返回值：int
## KEYCODE_POWER字段
>
> 返回值：int
## KEYCODE_POUND字段
>
> 返回值：int
## KEYCODE_DPAD_CENTER字段
>
> 返回值：int
## KEYCODE_NUM字段
>
> 返回值：int
## KEYCODE_EXPLORER字段
>
> 返回值：int
## KEYCODE_SLASH字段
>
> 返回值：int
## KEYCODE_BACK字段
>
> 返回值：int
## KEYCODE_1字段
>
> 返回值：int
## KEYCODE_2字段
>
> 返回值：int
## KEYCODE_SHIFT_RIGHT字段
>
> 返回值：int
## KEYCODE_SEMICOLON字段
>
> 返回值：int
## KEYCODE_0字段
>
> 返回值：int
## KEYCODE_DEL字段
>
> 返回值：int
## KEYCODE_CALL字段
>
> 返回值：int
## KEYCODE_NOTIFICATION字段
>
> 返回值：int
## KEYCODE_MEDIA_PREVIOUS字段
>
> 返回值：int
## KEYCODE_MEDIA_PLAY_PAUSE字段
>
> 返回值：int
## KEYCODE_VOLUME_DOWN字段
>
> 返回值：int
## KEYCODE_RIGHT_BRACKET字段
>
> 返回值：int
## KEYCODE_SPACE字段
>
> 返回值：int
## KEYCODE_STAR字段
>
> 返回值：int
## KEYCODE_I字段
>
> 返回值：int
## KEYCODE_J字段
>
> 返回值：int
## KEYCODE_G字段
>
> 返回值：int
## KEYCODE_PERIOD字段
>
> 返回值：int
## KEYCODE_H字段
>
> 返回值：int
## KEYCODE_E字段
>
> 返回值：int
## KEYCODE_MEDIA_STOP字段
>
> 返回值：int
## KEYCODE_F字段
>
> 返回值：int
## KEYCODE_C字段
>
> 返回值：int
## KEYCODE_D字段
>
> 返回值：int
## KEYCODE_Q字段
>
> 返回值：int
## KEYCODE_R字段
>
> 返回值：int
## KEYCODE_SOFT_LEFT字段
>
> 返回值：int
## KEYCODE_O字段
>
> 返回值：int
## KEYCODE_P字段
>
> 返回值：int
## KEYCODE_M字段
>
> 返回值：int
## KEYCODE_N字段
>
> 返回值：int
## KEYCODE_ENTER字段
>
> 返回值：int
## KEYCODE_K字段
>
> 返回值：int
## KEYCODE_SOFT_RIGHT字段
>
> 返回值：int
## KEYCODE_L字段
>
> 返回值：int
## KEYCODE_9字段
>
> 返回值：int
## KEYCODE_APOSTROPHE字段
>
> 返回值：int
## KEYCODE_MENU字段
>
> 返回值：int
## KEYCODE_MEDIA_NEXT字段
>
> 返回值：int
## KEYCODE_TAB字段
>
> 返回值：int
## KEYCODE_HOME字段
>
> 返回值：int
## KEYCODE_7字段
>
> 返回值：int
## KEYCODE_FOCUS字段
>
> 返回值：int
## KEYCODE_8字段
>
> 返回值：int
## KEYCODE_ALT_LEFT字段
>
> 返回值：int
## KEYCODE_5字段
>
> 返回值：int
## KEYCODE_6字段
>
> 返回值：int
## KEYCODE_CAMERA字段
>
> 返回值：int
## KEYCODE_3字段
>
> 返回值：int
## KEYCODE_SEARCH字段
>
> 返回值：int
## KEYCODE_4字段
>
> 返回值：int
## KEYCODE_A字段
>
> 返回值：int
## KEYCODE_B字段
>
> 返回值：int
## KEYCODE_DPAD_RIGHT字段
>
> 返回值：int

# 
完整类名：anywheresoftware.b4a.keywords.constants.Gravity
> 所有者：process

?> 说明：包含“重力”值的预定义对象。
```vbnet

Dim EditText1 As EditText
EditText1.Initialize("")
EditText1.Gravity = Gravity.CENTER
```

## CENTER字段
>
> 返回值：int
## NO_GRAVITY字段
>
> 返回值：int
## FILL字段
>
> 返回值：int
## TOP字段
>
> 返回值：int
## LEFT字段
>
> 返回值：int
## CENTER_HORIZONTAL字段
>
> 返回值：int
## RIGHT字段
>
> 返回值：int
## BOTTOM字段
>
> 返回值：int
## CENTER_VERTICAL字段
>
> 返回值：int

# 
完整类名：anywheresoftware.b4a.keywords.constants.DialogResponse
> 所有者：process

?> 说明：一个预定义的对象，包含对话框返回的可能值。
```vbnet

Dim result As Int
result = Msgbox2("Save changes?", "", "Yes", "", "No", Null)
If result = DialogResponse.POSITIVE Then
	'save changes
End If
```

## POSITIVE字段
>
> 返回值：int
## CANCEL字段
>
> 返回值：int
## NEGATIVE字段
>
> 返回值：int

# 
完整类名：anywheresoftware.b4a.keywords.constants.Colors
> 所有者：process

?> 说明：包含颜色常量的预定义对象。
```vbnet
Activity.Color = Colors.Green
```

## ARGB方法
**ARGB(Alpha,R,G,B)**

?> 说明：返回一个整数值，该整数值表示由三个组件构建的颜色，并带有指定的alpha值。
>
> 参数：Alpha，类型：int
>
> 参数：R，类型：int
>
> 参数：G，类型：int
>
> 参数：B，类型：int
>
> 返回值：int
## RGB方法
**RGB(R,G,B)**

?> 说明：返回一个整数值，表示由这三个组件构建的颜色。
>
> 参数：R，类型：int
>
> 参数：G，类型：int
>
> 参数：B，类型：int
>
> 返回值：int
## Red字段
>
> 返回值：int
## Gray字段
>
> 返回值：int
## DarkGray字段
>
> 返回值：int
## LightGray字段
>
> 返回值：int
## White字段
>
> 返回值：int
## Cyan字段
>
> 返回值：int
## Transparent字段
>
> 返回值：int
## Blue字段
>
> 返回值：int
## Yellow字段
>
> 返回值：int
## Magenta字段
>
> 返回值：int
## Black字段
>
> 返回值：int
## Green字段
>
> 返回值：int

# StateListDrawable
完整类名：anywheresoftware.b4a.objects.drawable.StateListDrawable
> 所有者：activity

> 包装器：android.graphics.drawable.StateListDrawable

?> 说明：容纳其他可绘制对象并根据视图状态选择当前可绘制对象的可绘制对象。
## AddState2方法
**AddState2(State,Drawable)**

?> 说明：添加状态和可抽绳对。国家是由国家的组合而成的。
>
> 参数：State，类型：int[]
>
> 参数：Drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：void
## AddState方法
**AddState(State,Drawable)**

?> 说明：添加状态和可抽绳对。
>
> 参数：State，类型：int
>
> 参数：Drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：void
## AddCatchAllState方法
**AddCatchAllState(Drawable)**

?> 说明：添加在没有其他状态与当前状态匹配的情况下将使用的绘图。
>
> 参数：Drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize()**

?> 说明：初始化对象。
```vbnet

Dim Button1 As Button
Button1.Initialize("")
Dim sld As StateListDrawable
sld.Initiailize
sld.AddState (sld.State_Disabled, DisabledDrawable)
sld.AddState (sld.State_Pressed, PressedDrawable)
sld.AddCatchAllState (DefaultDrawable)
Button1.Background = sld
```

>
> 返回值：void
## State_Enabled字段
>
> 返回值：int
## State_Checked字段
>
> 返回值：int
## State_Focused字段
>
> 返回值：int
## State_Unchecked字段
>
> 返回值：int
## State_Pressed字段
>
> 返回值：int
## State_Disabled字段
>
> 返回值：int
## State_Selected字段
>
> 返回值：int

# GradientDrawable
完整类名：anywheresoftware.b4a.objects.drawable.GradientDrawable
> 所有者：activity

> 包装器：android.graphics.drawable.GradientDrawable

?> 说明：一种渐变色的抽屉，可以有圆角。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Orientation,Colors)**

?> 说明：初始化此对象。
```vbnet

Dim Gradient1 As GradientDrawable
Dim Clrs(2) As Int
Clrs(0) = Colors.Black
Clrs(1) = Colors.White
Gradient1.Initialize("TOP_BOTTOM", Clrs)
```

>
> 参数：Orientation，类型：android.graphics.drawable.GradientDrawable.Orientation
>
> 参数：Colors，类型：int[]
>
> 返回值：void
## CornerRadius属性

?> 说明：设置“矩形”角的半径。
```vbnet

Gradient1.CornerRadius = 20dip
```

>
> 参数：Radius，类型：float
>
> 返回值：

# ColorDrawable
完整类名：anywheresoftware.b4a.objects.drawable.ColorDrawable
> 所有者：activity

> 包装器：android.graphics.drawable.Drawable

?> 说明：一种纯色的抽屉，可以有圆角。
```vbnet

Dim cd As ColorDrawable
cd.Initialize(Colors.Green, 5dip)
Button1.Background = cd
```

## Initialize2方法
**Initialize2(Color,CornerRadius,BorderWidth,BorderColor)**
>
> 参数：Color，类型：int
>
> 参数：CornerRadius，类型：int
>
> 参数：BorderWidth，类型：int
>
> 参数：BorderColor，类型：int
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Color,CornerRadius)**

?> 说明：使用给定的颜色和圆角半径初始化绘图。
>
> 参数：Color，类型：int
>
> 参数：CornerRadius，类型：int
>
> 返回值：void

# Canvas
完整类名：anywheresoftware.b4a.objects.drawable.CanvasWrapper
> 所有者：activity

?> 说明：Canvas是在其他视图或（可变）位图上绘制的对象。
## DrawText方法
**DrawText(ba,Text,x,y,Typeface1,TextSize,Color,Align1)**

?> 说明：绘制文本。
```vbnet

Canvas1.DrawText("This is a nice sentence.", 200dip, 200dip, Typeface.DEFAULT_BOLD, 30, Colors.Blue, "LEFT")
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Text，类型：java.lang.String
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 参数：Typeface1，类型：android.graphics.Typeface
>
> 参数：TextSize，类型：float
>
> 参数：Color，类型：int
>
> 参数：Align1，类型：android.graphics.Paint.Align
>
> 返回值：void
## MeasureStringWidth方法
**MeasureStringWidth(Text,Typeface,TextSize)**

?> 说明：返回给定文本的宽度。
```vbnet

Dim Rect1 As Rect
Dim width, height As Float
Dim t As String
t = "Text to write"
width = Canvas1.MeasureStringWidth(t, Typeface.DEFAULT, 14)
height = Canvas1.MeasureStringHeight(t, Typeface.DEFAULT, 14)
Rect1.Initialize(100dip, 100dip, 100dip + width, 100dip + height)
Canvas1.DrawRect(Rect1, Colors.White, True, 0)
Canvas1.DrawText(t, Rect1.Left, Rect1.Bottom, Typeface.DEFAULT, 14, Colors.Blue, "LEFT")
```

>
> 参数：Text，类型：java.lang.String
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 参数：TextSize，类型：float
>
> 返回值：float
## DrawBitmap方法
**DrawBitmap(Bitmap1,SrcRect,DestRect)**

?> 说明：绘制位图。
```vbnet

Dim Bitmap1 As Bitmap
Bitmap1.Initialize(File.DirAssets, "X.jpg")
Dim DestRect As Rect
DestRect.Initialize(10dip, 10dip, 10dip + 100dip, 10dip + 100dip)
Canvas1.DrawBitmap(Bitmap1, Null, DestRect) 'draws the bitmap to the destination rectangle.

Dim SrcRect As Rect
SrcRect.Initialize(0, 0, Bitmap1.Width / 2, Bitmap1.Height) 'the left half of the bitmap.
DestRect.Top = 200dip
DestRect.Bottom = 200dip + 100dip
Canvas1.DrawBitmap(Bitmap1, SrcRect, DestRect) 'draws half of the bitmap.
Activity.Invalidate
```

>
> 参数：Bitmap1，类型：android.graphics.Bitmap
>
> 参数：SrcRect，类型：android.graphics.Rect
>
> 参数：DestRect，类型：android.graphics.Rect
>
> 返回值：void
## DrawDrawable方法
**DrawDrawable(Drawable1,DestRect)**

?> 说明：将Drawable绘制到指定的矩形中。
```vbnet

Dim Gradient1 As GradientDrawable
Dim Clrs(2) As Int
Clrs(0) = Colors.Green
Clrs(1) = Colors.Blue
Gradient1.Initialize("TOP_BOTTOM", Clrs)
Canvas1.DrawDrawable(Gradient1, DestRect)
Activity.Invalidate
```

>
> 参数：Drawable1，类型：android.graphics.drawable.Drawable
>
> 参数：DestRect，类型：android.graphics.Rect
>
> 返回值：void
## DrawPath方法
**DrawPath(Path1,Color,Filled,StrokeWidth)**

?> 说明：绘制路径。
```vbnet

Dim Path1 As Path
Path1.Initialize(50%x, 100%y)
Path1.LineTo(100%x, 50%y)
Path1.LineTo(50%x, 0%y)
Path1.LineTo(0%x, 50%y)
Path1.LineTo(50%x, 100%y)
Canvas1.DrawPath(Path1, Colors.Magenta, False, 10dip)
```

>
> 参数：Path1，类型：android.graphics.Path
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 返回值：void
## DrawTextRotated方法
**DrawTextRotated(ba,Text,x,y,Typeface1,TextSize,Color,Align1,Degree)**

?> 说明：旋转文本并绘制它。
```vbnet

Canvas1.DrawTextRotated("This is a nice sentence.", 200dip, 200dip, _
  Typeface.DEFAULT_BOLD, 30, Colors.Blue, "CENTER", -45)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Text，类型：java.lang.String
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 参数：Typeface1，类型：android.graphics.Typeface
>
> 参数：TextSize，类型：float
>
> 参数：Color，类型：int
>
> 参数：Align1，类型：android.graphics.Paint.Align
>
> 参数：Degree，类型：float
>
> 返回值：void
## DrawBitmapFlipped方法
**DrawBitmapFlipped(Bitmap1,SrcRect,DestRect,Vertically,Horizontally)**

?> 说明：翻转位图并绘制它。
```vbnet

Canvas1.DrawBitmapFlipped(Bitmap1, Null, DestRect, False, True)
```

>
> 参数：Bitmap1，类型：android.graphics.Bitmap
>
> 参数：SrcRect，类型：android.graphics.Rect
>
> 参数：DestRect，类型：android.graphics.Rect
>
> 参数：Vertically，类型：boolean
>
> 参数：Horizontally，类型：boolean
>
> 返回值：void
## DrawOvalRotated方法
**DrawOvalRotated(Rect1,Color,Filled,StrokeWidth,Degrees)**

?> 说明：旋转椭圆并绘制它。
>
> 参数：Rect1，类型：android.graphics.Rect
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 参数：Degrees，类型：float
>
> 返回值：void
## Initialize方法
**Initialize(Target)**

?> 说明：初始化画布以便在视图上绘制。
```vbnet

Dim Canvas1 As Canvas
Canvas1.Initialize(Activity) 'this canvas will draw on the activity background
```

>
> 参数：Target，类型：android.view.View
>
> 返回值：void
## DrawCircle方法
**DrawCircle(x,y,Radius,Color,Filled,StrokeWidth)**

?> 说明：画一个圆。
```vbnet

Canvas1.DrawCircle(150dip, 150dip, 20dip, Colors.Red, False, 10dip)
```

>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 参数：Radius，类型：float
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 返回值：void
## DrawPoint方法
**DrawPoint(x,y,Color)**

?> 说明：在指定的位置和颜色处绘制点。
```vbnet

Canvas1.DrawPoint(50%x, 50%y, Colors.Yellow) 'draws a point in the middle of the screen.
```

>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 参数：Color，类型：int
>
> 返回值：void
## RemoveClip方法
**RemoveClip()**

?> 说明：删除上一个剪裁区域。
>
> 返回值：void
## DrawBitmapRotated方法
**DrawBitmapRotated(Bitmap1,SrcRect,DestRect,Degrees)**

?> 说明：旋转位图并绘制它。
```vbnet

Canvas1.DrawBitmapRotated(Bitmap1, Null, DestRect, 70)
```

>
> 参数：Bitmap1，类型：android.graphics.Bitmap
>
> 参数：SrcRect，类型：android.graphics.Rect
>
> 参数：DestRect，类型：android.graphics.Rect
>
> 参数：Degrees，类型：float
>
> 返回值：void
## Initialize2方法
**Initialize2(Bitmap)**

?> 说明：初始化画布以便在此位图上绘制。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：void
## DrawLine方法
**DrawLine(x1,y1,x2,y2,Color,StrokeWidth)**

?> 说明：绘制一条从（x1，y1）到（x2，y2）的直线。笔划宽度确定线条的宽度。
```vbnet

Canvas1.DrawLine(100dip, 100dip, 200dip, 200dip, Colors.Red, 10dip)
Activity.Invalidate

```

>
> 参数：x1，类型：float
>
> 参数：y1，类型：float
>
> 参数：x2，类型：float
>
> 参数：y2，类型：float
>
> 参数：Color，类型：int
>
> 参数：StrokeWidth，类型：float
>
> 返回值：void
## DrawOval方法
**DrawOval(Rect1,Color,Filled,StrokeWidth)**

?> 说明：绘制一个椭圆形。
```vbnet

Dim Rect1 As Rect
Rect1.Initialize(100dip, 100dip, 200dip, 150dip)
Canvas1.DrawOval(Rect1, Colors.Gray, False, 5dip)
Activity.Invalidate
```

>
> 参数：Rect1，类型：android.graphics.Rect
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 返回值：void
## DrawRect方法
**DrawRect(Rect1,Color,Filled,StrokeWidth)**

?> 说明：绘制一个矩形。
```vbnet

Dim Rect1 As Rect
Rect1.Initialize(100dip, 100dip, 200dip, 150dip)
Canvas1.DrawRect(Rect1, Colors.Gray, False, 5dip)
Activity.Invalidate
```

>
> 参数：Rect1，类型：android.graphics.Rect
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 返回值：void
## MeasureStringHeight方法
**MeasureStringHeight(Text,Typeface,TextSize)**

?> 说明：返回给定文本的高度。
```vbnet

Dim Rect1 As Rect
Dim width, height As Float
Dim t As String
t = "Text to write"
width = Canvas1.MeasureStringWidth(t, Typeface.DEFAULT, 14)
height = Canvas1.MeasureStringHeight(t, Typeface.DEFAULT, 14)
Rect1.Initialize(100dip, 100dip, 100dip + width, 100dip + height)
Canvas1.DrawRect(Rect1, Colors.White, True, 0)
Canvas1.DrawText(t, Rect1.Left, Rect1.Bottom, Typeface.DEFAULT, 14, Colors.Blue, "LEFT")
```

>
> 参数：Text，类型：java.lang.String
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 参数：TextSize，类型：float
>
> 返回值：float
## DrawRectRotated方法
**DrawRectRotated(Rect1,Color,Filled,StrokeWidth,Degrees)**

?> 说明：旋转矩形并绘制它。
>
> 参数：Rect1，类型：android.graphics.Rect
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 参数：Degrees，类型：float
>
> 返回值：void
## DrawDrawableRotate方法
**DrawDrawableRotate(Drawable1,DestRect,Degrees)**

?> 说明：将Drawable旋转并绘制到指定的矩形中。
>
> 参数：Drawable1，类型：android.graphics.drawable.Drawable
>
> 参数：DestRect，类型：android.graphics.Rect
>
> 参数：Degrees，类型：float
>
> 返回值：void
## ClipPath方法
**ClipPath(Path1)**

?> 说明：将绘图区域剪裁到给定的路径。
```vbnet

Dim Gradient1 As GradientDrawable
Dim Clrs(2) As Int
Clrs(0) = Colors.Black
Clrs(1) = Colors.White
Gradient1.Initialize("TOP_BOTTOM", Clrs)
Dim Path1 As Path
Path1.Initialize(50%x, 100%y)
Path1.LineTo(100%x, 50%y)
Path1.LineTo(50%x, 0%y)
Path1.LineTo(0%x, 50%y)
Path1.LineTo(50%x, 100%y)
Canvas1.ClipPath(Path1) 'clip the drawing area to the path.
DestRect.Left = 0%y
DestRect.Top = 0%y
DestRect.Right = 100%x
DestRect.Bottom = 100%y
Canvas1.DrawDrawable(Gradient1, DestRect) 'fill the drawing area with the gradient.
Activity.Invalidate
```

>
> 参数：Path1，类型：android.graphics.Path
>
> 返回值：void
## DrawColor方法
**DrawColor(Color)**

?> 说明：用给定的颜色填充整个画布。
```vbnet

Canvas1.DrawColor(Colors.ARGB(100, 255, 0, 0)) 'fills with semi-transparent red color.
Activity.Invalidate
```

>
> 参数：Color，类型：int
>
> 返回值：void
## Bitmap属性

?> 说明：返回画布绘制到的位图。
```vbnet

Dim Out As OutputStream
Out = File.OpenOutput(File.DirRootExternal, "Test.png", False)
Canvas1.Bitmap.WriteToStream(out, 100, "PNG")
Out.Close
```

>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## AntiAlias属性

?> 说明：获取或设置是否应用抗锯齿。
>
> 参数：b，类型：boolean
>
> 返回值：boolean

# Bitmap
完整类名：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
> 所有者：process

> 包装器：android.graphics.Bitmap

?> 说明：保存位图图像的对象。位图可以从文件或其他输入流加载，也可以从不同的位图进行设置。
## InitializeSample方法
**InitializeSample(Dir,FileName,MaxWidth,MaxHeight)**

?> 说明：初始化给定文件中的位图。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：MaxWidth，类型：int
>
> 参数：MaxHeight，类型：int
>
> 返回值：void
## GetPixel方法
**GetPixel(x,y)**

?> 说明：返回指定位置的像素的颜色。
>
> 参数：x，类型：int
>
> 参数：y，类型：int
>
> 返回值：int
## Rotate方法
**Rotate(Degrees)**

?> 说明：返回<b>新的</b>旋转位图。位图将顺时针旋转。
>
> 参数：Degrees，类型：float
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## Resize方法
**Resize(Width,Height,KeepAspectRatio)**

?> 说明：返回具有给定宽度和高度的<b>新</b>位图。
>
> 参数：Width，类型：float
>
> 参数：Height，类型：float
>
> 参数：KeepAspectRatio，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Dir,FileName)**

?> 说明：初始化给定文件中的位图。
```vbnet

Dim Bitmap1 As Bitmap
Bitmap1.Initialize(File.DirAssets, "X.jpg")
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：void
## Crop方法
**Crop(Left,Top,Width,Height)**

?> 说明：返回<b>新的</b>裁剪位图。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## Initialize3方法
**Initialize3(Bitmap)**

?> 说明：使用原始图像的副本初始化位图（如有必要，可进行复制）。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：void
## Initialize2方法
**Initialize2(InputStream)**

?> 说明：初始化给定流中的位图。
>
> 参数：InputStream，类型：java.io.InputStream
>
> 返回值：void
## InitializeMutable方法
**InitializeMutable(Width,Height)**

?> 说明：使用指定的维度创建一个新的可变位图。可以使用Canvas对象在此位图上绘制。
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## InitializeResize方法
**InitializeResize(Dir,FileName,Width,Height,KeepAspectRatio)**

?> 说明：初始化位图并设置其大小。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 参数：KeepAspectRatio，类型：boolean
>
> 返回值：void
## WriteToStream方法
**WriteToStream(OutputStream,Quality,Format)**

?> 说明：将位图写入输出流。
```vbnet

Dim Out As OutputStream
Out = File.OpenOutput(File.DirRootExternal, "Test.png", False)
Bitmap1.WriteToStream(out, 100, "PNG")
Out.Close
```

>
> 参数：OutputStream，类型：java.io.OutputStream
>
> 参数：Quality，类型：int
>
> 参数：Format，类型：android.graphics.Bitmap.CompressFormat
>
> 返回值：void
## Height属性

?> 说明：返回位图高度。
>
> 返回值：int
## Scale属性

?> 说明：返回位图比例。
>
> 返回值：float
## Width属性

?> 说明：返回位图宽度。
>
> 返回值：int

# Rect
完整类名：anywheresoftware.b4a.objects.drawable.CanvasWrapper.RectWrapper
> 所有者：process

> 包装器：android.graphics.Rect

?> 说明：包含四个坐标，表示一个矩形。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Left,Top,Right,Bottom)**
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Left属性
>
> 参数：Left，类型：int
>
> 返回值：int
## Top属性
>
> 参数：Top，类型：int
>
> 返回值：int
## Right属性
>
> 参数：Right，类型：int
>
> 返回值：int
## Bottom属性
>
> 参数：Bottom，类型：int
>
> 返回值：int
## Height属性

?> 说明：获取或设置矩形高度。
>
> 参数：h，类型：int
>
> 返回值：int
## CenterY属性

?> 说明：返回垂直中心。
>
> 返回值：int
## CenterX属性

?> 说明：返回水平中心。
>
> 返回值：int
## Width属性

?> 说明：获取或设置矩形宽度。
>
> 参数：w，类型：int
>
> 返回值：int

# Path
完整类名：anywheresoftware.b4a.objects.drawable.CanvasWrapper.PathWrapper
> 所有者：process

> 包装器：android.graphics.Path

?> 说明：路径是表示连接路径的点的集合。
## LineTo方法
**LineTo(x,y)**

?> 说明：添加从最后一个点到指定点的直线。
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(x,y)**

?> 说明：初始化路径并设置第一个点的值。
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 返回值：void

# BitmapDrawable
完整类名：anywheresoftware.b4a.objects.drawable.BitmapDrawable
> 所有者：activity

> 包装器：android.graphics.drawable.BitmapDrawable

?> 说明：绘制位图的可绘制文件。位图是在初始化期间设置的。
```vbnet

Dim bd As BitmapDrawable
bd.Initialize(LoadBitmap(File.DirAssets, "SomeImage.png"))
bd.Gravity = Gravity.FILL
Activity.Background = bd
```

## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Bitmap)**
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：void
## Bitmap属性

?> 说明：返回内部位图。
>
> 返回值：android.graphics.Bitmap
## Gravity属性

?> 说明：获取或设置重力值。该值会影响图像的绘制方式。
```vbnet

BitmapDrawable1.Gravity = Gravity.FILL
```

>
> 参数：value，类型：int
>
> 返回值：int

# WebView
完整类名：anywheresoftware.b4a.objects.WebViewWrapper
> 所有者：activity

> 包装器：android.webkit.WebView

?> 说明：WebView视图使用内部WebKit引擎来显示Html页面。
```vbnet
Return Array As String("someuser", "password123")
```

> 事件：
>
> PageFinished (Url As String)
>
> OverrideUrl (Url As String) As Boolean
>
> UserAndPasswordRequired (Host As String, Realm As String) As String()

> 所需权限：
android.permission.INTERNET
## LoadUrl方法
**LoadUrl(Url)**

?> 说明：加载给定的Url。
```vbnet

WebView1.LoadUrl("http://www.google.com")
```

>
> 参数：Url，类型：java.lang.String
>
> 返回值：void
## LoadHtml方法
**LoadHtml(Html)**

?> 说明：加载给定的Html。
```vbnet

WebView1.LoadHtml("<html><body>Hello world!</body></html>")
```

>
> 参数：Html，类型：java.lang.String
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## Back方法
**Back()**

?> 说明：返回到上一个Url。
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## Zoom方法
**Zoom(In)**

?> 说明：根据in的值放大或缩小。
>
> 参数：In，类型：boolean
>
> 返回值：boolean
## CaptureBitmap方法
**CaptureBitmap()**

?> 说明：以位图形式返回完整的html页面。
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## StopLoading方法
**StopLoading()**

?> 说明：停止当前负载。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Forward方法
**Forward()**

?> 说明：转到下一个Url。
>
> 返回值：void
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## JavaScriptEnabled属性

?> 说明：获取或设置是否启用JavaScript。
>
> 参数：value，类型：boolean
>
> 返回值：boolean
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Url属性

?> 说明：返回当前Url。
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## ZoomEnabled属性

?> 说明：获取或设置是否启用了内部缩放功能。
>
> 参数：v，类型：boolean
>
> 返回值：boolean
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int

# Timer
完整类名：anywheresoftware.b4a.objects.Timer
> 所有者：process

?> 说明：Timer对象以指定的间隔生成ticks事件。
> 事件：
>
> Tick
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName,Interval)**

?> 说明：使用事件子前缀和指定的间隔（以毫秒为单位）初始化计时器。
```vbnet

Timer1.Initialize("Timer1", 1000)
Timer1.Enabled = True

Sub Timer1_Tick
 'Handle tick events
End Sub

```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Interval，类型：long
>
> 返回值：void
## Enabled属性

?> 说明：获取或设置计时器是否已启用（勾选）。
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Interval属性

?> 说明：获取或设置刻度事件之间的间隔（以毫秒为单位）。
>
> 参数：Interval，类型：long
>
> 返回值：long

# TabHost
完整类名：anywheresoftware.b4a.objects.TabHostWrapper
> 所有者：activity

> 包装器：android.widget.TabHost

?> 说明：TabHost是一个包含多个选项卡页的视图。每个选项卡页都包含其他子视图。
> 事件：
>
> TabChanged
>
> Click
>
> LongClick
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## AddTab方法
**AddTab(ba,Title,LayoutFile)**

?> 说明：添加选项卡页。
```vbnet

TabHost1.AddTab("Page 1", "page1.bal")
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Title，类型：java.lang.String
>
> 参数：LayoutFile，类型：java.lang.String
>
> 返回值：void
## AddTabWithIcon2方法
**AddTabWithIcon2(Title,DefaultBitmap,SelectedBitmap,View)**

?> 说明：添加选项卡页。选项卡标题包括一个图标。
>
> 参数：Title，类型：java.lang.String
>
> 参数：DefaultBitmap，类型：android.graphics.Bitmap
>
> 参数：SelectedBitmap，类型：android.graphics.Bitmap
>
> 参数：View，类型：android.view.View
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## AddTab2方法
**AddTab2(Title,View)**

?> 说明：添加选项卡页。
>
> 参数：Title，类型：java.lang.String
>
> 参数：View，类型：android.view.View
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## AddTabWithIcon方法
**AddTabWithIcon(ba,Title,DefaultBitmap,SelectedBitmap,LayoutFile)**

?> 说明：添加选项卡页。选项卡标题包括一个图标。
```vbnet

Dim bmp1, bmp2 As Bitmap
bmp1 = LoadBitmap(File.DirAssets, "ic.png")
bmp2 = LoadBitmap(File.DirAssets, "ic_selected.png")
TabHost1.AddTabWithIcon("Page 1", bmp1, bmp2,"tabpage1.bal")
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Title，类型：java.lang.String
>
> 参数：DefaultBitmap，类型：android.graphics.Bitmap
>
> 参数：SelectedBitmap，类型：android.graphics.Bitmap
>
> 参数：LayoutFile，类型：java.lang.String
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## TabCount属性

?> 说明：返回选项卡页数。
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## CurrentTab属性

?> 说明：获取或设置当前选项卡。
```vbnet

TabHost1.CurrentTab = (TabHost1.CurrentTab + 1) Mod TabHost1.TabCount 'switch to the next tab.

```

>
> 参数：Index，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int

# 
完整类名：anywheresoftware.b4a.objects.String2
> 所有者：process

?> 说明：字符串在Basic4android中是不可变的，这意味着您可以更改字符串变量的值，但不能更改存储在字符串对象中的文本。
```vbnet

Dim s As String
s = "some text"
s = s.Replace("a", "b")
```

## equalsIgnoreCase方法
**equalsIgnoreCase(other)**

?> 说明：如果忽略大小写，两个字符串相等，则返回true。
>
> 参数：other，类型：java.lang.String
>
> 返回值：boolean
## getBytes方法
**getBytes(Charset)**

?> 说明：将字符串编码为新的字节数组。
```vbnet

 Dim Data() As Byte
 Data = "Some string".GetBytes("UTF8")
```

>
> 参数：Charset，类型：java.lang.String
>
> 返回值：byte[]
## replace方法
**replace(Target,Replacement)**

?> 说明：返回将所有出现的Target替换为replacement后产生的新字符串。
>
> 参数：Target，类型：java.lang.String
>
> 参数：Replacement，类型：java.lang.String
>
> 返回值：java.lang.String
## indexOf方法
**indexOf(SearchFor)**

?> 说明：返回字符串中第一次出现SearchFor字符串的索引。
>
> 参数：SearchFor，类型：java.lang.String
>
> 返回值：int
## trim方法
**trim()**

?> 说明：返回原始字符串的副本，不包含任何前导或尾随空格。
>
> 返回值：java.lang.String
## indexOf方法
**indexOf(SearchFor,Index)**

?> 说明：返回字符串中第一次出现SearchFor字符串的索引。
>
> 参数：SearchFor，类型：java.lang.String
>
> 参数：Index，类型：int
>
> 返回值：int
## substring方法
**substring(BeginIndex)**

?> 说明：返回一个新字符串，该字符串是原始字符串的子字符串。
```vbnet
"012345".SubString(2) 'returns "2345"
```

>
> 参数：BeginIndex，类型：int
>
> 返回值：java.lang.String
## lastIndexOf方法
**lastIndexOf(SearchFor,Index)**

?> 说明：返回字符串中第一次出现SearchFor字符串的索引。
>
> 参数：SearchFor，类型：java.lang.String
>
> 参数：Index，类型：int
>
> 返回值：int
## startsWith方法
**startsWith(Prefix)**

?> 说明：如果此字符串以给定前缀开头，则返回true。
>
> 参数：Prefix，类型：java.lang.String
>
> 返回值：boolean
## toLowerCase方法
**toLowerCase()**

?> 说明：返回一个新字符串，该字符串是此字符串小写的结果。
>
> 返回值：java.lang.String
## toUpperCase方法
**toUpperCase()**

?> 说明：返回一个新字符串，它是此字符串的大写结果。
>
> 返回值：java.lang.String
## length方法
**length()**

?> 说明：返回此字符串的长度。
>
> 返回值：int
## charAt方法
**charAt(Index)**

?> 说明：返回给定索引处的字符。
>
> 参数：Index，类型：int
>
> 返回值：char
## lastIndexOf方法
**lastIndexOf(SearchFor)**

?> 说明：返回字符串中第一次出现SearchFor字符串的索引。
>
> 参数：SearchFor，类型：java.lang.String
>
> 返回值：int
## contains方法
**contains(SearchFor)**

?> 说明：测试字符串是否包含给定的字符串参数。
>
> 参数：SearchFor，类型：java.lang.String
>
> 返回值：boolean
## substring方法
**substring(BeginIndex,EndIndex)**

?> 说明：返回一个新字符串，该字符串是原始字符串的子字符串。
```vbnet
"012345".SubString2(2, 4) 'returns "23"
```

>
> 参数：BeginIndex，类型：int
>
> 参数：EndIndex，类型：int
>
> 返回值：java.lang.String
## compareTo方法
**compareTo(Other)**

?> 说明：从词法角度比较这两个字符串。
```vbnet

"abc".CompareTo("da") ' < 0 
"abc".CompareTo("Abc") ' > 0
"abc".CompareTo("abca")' < 0 
```

>
> 参数：Other，类型：java.lang.String
>
> 返回值：int
## endsWith方法
**endsWith(Suffix)**

?> 说明：如果此字符串以给定的后缀结尾，则返回true。
>
> 参数：Suffix，类型：java.lang.String
>
> 返回值：boolean

# Spinner
完整类名：anywheresoftware.b4a.objects.SpinnerWrapper
> 所有者：activity

> 包装器：anywheresoftware.b4a.objects.SpinnerWrapper.B4ASpinner

?> 说明：一个折叠列表，当用户单击它时打开，并允许用户选择一个项目。类似于WinForms组合框。
> 事件：
>
> ItemClick (Position As Int, Value As Object)
## Add方法
**Add(Item)**

?> 说明：添加项目。
```vbnet

Spinner1.Add("Sunday")
```

>
> 参数：Item，类型：java.lang.String
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Clear方法
**Clear()**

?> 说明：清除所有项目。
>
> 返回值：void
## GetItem方法
**GetItem(Index)**

?> 说明：返回指定索引处的项。
>
> 参数：Index，类型：int
>
> 返回值：java.lang.String
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## IndexOf方法
**IndexOf(value)**
>
> 参数：value，类型：java.lang.String
>
> 返回值：int
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## AddAll方法
**AddAll(List)**

?> 说明：添加多个项目。
```vbnet

Spinner1.AddAll(Array As String("Sunday", "Monday", ...))
```

>
> 参数：List，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## RemoveAt方法
**RemoveAt(Index)**

?> 说明：删除指定索引处的项。
>
> 参数：Index，类型：int
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## SelectedIndex属性

?> 说明：获取或设置所选项的索引。如果未选择任何项目，则返回-1。
>
> 参数：value，类型：int
>
> 返回值：int
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Size属性

?> 说明：返回项目数。
>
> 返回值：int
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## TextSize属性

?> 说明：获取或设置文本大小。应在添加项目之前设置大小。
>
> 参数：TextSize，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## DropdownBackgroundColor属性

?> 说明：获取或设置下拉项的背景颜色。应在添加项目之前设置颜色。
>
> 参数：Color，类型：int
>
> 返回值：int
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Prompt属性

?> 说明：获取或设置打开微调器时将显示的标题。
>
> 参数：title，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## DropdownTextColor属性

?> 说明：获取或设置下拉文本的颜色。应在添加项目之前设置颜色。
>
> 参数：Color，类型：int
>
> 返回值：int
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## TextColor属性

?> 说明：获取或设置文本颜色。应在添加项目之前设置颜色。
>
> 参数：Color，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## SelectedItem属性

?> 说明：返回所选项目的值。
>
> 返回值：java.lang.String
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int

# 
完整类名：anywheresoftware.b4a.objects.SimpleListAdapter.SingleLineLayout
> 所有者：process
## ItemHeight属性

?> 说明：获取或设置具有此布局的项的高度。
>
> 参数：Height，类型：int
>
> 返回值：int
## Background字段

?> 说明：具有此布局的项目的背景。
>
> 返回值：android.graphics.drawable.Drawable
## Label字段

?> 说明：用于第一行（也是SingleLineLayout情况下的唯一一行）的标签。
>
> 返回值：anywheresoftware.b4a.objects.LabelWrapper

# 
完整类名：anywheresoftware.b4a.objects.SimpleListAdapter.TwoLinesLayout
> 所有者：process
## ItemHeight属性

?> 说明：获取或设置具有此布局的项的高度。
>
> 参数：Height，类型：int
>
> 返回值：int
## Background字段

?> 说明：具有此布局的项目的背景。
>
> 返回值：android.graphics.drawable.Drawable
## SecondLabel字段

?> 说明：用于第二行的标签。
>
> 返回值：anywheresoftware.b4a.objects.LabelWrapper
## Label字段

?> 说明：用于第一行（也是SingleLineLayout情况下的唯一一行）的标签。
>
> 返回值：anywheresoftware.b4a.objects.LabelWrapper

# 
完整类名：anywheresoftware.b4a.objects.SimpleListAdapter.TwoLinesAndBitmapLayout
> 所有者：process
## ItemHeight属性

?> 说明：获取或设置具有此布局的项的高度。
>
> 参数：Height，类型：int
>
> 返回值：int
## Background字段

?> 说明：具有此布局的项目的背景。
>
> 返回值：android.graphics.drawable.Drawable
## SecondLabel字段

?> 说明：用于第二行的标签。
>
> 返回值：anywheresoftware.b4a.objects.LabelWrapper
## Label字段

?> 说明：用于第一行（也是SingleLineLayout情况下的唯一一行）的标签。
>
> 返回值：anywheresoftware.b4a.objects.LabelWrapper
## ImageView字段

?> 说明：保存位图的ImageView。
>
> 返回值：anywheresoftware.b4a.objects.ImageViewWrapper

# 
完整类名：anywheresoftware.b4a.objects.ServiceHelper
> 所有者：activity

?> 说明：每个服务模块都包括一个服务对象。
## StopForeground方法
**StopForeground(Id)**

?> 说明：使当前服务脱离前台状态，并取消具有给定Id的通知。
>
> 参数：Id，类型：int
>
> 返回值：void
## StartForeground方法
**StartForeground(Id,Notification)**

?> 说明：使当前服务处于前台状态并显示给定的通知。
>
> 参数：Id，类型：int
>
> 参数：Notification，类型：android.app.Notification
>
> 返回值：void
## StopAutomaticForeground方法
**StopAutomaticForeground()**

?> 说明：停止自动前台状态。如果服务不处于该状态，则不执行任何操作。
>
> 返回值：void
## AutomaticForegroundMode字段

?> 说明：设置自动前景模式。它应该是AUTOMATIC_FOREGROUND常量之一。
>
> 返回值：int
## AutomaticForegroundNotification字段

?> 说明：进入自动前台状态时将显示的通知。
>
> 返回值：android.app.Notification
## AUTOMATIC_FOREGROUND_WHEN_NEEDED字段

?> 说明：自动前台模式将在需要时设置。只有当应用程序处于后台时启动服务时，才会在Android 8+设备上发生这种情况。
>
> 返回值：int
## AUTOMATIC_FOREGROUND_NEVER字段

?> 说明：切勿进入自动前景模式。这意味着你必须自己处理，以避免应用程序崩溃。
>
> 返回值：int
## AUTOMATIC_FOREGROUND_ALWAYS字段

?> 说明：启动服务时始终进入前台模式。当您想确保操作系统在任务完成之前不会终止进程时，这很有用。
>
> 返回值：int

# SeekBar
完整类名：anywheresoftware.b4a.objects.SeekBarWrapper
> 所有者：activity

> 包装器：android.widget.SeekBar

?> 说明：允许用户通过拖动滑块来设置值的视图。类似于WinForms TrackBar。
> 事件：
>
> ValueChanged (Value As Int, UserChanged As Boolean)
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Max属性

?> 说明：获取或设置允许的最大值。
>
> 参数：value，类型：int
>
> 返回值：int
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Value属性

?> 说明：获取或设置当前值。
>
> 参数：value，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int

# ScrollView
完整类名：anywheresoftware.b4a.objects.ScrollViewWrapper
> 所有者：activity

> 包装器：android.widget.ScrollView

?> 说明：ScrollView是一个包含其他视图并允许用户垂直滚动这些视图的视图。
```vbnet
ScrollView1.Panel.AddView(...)
```

> 事件：
>
> ScrollChanged(Position As Int)
## ScrollToNow方法
**ScrollToNow(Scroll)**

?> 说明：立即滚动滚动视图（无动画）。
>
> 参数：Scroll，类型：int
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,Height)**

?> 说明：初始化ScrollView并将其内部面板高度设置为给定高度。
```vbnet

Dim ScrollView1 As ScrollView
ScrollView1.Initialize(1000dip)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## FullScroll方法
**FullScroll(Bottom)**

?> 说明：将滚动视图滚动到顶部或底部。
>
> 参数：Bottom，类型：boolean
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Initialize2方法
**Initialize2(ba,Height,EventName)**

?> 说明：类似于初始化。设置将处理ScrollChanged事件的Sub。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Height，类型：int
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Panel属性

?> 说明：返回可用于向其中添加视图的面板。
```vbnet

ScrollView1.Panel.AddView(...)
```

>
> 返回值：anywheresoftware.b4a.objects.PanelWrapper
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## ScrollPosition属性

?> 说明：获取或设置滚动位置。
>
> 参数：Scroll，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int

# RemoteViews
完整类名：anywheresoftware.b4a.objects.RemoteViewsWrapper
> 所有者：process

?> 说明：RemoteViews允许间接访问主屏幕小部件。
> 事件：
>
> RequestUpdate
>
> Disabled
## HandleWidgetEvents方法
**HandleWidgetEvents(ba,StartingIntent)**

?> 说明：检查启动此服务的意图是否是从小部件发送的，并根据该意图引发事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：StartingIntent，类型：android.content.Intent
>
> 返回值：boolean
## SetVisible方法
**SetVisible(ba,ViewName,Visible)**

?> 说明：设置给定视图的可见性。
```vbnet
rv.SetVisibile("Button1", False)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ViewName，类型：java.lang.String
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## SetTextColor方法
**SetTextColor(ba,ViewName,Color)**

?> 说明：设置给定按钮或标签的文本颜色。
```vbnet
rv.SetTextColor("Label1", Colors.Red)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ViewName，类型：java.lang.String
>
> 参数：Color，类型：int
>
> 返回值：void
## SetText方法
**SetText(ba,ViewName,Text)**

?> 说明：设置给定视图的文本。
```vbnet
rv.SetText("Label1", "New text")
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ViewName，类型：java.lang.String
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：void
## SetImage方法
**SetImage(ba,ImageViewName,Image)**

?> 说明：设置给定ImageView的图像。
```vbnet
rv.SetImage("ImageView1", LoadBitmap(File.DirAssets, "1.jpg"))
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ImageViewName，类型：java.lang.String
>
> 参数：Image，类型：android.graphics.Bitmap
>
> 返回值：void
## SetTextSize方法
**SetTextSize(ba,ViewName,Size)**

?> 说明：设置给定按钮或标签的文本大小。
```vbnet
rv.SetTextSize("Label1", 20)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ViewName，类型：java.lang.String
>
> 参数：Size，类型：float
>
> 返回值：void
## SetProgress方法
**SetProgress(ba,ProgressBarName,Progress)**

?> 说明：设置给定ProgressBar的进度值。值应介于0到100之间。
```vbnet
rv.SetProgress("ProgressBar1", 50)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ProgressBarName，类型：java.lang.String
>
> 参数：Progress，类型：int
>
> 返回值：void
## UpdateWidget方法
**UpdateWidget(ba)**

?> 说明：使用所做的更改更新小部件。此方法还负责配置事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void

# 
完整类名：anywheresoftware.b4a.objects.ReceiverHelper
> 所有者：process

# ProgressBar
完整类名：anywheresoftware.b4a.objects.ProgressBarWrapper
> 所有者：activity

> 包装器：android.widget.ProgressBar

?> 说明：进度条视图。Progress属性设置介于0到100之间的进度值。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Progress属性

?> 说明：获取或设置进度值。
>
> 参数：value，类型：int
>
> 返回值：int
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Indeterminate属性

?> 说明：获取或设置进度条是否处于不确定模式（循环动画）。
>
> 参数：value，类型：boolean
>
> 返回值：boolean
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int

# Panel
完整类名：anywheresoftware.b4a.objects.PanelWrapper
> 所有者：activity

> 包装器：android.view.ViewGroup

?> 说明：Panel是包含其他子视图的视图。
> 事件：
>
> Touch (Action As Int, X As Float, Y As Float)
>
> Click
>
> LongClick
## GetView方法
**GetView(Index)**

?> 说明：获取存储在指定索引中的视图。
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.ConcreteViewWrapper
## AddView方法
**AddView(View,Left,Top,Width,Height)**

?> 说明：将视图添加到此面板中。
>
> 参数：View，类型：android.view.View
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## GetAllViewsRecursive方法
**GetAllViewsRecursive()**

?> 说明：返回一个迭代器，该迭代器遍历所有子视图，包括添加到其他子视图的视图。
```vbnet

For Each v As View In Panel1.GetAllViewsRecursive
	...
Next
```

>
> 返回值：anywheresoftware.b4a.BA.IterableList
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RemoveViewAt方法
**RemoveViewAt(Index)**

?> 说明：删除存储在指定索引中的视图。
>
> 参数：Index，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## LoadLayout方法
**LoadLayout(LayoutFile,ba)**

?> 说明：将布局文件加载到此面板。返回所选布局变量的值。
>
> 参数：LayoutFile，类型：java.lang.String
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4a.keywords.LayoutValues
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## SetElevationAnimated方法
**SetElevationAnimated(Duration,Elevation)**
>
> 参数：Duration，类型：int
>
> 参数：Elevation，类型：float
>
> 返回值：void
## RemoveAllViews方法
**RemoveAllViews()**

?> 说明：删除所有子视图。
>
> 返回值：void
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## NumberOfViews属性

?> 说明：返回子视图的数目。
>
> 返回值：int
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Elevation属性
>
> 参数：e，类型：float
>
> 返回值：float
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## ACTION_MOVE字段
>
> 返回值：int
## ACTION_DOWN字段
>
> 返回值：int
## ACTION_UP字段
>
> 返回值：int

# Notification
完整类名：anywheresoftware.b4a.objects.NotificationWrapper
> 所有者：process

> 包装器：java.lang.Object

?> 说明：状态栏通知。用户可以打开通知屏幕并按下通知。
```vbnet

Dim n As Notification
n.Initialize
n.Icon = "icon"
n.SetInfo("This is the title", "and this is the body.", Main) 'Change Main to "" if this code is in the main module.
n.Notify(1)
```


> 所需权限：
android.permission.VIBRATE
android.permission.POST_NOTIFICATIONS
## SetInfo2New方法
**SetInfo2New(ba,Title,Body,Tag,Activity)**

?> 说明：类似于SetInfo。还设置一个可以稍后在Activity_Sume中提取的字符串。
```vbnet

Sub Activity_Resume
	Dim in As Intent
	in = Activity.GetStartingIntent
	If in.HasExtra("Notification_Tag") Then
		Log(in.GetExtra("Notification_Tag")) 'Will log the tag
	End If
End Sub
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Body，类型：java.lang.CharSequence
>
> 参数：Tag，类型：java.lang.CharSequence
>
> 参数：Activity，类型：java.lang.Object
>
> 返回值：void
## Notify方法
**Notify(Id)**

?> 说明：显示通知。
>
> 参数：Id，类型：int
>
> 返回值：void
## Cancel方法
**Cancel(Id)**

?> 说明：取消具有给定Id的通知。
>
> 参数：Id，类型：int
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize()**

?> 说明：初始化通知。默认情况下，通知会播放声音、显示灯光并振动手机。
>
> 返回值：void
## SetInfoNew方法
**SetInfoNew(ba,Title,Body,Activity)**

?> 说明：设置消息文本和操作。
```vbnet

n.SetInfo("Some title", "Some text", Main)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Body，类型：java.lang.CharSequence
>
> 参数：Activity，类型：java.lang.Object
>
> 返回值：void
## Initialize2方法
**Initialize2(ImportanceLevel)**

?> 说明：初始化通知并设置通知通道的重要性级别。
```vbnet

Dim no As Notification
no.Initialize2(no.IMPORTANCE_DEFAULT)
```

>
> 参数：ImportanceLevel，类型：int
>
> 返回值：void
## Vibrate属性

?> 说明：设置通知是否会振动。
```vbnet

n.Vibrate = False
```

>
> 参数：v，类型：boolean
>
> 返回值：
## Number属性

?> 说明：获取或设置将显示在图标上的数字。这对于在单个通知中表示多个事件非常有用。
>
> 参数：v，类型：int
>
> 返回值：int
## Light属性

?> 说明：设置通知是否显示灯光。
```vbnet

n.Light = False
```

>
> 参数：v，类型：boolean
>
> 返回值：
## Insistent属性

?> 说明：设置在用户打开通知屏幕之前是否重复播放声音。
>
> 参数：v，类型：boolean
>
> 返回值：
## Sound属性

?> 说明：设置通知是否播放声音。
```vbnet

n.Sound = False
```

>
> 参数：v，类型：boolean
>
> 返回值：
## Icon属性

?> 说明：设置显示的图标。
```vbnet

n.Icon = "icon"
```

>
> 参数：s，类型：java.lang.String
>
> 返回值：
## AutoCancel属性

?> 说明：设置用户单击通知时是否自动取消通知。
>
> 参数：v，类型：boolean
>
> 返回值：
## OnGoingEvent属性

?> 说明：设置此通知是否为“正在进行的事件”。通知将显示在正在进行的部分
>
> 参数：v，类型：boolean
>
> 返回值：
## IMPORTANCE_HIGH字段

?> 说明：更高的通知重要性：到处显示，发出噪音和偷看。可以使用全屏
>
> 返回值：int
## IMPORTANCE_LOW字段

?> 说明：通知重要性低：显示在各处，但不具有侵入性。
>
> 返回值：int
## IMPORTANCE_DEFAULT字段

?> 说明：默认通知重要性：到处显示，发出噪音，但不会在视觉上干扰。
>
> 返回值：int
## IMPORTANCE_MIN字段

?> 说明：最低通知重要性：仅显示在折叠下方的阴影中。
>
> 返回值：int

# MediaPlayer
完整类名：anywheresoftware.b4a.objects.MediaPlayerWrapper
> 所有者：process

?> 说明：MediaPlayer可用于播放音频文件。
> 事件：
>
> Complete
## Play方法
**Play()**

?> 说明：开始（或继续）播放加载的音频文件。
>
> 返回值：void
## Load方法
**Load(Dir,FileName)**

?> 说明：加载音频文件并准备播放。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：void
## Pause方法
**Pause()**

?> 说明：暂停播放。您可以通过调用“播放”从当前位置恢复播放。
>
> 返回值：void
## Initialize2方法
**Initialize2(ba,EventName)**

?> 说明：类似于Initialize2。回放完成时将引发完整事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Stop方法
**Stop()**

?> 说明：停止播放。在尝试再次播放之前，必须调用Load。
>
> 返回值：void
## SetVolume方法
**SetVolume(Left,Right)**

?> 说明：设置每个频道的播放音量。该值应介于0到1之间。
>
> 参数：Left，类型：float
>
> 参数：Right，类型：float
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## IsPlaying方法
**IsPlaying()**

?> 说明：如果媒体播放器当前正在播放，则返回true。
>
> 返回值：boolean
## Initialize方法
**Initialize()**

?> 说明：初始化对象。
```vbnet

Dim MP As MediaPlayer 'should be done in Sub Process_Globals
MP.Initialize2("MP")
MP.Load(File.DirAssets, "SomeFile.mp3")
MP.Play
```

>
> 返回值：void
## Release方法
**Release()**

?> 说明：释放媒体播放器分配的所有资源。
>
> 返回值：void
## Position属性

?> 说明：获取或设置当前位置（以毫秒为单位）。
>
> 参数：value，类型：int
>
> 返回值：int
## Looping属性

?> 说明：获取或设置媒体播放器是否将自动重新开始播放。
>
> 参数：value，类型：boolean
>
> 返回值：boolean
## Duration属性

?> 说明：返回加载文件的总持续时间（以毫秒为单位）。
>
> 返回值：int

# ListView
完整类名：anywheresoftware.b4a.objects.ListViewWrapper
> 所有者：activity

> 包装器：anywheresoftware.b4a.objects.ListViewWrapper.SimpleListView

?> 说明：ListView是一个非常有用的视图，可以处理大小列表。
> 事件：
>
> ItemClick (Position As Int, Value As Object)
>
> ItemLongClick (Position As Int, Value As Object)
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Clear方法
**Clear()**

?> 说明：清除列表中的所有项目。
>
> 返回值：void
## GetItem方法
**GetItem(Index)**

?> 说明：返回指定位置的项的值。
>
> 参数：Index，类型：int
>
> 返回值：java.lang.Object
## AddSingleLine2方法
**AddSingleLine2(Text,ReturnValue)**

?> 说明：添加单行项目。
```vbnet

ListView1.AddSingleLine2("Sunday", 1)
```

>
> 参数：Text，类型：java.lang.CharSequence
>
> 参数：ReturnValue，类型：java.lang.Object
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## AddTwoLines方法
**AddTwoLines(Text1,Text2)**

?> 说明：添加两行项目。
```vbnet

ListView1.AddTwoLines("This is the first line.", "And this is the second")
```

>
> 参数：Text1，类型：java.lang.CharSequence
>
> 参数：Text2，类型：java.lang.CharSequence
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## AddTwoLinesAndBitmap2方法
**AddTwoLinesAndBitmap2(Text1,Text2,Bitmap,ReturnValue)**

?> 说明：添加两行和一个位图项。
>
> 参数：Text1，类型：java.lang.CharSequence
>
> 参数：Text2，类型：java.lang.CharSequence
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 参数：ReturnValue，类型：java.lang.Object
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## SetSelection方法
**SetSelection(Position)**

?> 说明：设置当前选定的项目。调用此方法将使此项可见。
```vbnet
ListView1.SetSelection(10)
```

>
> 参数：Position，类型：int
>
> 返回值：void
## AddTwoLinesAndBitmap方法
**AddTwoLinesAndBitmap(Text1,Text2,Bitmap)**

?> 说明：添加两行和一个位图项。
```vbnet

ListView1.AddTwoLinesAndBitmap("First line", "Second line", LoadBitmap(File.DirAssets, "SomeImage.png"))
```

>
> 参数：Text1，类型：java.lang.CharSequence
>
> 参数：Text2，类型：java.lang.CharSequence
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：void
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## AddTwoLines2方法
**AddTwoLines2(Text1,Text2,ReturnValue)**

?> 说明：添加两行项目。
>
> 参数：Text1，类型：java.lang.CharSequence
>
> 参数：Text2，类型：java.lang.CharSequence
>
> 参数：ReturnValue，类型：java.lang.Object
>
> 返回值：void
## RemoveAt方法
**RemoveAt(Index)**

?> 说明：删除指定位置的项目。
>
> 参数：Index，类型：int
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## AddSingleLine方法
**AddSingleLine(Text)**

?> 说明：添加单行项目。
```vbnet

 ListView1.AddSingleLine("Sunday")
```

>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：void
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## ScrollingBackgroundColor属性

?> 说明：设置滚动列表时将使用的背景颜色。
```vbnet
Colors.Transparent
```

>
> 参数：Color，类型：int
>
> 返回值：
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Size属性

?> 说明：返回存储在列表中的项目数。
>
> 返回值：int
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## SingleLineLayout属性

?> 说明：返回用于显示单行项目的布局。
```vbnet

Dim Label1 As Label
Label1 = ListView1.SingleLineLayout.Label
Label1.TextSize = 20
Label1.TextColor = Colors.Green
```

>
> 返回值：anywheresoftware.b4a.objects.SimpleListAdapter.SingleLineLayout
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## TwoLinesAndBitmap属性

?> 说明：返回用于显示两行和位图项的布局。
```vbnet

ListView1.TwoLinesAndBitmap.SecondLabel.Visible = False
```

>
> 返回值：anywheresoftware.b4a.objects.SimpleListAdapter.TwoLinesAndBitmapLayout
## FastScrollEnabled属性

?> 说明：获取或设置用户滚动列表时是否显示快速滚动图标。
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## TwoLinesLayout属性

?> 说明：返回用于显示两行项目的布局。
```vbnet

Dim Label1 As Label
Label1 = ListView1.TwoLinesLayout.SecondLabel
Label1.TextSize = 20
Label1.TextColor = Colors.Green
```

>
> 返回值：anywheresoftware.b4a.objects.SimpleListAdapter.TwoLinesLayout
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int

# Label
完整类名：anywheresoftware.b4a.objects.LabelWrapper
> 所有者：activity

> 包装器：android.widget.TextView

?> 说明：显示只读文本的“标签”视图。
> 事件：
>
> Click
>
> LongClick
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(Duration,TextSize)**

?> 说明：使用动画效果更改文本大小。
>
> 参数：Duration，类型：int
>
> 参数：TextSize，类型：float
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(Duration,ToColor)**

?> 说明：使用当前颜色和ToColor颜色之间的过渡动画更改文本颜色。
>
> 参数：Duration，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## TextSize属性

?> 说明：获取或设置视图的文本大小。
>
> 参数：TextSize，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Ellipsize属性

?> 说明：获取或设置截断模式。仅影响单行字段。
>
> 参数：e，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## TextColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## SingleLine属性

?> 说明：设置文本字段应为单行模式还是多行模式。
>
> 参数：singleLine，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：Gravity，类型：int
>
> 返回值：int

# Intent
完整类名：anywheresoftware.b4a.objects.IntentWrapper
> 所有者：process

> 包装器：android.content.Intent

?> 说明：意向对象是可以发送到操作系统以执行某些外部操作的消息。
```vbnet
StartActivity
```

## SetComponent方法
**SetComponent(Component)**

?> 说明：显式设置将处理此意图的组件。
>
> 参数：Component，类型：java.lang.String
>
> 返回值：void
## ExtrasToString方法
**ExtrasToString()**

?> 说明：返回一个包含额外项的字符串。这对调试很有用。
>
> 返回值：java.lang.String
## AddCategory方法
**AddCategory(Category)**

?> 说明：添加描述意图所需操作的类别。
>
> 参数：Category，类型：java.lang.String
>
> 返回值：void
## GetExtra方法
**GetExtra(Name)**

?> 说明：返回具有给定键的项值。
>
> 参数：Name，类型：java.lang.String
>
> 返回值：java.lang.Object
## HasExtra方法
**HasExtra(Name)**

?> 说明：测试具有给定键的项是否存在。
>
> 参数：Name，类型：java.lang.String
>
> 返回值：boolean
## WrapAsIntentChooser方法
**WrapAsIntentChooser(Title)**

?> 说明：将意图包装在另一个“选择者”意图中。将向用户显示一个对话框，其中包含可以根据意图进行操作的可用服务。
```vbnet
WrapAsIntentChooser
```

>
> 参数：Title，类型：java.lang.String
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## PutExtra方法
**PutExtra(Name,Value)**

?> 说明：将额外数据添加到意图中。
>
> 参数：Name，类型：java.lang.String
>
> 参数：Value，类型：java.lang.Object
>
> 返回值：void
## Initialize方法
**Initialize(Action,Uri)**

?> 说明：使用给定的操作和数据Uri初始化对象。Action可以是其中一个Action常量或任何其他字符串。
>
> 参数：Action，类型：java.lang.String
>
> 参数：Uri，类型：java.lang.String
>
> 返回值：void
## SetPackage方法
**SetPackage(PackageName)**

?> 说明：显式设置目标应用程序的包名称。
>
> 参数：PackageName，类型：java.lang.String
>
> 返回值：void
## Initialize2方法
**Initialize2(Uri,Flags)**

?> 说明：通过分析Uri初始化对象。
```vbnet

Dim Intent1 As Intent
Intent1.Initialize2("http://www.basic4ppc.com", 0)
StartActivity(Intent1)
```

>
> 参数：Uri，类型：java.lang.String
>
> 参数：Flags，类型：int
>
> 返回值：void
## SetType方法
**SetType(Type)**

?> 说明：设置MIME类型。
```vbnet

Intent1.SetType("text/plain")
```

>
> 参数：Type，类型：java.lang.String
>
> 返回值：void
## GetData方法
**GetData()**

?> 说明：以字符串形式检索数据组件。
>
> 返回值：java.lang.String
## Action属性

?> 说明：获取或设置Intent操作。
>
> 参数：v，类型：java.lang.String
>
> 返回值：java.lang.String
## Flags属性

?> 说明：获取或设置标志组件。
>
> 参数：flags，类型：int
>
> 返回值：int
## ACTION_PICK字段
>
> 返回值：java.lang.String
## ACTION_APPWIDGET_UPDATE字段
>
> 返回值：java.lang.String
## ACTION_VIEW字段
>
> 返回值：java.lang.String
## ACTION_CALL字段
>
> 返回值：java.lang.String
## ACTION_EDIT字段
>
> 返回值：java.lang.String
## ACTION_SEND字段
>
> 返回值：java.lang.String
## ACTION_MAIN字段
>
> 返回值：java.lang.String

# ImageView
完整类名：anywheresoftware.b4a.objects.ImageViewWrapper
> 所有者：activity

> 包装器：android.widget.ImageView

?> 说明：显示图像的视图。
> 事件：
>
> Click
>
> LongClick
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。重力不会改变。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Bitmap属性

?> 说明：获取或设置分配给ImageView的位图。
```vbnet

ImageView1.Bitmap = LoadBitmap(File.DirAssets, "someimage.jpg")
```

>
> 参数：value，类型：android.graphics.Bitmap
>
> 返回值：android.graphics.Bitmap
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## Gravity属性

?> 说明：获取或设置分配给位图的重力。
```vbnet

ImageView1.Gravity = Gravity.Fill
```

>
> 参数：value，类型：int
>
> 返回值：int

# HorizontalScrollView
完整类名：anywheresoftware.b4a.objects.HorizontalScrollViewWrapper
> 所有者：activity

> 包装器：android.widget.HorizontalScrollView

?> 说明：HorizontalScrollView是一个包含其他视图并允许用户水平滚动这些视图的视图。
```vbnet
HorizontalScrollView1.Panel.AddView(...)
```

> 事件：
>
> ScrollChanged(Position As Int)
## ScrollToNow方法
**ScrollToNow(Scroll)**

?> 说明：立即滚动“水平滚动视图”（不带动画）。
>
> 参数：Scroll，类型：int
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,Width,EventName)**

?> 说明：初始化对象。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Width，类型：int
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## FullScroll方法
**FullScroll(Right)**

?> 说明：向右或向左滚动视图。
>
> 参数：Right，类型：boolean
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Panel属性

?> 说明：返回可用于向其中添加视图的面板。
```vbnet

HorizontalScrollView1.Panel.AddView(...)
```

>
> 返回值：anywheresoftware.b4a.objects.PanelWrapper
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## ScrollPosition属性

?> 说明：获取或设置滚动位置。
>
> 参数：Scroll，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int

# EditText
完整类名：anywheresoftware.b4a.objects.EditTextWrapper
> 所有者：activity

> 包装器：android.widget.EditText

?> 说明：EditText视图是允许用户编写自由文本的视图（类似于WinForms TextBox）。
```vbnet
EditText1.SingleLine = False
```

> 事件：
>
> TextChanged (Old As String, New As String)
>
> EnterPressed
>
> FocusChanged (HasFocus As Boolean)
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## SelectAll方法
**SelectAll()**

?> 说明：选择整个文本。
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(Duration,TextSize)**

?> 说明：使用动画效果更改文本大小。
>
> 参数：Duration，类型：int
>
> 参数：TextSize，类型：float
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(Duration,ToColor)**

?> 说明：使用当前颜色和ToColor颜色之间的过渡动画更改文本颜色。
>
> 参数：Duration，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## SetSelection方法
**SetSelection(Start,Length)**

?> 说明：设置选定的文本。
>
> 参数：Start，类型：int
>
> 参数：Length，类型：int
>
> 返回值：void
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Wrap属性

?> 说明：设置文本内容是否在EditText边界内换行。当EditText处于多行模式时相关。
```vbnet

EditText1.Wrap = False
```

>
> 参数：value，类型：boolean
>
> 返回值：
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## ForceDoneButton属性

?> 说明：默认情况下，操作系统会根据特定布局将虚拟键盘动作键设置为显示“完成”或“下一步”。
```vbnet

EditText1.ForceDoneButton = True
```

>
> 参数：value，类型：boolean
>
> 返回值：
## Hint属性

?> 说明：获取或设置EditText为空时将显示的文本。
```vbnet

EditText1.Hint = "Enter username"
```

>
> 参数：text，类型：java.lang.String
>
> 返回值：java.lang.String
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## SelectionStart属性

?> 说明：获取或设置选择的开始位置（或光标位置）。
>
> 参数：value，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## TextColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## Gravity属性
>
> 参数：Gravity，类型：int
>
> 返回值：int
## HintColor属性

?> 说明：获取或设置提示文本的颜色。
```vbnet

EditText1.HintColor = Colors.Gray
```

>
> 参数：Color，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## TextSize属性

?> 说明：获取或设置视图的文本大小。
>
> 参数：TextSize，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## PasswordMode属性

?> 说明：设置EditText是否应处于密码模式并隐藏实际字符。
>
> 参数：value，类型：boolean
>
> 返回值：
## Text属性
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Ellipsize属性

?> 说明：获取或设置截断模式。仅影响单行字段。
>
> 参数：e，类型：java.lang.String
>
> 返回值：java.lang.String
## InputType属性

?> 说明：获取或设置输入类型标志。此标志用于确定虚拟键盘的设置。
```vbnet

EditText1.InputType = EditText1.INPUT_TYPE_NUMBERS
```

>
> 参数：value，类型：int
>
> 返回值：int
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## SingleLine属性

?> 说明：设置EditText应处于单行模式还是多行模式。
>
> 参数：singleLine，类型：boolean
>
> 返回值：
## SelectionLength属性

?> 说明：获取选择长度。
>
> 返回值：int
## INPUT_TYPE_NONE字段

?> 说明：不会显示任何键盘。
>
> 返回值：int
## INPUT_TYPE_TEXT字段

?> 说明：默认文本模式。
>
> 返回值：int
## INPUT_TYPE_NUMBERS字段

?> 说明：将显示数字键盘。只接受数字。
>
> 返回值：int
## INPUT_TYPE_DECIMAL_NUMBERS字段

?> 说明：将显示数字键盘。接受数字、小数点和减号。
>
> 返回值：int
## INPUT_TYPE_PHONE字段

?> 说明：键盘将在电话模式下显示。
>
> 返回值：int

# CSBuilder
完整类名：anywheresoftware.b4a.objects.CSBuilder
> 所有者：process

> 包装器：android.text.SpannableStringBuilder

?> 说明：CSBuilder类似于StringBuilder，但它创建的是CharSequences而不是常规字符串。
```vbnet

Dim cs As CSBuilder
cs.Initialize.Color(Colors.Red).Bold.Append("Hello ").Pop.Underline.Append("World!!!").PopAll
Label1.Text = cs
```

> 事件：
>
> Click (Tag As Object)
## Size方法
**Size(Size)**

?> 说明：开始一个文本大小范围。请注意，不应将“dip”单位与文本大小标注一起使用。
>
> 参数：Size，类型：int
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Image方法
**Image(Bitmap,Width,Height,Baseline)**

?> 说明：添加图像跨度。此方法将添加一个空格字符作为图像的占位符。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 参数：Baseline，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Initialize方法
**Initialize()**

?> 说明：初始化生成器。您可以多次调用此方法来创建新的CharSequences。
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Alignment方法
**Alignment(Alignment)**

?> 说明：启动路线跨度。
>
> 参数：Alignment，类型：android.text.Layout.Alignment
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Strikethrough方法
**Strikethrough()**

?> 说明：开始删除线跨度。
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Clickable方法
**Clickable(ba,EventName,Tag)**

?> 说明：启动可单击的跨度。对于要引发的事件，您需要调用EnableClickEvents方法。
```vbnet

Sub Activity_Create(FirstTime As Boolean)
	Dim lbl As Label
	lbl.Initialize("")
	Activity.AddView(lbl, 0, 20dip, 100%x, 50dip)
	Dim cs As CSBuilder
	cs.Initialize.Size(20).Append("Click on underine word: ")
	cs.Clickable("cs", 1).Underline.Append("One").Pop.Pop
	cs.Append(", ").Clickable("cs", 2).Underline.Append("Two").PopAll
	cs.EnableClickEvents(lbl)
	lbl.Text = cs
End Sub

Sub cs_Click (Tag As Object)
	Log($"You have clicked on word: ${Tag}"$)
End Sub
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Tag，类型：java.lang.Object
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Underline方法
**Underline()**

?> 说明：开始下划线范围。
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## RelativeSize方法
**RelativeSize(Proportion)**

?> 说明：开始一个相对大小范围。实际文本大小将与设置的“比例”相乘。
>
> 参数：Proportion，类型：float
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## EnableClickEvents方法
**EnableClickEvents(Label)**

?> 说明：使用可单击跨度时应调用此方法。
>
> 参数：Label，类型：android.widget.TextView
>
> 返回值：void
## VerticalAlign方法
**VerticalAlign(Shift)**

?> 说明：开始垂直对齐跨度。
>
> 参数：Shift，类型：int
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## PopAll方法
**PopAll()**

?> 说明：关闭所有打开的跨度。
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Typeface方法
**Typeface(Typeface)**

?> 说明：开始自定义字体跨度。
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Color方法
**Color(Color)**

?> 说明：开始前景色范围。
>
> 参数：Color，类型：int
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## ScaleX方法
**ScaleX(Proportion)**

?> 说明：开始缩放X跨度。它水平缩放文本。
>
> 参数：Proportion，类型：float
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Pop方法
**Pop()**

?> 说明：关闭最近的跨度。所有跨度必须闭合。您可以调用PopAll来关闭所有打开的跨度。
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Append方法
**Append(Text)**

?> 说明：追加提供的字符串或字符序列。
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Bold方法
**Bold()**

?> 说明：以粗体开始。
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## ToString方法
**ToString()**

?> 说明：返回一个包含字符的字符串。
>
> 返回值：java.lang.String
## BackgroundColor方法
**BackgroundColor(Color)**

?> 说明：启动背景色范围。
>
> 参数：Color，类型：int
>
> 返回值：anywheresoftware.b4a.objects.CSBuilder
## Length属性

?> 说明：返回字符数。
>
> 返回值：int

# View
完整类名：anywheresoftware.b4a.objects.ConcreteViewWrapper
> 所有者：activity

> 包装器：android.view.View

?> 说明：视图是一种特殊类型的对象。无法创建新的视图对象。但是，所有其他视图类型都可以指定给视图变量。
```vbnet

For i = 0 To Activity.NumberOfViews - 1
	Dim v As View
	v = Activity.GetView(i)
	v.Visible = False
Next
```

> 事件：
>
> Click
>
> LongClick
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int

# CheckBox
完整类名：anywheresoftware.b4a.objects.CompoundButtonWrapper.CheckBoxWrapper
> 所有者：activity

> 包装器：android.widget.CheckBox

?> 说明：复选框视图。与单选按钮不同，每个复选框都可以独立检查。
> 事件：
>
> CheckedChange(Checked As Boolean)
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(Duration,TextSize)**

?> 说明：使用动画效果更改文本大小。
>
> 参数：Duration，类型：int
>
> 参数：TextSize，类型：float
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(Duration,ToColor)**

?> 说明：使用当前颜色和ToColor颜色之间的过渡动画更改文本颜色。
>
> 参数：Duration，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## TextSize属性

?> 说明：获取或设置视图的文本大小。
>
> 参数：TextSize，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Checked属性
>
> 参数：Value，类型：boolean
>
> 返回值：boolean
## Ellipsize属性

?> 说明：获取或设置截断模式。仅影响单行字段。
>
> 参数：e，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## TextColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## SingleLine属性

?> 说明：设置文本字段应为单行模式还是多行模式。
>
> 参数：singleLine，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：Gravity，类型：int
>
> 返回值：int

# RadioButton
完整类名：anywheresoftware.b4a.objects.CompoundButtonWrapper.RadioButtonWrapper
> 所有者：activity

> 包装器：android.widget.RadioButton

?> 说明：RadioButton视图。一个组中只能选中一个单选按钮。当选中不同的单选按钮时，所有其他按钮都将
> 事件：
>
> CheckedChange(Checked As Boolean)
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(Duration,TextSize)**

?> 说明：使用动画效果更改文本大小。
>
> 参数：Duration，类型：int
>
> 参数：TextSize，类型：float
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(Duration,ToColor)**

?> 说明：使用当前颜色和ToColor颜色之间的过渡动画更改文本颜色。
>
> 参数：Duration，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## TextSize属性

?> 说明：获取或设置视图的文本大小。
>
> 参数：TextSize，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Checked属性
>
> 参数：Value，类型：boolean
>
> 返回值：boolean
## Ellipsize属性

?> 说明：获取或设置截断模式。仅影响单行字段。
>
> 参数：e，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## TextColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## SingleLine属性

?> 说明：设置文本字段应为单行模式还是多行模式。
>
> 参数：singleLine，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：Gravity，类型：int
>
> 返回值：int

# ToggleButton
完整类名：anywheresoftware.b4a.objects.CompoundButtonWrapper.ToggleButtonWrapper
> 所有者：activity

> 包装器：android.widget.ToggleButton

?> 说明：ToggleButton视图。该视图类似于按钮，有两种模式：打开和关闭。
> 事件：
>
> CheckedChange(Checked As Boolean)
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(Duration,TextSize)**

?> 说明：使用动画效果更改文本大小。
>
> 参数：Duration，类型：int
>
> 参数：TextSize，类型：float
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(Duration,ToColor)**

?> 说明：使用当前颜色和ToColor颜色之间的过渡动画更改文本颜色。
>
> 参数：Duration，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## TextSize属性

?> 说明：获取或设置视图的文本大小。
>
> 参数：TextSize，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Checked属性
>
> 参数：Value，类型：boolean
>
> 返回值：boolean
## TextOn属性

?> 说明：获取或设置将在ON模式下显示的文本。
>
> 参数：value，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Ellipsize属性

?> 说明：获取或设置截断模式。仅影响单行字段。
>
> 参数：e，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## TextOff属性

?> 说明：获取或设置将在OFF模式下显示的文本。
>
> 参数：value，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## TextColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## SingleLine属性

?> 说明：设置文本字段应为单行模式还是多行模式。
>
> 参数：singleLine，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：Gravity，类型：int
>
> 返回值：int

# Button
完整类名：anywheresoftware.b4a.objects.ButtonWrapper
> 所有者：activity

> 包装器：android.widget.Button

?> 说明：按钮视图。
> 事件：
>
> Click
>
> LongClick
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(Duration,TextSize)**

?> 说明：使用动画效果更改文本大小。
>
> 参数：Duration，类型：int
>
> 参数：TextSize，类型：float
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(Duration,ToColor)**

?> 说明：使用当前颜色和ToColor颜色之间的过渡动画更改文本颜色。
>
> 参数：Duration，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## TextSize属性

?> 说明：获取或设置视图的文本大小。
>
> 参数：TextSize，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Ellipsize属性

?> 说明：获取或设置截断模式。仅影响单行字段。
>
> 参数：e，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## TextColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## SingleLine属性

?> 说明：设置文本字段应为单行模式还是多行模式。
>
> 参数：singleLine，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：Gravity，类型：int
>
> 返回值：int

# Exception
完整类名：anywheresoftware.b4a.objects.B4AException
> 所有者：process

> 包装器：java.lang.Exception

?> 说明：持有抛出的异常。
```vbnet

Try
   Dim in As InputStream
   in = File.OpenInput(File.DirInternal, "SomeMissingFile.txt")
   '...
Catch
   Log(LastException.Message)
End Try
If in.IsInitialized Then in.Close
```

## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Message属性
>
> 返回值：java.lang.String

# AutoCompleteEditText
完整类名：anywheresoftware.b4a.objects.AutoCompleteEditTextWrapper
> 所有者：process

> 包装器：android.widget.EditText

?> 说明：EditText的增强版，它向用户显示一个下拉列表，其中包含与当前输入的字符匹配的所有项目。
```vbnet

Sub Process_Globals

End Sub

Sub Globals
	Dim ACT As AutoCompleteEditText
End Sub

Sub Activity_Create(FirstTime As Boolean)
	ACT.Initialize("ACT")
	Activity.AddView(ACT, 10dip, 10dip, 500dip, 80dip)
	Dim countries() As String
	countries = Array As String( _
		"Afghanistan", "Albania", "Algeria", "American Samoa", "Andorra", _
		"Angola", "Anguilla", "Antarctica", "Antigua and Barbuda", "Argentina", _
		"Armenia", "Aruba", "Australia", "Austria", "Azerbaijan", _
		"Bahrain", "Bangladesh", "Barbados", "Belarus", "Belgium", _
		"Belize", "Benin", "Bermuda", "Bhutan", "Bolivia", _
		"Bosnia and Herzegovina", "Botswana", "Bouvet Island", "Brazil", "British Indian Ocean Territory", _
		"British Virgin Islands", "Brunei", "Bulgaria", "Burkina Faso", "Burundi", _
		"Cote d'Ivoire", "Cambodia", "Cameroon", "Canada", "Cape Verde", _
		"Cayman Islands", "Central African Republic", "Chad", "Chile", "China", _
		"Christmas Island", "Cocos (Keeling) Islands", "Colombia", "Comoros", "Congo", _
		"Cook Islands", "Costa Rica", "Croatia", "Cuba", "Cyprus", "Czech Republic", _
		"Democratic Republic of the Congo", "Denmark", "Djibouti", "Dominica", "Dominican Republic", _
		"East Timor", "Ecuador", "Egypt", "El Salvador", "Equatorial Guinea", "Eritrea", _
		"Estonia", "Ethiopia", "Faeroe Islands", "Falkland Islands", "Fiji", "Finland", _
		"Former Yugoslav Republic of Macedonia", "France", "French Guiana", "French Polynesia", _
		"French Southern Territories", "Gabon", "Georgia", "Germany", "Ghana", "Gibraltar", _
		"Greece", "Greenland", "Grenada", "Guadeloupe", "Guam", "Guatemala", "Guinea", "Guinea-Bissau", _
		"Guyana", "Haiti", "Heard Island and McDonald Islands", "Honduras", "Hong Kong", "Hungary", _
		"Iceland", "India", "Indonesia", "Iran", "Iraq", "Ireland", "Israel", "Italy", "Jamaica", _
		"Japan", "Jordan", "Kazakhstan", "Kenya", "Kiribati", "Kuwait", "Kyrgyzstan", "Laos", _
		"Latvia", "Lebanon", "Lesotho", "Liberia", "Libya", "Liechtenstein", "Lithuania", "Luxembourg", _
		"Macau", "Madagascar", "Malawi", "Malaysia", "Maldives", "Mali", "Malta", "Marshall Islands", _
		"Martinique", "Mauritania", "Mauritius", "Mayotte", "Mexico", "Micronesia", "Moldova", _
		"Monaco", "Mongolia", "Montserrat", "Morocco", "Mozambique", "Myanmar", "Namibia", _
		"Nauru", "Nepal", "Netherlands", "Netherlands Antilles", "New Caledonia", "New Zealand", _
		"Nicaragua", "Niger", "Nigeria", "Niue", "Norfolk Island", "North Korea", "Northern Marianas", _
		"Norway", "Oman", "Pakistan", "Palau", "Panama", "Papua New Guinea", "Paraguay", "Peru", _
		"Philippines", "Pitcairn Islands", "Poland", "Portugal", "Puerto Rico", "Qatar", _
		"Reunion", "Romania", "Russia", "Rwanda", "Sqo Tome and Principe", "Saint Helena", _
		"Saint Kitts and Nevis", "Saint Lucia", "Saint Pierre and Miquelon", _
		"Saint Vincent and the Grenadines", "Samoa", "San Marino", "Saudi Arabia", "Senegal", _
		"Seychelles", "Sierra Leone", "Singapore", "Slovakia", "Slovenia", "Solomon Islands", _
		"Somalia", "South Africa", "South Georgia and the South Sandwich Islands", "South Korea", _
		"Spain", "Sri Lanka", "Sudan", "Suriname", "Svalbard and Jan Mayen", "Swaziland", "Sweden", _
		"Switzerland", "Syria", "Taiwan", "Tajikistan", "Tanzania", "Thailand", "The Bahamas", _
		"The Gambia", "Togo", "Tokelau", "Tonga", "Trinidad and Tobago", "Tunisia", "Turkey", _
		"Turkmenistan", "Turks and Caicos Islands", "Tuvalu", "Virgin Islands", "Uganda", _
		"Ukraine", "United Arab Emirates", "United Kingdom", _
		"United States", "United States Minor Outlying Islands", "Uruguay", "Uzbekistan", _
		"Vanuatu", "Vatican City", "Venezuela", "Vietnam", "Wallis and Futuna", "Western Sahara", _
		"Yemen", "Yugoslavia", "Zambia", "Zimbabwe")
	ACT.SetItems(countries)
End Sub

Sub Activity_Pause (UserClosed As Boolean)

End Sub
```

> 事件：
>
> ItemClick (Value As String)
>
> TextChanged (Old As String, New As String)
>
> EnterPressed
>
> FocusChanged (HasFocus As Boolean)
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## SelectAll方法
**SelectAll()**

?> 说明：选择整个文本。
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(Duration,TextSize)**

?> 说明：使用动画效果更改文本大小。
>
> 参数：Duration，类型：int
>
> 参数：TextSize，类型：float
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(Duration,ToColor)**

?> 说明：使用当前颜色和ToColor颜色之间的过渡动画更改文本颜色。
>
> 参数：Duration，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetItems方法
**SetItems(ba,Items)**

?> 说明：设置可能项目的列表。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Items，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## ShowDropDown方法
**ShowDropDown()**

?> 说明：强制显示下拉列表。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**

?> 说明：从其父视图中删除此视图。
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## DismissDropDown方法
**DismissDropDown()**

?> 说明：强制下拉列表消失。
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetItems2方法
**SetItems2(ba,Items,Typeface,Gravity,TextSize,TextColor)**

?> 说明：设置可能项目的列表并指定其样式。
```vbnet

Dim act As AutoCompleteEditText
act.Initialize("act")
Activity.AddView(act, 10dip, 10dip, 200dip, 80dip)
act.SetItems2(Array As String("aab", "abc"), act.Typeface, Gravity.LEFT, 12, Colors.Green) 
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Items，类型：anywheresoftware.b4a.objects.collections.List
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 参数：Gravity，类型：int
>
> 参数：TextSize，类型：float
>
> 参数：TextColor，类型：int
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## SetSelection方法
**SetSelection(Start,Length)**

?> 说明：设置选定的文本。
>
> 参数：Start，类型：int
>
> 参数：Length，类型：int
>
> 返回值：void
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Wrap属性

?> 说明：设置文本内容是否在EditText边界内换行。当EditText处于多行模式时相关。
```vbnet

EditText1.Wrap = False
```

>
> 参数：value，类型：boolean
>
> 返回值：
## Left属性

?> 说明：获取或设置视图的左侧位置。
>
> 参数：left，类型：int
>
> 返回值：int
## ForceDoneButton属性

?> 说明：默认情况下，操作系统会根据特定布局将虚拟键盘动作键设置为显示“完成”或“下一步”。
```vbnet

EditText1.ForceDoneButton = True
```

>
> 参数：value，类型：boolean
>
> 返回值：
## Hint属性

?> 说明：获取或设置EditText为空时将显示的文本。
```vbnet

EditText1.Hint = "Enter username"
```

>
> 参数：text，类型：java.lang.String
>
> 返回值：java.lang.String
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## SelectionStart属性

?> 说明：获取或设置选择的开始位置（或光标位置）。
>
> 参数：value，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## TextColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## Gravity属性
>
> 参数：Gravity，类型：int
>
> 返回值：int
## HintColor属性

?> 说明：获取或设置提示文本的颜色。
```vbnet

EditText1.HintColor = Colors.Gray
```

>
> 参数：Color，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## TextSize属性

?> 说明：获取或设置视图的文本大小。
>
> 参数：TextSize，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## PasswordMode属性

?> 说明：设置EditText是否应处于密码模式并隐藏实际字符。
>
> 参数：value，类型：boolean
>
> 返回值：
## Text属性
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Ellipsize属性

?> 说明：获取或设置截断模式。仅影响单行字段。
>
> 参数：e，类型：java.lang.String
>
> 返回值：java.lang.String
## InputType属性

?> 说明：获取或设置输入类型标志。此标志用于确定虚拟键盘的设置。
```vbnet

EditText1.InputType = EditText1.INPUT_TYPE_NUMBERS
```

>
> 参数：value，类型：int
>
> 返回值：int
## Top属性

?> 说明：获取或设置视图的顶部位置。
>
> 参数：top，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## SingleLine属性

?> 说明：设置EditText应处于单行模式还是多行模式。
>
> 参数：singleLine，类型：boolean
>
> 返回值：
## SelectionLength属性

?> 说明：获取选择长度。
>
> 返回值：int
## INPUT_TYPE_NONE字段

?> 说明：不会显示任何键盘。
>
> 返回值：int
## INPUT_TYPE_TEXT字段

?> 说明：默认文本模式。
>
> 返回值：int
## INPUT_TYPE_NUMBERS字段

?> 说明：将显示数字键盘。只接受数字。
>
> 返回值：int
## INPUT_TYPE_DECIMAL_NUMBERS字段

?> 说明：将显示数字键盘。接受数字、小数点和减号。
>
> 返回值：int
## INPUT_TYPE_PHONE字段

?> 说明：键盘将在电话模式下显示。
>
> 返回值：int

# Activity
完整类名：anywheresoftware.b4a.objects.ActivityWrapper
> 所有者：activity

> 包装器：anywheresoftware.b4a.BALayout

?> 说明：每个活动模块都包括一个预定义的“活动”对象。
```vbnet

Sub Activity_KeyPress (KeyCode As Int) As Boolean
	If Keycode = KeyCodes.KEYCODE_BACK Then
		Return True
	Else
		Return False
	End If
End Sub
```

> 事件：
>
> Touch (Action As Int, X As Float, Y As Float)
>
> KeyPress (KeyCode As Int) As Boolean 'Return True to consume the event
>
> KeyUp (KeyCode As Int) As Boolean
>
> WindowFocusChanged (Focused As Boolean)
>
> ActionBarHomeClick
>
> PermissionResult (Permission As String, Result As Boolean)
>
> Click
>
> LongClick
## AddMenuItem2方法
**AddMenuItem2(Title,EventName,Bitmap)**

?> 说明：将菜单项添加到活动中。
```vbnet

Activity.AddMenuItem2("Open File", "OpenFile", LoadBitmap(File.DirAssets, "SomeImage.png"))
...
Sub OpenFile_Click
...
End Sub
```

>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：void
## GetView方法
**GetView(Index)**

?> 说明：获取存储在指定索引中的视图。
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.ConcreteViewWrapper
## RerunDesignerScript方法
**RerunDesignerScript(Layout,ba,Width,Height)**

?> 说明：<b>此方法已弃用</b> 它会忽略锚定功能，并且在快速调试模式下会失败。
>
> 参数：Layout，类型：java.lang.String
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## AddView方法
**AddView(View,Left,Top,Width,Height)**

?> 说明：将视图添加到此活动中。
>
> 参数：View，类型：android.view.View
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## GetStartingIntent方法
**GetStartingIntent()**

?> 说明：（高级）获取启动此“活动”的intent对象。
>
> 返回值：anywheresoftware.b4a.objects.IntentWrapper
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## GetAllViewsRecursive方法
**GetAllViewsRecursive()**

?> 说明：返回一个迭代器，该迭代器遍历所有子视图，包括添加到其他子视图的视图。
```vbnet

For Each v As View In Activity.GetAllViewsRecursive
	...
Next
```

>
> 返回值：anywheresoftware.b4a.BA.IterableList
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化视图并设置将处理事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RemoveViewAt方法
**RemoveViewAt(Index)**

?> 说明：删除存储在指定索引中的视图。
>
> 参数：Index，类型：int
>
> 返回值：void
## Finish方法
**Finish()**

?> 说明：关闭此活动。
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：使用淡入或淡出动画更改视图可见性。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## SetActivityResult方法
**SetActivityResult(Result,Data)**

?> 说明：（高级）设置调用StartActivityForResult后调用“活动”将获得的结果。
>
> 参数：Result，类型：int
>
> 参数：Data，类型：anywheresoftware.b4a.objects.IntentWrapper
>
> 返回值：void
## AddMenuItem方法
**AddMenuItem(Title,EventName)**

?> 说明：将菜单项添加到活动中。
```vbnet

Activity.AddMenuItem("Open File", "OpenFile")
...
Sub OpenFile_Click
...
End Sub
```

>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使给定的矩形无效。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使给定的矩形无效。
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## LoadLayout方法
**LoadLayout(LayoutFile,ba)**

?> 说明：加载布局文件（.bal）。
>
> 参数：LayoutFile，类型：java.lang.String
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4a.keywords.LayoutValues
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## OpenMenu方法
**OpenMenu()**

?> 说明：以编程方式打开菜单。
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(Bitmap)**

?> 说明：使用给定的位图创建BitmapDrawable，并将其设置为视图的背景。“重力”设置为“填充”。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## DisableAccessibility方法
**DisableAccessibility(Disable)**

?> 说明：添加此方法是为了解决以下Android错误。
>
> 参数：Disable，类型：boolean
>
> 返回值：void
## RemoveAllViews方法
**RemoveAllViews()**

?> 说明：删除所有子视图。
>
> 返回值：void
## Invalidate方法
**Invalidate()**

?> 说明：使整个视图无效，强制视图重新绘制自身。
>
> 返回值：void
## CloseMenu方法
**CloseMenu()**

?> 说明：以编程方式关闭菜单。
>
> 返回值：void
## AddMenuItem3方法
**AddMenuItem3(Title,EventName,Bitmap,AddToActionBar)**

?> 说明：类似于AddMenuItem2。如果AddToActionBar为true，那么如果有足够的空间，该项目将显示在动作栏中（在Android 3.0+设备上）。
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 参数：AddToActionBar，类型：boolean
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**

?> 说明：尝试将焦点设置为此视图。
>
> 返回值：boolean
## Left属性
>
> 参数：left，类型：int
>
> 返回值：int
## Background属性

?> 说明：获取或设置可绘制的背景。
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Parent属性

?> 说明：返回视图的父级。在大多数情况下，可以将返回的值强制转换为Panel。
>
> 返回值：java.lang.Object
## Color属性

?> 说明：将视图的背景设置为具有给定颜色的ColorDrawable。
>
> 参数：color，类型：int
>
> 返回值：
## NumberOfViews属性

?> 说明：返回子视图的数目。
>
> 返回值：int
## Title属性
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：java.lang.CharSequence
## Top属性
>
> 参数：top，类型：int
>
> 返回值：int
## Padding属性

?> 说明：获取或设置视图的填充（边框和内容之间的距离）。
```vbnet
Button1.Padding = Array As Int (30dip, 10dip, 10dip, 10dip)
```

>
> 参数：p，类型：int[]
>
> 返回值：int[]
## TitleColor属性

?> 说明：获取或设置标题颜色。此属性仅由Android 2.x设备支持。它不会在更新的设备上执行任何操作。
>
> 参数：Color，类型：int
>
> 返回值：int
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：height，类型：int
>
> 返回值：int
## Tag属性

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 参数：tag，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：width，类型：int
>
> 返回值：int
## ACTION_MOVE字段
>
> 返回值：int
## ACTION_DOWN字段
>
> 返回值：int
## ACTION_UP字段
>
> 返回值：int

# StringBuilder
完整类名：anywheresoftware.b4a.keywords.StringBuilderWrapper
> 所有者：process

> 包装器：java.lang.StringBuilder

?> 说明：StringBuilder是一个可变的字符串，与不可变的常规字符串不同。
```vbnet

Dim start As Long
start = DateTime.Now
'Regular string
Dim s As String
For i = 1 To 5000
	s = s & i
Next
Log(DateTime.Now - start)
'StringBuilder
start = DateTime.Now
Dim sb As StringBuilder
sb.Initialize
For i = 1 To 5000
	sb.Append(i)
Next
Log(DateTime.Now - start)
```

## Remove方法
**Remove(StartOffset,EndOffset)**

?> 说明：删除指定的字符。
>
> 参数：StartOffset，类型：int
>
> 参数：EndOffset，类型：int
>
> 返回值：anywheresoftware.b4a.keywords.StringBuilderWrapper
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Insert方法
**Insert(Offset,Text)**

?> 说明：以指定的偏移量插入指定的文本。
>
> 参数：Offset，类型：int
>
> 参数：Text，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.keywords.StringBuilderWrapper
## Initialize方法
**Initialize()**

?> 说明：初始化对象。
```vbnet

Dim sb As StringBuilder
sb.Initialize
sb.Append("The value is: ").Append(SomeOtherVariable).Append(CRLF)
```

>
> 返回值：void
## Append方法
**Append(Text)**

?> 说明：在末尾追加指定的文本。
```vbnet

sb.Append("First line").Append(CRLF).Append("Second line")
```

>
> 参数：Text，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.keywords.StringBuilderWrapper
## ToString方法
**ToString()**

?> 说明：将对象转换为字符串。
>
> 返回值：java.lang.String
## Length属性

?> 说明：返回字符数。
>
> 返回值：int

# 
完整类名：anywheresoftware.b4a.keywords.Regex
> 所有者：process

?> 说明：Regex是一个预定义的对象，包含正则表达式方法。
## Replace方法
**Replace(Pattern,Text,Template)**

?> 说明：根据指定的模式和模板替换文本中的所有匹配项。
```vbnet

Log(Regex.Replace("\d", "1 2 3 4", "-$0-")) '-1- -2- -3- -4-
```

>
> 参数：Pattern，类型：java.lang.String
>
> 参数：Text，类型：java.lang.String
>
> 参数：Template，类型：java.lang.String
>
> 返回值：java.lang.String
## IsMatch2方法
**IsMatch2(Pattern,Options,Text)**

?> 说明：测试给定的文本是否与给定的模式匹配。
>
> 参数：Pattern，类型：java.lang.String
>
> 参数：Options，类型：int
>
> 参数：Text，类型：java.lang.String
>
> 返回值：boolean
## IsMatch方法
**IsMatch(Pattern,Text)**

?> 说明：测试给定的文本是否与给定的模式匹配。
```vbnet

If Regex.IsMatch("\d\d\d", EditText1.Text) = False Then ...
```

>
> 参数：Pattern，类型：java.lang.String
>
> 参数：Text，类型：java.lang.String
>
> 返回值：boolean
## Matcher方法
**Matcher(Pattern,Text)**

?> 说明：返回Matcher对象，该对象可用于查找文本中给定模式的匹配项。
```vbnet

Dim text, pattern As String
text = "This is an interesting sentence with two numbers: 123456 and 7890."
pattern = "\d+" 'one or more digits
Dim Matcher1 As Matcher
Matcher1 = Regex.Matcher(pattern, text)
Do While Matcher1.Find
	Log("Found: " & Matcher1.Match)
Loop
```

>
> 参数：Pattern，类型：java.lang.String
>
> 参数：Text，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.keywords.Regex.MatcherWrapper
## Split2方法
**Split2(Pattern,Options,Text)**

?> 说明：与其他填充图案选项的“拆分”相同。
>
> 参数：Pattern，类型：java.lang.String
>
> 参数：Options，类型：int
>
> 参数：Text，类型：java.lang.String
>
> 返回值：java.lang.String[]
## Replace2方法
**Replace2(Pattern,Options,Text,Template)**

?> 说明：类似于替换。允许设置正则表达式选项。
>
> 参数：Pattern，类型：java.lang.String
>
> 参数：Options，类型：int
>
> 参数：Text，类型：java.lang.String
>
> 参数：Template，类型：java.lang.String
>
> 返回值：java.lang.String
## Split方法
**Split(Pattern,Text)**

?> 说明：将给定的文本拆分为与模式匹配的文本。
```vbnet

Dim components() As String
components = Regex.Split(",", "abc,def,,ghi") 'returns: "abc", "def", "", "ghi"
components = Regex.Split("\|", "abd|def||ghi") 'the pipe needs to be escaped as it has special meaning in Regex.
```

>
> 参数：Pattern，类型：java.lang.String
>
> 参数：Text，类型：java.lang.String
>
> 返回值：java.lang.String[]
## Matcher2方法
**Matcher2(Pattern,Options,Text)**

?> 说明：与Matcher相同，具有其他模式选项。
>
> 参数：Pattern，类型：java.lang.String
>
> 参数：Options，类型：int
>
> 参数：Text，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.keywords.Regex.MatcherWrapper
## CASE_INSENSITIVE字段

?> 说明：启用不区分大小写的匹配。
>
> 返回值：int
## MULTILINE字段

?> 说明：更改^和$以匹配每行的开始和结束，而不是整个字符串。
>
> 返回值：int

# Matcher
完整类名：anywheresoftware.b4a.keywords.Regex.MatcherWrapper
> 所有者：process

> 包装器：java.util.regex.Matcher

?> 说明：Matcher对象用于搜索字符串中的模式。
```vbnet
Regex.Matcher
```

## Group方法
**Group(Index)**

?> 说明：返回指定捕获组的值。
>
> 参数：Index，类型：int
>
> 返回值：java.lang.String
## Find方法
**Find()**

?> 说明：搜索与模式匹配的下一个子字符串。
```vbnet

Dim text, pattern As String
text = "This is an interesting sentence with two numbers: 123456 and 7890."
pattern = "\d+" 'one or more digits
Dim Matcher1 As Matcher
Matcher1 = Regex.Matcher(pattern, text)
Do While Matcher1.Find
	Log("Found: " & Matcher1.Match)
Loop
```

>
> 返回值：boolean
## GetEnd方法
**GetEnd(Index)**

?> 说明：返回指定捕获组的结束偏移量。
>
> 参数：Index，类型：int
>
> 返回值：int
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## GetStart方法
**GetStart(Index)**

?> 说明：返回指定捕获组的起始偏移量。
>
> 参数：Index，类型：int
>
> 返回值：int
## GroupCount属性

?> 说明：返回模式中捕获组的数目。
>
> 返回值：int
## Match属性

?> 说明：返回匹配的值。这与调用组（0）相同。
>
> 返回值：java.lang.String

# LayoutValues
完整类名：anywheresoftware.b4a.keywords.LayoutValues
> 所有者：process

?> 说明：保存与显示相关的值。
```vbnet
GetDeviceLayoutValues
```

## toString方法
**toString()**
>
> 返回值：java.lang.String
## ApproximateScreenSize属性

?> 说明：返回大致的屏幕大小。
>
> 返回值：double
## Scale字段

?> 说明：等于“每英寸点数”/160的设备刻度值。
>
> 返回值：float
## Height字段

?> 说明：显示高度（像素）。
>
> 返回值：int
## Width字段

?> 说明：显示宽度（像素）。
>
> 返回值：int

# 
完整类名：anywheresoftware.b4a.keywords.LayoutBuilder.LayoutValuesAndMap
> 所有者：process
## map字段
>
> 返回值：java.util.LinkedHashMap
## layoutValues字段
>
> 返回值：anywheresoftware.b4a.keywords.LayoutValues

# DesignerArgs
完整类名：anywheresoftware.b4a.keywords.DesignerArgs
> 所有者：process
## GetViewByName方法
**GetViewByName(Name)**

?> 说明：返回具有集合名称的视图。
>
> 参数：Name，类型：java.lang.String
>
> 返回值：android.view.View
## GetViewFromArgs方法
**GetViewFromArgs(Index)**

?> 说明：GetViewByName的缩写（Args（Index））。
>
> 参数：Index，类型：int
>
> 返回值：android.view.View
## ParentHeight属性

?> 说明：返回布局父级高度。
>
> 返回值：int
## ChosenVariant属性

?> 说明：返回所选变量的参数。
>
> 返回值：anywheresoftware.b4a.keywords.LayoutValues
## LayoutModule属性

?> 说明：返回对正在加载布局的模块的引用。可与CallSub一起使用。
>
> 返回值：java.lang.Object
## Views属性

?> 说明：返回包含布局视图的列表。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## Parent属性

?> 说明：返回布局父级。
>
> 返回值：android.view.View
## ViewsNames属性

?> 说明：返回包含视图名称的列表。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## Arguments属性

?> 说明：返回传递的参数。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## FirstRun属性

?> 说明：如果当前正在创建布局，则返回true。
>
> 返回值：boolean
## ParentWidth属性

?> 说明：返回布局父级宽度。
>
> 返回值：int
## DesignerProperties属性

?> 说明：返回低级别布局数据。
>
> 返回值：anywheresoftware.b4a.objects.collections.Map

# 
完整类名：anywheresoftware.b4a.keywords.DateTime
> 所有者：process

?> 说明：与日期和时间相关的方法。
```vbnet
DateTime.Date
```

> 事件：
>
> TimeChanged
## Add方法
**Add(Ticks,Years,Months,Days)**

?> 说明：返回一个刻度值，该值是将指定的时间跨度添加到给定刻度值的结果。
```vbnet

Dim Tomorrow As Long
Tomorrow = DateTime.Add(DateTime.Now, 0, 0, 1)
Log("Tomorrow date is: " & DateTime.Date(Tomorrow))
```

>
> 参数：Ticks，类型：long
>
> 参数：Years，类型：int
>
> 参数：Months，类型：int
>
> 参数：Days，类型：int
>
> 返回值：long
## GetHour方法
**GetHour(Ticks)**

?> 说明：从刻度值返回一天中的小时组件。
>
> 参数：Ticks，类型：long
>
> 返回值：int
## TimeParse方法
**TimeParse(Time)**

?> 说明：分析给定的时间字符串并返回其ticks表示形式。
>
> 参数：Time，类型：java.lang.String
>
> 返回值：long
## DateParse方法
**DateParse(Date)**

?> 说明：分析给定的日期字符串并返回其ticks表示形式。
```vbnet

Dim SomeTime As Long
SomeTime = DateTime.DateParse("02/23/2007")
```

>
> 参数：Date，类型：java.lang.String
>
> 返回值：long
## DateTimeParse方法
**DateTimeParse(Date,Time)**

?> 说明：分析给定的日期和时间字符串并返回ticks表示形式。
>
> 参数：Date，类型：java.lang.String
>
> 参数：Time，类型：java.lang.String
>
> 返回值：long
## GetMonth方法
**GetMonth(Ticks)**

?> 说明：从刻度值返回年中的月份组件。
>
> 参数：Ticks，类型：long
>
> 返回值：int
## Time方法
**Time(Ticks)**

?> 说明：返回时间的字符串表示形式（存储为刻度）。
```vbnet

Log("The time now is: " & DateTime.Time(DateTime.Now))
```

>
> 参数：Ticks，类型：long
>
> 返回值：java.lang.String
## Date方法
**Date(Ticks)**

?> 说明：返回日期的字符串表示形式（存储为刻度）。
```vbnet

Log("Today is: " & DateTime.Date(DateTime.Now))
```

>
> 参数：Ticks，类型：long
>
> 返回值：java.lang.String
## GetSecond方法
**GetSecond(Ticks)**

?> 说明：从刻度值返回一分钟内的秒数。
>
> 参数：Ticks，类型：long
>
> 返回值：int
## GetMinute方法
**GetMinute(Ticks)**

?> 说明：从刻度值返回小时内的分钟数。
>
> 参数：Ticks，类型：long
>
> 返回值：int
## GetTimeZoneOffsetAt方法
**GetTimeZoneOffsetAt(Date)**

?> 说明：返回指定日期从UTC开始以小时为单位测量的偏移量（偏移量可能会因夏令时设置而更改）。
>
> 参数：Date，类型：long
>
> 返回值：double
## GetYear方法
**GetYear(Ticks)**

?> 说明：从刻度值中返回年份成分。
>
> 参数：Ticks，类型：long
>
> 返回值：int
## GetDayOfYear方法
**GetDayOfYear(Ticks)**

?> 说明：从刻度值中返回一年中的某一天组件。
>
> 参数：Ticks，类型：long
>
> 返回值：int
## SetTimeZone方法
**SetTimeZone(OffsetHours)**

?> 说明：设置应用程序时区。此设置会影响日期到刻度值的转换，反之亦然（设备默认设置不会更改）。
>
> 参数：OffsetHours，类型：double
>
> 返回值：void
## GetDayOfMonth方法
**GetDayOfMonth(Ticks)**

?> 说明：从刻度值中返回月中的某一天组件。
>
> 参数：Ticks，类型：long
>
> 返回值：int
## GetDayOfWeek方法
**GetDayOfWeek(Ticks)**

?> 说明：从刻度值返回星期几组件。
>
> 参数：Ticks，类型：long
>
> 返回值：int
## ListenToExternalTimeChanges方法
**ListenToExternalTimeChanges(ba)**

?> 说明：创建一个动态广播接收器，用于侦听“时区更改”事件和“时间设置”事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## TimeFormat属性

?> 说明：获取或设置用于分析时间字符串的格式。
>
> 参数：Pattern，类型：java.lang.String
>
> 返回值：java.lang.String
## DeviceDefaultTimeFormat属性

?> 说明：返回基于设备所选语言的默认时间格式。
>
> 返回值：java.lang.String
## Now属性

?> 说明：以刻度形式获取当前时间（自1970年1月1日以来的毫秒数）。
>
> 返回值：long
## DateFormat属性

?> 说明：获取或设置用于分析日期字符串的格式。
>
> 参数：Pattern，类型：java.lang.String
>
> 返回值：java.lang.String
## DeviceDefaultDateFormat属性

?> 说明：返回基于设备所选语言的默认日期格式。
>
> 返回值：java.lang.String
## TimeZoneOffset属性

?> 说明：返回从UTC开始以小时为单位测量的当前偏移量。
>
> 返回值：double
## TicksPerSecond字段
>
> 返回值：long
## TicksPerMinute字段
>
> 返回值：long
## TicksPerDay字段
>
> 返回值：long
## TicksPerHour字段
>
> 返回值：long

# 
完整类名：anywheresoftware.b4a.keywords.Common
> 所有者：activity
## PerYToCurrent方法
**PerYToCurrent(Percentage,ba)**

?> 说明：返回给定百分比的活动高度的实际大小。
>
> 参数：Percentage，类型：float
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：int
## CallSubDelayed3方法
**CallSubDelayed3(mine,Component,Sub,Argument1,Argument2)**

?> 说明：类似于CallSubDelayed。调用具有两个参数的sub。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Component，类型：java.lang.Object
>
> 参数：Sub，类型：java.lang.String
>
> 参数：Argument1，类型：java.lang.Object
>
> 参数：Argument2，类型：java.lang.Object
>
> 返回值：void
## RndSeed方法
**RndSeed(Seed)**

?> 说明：设置随机种子值。
>
> 参数：Seed，类型：long
>
> 返回值：void
## CallSubDelayed2方法
**CallSubDelayed2(mine,Component,Sub,Argument)**

?> 说明：类似于CallSubDelayed。使用单个参数调用子。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Component，类型：java.lang.Object
>
> 参数：Sub，类型：java.lang.String
>
> 参数：Argument，类型：java.lang.Object
>
> 返回值：void
## GetDeviceLayoutValues方法
**GetDeviceLayoutValues(ba)**

?> 说明：返回设备布局值。
```vbnet

Log(GetDeviceLayoutValues)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4a.keywords.LayoutValues
## CallSubNew方法
**CallSubNew(mine,Component,Sub)**

?> 说明：调用给定的子。CallSub可用于调用属于不同模块的子。
```vbnet

CallSub(Main, "RefreshData")
```

>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Component，类型：java.lang.Object
>
> 参数：Sub，类型：java.lang.String
>
> 返回值：java.lang.Object
## StartActivity方法
**StartActivity(mine,Activity)**

?> 说明：启动一个活动或将其置于最前面（如果该活动已存在）。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Activity，类型：java.lang.Object
>
> 返回值：void
## InputListAsync方法
**InputListAsync(Items,Title,CheckedItem,mine,Cancelable)**

?> 说明：显示包含项目列表和单选按钮的非模式对话框。按下某个项目将关闭对话框。
```vbnet

Dim options As List = Array("Red", "Green", "Blue")
InputListAsync(options, "Select Color", 0, False)
Wait For InputList_Result (Index As Int)
If Index <> DialogResponse.CANCEL Then
	Log("Selected color: " & options.Get(Index))
End If
```

>
> 参数：Items，类型：anywheresoftware.b4a.objects.collections.List
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：CheckedItem，类型：int
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Cancelable，类型：boolean
>
> 返回值：java.lang.Object
## StartService方法
**StartService(mine,Service)**

?> 说明：启动给定的服务。如果以前未启动该服务，则将首先创建该服务。
```vbnet

StartService(SQLService)
```

>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Service，类型：java.lang.Object
>
> 返回值：void
## CallSubNew3方法
**CallSubNew3(mine,Component,Sub,Argument1,Argument2)**

?> 说明：类似于CallSub。调用具有两个参数的sub。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Component，类型：java.lang.Object
>
> 参数：Sub，类型：java.lang.String
>
> 参数：Argument1，类型：java.lang.Object
>
> 参数：Argument2，类型：java.lang.Object
>
> 返回值：java.lang.Object
## ATanD方法
**ATanD(Value)**

?> 说明：返回以度为单位测量的角度。
>
> 参数：Value，类型：double
>
> 返回值：double
## CallSubNew2方法
**CallSubNew2(mine,Component,Sub,Argument)**

?> 说明：类似于CallSub。使用单个参数调用子。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Component，类型：java.lang.Object
>
> 参数：Sub，类型：java.lang.String
>
> 参数：Argument，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Exit方法
**Exit()**

?> 说明：退出最内部的循环。
>
> 返回值：void
## Msgbox方法
**Msgbox(Message,Title,ba)**

?> 说明：显示具有指定消息和标题的模式消息框。
>
> 参数：Message，类型：java.lang.CharSequence
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Msgbox2Async方法
**Msgbox2Async(Message,Title,Positive,Cancel,Negative,Icon,mine,Cancelable)**

?> 说明：显示具有指定消息和标题的非模态消息框。结果将引发Msgbox_Result事件。
```vbnet

Msgbox2Async("Question?", "Title", "Yes", "Cancel", "No", Null, False)
Wait For Msgbox_Result (Result As Int)
If Result = DialogResponse.POSITIVE Then
	'...
End If
```

>
> 参数：Message，类型：java.lang.CharSequence
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Positive，类型：java.lang.String
>
> 参数：Cancel，类型：java.lang.String
>
> 参数：Negative，类型：java.lang.String
>
> 参数：Icon，类型：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Cancelable，类型：boolean
>
> 返回值：java.lang.Object
## Sub方法
**Sub()**

?> 说明：使用参数和返回类型声明子。
```vbnet

Sub MySub (FirstName As String, LastName As String, Age As Int, OtherValues() As Double) As Boolean
 ...
End Sub
```

>
> 返回值：void
## Log方法
**Log(Message)**

?> 说明：记录一条消息。可以在日志选项卡中查看日志。
>
> 参数：Message，类型：java.lang.String
>
> 返回值：void
## ProgressDialogHide方法
**ProgressDialogHide()**

?> 说明：隐藏可见的进度对话框。如果没有可见的进度对话框，则不执行任何操作。
>
> 返回值：void
## ATan2方法
**ATan2(Y,X)**

?> 说明：返回以弧度测量的角度。
>
> 参数：Y，类型：double
>
> 参数：X，类型：double
>
> 返回值：double
## CallSubDelayed方法
**CallSubDelayed(mine,Component,Sub)**

?> 说明：CallSubDelayed是StartActivity、StartService和CallSub的组合。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Component，类型：java.lang.Object
>
> 参数：Sub，类型：java.lang.String
>
> 返回值：void
## StopService方法
**StopService(mine,Service)**

?> 说明：停止给定的服务。将调用Service_Destory。之后调用StartService将首先创建服务。
```vbnet

StopService(SQLService)
```

>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Service，类型：java.lang.Object
>
> 返回值：void
## StartReceiverAt方法
**StartReceiverAt(mine,Receiver,Time,DuringSleep)**

?> 说明：安排给定的接收器在给定的时间启动。不适用于新版本的Android中的服务。
```vbnet

StartReceiverAt(Receiver1, DateTime.Now + 30 * 1000, false) 'will start after 30 seconds.
```

>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Receiver，类型：java.lang.Object
>
> 参数：Time，类型：long
>
> 参数：DuringSleep，类型：boolean
>
> 返回值：void
## GetType方法
**GetType(object)**

?> 说明：返回表示对象的java类型的字符串。
>
> 参数：object，类型：java.lang.Object
>
> 返回值：java.lang.String
## Sender方法
**Sender(ba)**

?> 说明：返回引发事件的对象。
```vbnet

Sub Button_Click
 Dim b As B4XView = Sender
 b.Text = "I've been clicked"
End Sub
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：java.lang.Object
## StartServiceAt方法
**StartServiceAt(mine,Receiver,Time,DuringSleep)**

?> 说明：请改用StartReceiverAt。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Receiver，类型：java.lang.Object
>
> 参数：Time，类型：long
>
> 参数：DuringSleep，类型：boolean
>
> 返回值：void
## Min方法
**Min(Number1,Number2)**

?> 说明：返回两个数字之间的较小数字。
>
> 参数：Number1，类型：double
>
> 参数：Number2，类型：double
>
> 返回值：double
## MsgboxAsync方法
**MsgboxAsync(Message,Title,mine)**

?> 说明：显示具有指定消息和标题的非模态消息框。
```vbnet

MsgboxAsync("Hello world", "This is the title")
```

>
> 参数：Message，类型：java.lang.CharSequence
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Ceil方法
**Ceil(Number)**

?> 说明：返回大于或等于指定数字且等于整数的最小双精度。
>
> 参数：Number，类型：double
>
> 返回值：double
## LoadBitmapSample方法
**LoadBitmapSample(Dir,FileName,MaxWidth,MaxHeight)**

?> 说明：加载位图。
```vbnet

Activity.SetBackgroundImage(LoadBitmapSample(File.DirAssets, "SomeFile.jpg", Activity.Width, Activity.Height))
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：MaxWidth，类型：int
>
> 参数：MaxHeight，类型：int
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## If方法
**If()**

?> 说明：单线：
>
> 返回值：void
## InputList方法
**InputList(Items,Title,CheckedItem,ba)**

?> 说明：显示带有项目列表和单选按钮的模式对话框。按下某个项目将关闭对话框。
>
> 参数：Items，类型：anywheresoftware.b4a.objects.collections.List
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：CheckedItem，类型：int
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：int
## Max方法
**Max(Number1,Number2)**

?> 说明：返回两个数字之间较大的数字。
>
> 参数：Number1，类型：double
>
> 参数：Number2，类型：double
>
> 返回值：double
## Catch方法
**Catch()**

?> 说明：在try块内抛出的任何异常都将在catch块中被捕获。
>
> 返回值：void
## IIf方法
**IIf(Condition,TrueValue,FalseValue)**

?> 说明：Inline If-如果Condition为True则返回TrueValue，否则返回False。只计算相关表达式。
>
> 参数：Condition，类型：boolean
>
> 参数：TrueValue，类型：java.lang.Object
>
> 参数：FalseValue，类型：java.lang.Object
>
> 返回值：java.lang.Object
## ATan2D方法
**ATan2D(Y,X)**

?> 说明：返回以度为单位测量的角度。
>
> 参数：Y，类型：double
>
> 参数：X，类型：double
>
> 返回值：double
## Is方法
**Is()**

?> 说明：测试对象是否属于给定类型。
```vbnet

For i = 0 To Activity.NumberOfViews - 1
  If Activity.GetView(i) Is Button Then
   Dim b As Button
   b = Activity.GetView(i)
   b.Color = Colors.Blue
  End If
Next
```

>
> 返回值：void
## Asc方法
**Asc(Char)**

?> 说明：返回给定字符或字符串中第一个字符的unicode代码点。
>
> 参数：Char，类型：char
>
> 返回值：int
## Abs方法
**Abs(Number)**

?> 说明：返回绝对值。
>
> 参数：Number，类型：double
>
> 返回值：double
## IsNumber方法
**IsNumber(Text)**

?> 说明：测试指定的字符串是否可以安全地解析为数字。
>
> 参数：Text，类型：java.lang.String
>
> 返回值：boolean
## ExitApplication方法
**ExitApplication()**

?> 说明：立即结束应用程序并停止进程。
>
> 返回值：void
## PerXToCurrent方法
**PerXToCurrent(Percentage,ba)**

?> 说明：返回给定百分比的活动宽度的实际大小。
>
> 参数：Percentage，类型：float
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：int
## SubExists方法
**SubExists(mine,Object,Sub)**

?> 说明：测试对象是否包括指定的方法。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Object，类型：java.lang.Object
>
> 参数：Sub，类型：java.lang.String
>
> 返回值：boolean
## InputMultiList方法
**InputMultiList(Items,Title,ba)**

?> 说明：显示带有项目列表和复选框的模式对话框。用户可以选择多个项目。
>
> 参数：Items，类型：anywheresoftware.b4a.objects.collections.List
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## Cos方法
**Cos(Radians)**

?> 说明：计算三角余弦函数。以弧度为单位测量的角度。
>
> 参数：Radians，类型：double
>
> 返回值：double
## Sqrt方法
**Sqrt(Value)**

?> 说明：返回正平方根。
>
> 参数：Value，类型：double
>
> 返回值：double
## Dim方法
**Dim()**

?> 说明：声明一个变量。
```vbnet
Dim a = 1, b = 2, c = 3 As Int
```

>
> 返回值：void
## ProgressDialogShow2方法
**ProgressDialogShow2(ba,Text,Cancelable)**

?> 说明：显示一个带有圆形旋转条和指定文本的对话框。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Text，类型：java.lang.CharSequence
>
> 参数：Cancelable，类型：boolean
>
> 返回值：void
## IsDevTool方法
**IsDevTool(ToolName)**

?> 说明：如果ToolName等于B4A，则返回true。
>
> 参数：ToolName，类型：java.lang.String
>
> 返回值：boolean
## Type方法
**Type()**

?> 说明：声明一个结构。
```vbnet

Type MyType (Name As String, Items(10) As Int)
Dim a, b As MyType
a.Initialize
a.Items(2) = 123
```

>
> 返回值：void
## Sleep方法
**Sleep(Milliseconds)**

?> 说明：暂停当前子执行，并在指定时间后继续执行。
>
> 参数：Milliseconds，类型：int
>
> 返回值：void
## InputMapAsync方法
**InputMapAsync(Items,Title,mine,Cancelable)**

?> 说明：显示一个包含项目列表和复选框的非模式对话框。用户可以选择多个项目。
```vbnet

Dim m As Map = CreateMap("Item #1": True, "Item #2": True, "Item #3": False)
InputMapAsync(m, "Select items", True)
Wait For InputMap_Result
Log(m)
```

>
> 参数：Items，类型：anywheresoftware.b4a.objects.collections.Map
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Cancelable，类型：boolean
>
> 返回值：java.lang.Object
## Select方法
**Select()**

?> 说明：将单个值与多个值进行比较。
```vbnet

Dim value As Int
value = 7
Select value
	Case 1
		Log("One")
	Case 2, 4, 6, 8
		Log("Even")
	Case 3, 5, 7, 9
		Log("Odd larger than one")
	Case Else
		Log("Larger than 9")
End Select
```

>
> 返回值：void
## Power方法
**Power(Base,Exponent)**

?> 说明：返回提升到Exponent幂的基数。
>
> 参数：Base，类型：double
>
> 参数：Exponent，类型：double
>
> 返回值：double
## Tan方法
**Tan(Radians)**

?> 说明：计算三角正切函数。以弧度为单位测量的角度。
>
> 参数：Radians，类型：double
>
> 返回值：double
## LoadBitmapResize方法
**LoadBitmapResize(Dir,FileName,Width,Height,KeepAspectRatio)**

?> 说明：加载位图并设置其大小。
```vbnet

Dim bd As BitmapDrawable = Activity.SetBackgroundImage(LoadBitmapResize(File.DirAssets, "SomeFile.jpg", 100%x, 100%y, True))
bd.Gravity = Gravity.CENTER
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 参数：KeepAspectRatio，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## Rnd方法
**Rnd(Min,Max)**

?> 说明：返回一个介于最小值（包括最小值）和最大值（不包括最大值）之间的随机整数。
>
> 参数：Min，类型：int
>
> 参数：Max，类型：int
>
> 返回值：int
## Chr方法
**Chr(UnicodeValue)**

?> 说明：返回由给定的unicode值表示的字符。
>
> 参数：UnicodeValue，类型：int
>
> 返回值：char
## LoadBitmap方法
**LoadBitmap(Dir,FileName)**

?> 说明：加载位图。
```vbnet

Activity.SetBackgroundImage(LoadBitmap(File.DirAssets, "SomeFile.jpg"))
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## ProgressDialogShow方法
**ProgressDialogShow(ba,Text)**

?> 说明：显示一个带有圆形旋转条和指定文本的对话框。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：void
## ACos方法
**ACos(Value)**

?> 说明：返回以弧度测量的角度。
>
> 参数：Value，类型：double
>
> 返回值：double
## Try方法
**Try()**

?> 说明：在try块内抛出的任何异常都将在catch块中被捕获。
>
> 返回值：void
## CosD方法
**CosD(Degrees)**

?> 说明：计算三角余弦函数。以度为单位测量的角度。
>
> 参数：Degrees，类型：double
>
> 返回值：double
## For方法
**For()**

?> 说明：语法：
```vbnet

For i = 1 To 10
 Log(i) 'Will print 1 to 10 (inclusive).
Next
For Each n As Int In Numbers 'an array
 Sum = Sum + n
Next

```

>
> 返回值：void
## SinD方法
**SinD(Degrees)**

?> 说明：计算三角正弦函数。以度为单位测量的角度。
>
> 参数：Degrees，类型：double
>
> 返回值：double
## IsPaused方法
**IsPaused(mine,Component)**

?> 说明：测试给定组件是否已暂停。对于尚未启动的组件，也将返回true。
```vbnet

If IsPaused(Main) = False Then CallSub(Main, "RefreshData")
```

>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Component，类型：java.lang.Object
>
> 返回值：boolean
## StartReceiver方法
**StartReceiver(mine,Receiver)**

?> 说明：启动给定的接收器。这将导致Receiver_Receive运行。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Receiver，类型：java.lang.Object
>
> 返回值：void
## Not方法
**Not(Value)**

?> 说明：反转给定布尔值的值。
>
> 参数：Value，类型：boolean
>
> 返回值：boolean
## DoEvents方法
**DoEvents()**

?> 说明：<b>不赞成使用DoEvents</b> 它可能导致稳定问题。
>
> 返回值：void
## ConfigureHomeWidget方法
**ConfigureHomeWidget(LayoutFile,EventName,UpdateIntervalMinutes,WidgetName,CenterWidget)**

?> 说明：基于布局文件创建RemoteViews对象。编译器将根据参数生成所需的XML文件。
>
> 参数：LayoutFile，类型：java.lang.String
>
> 参数：EventName，类型：java.lang.String
>
> 参数：UpdateIntervalMinutes，类型：int
>
> 参数：WidgetName，类型：java.lang.String
>
> 参数：CenterWidget，类型：boolean
>
> 返回值：android.widget.RemoteViews
## Me方法
**Me(ba)**

?> 说明：对于类：返回对当前实例的引用。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：java.lang.Object
## Sin方法
**Sin(Radians)**

?> 说明：计算三角正弦函数。以弧度为单位测量的角度。
>
> 参数：Radians，类型：double
>
> 返回值：double
## InputMap方法
**InputMap(Items,Title,ba)**

?> 说明：显示带有项目列表和复选框的模式对话框。用户可以选择多个项目。
>
> 参数：Items，类型：anywheresoftware.b4a.objects.collections.Map
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## CreateMap方法
**CreateMap()**

?> 说明：使用给定的键/值对创建映射。
```vbnet

Dim m As Map = CreateMap("January": 1, "February": 2)
```

>
> 返回值：void
## ATan方法
**ATan(Value)**

?> 说明：返回以弧度测量的角度。
>
> 参数：Value，类型：double
>
> 返回值：double
## LastException方法
**LastException(ba)**

?> 说明：返回捕获的最后一个异常（如果存在）。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4a.objects.B4AException
## TanD方法
**TanD(Degrees)**

?> 说明：计算三角正切函数。以度为单位测量的角度。
>
> 参数：Degrees，类型：double
>
> 返回值：double
## Round2方法
**Round2(Number,DecimalPlaces)**

?> 说明：对给定的数字进行四舍五入，并保留指定的小数位数。
>
> 参数：Number，类型：double
>
> 参数：DecimalPlaces，类型：int
>
> 返回值：double
## NumberFormat2方法
**NumberFormat2(Number,MinimumIntegers,MaximumFractions,MinimumFractions,GroupingUsed)**

?> 说明：将指定的数字转换为字符串。
```vbnet

Log(NumberFormat2(12345.67, 0, 3, 3, false)) '"12345.670"
```

>
> 参数：Number，类型：double
>
> 参数：MinimumIntegers，类型：int
>
> 参数：MaximumFractions，类型：int
>
> 参数：MinimumFractions，类型：int
>
> 参数：GroupingUsed，类型：boolean
>
> 返回值：java.lang.String
## ASin方法
**ASin(Value)**

?> 说明：返回以弧度测量的角度。
>
> 参数：Value，类型：double
>
> 返回值：double
## CharsToString方法
**CharsToString(Chars,StartOffset,Length)**

?> 说明：通过从数组中复制字符来创建新的字符串。
>
> 参数：Chars，类型：char[]
>
> 参数：StartOffset，类型：int
>
> 参数：Length，类型：int
>
> 返回值：java.lang.String
## ACosD方法
**ACosD(Value)**

?> 说明：返回以度为单位测量的角度。
>
> 参数：Value，类型：double
>
> 返回值：double
## DipToCurrent方法
**DipToCurrent(Length)**

?> 说明：缩放该值，该值表示默认密度设备上的特定长度（密度=1.0），
>
> 参数：Length，类型：int
>
> 返回值：int
## LogColor方法
**LogColor(Message,Color)**

?> 说明：记录一条消息。该消息将以指定的颜色显示在IDE中。
>
> 参数：Message，类型：java.lang.String
>
> 参数：Color，类型：int
>
> 返回值：void
## Continue方法
**Continue()**

?> 说明：停止执行当前迭代并继续执行下一个迭代。
>
> 返回值：void
## SmartStringFormatter方法
**SmartStringFormatter(Format,Value)**

?> 说明：智能字符串文字使用的内部关键字。
>
> 参数：Format，类型：java.lang.String
>
> 参数：Value，类型：java.lang.Object
>
> 返回值：java.lang.String
## Logarithm方法
**Logarithm(Number,Base)**
>
> 参数：Number，类型：double
>
> 参数：Base，类型：double
>
> 返回值：double
## Round方法
**Round(Number)**

?> 说明：返回与给定数字最接近的长数字。
>
> 参数：Number，类型：double
>
> 返回值：long
## ToastMessageShow方法
**ToastMessageShow(Message,LongDuration)**

?> 说明：显示自动发出的快速小消息。
>
> 参数：Message，类型：java.lang.CharSequence
>
> 参数：LongDuration，类型：boolean
>
> 返回值：void
## BytesToString方法
**BytesToString(Data,StartOffset,Length,CharSet)**

?> 说明：将给定的字节数组解码为字符串。
```vbnet

Dim s As String
s = BytesToString(Buffer, 0, Buffer.Length, "UTF-8")
```

>
> 参数：Data，类型：byte[]
>
> 参数：StartOffset，类型：int
>
> 参数：Length，类型：int
>
> 参数：CharSet，类型：java.lang.String
>
> 返回值：java.lang.String
## Until方法
**Until()**

?> 说明：循环直到条件为true。
>
> 返回值：void
## CancelScheduledService方法
**CancelScheduledService(mine,Service)**

?> 说明：取消此服务以前计划的任务。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Service，类型：java.lang.Object
>
> 返回值：void
## Floor方法
**Floor(Number)**

?> 说明：返回小于或等于指定数字且等于整数的最大双精度。
>
> 参数：Number，类型：double
>
> 返回值：double
## Return方法
**Return()**

?> 说明：从当前子中返回，并可选择返回给定值。
>
> 返回值：void
## While方法
**While()**

?> 说明：条件为true时循环。
>
> 返回值：void
## Array方法
**Array()**

?> 说明：创建指定类型的一维数组。
```vbnet

Dim Days() As String
Days = Array As String("Sunday", "Monday", ...)
```

>
> 返回值：void
## IsBackgroundTaskRunning方法
**IsBackgroundTaskRunning(ba,ContainerObject,TaskId)**

?> 说明：测试由容器对象提交并具有指定id的后台任务是否正在运行。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ContainerObject，类型：java.lang.Object
>
> 参数：TaskId，类型：int
>
> 返回值：boolean
## ASinD方法
**ASinD(Value)**

?> 说明：返回以度为单位测量的角度。
>
> 参数：Value，类型：double
>
> 返回值：double
## StartServiceAtExact方法
**StartServiceAtExact(mine,Receiver,Time,DuringSleep)**

?> 说明：类似于StartServiceAt。
>
> 参数：mine，类型：anywheresoftware.b4a.BA
>
> 参数：Receiver，类型：java.lang.Object
>
> 参数：Time，类型：long
>
> 参数：DuringSleep，类型：boolean
>
> 返回值：void
## Msgbox2方法
**Msgbox2(Message,Title,Positive,Cancel,Negative,Icon,ba)**

?> 说明：显示具有指定消息和标题的模式消息框。
```vbnet

Dim result As Int
result = Msgbox2("This is the message", "This is the title", "Good", "", "Bad", LoadBitmap(File.DirAssets, "smiley.gif"))
If result = DialogResponse.Positive Then ...

```

>
> 参数：Message，类型：java.lang.CharSequence
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Positive，类型：java.lang.String
>
> 参数：Cancel，类型：java.lang.String
>
> 参数：Negative，类型：java.lang.String
>
> 参数：Icon，类型：android.graphics.Bitmap
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：int
## NumberFormat方法
**NumberFormat(Number,MinimumIntegers,MaximumFractions)**

?> 说明：将指定的数字转换为字符串。
```vbnet

Log(NumberFormat(12345.6789, 0, 2)) '"12,345.68"
Log(NumberFormat(1, 3 ,0)) '"001"
```

>
> 参数：Number，类型：double
>
> 参数：MinimumIntegers，类型：int
>
> 参数：MaximumFractions，类型：int
>
> 返回值：java.lang.String
## QUOTE字段

?> 说明：引号字符。Chr（34）的值。
>
> 返回值：java.lang.String
## Null字段
>
> 返回值：java.lang.Object
## cE字段

?> 说明：e（自然对数底）常数。
>
> 返回值：double
## Typeface字段

?> 说明：与字体相关的方法。
>
> 返回值：anywheresoftware.b4a.keywords.constants.TypefaceWrapper
## True字段
>
> 返回值：boolean
## False字段
>
> 返回值：boolean
## KeyCodes字段

?> 说明：密钥编码常量。
>
> 返回值：anywheresoftware.b4a.keywords.constants.KeyCodes
## Bit字段

?> 说明：比特相关方法。
>
> 返回值：anywheresoftware.b4a.keywords.Bit
## Density字段

?> 说明：返回设备比例，即DPI/160。
>
> 返回值：float
## DialogResponse字段

?> 说明：对话框相关常量。
>
> 返回值：anywheresoftware.b4a.keywords.constants.DialogResponse
## DateTime字段

?> 说明：与日期和时间相关的方法。
>
> 返回值：anywheresoftware.b4a.keywords.DateTime
## Colors字段

?> 说明：与颜色相关的方法和常量。
>
> 返回值：anywheresoftware.b4a.keywords.constants.Colors
## TAB字段

?> 说明：制表符。
>
> 返回值：java.lang.String
## Regex字段

?> 说明：与正则表达式相关的方法。
>
> 返回值：anywheresoftware.b4a.keywords.Regex
## CRLF字段

?> 说明：换行符。Chr（10）的值。
>
> 返回值：java.lang.String
## cPI字段

?> 说明：PI常数。
>
> 返回值：double
## File字段

?> 说明：文件相关方法。
>
> 返回值：anywheresoftware.b4a.objects.streams.File
## Application字段

?> 说明：与应用程序相关的属性。
>
> 返回值：anywheresoftware.b4a.keywords.B4AApplication
## Gravity字段

?> 说明：重力常数。
>
> 返回值：anywheresoftware.b4a.keywords.constants.Gravity

# ResumableSub
完整类名：anywheresoftware.b4a.keywords.Common.ResumableSubWrapper
> 所有者：process

> 包装器：anywheresoftware.b4a.BA.ResumableSub

?> 说明：此对象是从对非无效可恢复子对象的调用返回的。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Completed属性

?> 说明：测试可恢复潜艇是否已经完成。
>
> 返回值：boolean

# 
完整类名：anywheresoftware.b4a.keywords.Bit
> 所有者：process

?> 说明：Bit是一个预定义的对象，包含按位相关的方法。
```vbnet

Dim flags As Int
flags = Bit.Or(100, 200)
```

## ShiftRight方法
**ShiftRight(N,Shift)**

?> 说明：向右移动N。
>
> 参数：N，类型：int
>
> 参数：Shift，类型：int
>
> 返回值：int
## Or方法
**Or(N1,N2)**

?> 说明：返回两个值的按位“或”。
>
> 参数：N1，类型：int
>
> 参数：N2，类型：int
>
> 返回值：int
## ShiftLeft方法
**ShiftLeft(N,Shift)**

?> 说明：向左移动N。
>
> 参数：N，类型：int
>
> 参数：Shift，类型：int
>
> 返回值：int
## ParseLong方法
**ParseLong(Value,Radix)**

?> 说明：使用指定的基数将值解析为长。
>
> 参数：Value，类型：java.lang.String
>
> 参数：Radix，类型：int
>
> 返回值：long
## OrLong方法
**OrLong(N1,N2)**

?> 说明：返回两个值的按位“或”。
>
> 参数：N1，类型：long
>
> 参数：N2，类型：long
>
> 返回值：long
## UnsignedShiftRight方法
**UnsignedShiftRight(N,Shift)**

?> 说明：向右移动N。
>
> 参数：N，类型：int
>
> 参数：Shift，类型：int
>
> 返回值：int
## XorLong方法
**XorLong(N1,N2)**

?> 说明：返回两个值的逐位异或。
>
> 参数：N1，类型：long
>
> 参数：N2，类型：long
>
> 返回值：long
## ToOctalString方法
**ToOctalString(N)**

?> 说明：返回以8为底的N的字符串表示形式。
>
> 参数：N，类型：int
>
> 返回值：java.lang.String
## ToHexString方法
**ToHexString(N)**

?> 说明：返回以16为底的N的字符串表示形式。
>
> 参数：N，类型：int
>
> 返回值：java.lang.String
## Not方法
**Not(N)**

?> 说明：返回给定值的按位补码。
>
> 参数：N，类型：int
>
> 返回值：int
## ToBinaryString方法
**ToBinaryString(N)**

?> 说明：返回以2为底的N的字符串表示形式。
>
> 参数：N，类型：int
>
> 返回值：java.lang.String
## ToHexStringLong方法
**ToHexStringLong(N)**

?> 说明：返回以16为底的N的字符串表示形式。
>
> 参数：N，类型：long
>
> 返回值：java.lang.String
## ArrayCopy方法
**ArrayCopy(SrcArray,SrcOffset,DestArray,DestOffset,Count)**

?> 说明：将元素从SrcArray复制到DestArray。
>
> 参数：SrcArray，类型：java.lang.Object
>
> 参数：SrcOffset，类型：int
>
> 参数：DestArray，类型：java.lang.Object
>
> 参数：DestOffset，类型：int
>
> 参数：Count，类型：int
>
> 返回值：void
## And方法
**And(N1,N2)**

?> 说明：返回这两个值的按位“与”。
>
> 参数：N1，类型：int
>
> 参数：N2，类型：int
>
> 返回值：int
## ShiftRightLong方法
**ShiftRightLong(N,Shift)**

?> 说明：向右移动N。
>
> 参数：N，类型：long
>
> 参数：Shift，类型：int
>
> 返回值：long
## NotLong方法
**NotLong(N)**

?> 说明：返回给定值的按位补码。
>
> 参数：N，类型：long
>
> 返回值：long
## ShiftLeftLong方法
**ShiftLeftLong(N,Shift)**

?> 说明：向左移动N。
>
> 参数：N，类型：long
>
> 参数：Shift，类型：int
>
> 返回值：long
## Xor方法
**Xor(N1,N2)**

?> 说明：返回两个值的逐位异或。
>
> 参数：N1，类型：int
>
> 参数：N2，类型：int
>
> 返回值：int
## ParseInt方法
**ParseInt(Value,Radix)**

?> 说明：使用指定的基数将值解析为整数。
>
> 参数：Value，类型：java.lang.String
>
> 参数：Radix，类型：int
>
> 返回值：int
## AndLong方法
**AndLong(N1,N2)**

?> 说明：返回这两个值的按位“与”。
>
> 参数：N1，类型：long
>
> 参数：N2，类型：long
>
> 返回值：long
## UnsignedShiftRightLong方法
**UnsignedShiftRightLong(N,Shift)**

?> 说明：向右移动N。
>
> 参数：N，类型：long
>
> 参数：Shift，类型：int
>
> 返回值：long
## InputStreamToBytes方法
**InputStreamToBytes(In)**

?> 说明：从输入流中读取数据并将其写入字节数组。
>
> 参数：In，类型：java.io.InputStream
>
> 返回值：byte[]

# 
完整类名：anywheresoftware.b4a.keywords.B4AApplication
> 所有者：process
## VersionCode属性

?> 说明：返回应用程序版本代码（VersionCode属性）。
>
> 返回值：int
## PackageName属性

?> 说明：返回应用程序包名称。
>
> 返回值：java.lang.String
## LabelName属性

?> 说明：返回应用程序名称（ApplicationLabel属性）。
>
> 返回值：java.lang.String
## VersionName属性

?> 说明：返回应用程序版本名称（VersionName属性）。
>
> 返回值：java.lang.String
## Icon属性

?> 说明：返回应用程序图标。
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper

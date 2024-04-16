# rESP8266FileSystem

版本:1.11
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rESP8266FileSystem)

# File
完整类名：B4R::B4RFile
## Size属性

?> 说明：返回文件大小（字节数）。
>
> 返回值：ULong
## Name属性

?> 说明：返回文件名。
>
> 返回值：B4R::B4RString*

# ESP8266FileSystem
完整类名：B4R::B4RFileSystem
## Initialize方法
**Initialize()**

?> 说明：初始化文件系统。如果成功，则返回True。
>
> 返回值：bool
## Format方法
**Format()**

?> 说明：格式化文件系统。请注意，这可能需要一分钟以上的时间才能完成。
>
> 返回值：bool
## OpenRead方法
**OpenRead(FileName)**

?> 说明：以只读模式打开文件。如果文件已成功打开，则返回true。
>
> 参数：FileName，类型：B4R::B4RString*
>
> 返回值：bool
## OpenReadWrite方法
**OpenReadWrite(FileName)**

?> 说明：以读写模式打开文件。如果文件已成功打开，则返回true。
>
> 参数：FileName，类型：B4R::B4RString*
>
> 返回值：bool
## Close方法
**Close()**

?> 说明：关闭当前打开的文件。
>
> 返回值：B4R::void
## Exists方法
**Exists(FileName)**

?> 说明：检查给定的文件或目录是否存在。
>
> 参数：FileName，类型：B4R::B4RString*
>
> 返回值：bool
## Remove方法
**Remove(FileName)**

?> 说明：删除给定的文件。如果文件已成功删除，则返回true。
>
> 参数：FileName，类型：B4R::B4RString*
>
> 返回值：bool
## ListFiles方法
**ListFiles(DirName)**

?> 说明：可以在For Each循环中使用，以迭代文件夹中的文件。
```vbnet

For Each f As File In fs.ListFiles("/")
	Log("Name: ", f.Name, ", Size: ", f.Size)
Next
```

>
> 参数：DirName，类型：B4R::B4RString*
>
> 返回值：B4R::FileIterator*
## CurrentFile属性

?> 说明：返回当前打开的文件。
>
> 返回值：B4R::B4RFile*
## Stream属性

?> 说明：返回当前打开文件的流。
>
> 返回值：B4R::B4RStream*
## Position属性

?> 说明：获取或设置当前打开文件中的位置。
>
> 参数：p，类型：ULong
>
> 返回值：ULong
## TotalSize属性
>
> 返回值：ULong
## UsedSize属性
>
> 返回值：ULong

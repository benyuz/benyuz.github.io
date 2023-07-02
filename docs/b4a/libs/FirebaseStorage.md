# FirebaseStorage

版本:3.0
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=FirebaseStorage)

# FirebaseStorage
完整类名：anywheresoftware.b4x.objects.FirebaseStorageWrapper
> 所有者：process

> 依赖：com.google.firebase:firebase-storage | com.google.firebase:firebase-auth
> 事件：
>
> UploadCompleted (ServerPath As String, Success As Boolean)
>
> DownloadCompleted (ServerPath As String, Success As Boolean)
>
> MetadataCompleted (Metadata As StorageMetadata, Success As Boolean)
>
> DeleteCompleted (ServerPath As String, Success As Boolean)
## UploadFile方法
**UploadFile(ba,Dir,FileName,ServerPath)**

?> 说明：从文件中读取数据并将其上载到指定的ServerPath。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：ServerPath，类型：java.lang.String
>
> 返回值：void
## DownloadFile方法
**DownloadFile(ba,ServerPath,Dir,FileName)**

?> 说明：下载远程资源并将其写入指定的文件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ServerPath，类型：java.lang.String
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：void
## GetMetadata方法
**GetMetadata(ba,ServerPath)**

?> 说明：检索远程资源的元数据。MetadataCompleted事件将在当前模块中引发。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ServerPath，类型：java.lang.String
>
> 返回值：void
## UploadStream方法
**UploadStream(ba,InputStream,ServerPath)**

?> 说明：从输入流中读取数据并将其上载到指定的ServerPath。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：InputStream，类型：java.io.InputStream
>
> 参数：ServerPath，类型：java.lang.String
>
> 返回值：void
## Initialize方法
**Initialize(EventName,Bucket)**

?> 说明：初始化对象。
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Bucket，类型：java.lang.String
>
> 返回值：void
## DownloadStream方法
**DownloadStream(ba,ServerPath,OutputStream)**

?> 说明：下载远程资源并将其写入OutputStream。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ServerPath，类型：java.lang.String
>
> 参数：OutputStream，类型：java.io.OutputStream
>
> 返回值：void
## DeleteFile方法
**DeleteFile(ba,ServerPath)**

?> 说明：删除远程资源。DeleteCompleted事件将在当前模块中引发。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：ServerPath，类型：java.lang.String
>
> 返回值：void

# StorageMetadata
完整类名：anywheresoftware.b4x.objects.FirebaseStorageWrapper.StorageMetadataWrapper
> 所有者：process

> 包装器：com.google.firebase.storage.StorageMetadata

> 依赖：com.google.firebase:firebase-storage | com.google.firebase:firebase-auth
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Path属性

?> 说明：返回资源路径。
>
> 返回值：java.lang.String
## Size属性

?> 说明：返回以字节为单位的资源大小。
>
> 返回值：long
## Timestamp属性

?> 说明：以刻度形式返回上次更新的时间。
>
> 返回值：long
## Name属性

?> 说明：返回资源名称。
>
> 返回值：java.lang.String

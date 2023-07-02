# Camera2

版本:1.11
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Camera2)

# Camera2
完整类名：anywheresoftware.b4a.objects.Camera2
> 所有者：process

?> 说明：基于Camera2 API的摄像头库。它应该与CamEx2类一起使用。
> 事件：
>
> PictureTaken (Data() As Byte)
>
> CameraState (Open As Boolean)
>
> CameraClosed
>
> SurfaceReady
>
> SessionConfigured (Success As Boolean)
>
> PreviewCaptureComplete (CaptureResult As Object)
>
> PreviewTaken (Image As Object)
>
> CaptureComplete (CaptureResult As Object)

> 所需权限：
android.permission.CAMERA
## CreateSurface方法
**CreateSurface(ba)**

?> 说明：创建将用于显示预览帧的曲面视图（TextureView）。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4a.objects.ConcreteViewWrapper
## GetSupportedPreviewSizes方法
**GetSupportedPreviewSizes(Id)**

?> 说明：返回具有支持的预览大小的列表。
>
> 参数：Id，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## FindCameraId方法
**FindCameraId(Front)**

?> 说明：返回相关的摄像机id。如果未找到，则返回一个空字符串。
>
> 参数：Front，类型：boolean
>
> 返回值：java.lang.String
## Stop方法
**Stop()**

?> 说明：停止相机。
>
> 返回值：void
## CreateCaptureBuilder方法
**CreateCaptureBuilder()**

?> 说明：创建静态捕捉生成器。
>
> 返回值：java.lang.Object
## SetRepeatingRequest方法
**SetRepeatingRequest(Builder)**

?> 说明：设置重复请求（预览请求）。清除以前的任何重复请求。
>
> 参数：Builder，类型：java.lang.Object
>
> 返回值：java.lang.Object
## CreateVideoRequestBuilder方法
**CreateVideoRequestBuilder()**
>
> 返回值：java.lang.Object
## StartSession方法
**StartSession(Surface,PreviewSize,CaptureSize,CaptureFormat,PreviewFormat,Video)**

?> 说明：启动捕获会话。将引发SessionConfigured事件。
>
> 参数：Surface，类型：android.view.TextureView
>
> 参数：PreviewSize，类型：anywheresoftware.b4a.objects.Camera2.CameraSizeWrapper
>
> 参数：CaptureSize，类型：anywheresoftware.b4a.objects.Camera2.CameraSizeWrapper
>
> 参数：CaptureFormat，类型：int
>
> 参数：PreviewFormat，类型：int
>
> 参数：Video，类型：boolean
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## AddCaptureRequest方法
**AddCaptureRequest(Builder)**

?> 说明：添加捕获请求。
>
> 参数：Builder，类型：java.lang.Object
>
> 返回值：java.lang.Object
## CreatePreviewBuilder方法
**CreatePreviewBuilder()**

?> 说明：创建预览请求生成器。
>
> 返回值：java.lang.Object
## OpenCamera方法
**OpenCamera(Id)**

?> 说明：打开相机。将提出CameraState事件。
>
> 参数：Id，类型：java.lang.String
>
> 返回值：void
## AbortCaptures方法
**AbortCaptures()**

?> 说明：取消以前的请求。
>
> 返回值：void
## GetSupportedCaptureSizes方法
**GetSupportedCaptureSizes(Id)**

?> 说明：返回具有支持的捕获大小的列表。
>
> 参数：Id，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetSupportedVideoSizes方法
**GetSupportedVideoSizes(Id)**
>
> 参数：Id，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## CreateMediaRecorder方法
**CreateMediaRecorder(VideoSize,Dir,FileName)**
>
> 参数：VideoSize，类型：anywheresoftware.b4a.objects.Camera2.CameraSizeWrapper
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：java.lang.Object
## GetCameraCharacteristics方法
**GetCameraCharacteristics(Id)**

?> 说明：返回一个包含摄影机支持的功能的对象。
>
> 参数：Id，类型：java.lang.String
>
> 返回值：java.lang.Object
## CameraIDs属性

?> 说明：返回可用摄影机的ID。
>
> 返回值：java.lang.String[]
## IsCameraOpen属性
>
> 返回值：boolean

# CameraSize
完整类名：anywheresoftware.b4a.objects.Camera2.CameraSizeWrapper
> 所有者：process

> 包装器：android.util.Size
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Width,Height)**
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## Height属性
>
> 返回值：int
## Width属性
>
> 返回值：int

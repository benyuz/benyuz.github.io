# Camera

版本:2.2
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Camera)

# Camera
完整类名：anywheresoftware.b4a.objects.CameraW
> 所有者：activity

?> 说明：摄像头对象允许您访问设备摄像头。
> 事件：
>
> Ready (Success As Boolean)
>
> PictureTaken (Data() As Byte)
>
> Preview (Data() As Byte)
>
> FocusDone (Success As Boolean)

> 所需权限：
android.permission.CAMERA
## Release方法
**Release()**

?> 说明：释放摄影机对象并允许其他进程访问摄影机。
>
> 返回值：void
## Initialize方法
**Initialize(ba,Panel,EventName)**

?> 说明：初始化背面摄像头。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Panel，类型：android.view.ViewGroup
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## TakePicture方法
**TakePicture()**

?> 说明：拍张照片。当图片准备就绪时，将引发PictureTaked事件。
>
> 返回值：void
## StopPreview方法
**StopPreview()**

?> 说明：停止显示预览图像。
>
> 返回值：void
## StartPreview方法
**StartPreview()**

?> 说明：开始显示预览图像。
>
> 返回值：void
## CancelAutoFocus方法
**CancelAutoFocus()**

?> 说明：取消自动对焦操作。如果没有进行此类操作，则不执行任何操作。
>
> 返回值：void
## Initialize2方法
**Initialize2(ba,Panel,EventName,CameraId)**

?> 说明：与初始化相同。CameraId是硬件相机的id。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Panel，类型：android.view.ViewGroup
>
> 参数：EventName，类型：java.lang.String
>
> 参数：CameraId，类型：int
>
> 返回值：void
## AutoFocus方法
**AutoFocus()**

?> 说明：启动自动对焦功能。操作完成后将引发FocusDone事件。
>
> 返回值：void

# LiveWallpaper

版本:1.01
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=LiveWallpaper)

# LWManager
完整类名：anywheresoftware.b4a.objects.WallpaperInternalService.LWManager
> 所有者：process

?> 说明：管理壁纸事件和计时器。
> 事件：
>
> SizeChanged (Engine As LWEngine)
>
> Touch (Engine As LWEngine, Action As Int, X As Float, Y As Float)
>
> VisibilityChanged (Engine As LWEngine, Visible As Boolean)
>
> EngineDestroyed (Engine As LWEngine)
>
> Tick (Engine As LWEngine)
>
> OffsetChanged (Engine As LWEngine)
## Initialize方法
**Initialize(EventName,TouchEventsEnabled,ba)**

?> 说明：初始化对象。
>
> 参数：EventName，类型：java.lang.String
>
> 参数：TouchEventsEnabled，类型：boolean
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## StopTicking方法
**StopTicking()**

?> 说明：停止内部计时器。
>
> 返回值：void
## StartTicking方法
**StartTicking(IntervalMs)**

?> 说明：启动内部计时器。
>
> 参数：IntervalMs，类型：int
>
> 返回值：void

# LWEngine
完整类名：anywheresoftware.b4a.objects.WallpaperInternalService.LWEngine
> 所有者：process

?> 说明：表示壁纸实例。
## RefreshAll方法
**RefreshAll()**

?> 说明：刷新整个屏幕。
>
> 返回值：void
## Refresh方法
**Refresh(DirtyRect)**

?> 说明：刷新给定区域。
>
> 参数：DirtyRect，类型：android.graphics.Rect
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**

?> 说明：测试此对象是否已初始化。
>
> 返回值：boolean
## CurrentOffsetY属性

?> 说明：返回与壁纸全高相关的当前垂直偏移。
>
> 返回值：int
## CurrentOffsetX属性

?> 说明：返回与壁纸全宽相关的当前水平偏移量。
>
> 返回值：int
## FullWallpaperWidth属性

?> 说明：返回壁纸的完整宽度。一张壁纸可以由几个屏幕组成。
>
> 返回值：int
## IsVisible属性

?> 说明：测试此壁纸是否可见。
>
> 返回值：boolean
## ScreenHeight属性

?> 说明：返回屏幕高度。
>
> 返回值：int
## Canvas属性

?> 说明：返回用于在壁纸上绘制的画布。
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper
## IsPreview属性

?> 说明：测试此壁纸是否在“预览模式”下运行。
>
> 返回值：boolean
## FullWallpaperHeight属性

?> 说明：返回壁纸的全部高度。
>
> 返回值：int
## ScreenWidth属性

?> 说明：返回屏幕宽度。
>
> 返回值：int
## Rect字段

?> 说明：一个方便的Rect对象，您可以使用它。此对象未在内部使用。
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.RectWrapper
## Tag字段

?> 说明：获取或设置Tag值。这是一个可以用来存储额外数据的占位符。
>
> 返回值：java.lang.Object

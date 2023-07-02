# GameView

版本:0.9
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=GameView)

# GameView
完整类名：anywheresoftware.b4a.objects.GameViewWrapper
> 所有者：activity

> 包装器：anywheresoftware.b4a.objects.GameViewWrapper.MyPanel

?> 说明：使用硬件加速图形绘制自己的视图。适用于2d游戏。
> 事件：
>
> Touch (Action As Int, X As Float, Y As Float)
## Initialize方法
**Initialize(arg0,arg1)**
>
> 参数：arg0，类型：anywheresoftware.b4a.BA
>
> 参数：arg1，类型：java.lang.String
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## SetBackgroundImage方法
**SetBackgroundImage(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayout方法
**SetLayout(arg0,arg1,arg2,arg3)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 参数：arg2，类型：int
>
> 参数：arg3，类型：int
>
> 返回值：void
## Invalidate3方法
**Invalidate3(arg0,arg1,arg2,arg3)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 参数：arg2，类型：int
>
> 参数：arg3，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(arg0)**
>
> 参数：arg0，类型：android.graphics.Rect
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Top属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## BitmapsData属性

?> 说明：返回BitmapData对象的列表。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## Visible属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## IsHardwareAccelerated属性

?> 说明：测试是否支持硬件加速。
>
> 返回值：boolean
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Height属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## Left属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## Tag属性
>
> 参数：arg0，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性
>
> 参数：arg0，类型：int
>
> 返回值：int

# BitmapData
完整类名：anywheresoftware.b4a.objects.GameViewWrapper.BitmapData
> 所有者：process
## FLIP_BOTH字段
>
> 返回值：int
## Bitmap字段

?> 说明：将要绘制的位图。
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## FLIP_VERTICALLY字段
>
> 返回值：int
## FLIP_NONE字段
>
> 返回值：int
## Rotate字段

?> 说明：旋转位图的度数。
>
> 返回值：int
## Delete字段

?> 说明：如果Delete为True，则在重新绘制GameView时，BitmapData将从列表中删除。
>
> 返回值：boolean
## DestRect字段

?> 说明：目标矩形。确定绘制位图的位置和大小。
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.RectWrapper
## Flip字段

?> 说明：根据其中一个FLIP常量翻转位图。
>
> 返回值：int
## FLIP_HORIZONTALLY字段
>
> 返回值：int
## SrcRect字段

?> 说明：源矩形。确定要绘制的位图区域。完整的位图将
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.RectWrapper

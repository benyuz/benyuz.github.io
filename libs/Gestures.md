# Gestures

版本:1.2
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Gestures)

# Gestures
完整类名：anywheresoftware.b4a.agraham.gestures.Gestures
> 所有者：activity

?> 说明：此库允许视图支持手势（多点触摸）。
## SetOnTouchListener方法
**SetOnTouchListener(ba,view,sub)**

?> 说明：目标必须是某种类型的视图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：view，类型：android.view.View
>
> 参数：sub，类型：java.lang.String
>
> 返回值：void
## GetX方法
**GetX(pointerID)**

?> 说明：返回指定指针ID的X位置，如果该指针没有数据，则返回-1。
>
> 参数：pointerID，类型：int
>
> 返回值：float
## GetY方法
**GetY(pointerID)**

?> 说明：返回指定指针ID的Y位置，如果该指针没有数据，则返回-1。
>
> 参数：pointerID，类型：int
>
> 返回值：float
## GetPointerCount方法
**GetPointerCount()**

?> 说明：返回与屏幕接触的指针数。
>
> 返回值：int
## GetPointerID方法
**GetPointerID(pointerindex)**

?> 说明：指针数据以PointerCount长度的数组内部返回，该数组始终从索引0开始。
>
> 参数：pointerindex，类型：int
>
> 返回值：int
## Version属性

?> 说明：返回库的版本。
>
> 返回值：double
## ACTION_POINTER_DOWN字段
>
> 返回值：int
## ACTION_DOWN字段
>
> 返回值：int
## ACTION_POINTER_UP字段
>
> 返回值：int
## ACTION_UP字段
>
> 返回值：int
## ACTION_MOVE字段
>
> 返回值：int

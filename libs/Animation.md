# Animation

版本:1.02
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Animation)

# Animation
完整类名：anywheresoftware.b4a.objects.AnimationWrapper
> 所有者：activity

> 包装器：android.view.animation.Animation

?> 说明：使用“动画”对象可以设置视图的动画。
> 事件：
>
> AnimationEnd
## Start方法
**Start(View)**

?> 说明：开始设置给定视图的动画。
```vbnet
Animation1.Start(Button1)
```

>
> 参数：View，类型：android.view.View
>
> 返回值：void
## InitializeRotateCenter方法
**InitializeRotateCenter(ba,EventName,FromDegrees,ToDegrees,View)**

?> 说明：类似于InitializeRotate，将轴设置为给定视图的中心。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：FromDegrees，类型：float
>
> 参数：ToDegrees，类型：float
>
> 参数：View，类型：android.view.View
>
> 返回值：void
## InitializeScaleCenter方法
**InitializeScaleCenter(ba,EventName,FromX,FromY,ToX,ToY,View)**

?> 说明：类似于将轴心设置为给定视图中心的InitializeScale。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：FromX，类型：float
>
> 参数：FromY，类型：float
>
> 参数：ToX，类型：float
>
> 参数：ToY，类型：float
>
> 参数：View，类型：android.view.View
>
> 返回值：void
## InitializeRotate方法
**InitializeRotate(ba,EventName,FromDegrees,ToDegrees)**

?> 说明：初始化旋转动画。视图将在给定值之间旋转。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：FromDegrees，类型：float
>
> 参数：ToDegrees，类型：float
>
> 返回值：void
## Stop方法
**Stop(View)**

?> 说明：停止为给定视图设置动画。
>
> 参数：View，类型：android.view.View
>
> 返回值：void
## InitializeScale方法
**InitializeScale(ba,EventName,FromX,FromY,ToX,ToY)**

?> 说明：初始化缩放动画。视图将在动画过程中进行缩放。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：FromX，类型：float
>
> 参数：FromY，类型：float
>
> 参数：ToX，类型：float
>
> 参数：ToY，类型：float
>
> 返回值：void
## InitializeTranslate方法
**InitializeTranslate(ba,EventName,FromDX,FromDY,ToDX,ToDY)**

?> 说明：初始化平移动画。视图将根据给定的值移动。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：FromDX，类型：float
>
> 参数：FromDY，类型：float
>
> 参数：ToDX，类型：float
>
> 参数：ToDY，类型：float
>
> 返回值：void
## InitializeAlpha方法
**InitializeAlpha(ba,EventName,FromAlpha,ToAlpha)**

?> 说明：初始化alpha动画。此动画会影响视图的透明度（淡入效果）。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：FromAlpha，类型：float
>
> 参数：ToAlpha，类型：float
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## RepeatCount属性

?> 说明：获取或设置动画将重复的次数。值为0表示它将播放一次。
```vbnet
Animation1.RepeatCount = 1
```

>
> 参数：value，类型：int
>
> 返回值：int
## RepeatMode属性

?> 说明：获取或设置重复模式。RepeatCount大于0（或-1）时相关。
```vbnet
Animation1.RepeatMode = Animation1.REPEAT_REVERSE
```

>
> 参数：mode，类型：int
>
> 返回值：int
## Duration属性

?> 说明：获取或设置动画持续时间。值以毫秒为单位测量。
```vbnet
Animation1.Duration = 1000
```

>
> 参数：value，类型：long
>
> 返回值：long
## REPEAT_RESTART字段
>
> 返回值：int
## REPEAT_REVERSE字段
>
> 返回值：int

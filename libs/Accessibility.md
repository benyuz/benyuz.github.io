# Accessibility

版本:1.02
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Accessibility)

# Accessibility
完整类名：anywheresoftware.b4a.objects.Accessibility
> 所有者：process

?> 说明：此库包括几个与可访问性相关的方法。
## GetUserFontScale方法
**GetUserFontScale()**

?> 说明：返回用户设置的字体比例。用户可以在设备设置中调整此比例。
>
> 返回值：float
## SetNextFocusDown方法
**SetNextFocusDown(ThisView,NextView)**

?> 说明：设置当用户按下向下键时将获得焦点的下一个视图（并且ThisView处于焦点状态）。
```vbnet

Dim Access As Accessibility
Access.SetNextFocusDown(Button1, Button2) 'When the focus is on Button1 and the user presses on the down key,
'the focus will move to Button2.

```

>
> 参数：ThisView，类型：android.view.View
>
> 参数：NextView，类型：android.view.View
>
> 返回值：void
## SetNextFocusLeft方法
**SetNextFocusLeft(ThisView,NextView)**

?> 说明：设置当用户按下左键时将获得焦点的下一个视图（并且ThisView处于焦点状态）。
>
> 参数：ThisView，类型：android.view.View
>
> 参数：NextView，类型：android.view.View
>
> 返回值：void
## SetContentDescription方法
**SetContentDescription(View,Content)**

?> 说明：设置视图的描述。辅助功能服务将使用此文本来描述视图。
>
> 参数：View，类型：android.view.View
>
> 参数：Content，类型：java.lang.CharSequence
>
> 返回值：void
## SetNextFocusUp方法
**SetNextFocusUp(ThisView,NextView)**

?> 说明：设置当用户按下向上键时将获得焦点的下一个视图（并且ThisView处于焦点状态）。
>
> 参数：ThisView，类型：android.view.View
>
> 参数：NextView，类型：android.view.View
>
> 返回值：void
## SetNextFocusRight方法
**SetNextFocusRight(ThisView,NextView)**

?> 说明：设置下一个视图，该视图将在用户按下右键时获得焦点（并且ThisView处于焦点状态）。
>
> 参数：ThisView，类型：android.view.View
>
> 参数：NextView，类型：android.view.View
>
> 返回值：void

# Accessiblity
完整类名：anywheresoftware.b4a.objects.Accessibility.Accessibility2
> 所有者：process

?> 说明：与辅助功能类型相同，但有拼写错误。。。请改用辅助功能。
## GetUserFontScale方法
**GetUserFontScale()**

?> 说明：返回用户设置的字体比例。用户可以在设备设置中调整此比例。
>
> 返回值：float
## SetNextFocusDown方法
**SetNextFocusDown(ThisView,NextView)**

?> 说明：设置当用户按下向下键时将获得焦点的下一个视图（并且ThisView处于焦点状态）。
```vbnet

Dim Access As Accessibility
Access.SetNextFocusDown(Button1, Button2) 'When the focus is on Button1 and the user presses on the down key,
'the focus will move to Button2.

```

>
> 参数：ThisView，类型：android.view.View
>
> 参数：NextView，类型：android.view.View
>
> 返回值：void
## SetNextFocusLeft方法
**SetNextFocusLeft(ThisView,NextView)**

?> 说明：设置当用户按下左键时将获得焦点的下一个视图（并且ThisView处于焦点状态）。
>
> 参数：ThisView，类型：android.view.View
>
> 参数：NextView，类型：android.view.View
>
> 返回值：void
## SetContentDescription方法
**SetContentDescription(View,Content)**

?> 说明：设置视图的描述。辅助功能服务将使用此文本来描述视图。
>
> 参数：View，类型：android.view.View
>
> 参数：Content，类型：java.lang.CharSequence
>
> 返回值：void
## SetNextFocusUp方法
**SetNextFocusUp(ThisView,NextView)**

?> 说明：设置当用户按下向上键时将获得焦点的下一个视图（并且ThisView处于焦点状态）。
>
> 参数：ThisView，类型：android.view.View
>
> 参数：NextView，类型：android.view.View
>
> 返回值：void
## SetNextFocusRight方法
**SetNextFocusRight(ThisView,NextView)**

?> 说明：设置下一个视图，该视图将在用户按下右键时获得焦点（并且ThisView处于焦点状态）。
>
> 参数：ThisView，类型：android.view.View
>
> 参数：NextView，类型：android.view.View
>
> 返回值：void

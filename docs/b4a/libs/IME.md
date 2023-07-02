# IME

版本:1.1
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=IME)

# IME
完整类名：anywheresoftware.b4a.objects.IME
> 所有者：activity

?> 说明：IME包括几个实用程序，可以帮助您管理软键盘。
> 事件：
>
> HeightChanged (NewHeight As Int, OldHeight As Int)
>
> HandleAction As Boolean
## HideKeyboard方法
**HideKeyboard(ba)**

?> 说明：隐藏软键盘（如果可见）。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Initialize方法
**Initialize(EventName)**

?> 说明：初始化对象并设置将处理事件的子对象。
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetCustomFilter方法
**SetCustomFilter(EditText,DefaultInputType,AcceptedCharacters)**

?> 说明：设置自定义过滤器。
```vbnet

IME.SetCustomFilter(EditText1, EditText1.INPUT_TYPE_NUMBERS, "0123456789.")
```

>
> 参数：EditText，类型：android.widget.EditText
>
> 参数：DefaultInputType，类型：int
>
> 参数：AcceptedCharacters，类型：java.lang.String
>
> 返回值：void
## AddHandleActionEvent方法
**AddHandleActionEvent(EditText,ba)**

?> 说明：将HandleAction事件添加到给定的EditText中。
>
> 参数：EditText，类型：android.widget.EditText
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## AddHeightChangedEvent方法
**AddHeightChangedEvent(ba)**

?> 说明：启用HeightChanged事件。当软键盘状态更改时，会引发此事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## SetLengthFilter方法
**SetLengthFilter(EditText,MaxLength)**

?> 说明：设置将最大长度限制为指定值的过滤器。
>
> 参数：EditText，类型：android.widget.EditText
>
> 参数：MaxLength，类型：int
>
> 返回值：void
## ShowKeyboard方法
**ShowKeyboard(View)**

?> 说明：将焦点设置为给定视图并打开软键盘。
>
> 参数：View，类型：android.view.View
>
> 返回值：void

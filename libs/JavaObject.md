# JavaObject

版本:2.06
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=JavaObject)

# JavaObject
完整类名：anywheresoftware.b4j.object.JavaObject
> 所有者：process

> 包装器：java.lang.Object
> 事件：
>
> Event (MethodName As String, Args() As Object) As Object
## InitializeContext方法
**InitializeContext(ba)**

?> 说明：<b>仅B4A方法</b>
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4j.object.JavaObject
## InitializeNewInstance方法
**InitializeNewInstance(ClassName,Params)**

?> 说明：创建给定类的新实例。
>
> 参数：ClassName，类型：java.lang.String
>
> 参数：Params，类型：java.lang.Object[]
>
> 返回值：anywheresoftware.b4j.object.JavaObject
## InitializeStatic方法
**InitializeStatic(ClassName)**

?> 说明：初始化对象。该对象将包装给定的类（用于静态访问）。
>
> 参数：ClassName，类型：java.lang.String
>
> 返回值：anywheresoftware.b4j.object.JavaObject
## GetField方法
**GetField(Field)**

?> 说明：获取给定字段的值。
>
> 参数：Field，类型：java.lang.String
>
> 返回值：java.lang.Object
## CreateEvent方法
**CreateEvent(ba,Interface,EventName,DefaultReturnValue)**

?> 说明：创建接口的实例并将其绑定到对象。
```vbnet

Sub Activity_Create(FirstTime As Boolean)
   Dim b As Button
   b.Initialize("")
   Activity.AddView(b, 0, 0, 200dip, 200dip)
   Dim jo As JavaObject = b
   Dim e As Object = jo.CreateEvent("android.view.View.OnTouchListener", "btouch", False)
   jo.RunMethod("setOnTouchListener", Array As Object(e))
End Sub

Sub btouch_Event (MethodName As String, Args() As Object) As Object
   Dim motion As JavaObject = Args(1) 'args(0) is View
   Dim x As Float = motion.RunMethod("getX", Null)
   Dim y As Float = motion.RunMethod("getY", Null)
   Log(x & ", " & y)
   Return True
End Sub
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Interface，类型：java.lang.String
>
> 参数：EventName，类型：java.lang.String
>
> 参数：DefaultReturnValue，类型：java.lang.Object
>
> 返回值：java.lang.Object
## GetFieldJO方法
**GetFieldJO(Field)**

?> 说明：类似于GetField。返回一个JavaObject而不是Object。
>
> 参数：Field，类型：java.lang.String
>
> 返回值：anywheresoftware.b4j.object.JavaObject
## RunMethodJO方法
**RunMethodJO(MethodName,Params)**

?> 说明：类似于RunMethod。返回一个JavaObject而不是Object。
>
> 参数：MethodName，类型：java.lang.String
>
> 参数：Params，类型：java.lang.Object[]
>
> 返回值：anywheresoftware.b4j.object.JavaObject
## InitializeArray方法
**InitializeArray(ClassName,Values)**

?> 说明：创建一个具有给定类和值的数组。
>
> 参数：ClassName，类型：java.lang.String
>
> 参数：Values，类型：java.lang.Object[]
>
> 返回值：anywheresoftware.b4j.object.JavaObject
## SetField方法
**SetField(FieldName,Value)**

?> 说明：设置给定字段的值。
>
> 参数：FieldName，类型：java.lang.String
>
> 参数：Value，类型：java.lang.Object
>
> 返回值：void
## RunMethod方法
**RunMethod(MethodName,Params)**

?> 说明：运行给定的方法并返回方法返回值。
>
> 参数：MethodName，类型：java.lang.String
>
> 参数：Params，类型：java.lang.Object[]
>
> 返回值：java.lang.Object
## CreateEventFromUI方法
**CreateEventFromUI(ba,Interface,EventName,ReturnValue)**

?> 说明：类似于CreateEvent。事件将被发送到消息队列，然后进行处理（类似于CallSubDelayed）。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Interface，类型：java.lang.String
>
> 参数：EventName，类型：java.lang.String
>
> 参数：ReturnValue，类型：java.lang.Object
>
> 返回值：java.lang.Object
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean

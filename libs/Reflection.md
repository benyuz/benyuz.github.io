# Reflection

版本:2.4
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Reflection)

# Reflector
完整类名：anywheresoftware.b4a.agraham.reflection.Reflection
> 所有者：process

?> 说明：这是进行反射的对象。为了成功地使用它，您将
> 事件：
>
> Click(ViewTag As Object)
>
> LongClick(ViewTag As Object) As Boolean
>
> Focus(ViewTag As Object, Focus As Boolean)
>
> Key(ViewTag As Object, KeyCode As Int, KeyEvent As Object) As Boolean
>
> Touch(ViewTag As Object, Action As Int, X As Float, Y As Float, MotionEvent As Object) As Boolean
## GetArray方法
**GetArray(indeces)**

?> 说明：返回数组中由索引的内容指定的位置处的对象。
>
> 参数：indeces，类型：int[]
>
> 返回值：java.lang.Object
## SetStaticField方法
**SetStaticField(classname,field,value,type)**

?> 说明：将指定类的指定静态字段设置为提供的值。
>
> 参数：classname，类型：java.lang.String
>
> 参数：field，类型：java.lang.String
>
> 参数：value，类型：java.lang.String
>
> 参数：type，类型：java.lang.String
>
> 返回值：void
## RunMethod3方法
**RunMethod3(method,arg1,type1,arg2,type2)**

?> 说明：在当前对象上运行指定的方法，向其传递所提供的参数。
>
> 参数：method，类型：java.lang.String
>
> 参数：arg1，类型：java.lang.String
>
> 参数：type1，类型：java.lang.String
>
> 参数：arg2，类型：java.lang.String
>
> 参数：type2，类型：java.lang.String
>
> 返回值：java.lang.Object
## RunMethod2方法
**RunMethod2(method,arg1,type1)**

?> 说明：在当前目标上运行指定的方法，并将提供的参数传递给它。
>
> 参数：method，类型：java.lang.String
>
> 参数：arg1，类型：java.lang.String
>
> 参数：type1，类型：java.lang.String
>
> 返回值：java.lang.Object
## SetOnFocusListener方法
**SetOnFocusListener(ba,sub)**

?> 说明：目标必须是某种类型的视图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：sub，类型：java.lang.String
>
> 返回值：void
## SetField4方法
**SetField4(fieldinfo,value)**

?> 说明：将当前目标的指定字段设置为提供的值。
>
> 参数：fieldinfo，类型：java.lang.reflect.Field
>
> 参数：value，类型：java.lang.Object
>
> 返回值：void
## RunMethod4方法
**RunMethod4(method,args,types)**

?> 说明：在当前目标上运行指定的方法，并向其传递所提供的参数。
>
> 参数：method，类型：java.lang.String
>
> 参数：args，类型：java.lang.Object[]
>
> 参数：types，类型：java.lang.String[]
>
> 返回值：java.lang.Object
## GetActivity方法
**GetActivity(ba)**

?> 说明：返回当前活动（如果有）。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：android.app.Activity
## GetStaticField方法
**GetStaticField(classname,field)**

?> 说明：返回指定类的指定静态字段的值。
>
> 参数：classname，类型：java.lang.String
>
> 参数：field，类型：java.lang.String
>
> 返回值：java.lang.Object
## SetArray2方法
**SetArray2(indeces,value)**

?> 说明：将indeces的内容指定的数组中的位置设置为指定值。
>
> 参数：indeces，类型：int[]
>
> 参数：value，类型：java.lang.Object
>
> 返回值：void
## SetField2方法
**SetField2(field,value)**

?> 说明：将当前目标的指定字段设置为提供的值。受保护和
>
> 参数：field，类型：java.lang.String
>
> 参数：value，类型：java.lang.Object
>
> 返回值：void
## SetField3方法
**SetField3(fieldinfo,value,type)**

?> 说明：将当前目标的指定字段设置为提供的值。
>
> 参数：fieldinfo，类型：java.lang.reflect.Field
>
> 参数：value，类型：java.lang.String
>
> 参数：type，类型：java.lang.String
>
> 返回值：void
## SetOnTouchListener方法
**SetOnTouchListener(ba,sub)**

?> 说明：目标必须是某种类型的视图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：sub，类型：java.lang.String
>
> 返回值：void
## SetPublicField方法
**SetPublicField(field,value,type)**

?> 说明：将当前目标的指定字段设置为提供的值。
>
> 参数：field，类型：java.lang.String
>
> 参数：value，类型：java.lang.String
>
> 参数：type，类型：java.lang.String
>
> 返回值：void
## CreateObject方法
**CreateObject(type)**

?> 说明：使用默认构造函数创建并返回指定类型的新对象。
>
> 参数：type，类型：java.lang.String
>
> 返回值：java.lang.Object
## InvokeMethod方法
**InvokeMethod(instance,method,args)**

?> 说明：对提供的对象实例调用提供的方法并返回结果。
>
> 参数：instance，类型：java.lang.Object
>
> 参数：method，类型：java.lang.reflect.Method
>
> 参数：args，类型：java.lang.Object[]
>
> 返回值：java.lang.Object
## GetField方法
**GetField(field)**

?> 说明：返回当前目标的字段值。受保护和私人领域
>
> 参数：field，类型：java.lang.String
>
> 返回值：java.lang.Object
## SetStaticField2方法
**SetStaticField2(classname,field,value)**

?> 说明：将指定类的指定静态字段设置为提供的值。
>
> 参数：classname，类型：java.lang.String
>
> 参数：field，类型：java.lang.String
>
> 参数：value，类型：java.lang.Object
>
> 返回值：void
## GetB4AClass方法
**GetB4AClass(component)**

?> 说明：返回指定B4A活动、服务或代码模块的Java类。
>
> 参数：component，类型：java.lang.String
>
> 返回值：java.lang.Class
## GetMethod方法
**GetMethod(method,types)**

?> 说明：从字符串表示中查找方法的成本很高，因此可以使用此方法
>
> 参数：method，类型：java.lang.String
>
> 参数：types，类型：java.lang.String[]
>
> 返回值：java.lang.reflect.Method
## ToString方法
**ToString()**

?> 说明：返回运行当前对象的“toString（）”方法的结果。
>
> 返回值：java.lang.String
## TargetRank方法
**TargetRank()**

?> 说明：返回一个int数组，其长度为数组的维数，其内容为
>
> 返回值：int[]
## SetPublicField2方法
**SetPublicField2(field,value)**

?> 说明：将当前目标的指定字段设置为提供的值。
>
> 参数：field，类型：java.lang.String
>
> 参数：value，类型：java.lang.Object
>
> 返回值：void
## RunMethod方法
**RunMethod(method)**

?> 说明：在当前目标上运行指定的方法。受保护的和私有的方法
>
> 参数：method，类型：java.lang.String
>
> 返回值：java.lang.Object
## GetField2方法
**GetField2(fieldinfo)**

?> 说明：返回当前目标的字段值。
>
> 参数：fieldinfo，类型：java.lang.reflect.Field
>
> 返回值：java.lang.Object
## GetProcessBA方法
**GetProcessBA(component)**

?> 说明：返回指定B4A活动或服务模块的processBA实例。
>
> 参数：component，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.BA
## GetContext方法
**GetContext(ba)**

?> 说明：返回反射对象所属进程的上下文。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：android.content.Context
## RunStaticMethod方法
**RunStaticMethod(classname,method,args,types)**

?> 说明：运行指定类的指定静态方法，向其传递所提供的参数。
>
> 参数：classname，类型：java.lang.String
>
> 参数：method，类型：java.lang.String
>
> 参数：args，类型：java.lang.Object[]
>
> 参数：types，类型：java.lang.String[]
>
> 返回值：java.lang.Object
## GetActivityBA方法
**GetActivityBA(ba)**

?> 说明：返回当前活动的活动BA。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4a.BA
## SetOnKeyListener方法
**SetOnKeyListener(ba,sub)**

?> 说明：目标必须是某种类型的视图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：sub，类型：java.lang.String
>
> 返回值：void
## RunPublicmethod方法
**RunPublicmethod(Method,Args,types)**

?> 说明：在当前目标上运行指定的方法，并向其传递所提供的参数。
>
> 参数：Method，类型：java.lang.String
>
> 参数：Args，类型：java.lang.Object[]
>
> 参数：types，类型：java.lang.String[]
>
> 返回值：java.lang.Object
## GetMostCurrent方法
**GetMostCurrent(component)**

?> 说明：返回指定B4A活动或服务模块的当前实例。
>
> 参数：component，类型：java.lang.String
>
> 返回值：java.lang.Object
## SetOnLongClickListener方法
**SetOnLongClickListener(ba,sub)**

?> 说明：目标必须是某种类型的视图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：sub，类型：java.lang.String
>
> 返回值：void
## SetOnCreateContextMenuListener方法
**SetOnCreateContextMenuListener(ba,sub)**

?> 说明：目标必须是某种类型的视图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：sub，类型：java.lang.String
>
> 返回值：void
## GetProxy方法
**GetProxy(ba,interfacenames,b4asubname)**

?> 说明：在Java中，您可以在运行时生成一个接口，并让它运行一个预编译的方法。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：interfacenames，类型：java.lang.String[]
>
> 参数：b4asubname，类型：java.lang.String
>
> 返回值：java.lang.reflect.Proxy
## SetArray方法
**SetArray(indeces,value,type)**

?> 说明：将indeces的内容指定的数组中的位置设置为指定值。
>
> 参数：indeces，类型：int[]
>
> 参数：value，类型：java.lang.String
>
> 参数：type，类型：java.lang.String
>
> 返回值：void
## SetOnClickListener方法
**SetOnClickListener(ba,sub)**

?> 说明：目标必须是某种类型的视图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：sub，类型：java.lang.String
>
> 返回值：void
## GetPublicField方法
**GetPublicField(field)**

?> 说明：返回当前目标的公共字段的值。
>
> 参数：field，类型：java.lang.String
>
> 返回值：java.lang.Object
## SetField方法
**SetField(field,value,type)**

?> 说明：将当前目标的指定字段设置为提供的值。受保护和
>
> 参数：field，类型：java.lang.String
>
> 参数：value，类型：java.lang.String
>
> 参数：type，类型：java.lang.String
>
> 返回值：void
## GetFieldInfo方法
**GetFieldInfo(field)**

?> 说明：从字段的字符串表示中查找字段非常昂贵，因此可以使用此方法
>
> 参数：field，类型：java.lang.String
>
> 返回值：java.lang.reflect.Field
## CreateObject2方法
**CreateObject2(type,args,types)**

?> 说明：使用匹配的构造函数创建并返回指定类型的新对象
>
> 参数：type，类型：java.lang.String
>
> 参数：args，类型：java.lang.Object[]
>
> 参数：types，类型：java.lang.String[]
>
> 返回值：java.lang.Object
## IsNull属性

?> 说明：如果Target的prsent值为Null，则返回True。
>
> 返回值：boolean
## TypeName属性

?> 说明：返回当前对象的类的名称。
>
> 返回值：java.lang.String
## Version属性

?> 说明：返回库的版本号。
>
> 返回值：double
## Target字段

?> 说明：这个场包含被反射的物体。目标对象是
>
> 返回值：java.lang.Object

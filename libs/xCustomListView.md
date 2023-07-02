# xCustomListView

版本:1.73
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=xCustomListView)

# CLVItem
完整类名：b4a.example3.customlistview._clvitem
> 所有者：activity

> 依赖：stringutils | xui | javaobject
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Panel字段
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper
## Size字段
>
> 返回值：int
## Value字段
>
> 返回值：Object
## Color字段
>
> 返回值：int
## TextItem字段
>
> 返回值：boolean
## Offset字段
>
> 返回值：int

# CustomListView
完整类名：b4a.example3.customlistview
> 所有者：activity

> 依赖：stringutils | xui | javaobject
> 事件：
>
> ItemClick (Index As Int, Value As Object)
>
> ItemLongClick (Index As Int, Value As Object)
>
> ReachEnd
>
> VisibleRangeChanged (FirstIndex As Int, LastIndex as Int)
>
> ScrollChanged (Offset As Int)
## IsInitialized方法
**IsInitialized()**

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## _add方法
**_add(Pnl,Value)**

?> 说明：添加自定义项。
>
> 参数：Pnl，类型：anywheresoftware.b4a.objects.B4XViewWrapper
>
> 参数：Value，类型：Object
>
> 返回值：String
## _addtextitem方法
**_addtextitem(Text,Value)**

?> 说明：添加文本项。项目高度将根据文本进行调整。
>
> 参数：Text，类型：Object
>
> 参数：Value，类型：Object
>
> 返回值：String
## _asview方法
**_asview()**
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper
## _base_resize方法
**_base_resize(Width,Height)**
>
> 参数：Width，类型：double
>
> 参数：Height，类型：double
>
> 返回值：String
## _class_globals方法
**_class_globals()**
>
> 返回值：String
## _clear方法
**_clear()**

?> 说明：清除所有项目。
>
> 返回值：String
## _designercreateview方法
**_designercreateview(Base,Lbl,Props)**
>
> 参数：Base，类型：Object
>
> 参数：Lbl，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：Props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：String
## _findindexfromoffset方法
**_findindexfromoffset(Offset)**

?> 说明：根据偏移量查找项的索引（+分隔符）
>
> 参数：Offset，类型：int
>
> 返回值：int
## _getbase方法
**_getbase()**
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper
## _getdividersize方法
**_getdividersize()**
>
> 返回值：float
## _getfirstvisibleindex方法
**_getfirstvisibleindex()**

?> 说明：获取第一个可见项的索引。
>
> 返回值：int
## _getitemfromview方法
**_getitemfromview(v)**

?> 说明：返回包含给定视图的项的索引。
>
> 参数：v，类型：anywheresoftware.b4a.objects.B4XViewWrapper
>
> 返回值：int
## _getlastvisibleindex方法
**_getlastvisibleindex()**

?> 说明：获取最后一个可见项的索引。
>
> 返回值：int
## _getpanel方法
**_getpanel(Index)**

?> 说明：返回存储在指定索引中的面板。
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper
## _getrawlistitem方法
**_getrawlistitem(Index)**

?> 说明：返回CLVItem。在大多数情况下不应使用。
>
> 参数：Index，类型：int
>
> 返回值：b4a.example3.customlistview._clvitem
## _getsize方法
**_getsize()**

?> 说明：返回项目数。
>
> 返回值：int
## _getvalue方法
**_getvalue(Index)**

?> 说明：返回存储在指定索引处的值。
>
> 参数：Index，类型：int
>
> 返回值：Object
## _initialize方法
**_initialize(ba,vCallBack,vEventName)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：vCallBack，类型：Object
>
> 参数：vEventName，类型：String
>
> 返回值：String
## _insertat方法
**_insertat(Index,pnl,Value)**

?> 说明：在指定索引处添加自定义项。
>
> 参数：Index，类型：int
>
> 参数：pnl，类型：anywheresoftware.b4a.objects.B4XViewWrapper
>
> 参数：Value，类型：Object
>
> 返回值：String
## _insertattextitem方法
**_insertattextitem(Index,Text,Value)**

?> 说明：在指定的索引处插入文本项。
>
> 参数：Index，类型：int
>
> 参数：Text，类型：Object
>
> 参数：Value，类型：Object
>
> 返回值：String
## _jumptoitem方法
**_jumptoitem(Index)**

?> 说明：将列表滚动到指定项目（不设置滚动动画）。
>
> 参数：Index，类型：int
>
> 返回值：String
## _refresh方法
**_refresh()**

?> 说明：导致引发VisibleRangeChanged事件
>
> 返回值：String
## _removeat方法
**_removeat(Index)**

?> 说明：删除指定索引处的项。
>
> 参数：Index，类型：int
>
> 返回值：String
## _replaceat方法
**_replaceat(Index,pnl,ItemSize,Value)**

?> 说明：用新项替换指定索引处的项。
>
> 参数：Index，类型：int
>
> 参数：pnl，类型：anywheresoftware.b4a.objects.B4XViewWrapper
>
> 参数：ItemSize，类型：int
>
> 参数：Value，类型：Object
>
> 返回值：String
## _resizeitem方法
**_resizeitem(Index,ItemSize)**

?> 说明：更改现有项目的高度。
>
> 参数：Index，类型：int
>
> 参数：ItemSize，类型：int
>
> 返回值：String
## _scrolltoitem方法
**_scrolltoitem(Index)**

?> 说明：将列表平滑地滚动到指定的项目。
>
> 参数：Index，类型：int
>
> 返回值：String
## _dividersize属性
>
> 返回值：float
## _firstvisibleindex属性

?> 说明：获取第一个可见项的索引。
>
> 返回值：int
## _lastvisibleindex属性

?> 说明：获取最后一个可见项的索引。
>
> 返回值：int
## _size属性

?> 说明：返回项目数。
>
> 返回值：int
## _sv字段
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper
## _defaulttextcolor字段
>
> 返回值：int
## _defaulttextbackgroundcolor字段
>
> 返回值：int
## _animationduration字段
>
> 返回值：int
## _pressedcolor字段
>
> 返回值：int
## _designerlabel字段
>
> 返回值：anywheresoftware.b4a.objects.LabelWrapper
## _horizontal字段
>
> 返回值：boolean

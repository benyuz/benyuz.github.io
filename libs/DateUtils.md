# DateUtils

版本:1.05
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=DateUtils)

# DateUtils
完整类名：b4a.example.dateutils
> 所有者：activity

> 包装器：java.lang.Class
## _addperiod方法
**_addperiod(ba,Ticks,Per)**

?> 说明：在给定的日期实例中添加一个期间。不要忘记分配结果。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Ticks，类型：long
>
> 参数：Per，类型：b4a.example.dateutils._period
>
> 返回值：long
## _getdayofweekname方法
**_getdayofweekname(ba,Ticks)**

?> 说明：返回星期几的名称。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Ticks，类型：long
>
> 返回值：String
## _getdaysnames方法
**_getdaysnames(ba)**

?> 说明：使用设备设置的区域设置返回包含星期天名称的列表。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## _getmonthname方法
**_getmonthname(ba,Ticks)**

?> 说明：返回给定日期的月份名称。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Ticks，类型：long
>
> 返回值：String
## _getmonthsnames方法
**_getmonthsnames(ba)**

?> 说明：使用设备集区域设置返回一个包含月份名称的列表。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## _issameday方法
**_issameday(ba,Ticks1,Ticks2)**

?> 说明：测试两个刻度值是否表示同一天。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Ticks1，类型：long
>
> 参数：Ticks2，类型：long
>
> 返回值：boolean
## _numberofdaysinmonth方法
**_numberofdaysinmonth(ba,Month,Year)**

?> 说明：返回给定月份的天数
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Month，类型：int
>
> 参数：Year，类型：int
>
> 返回值：int
## _periodbetween方法
**_periodbetween(ba,Start,EndTime)**

?> 说明：计算两个日期实例之间的时间段。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Start，类型：long
>
> 参数：EndTime，类型：long
>
> 返回值：b4a.example.dateutils._period
## _periodbetweenindays方法
**_periodbetweenindays(ba,Start,EndTime)**

?> 说明：计算两个日期实例之间的时间段。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Start，类型：long
>
> 参数：EndTime，类型：long
>
> 返回值：b4a.example.dateutils._period
## _process_globals方法
**_process_globals()**
>
> 返回值：String
## _setdate方法
**_setdate(ba,Years,Months,Days)**

?> 说明：返回给定日期的刻度值（时间为00:00:00）。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Years，类型：int
>
> 参数：Months，类型：int
>
> 参数：Days，类型：int
>
> 返回值：long
## _setdateandtime方法
**_setdateandtime(ba,Years,Months,Days,Hours,Minutes,Seconds)**

?> 说明：返回给定日期和时间的刻度值
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Years，类型：int
>
> 参数：Months，类型：int
>
> 参数：Days，类型：int
>
> 参数：Hours，类型：int
>
> 参数：Minutes，类型：int
>
> 参数：Seconds，类型：int
>
> 返回值：long
## _setdateandtime2方法
**_setdateandtime2(ba,Years,Months,Days,Hours,Minutes,Seconds,TimeZone)**

?> 说明：返回具有指定时区偏移量的给定日期和时间的刻度值。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Years，类型：int
>
> 参数：Months，类型：int
>
> 参数：Days，类型：int
>
> 参数：Hours，类型：int
>
> 参数：Minutes，类型：int
>
> 参数：Seconds，类型：int
>
> 参数：TimeZone，类型：double
>
> 返回值：long
## _tickstostring方法
**_tickstostring(ba,Ticks)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Ticks，类型：long
>
> 返回值：String
## _tickstounixtime方法
**_tickstounixtime(ba,Ticks)**

?> 说明：将ticks值转换为unix时间。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Ticks，类型：long
>
> 返回值：long
## _unixtimetoticks方法
**_unixtimetoticks(ba,UnixTime)**

?> 说明：将unix时间转换为ticks值。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：UnixTime，类型：long
>
> 返回值：long

# Period
完整类名：b4a.example.dateutils._period
> 所有者：process
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Years字段
>
> 返回值：int
## Months字段
>
> 返回值：int
## Days字段
>
> 返回值：int
## Hours字段
>
> 返回值：int
## Minutes字段
>
> 返回值：int
## Seconds字段
>
> 返回值：int

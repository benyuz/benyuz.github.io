# GPS

版本:1.2
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=GPS)

# Location
完整类名：anywheresoftware.b4a.gps.LocationWrapper
> 所有者：process

> 包装器：android.location.Location

?> 说明：Location对象保存有关特定GPS定位的各种信息。
## Initialize方法
**Initialize()**

?> 说明：初始化一个空的位置对象。
>
> 返回值：void
## ConvertToSeconds方法
**ConvertToSeconds(Coordinate)**

?> 说明：将给定的坐标转换为使用以下格式格式化的字符串：
>
> 参数：Coordinate，类型：double
>
> 返回值：java.lang.String
## DistanceTo方法
**DistanceTo(TargetLocation)**

?> 说明：返回到给定位置的距离，单位为米。
>
> 参数：TargetLocation，类型：android.location.Location
>
> 返回值：float
## ConvertToMinutes方法
**ConvertToMinutes(Coordinate)**

?> 说明：将给定的坐标转换为使用以下格式格式化的字符串：
>
> 参数：Coordinate，类型：double
>
> 返回值：java.lang.String
## Initialize2方法
**Initialize2(Latitude,Longitude)**

?> 说明：使用给定的纬度和经度初始化位置对象。
```vbnet

Dim L1 As Location
L1.Initialize2("45:30:30", "45:20:15")
```

>
> 参数：Latitude，类型：java.lang.String
>
> 参数：Longitude，类型：java.lang.String
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## BearingTo方法
**BearingTo(TargetLocation)**

?> 说明：将方位返回到给定位置。
>
> 参数：TargetLocation，类型：android.location.Location
>
> 返回值：float
## AltitudeValid属性

?> 说明：如果修正包括海拔值，则返回true。
>
> 返回值：boolean
## Accuracy属性

?> 说明：获取或设置修复精度（米）。
>
> 参数：value，类型：float
>
> 返回值：float
## BearingValid属性

?> 说明：如果修复包含方位值，则返回true。
>
> 返回值：boolean
## SpeedValid属性

?> 说明：如果修复包含速度值，则返回true。
>
> 返回值：boolean
## Altitude属性

?> 说明：获取或设置固定高度（米）。
>
> 参数：value，类型：double
>
> 返回值：double
## Speed属性

?> 说明：获取或设置固定速度（米/秒）。
>
> 参数：value，类型：float
>
> 返回值：float
## Time属性

?> 说明：获取或设置修复时间。
>
> 参数：value，类型：long
>
> 返回值：long
## Latitude属性

?> 说明：获取或设置固定纬度（从-90（南）到90（北）的度数）。
>
> 参数：value，类型：double
>
> 返回值：double
## Longitude属性

?> 说明：获取或设置固定经度（-180到180度，正值表示东半球）。
>
> 参数：value，类型：double
>
> 返回值：double
## AccuracyValid属性

?> 说明：如果修复包含精度值，则返回true。
>
> 返回值：boolean
## Bearing属性

?> 说明：获取或设置正北以东的方位角。
>
> 参数：value，类型：float
>
> 返回值：float

# GPSSatellite
完整类名：anywheresoftware.b4a.gps.GpsSatelliteWrapper
> 所有者：process

> 包装器：android.location.GpsSatellite

?> 说明：GPSSatellite对象保存有关GPS卫星的各种信息。带有可用卫星的列表将传递给GpsStatus事件。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## UsedInFix属性

?> 说明：测试此卫星是否用于计算最近的修复。
>
> 返回值：boolean
## Prn属性

?> 说明：返回卫星的PRN（伪随机数）。
>
> 返回值：int
## Elevation属性

?> 说明：返回以度（0-90）为单位的卫星高程。
>
> 返回值：float
## Azimuth属性

?> 说明：返回卫星方位角，单位为度（0-360）。
>
> 返回值：float
## Snr属性

?> 说明：返回卫星的信噪比。
>
> 返回值：float

# GPS
完整类名：anywheresoftware.b4a.gps.GPS
> 所有者：process

?> 说明：引发GPS事件的主要对象。
> 事件：
>
> LocationChanged (Location1 As Location)
>
> UserEnabled (Enabled As Boolean)
>
> GpsStatus (Satellites As List)
>
> NMEA (TimeStamp As Long, Sentence As String)

> 所需权限：
android.permission.ACCESS_FINE_LOCATION
## Initialize方法
**Initialize(EventName)**
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Start方法
**Start(ba,MinimumTime,MinimumDistance)**

?> 说明：开始侦听事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：MinimumTime，类型：long
>
> 参数：MinimumDistance，类型：float
>
> 返回值：void
## Stop方法
**Stop()**

?> 说明：停止收听GPS。您通常需要在Sub-Activity_Pause中调用Stop。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## GPSEnabled属性

?> 说明：测试用户是否已启用GPS。
>
> 返回值：boolean
## LocationSettingsIntent属性

?> 说明：返回用于显示全局位置设置的意图。
```vbnet

If GPS1.GPSEnabled = False Then StartActivity(GPS1.LocationSettingsIntent)
```

>
> 返回值：android.content.Intent

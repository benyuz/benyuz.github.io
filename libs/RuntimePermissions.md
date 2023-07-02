# RuntimePermissions

版本:1.2
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=RuntimePermissions)

# RuntimePermissions
完整类名：anywheresoftware.b4a.objects.RuntimePermissions
> 所有者：process
## GetSafeDirDefaultExternal方法
**GetSafeDirDefaultExternal(SubFolder)**

?> 说明：返回辅助存储设备上应用程序默认文件夹的路径。
```vbnet
AddManifestText(<uses-permission
android:name="android.permission.WRITE_EXTERNAL_STORAGE"
android:maxSdkVersion="18" />
)
```

>
> 参数：SubFolder，类型：java.lang.String
>
> 返回值：java.lang.String
## GetAllSafeDirsExternal方法
**GetAllSafeDirsExternal(SubFolder)**

?> 说明：返回一个数组，其中包含应用程序可用的所有外部文件夹。
>
> 参数：SubFolder，类型：java.lang.String
>
> 返回值：java.lang.String[]
## Check方法
**Check(Permission)**

?> 说明：检查应用程序是否已被授予指定的权限。
>
> 参数：Permission，类型：java.lang.String
>
> 返回值：boolean
## CheckAndRequest方法
**CheckAndRequest(ba,Permission)**

?> 说明：检查应用程序是否已被授予指定的权限。如果没有，则会向用户显示一个请求权限的对话框。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Permission，类型：java.lang.String
>
> 返回值：void
## PERMISSION_CALL_PHONE字段
>
> 返回值：java.lang.String
## PERMISSION_READ_CALENDAR字段
>
> 返回值：java.lang.String
## PERMISSION_ADD_VOICEMAIL字段
>
> 返回值：java.lang.String
## PERMISSION_ACCESS_COARSE_LOCATION字段
>
> 返回值：java.lang.String
## PERMISSION_READ_CONTACTS字段
>
> 返回值：java.lang.String
## PERMISSION_READ_PHONE_STATE字段
>
> 返回值：java.lang.String
## PERMISSION_SEND_SMS字段
>
> 返回值：java.lang.String
## PERMISSION_BODY_SENSORS字段
>
> 返回值：java.lang.String
## PERMISSION_READ_SMS字段
>
> 返回值：java.lang.String
## PERMISSION_POST_NOTIFICATIONS字段
>
> 返回值：java.lang.String
## PERMISSION_READ_EXTERNAL_STORAGE字段
>
> 返回值：java.lang.String
## PERMISSION_RECORD_AUDIO字段
>
> 返回值：java.lang.String
## PERMISSION_READ_CALL_LOG字段
>
> 返回值：java.lang.String
## PERMISSION_WRITE_EXTERNAL_STORAGE字段
>
> 返回值：java.lang.String
## PERMISSION_ACCESS_FINE_LOCATION字段
>
> 返回值：java.lang.String
## PERMISSION_ACCESS_CHECKIN_PROPERTIES字段
>
> 返回值：java.lang.String
## PERMISSION_WRITE_CONTACTS字段
>
> 返回值：java.lang.String
## PERMISSION_GET_ACCOUNTS字段
>
> 返回值：java.lang.String
## PERMISSION_PROCESS_OUTGOING_CALLS字段
>
> 返回值：java.lang.String
## PERMISSION_CAMERA字段
>
> 返回值：java.lang.String
## PERMISSION_WRITE_CALL_LOG字段
>
> 返回值：java.lang.String
## PERMISSION_USE_SIP字段
>
> 返回值：java.lang.String
## PERMISSION_RECEIVE_WAP_PUSH字段
>
> 返回值：java.lang.String
## PERMISSION_RECEIVE_MMS字段
>
> 返回值：java.lang.String
## PERMISSION_WRITE_CALENDAR字段
>
> 返回值：java.lang.String
## PERMISSION_RECEIVE_SMS字段
>
> 返回值：java.lang.String

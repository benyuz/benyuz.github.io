# Administrator

版本:1.1
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Administrator)

# AdminManager
完整类名：anywheresoftware.b4a.objects.AdminManager
> 所有者：process

?> 说明：有关详细信息，请参阅此链接。
## ResetPassword方法
**ResetPassword(NewPassword)**

?> 说明：将给定的密码设置为设备密码。
>
> 参数：NewPassword，类型：java.lang.String
>
> 返回值：boolean
## Disable方法
**Disable()**

?> 说明：禁用管理策略。
>
> 返回值：void
## Enable方法
**Enable(ba,Explanation)**

?> 说明：启用管理策略。用户将看到一个具有所需功能的对话框。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Explanation，类型：java.lang.String
>
> 返回值：void
## RequestNewPassword方法
**RequestNewPassword(ba)**

?> 说明：显示新密码活动。请注意，用户可能会取消更改。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## SetPasswordQuality方法
**SetPasswordQuality(QualityFlag,MinimumLength)**

?> 说明：设置设备密码允许的最小长度和质量。
```vbnet

manager.SetPasswordQuality(manager.PASSWORD_QUALITY_ALPHANUMERIC, 4)
```

>
> 参数：QualityFlag，类型：int
>
> 参数：MinimumLength，类型：int
>
> 返回值：void
## LockScreen方法
**LockScreen()**

?> 说明：立即锁定屏幕。需要策略文件中的强制锁定标记。
>
> 返回值：void
## Enabled属性

?> 说明：如果管理策略处于活动状态，则返回true。
>
> 返回值：boolean
## PasswordSufficient属性

?> 说明：测试当前密码是否符合要求。
>
> 返回值：boolean
## MaximumTimeToLock属性

?> 说明：设置设备锁定前的最长时间（以毫秒为单位）。
>
> 参数：value，类型：long
>
> 返回值：
## PASSWORD_QUALITY_UNSPECIFIED字段
>
> 返回值：int
## PASSWORD_QUALITY_ALPHABETIC字段
>
> 返回值：int
## PASSWORD_QUALITY_ALPHANUMERIC字段
>
> 返回值：int
## PASSWORD_QUALITY_NUMERIC字段
>
> 返回值：int

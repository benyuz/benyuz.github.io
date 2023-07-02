# Phone

版本:2.53
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Phone)

# SmsMessages
完整类名：anywheresoftware.b4a.phone.SmsWrapper
> 所有者：process

?> 说明：提供对存储的SMS消息的访问。
```vbnet

Dim SmsMessages1 As SmsMessages
Dim List1 As List
List1 = SmsMessages1.GetAllSince(DateTime.Add(DateTime.Now, 0, 0, -7))
For i = 0 To List1.Size - 1
	Dim Sms As Sms
	Sms = List1.Get(i)
	Log(Sms)
Next
```


> 所需权限：
android.permission.READ_SMS
## GetByType方法
**GetByType(Type)**

?> 说明：返回包含给定类型的所有消息的列表。类型应该是类型常量之一。
>
> 参数：Type，类型：int
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetAll方法
**GetAll()**

?> 说明：返回所有存储的消息。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetBetweenDates方法
**GetBetweenDates(StartDate,EndDate)**

?> 说明：返回给定日期之间的所有消息。起始值为包含值，结束值为独占值。
>
> 参数：StartDate，类型：long
>
> 参数：EndDate，类型：long
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetByThreadId方法
**GetByThreadId(ThreadId)**

?> 说明：返回一个列表，其中包含具有给定ThreadId的所有消息。
>
> 参数：ThreadId，类型：int
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetByPersonId方法
**GetByPersonId(PersonId)**

?> 说明：返回一个列表，其中包含从具有给定id的人收到的所有消息。
>
> 参数：PersonId，类型：int
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetByMessageId方法
**GetByMessageId(Id)**
>
> 参数：Id，类型：int
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetAllSince方法
**GetAllSince(Date)**

?> 说明：返回自给定日期以来的所有消息。
>
> 参数：Date，类型：long
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetUnreadMessages方法
**GetUnreadMessages()**

?> 说明：返回所有未读邮件。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## TYPE_SENT字段
>
> 返回值：int
## TYPE_FAILED字段
>
> 返回值：int
## TYPE_INBOX字段
>
> 返回值：int
## TYPE_QUEUED字段
>
> 返回值：int
## TYPE_UNKNOWN字段
>
> 返回值：int
## TYPE_OUTBOX字段
>
> 返回值：int
## TYPE_DRAFT字段
>
> 返回值：int

# Sms
完整类名：anywheresoftware.b4a.phone.SmsWrapper.Sms
> 所有者：process

?> 说明：表示SMS消息。
## Read字段

?> 说明：是否已阅读此消息。
>
> 返回值：boolean
## Type字段

?> 说明：消息类型。SmsMessages常量值之一。
>
> 返回值：int
## PersonId字段

?> 说明：发送邮件的人的id。
```vbnet
Contacts.GetById
```

>
> 返回值：int
## Address字段

?> 说明：消息地址。
>
> 返回值：java.lang.String
## ThreadId字段

?> 说明：线程id。
>
> 返回值：int
## Id字段

?> 说明：消息内部id。
>
> 返回值：int
## Body字段

?> 说明：消息正文。
>
> 返回值：java.lang.String
## Date字段

?> 说明：此邮件的日期。
>
> 返回值：long

# RingtoneManager
完整类名：anywheresoftware.b4a.phone.RingtoneManagerWrapper
> 所有者：process

?> 说明：RingtoneManager对象允许您设置或获取默认铃声。
```vbnet

Sub Process_Globals
	Private rm As RingtoneManager
End Sub

Sub Globals

End Sub

Sub Activity_Create(FirstTime As Boolean)
	rm.ShowRingtonePicker("rm", rm.TYPE_RINGTONE, True, "")
End Sub

Sub rm_PickerResult (Success As Boolean, Uri As String)
	If Success Then
		If Uri = "" Then
			ToastMessageShow("Silent was chosen", True)
		Else
			rm.Play(Uri)
		End If
	Else
		ToastMessageShow("Error loading ringtone.", True)
	End If	
End Sub
```

> 事件：
>
> PickerResult (Success As Boolean, Uri As String)

> 所需权限：
android.permission.WRITE_SETTINGS
## Play方法
**Play(ba,Uri)**

?> 说明：播放铃声Uri。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Uri，类型：java.lang.String
>
> 返回值：java.lang.Object
## Stop方法
**Stop(Ringtone)**

?> 说明：停止播放以前播放的铃声。
>
> 参数：Ringtone，类型：java.lang.Object
>
> 返回值：void
## GetDefault方法
**GetDefault(Type)**

?> 说明：返回特定类型的默认铃声的Uri。
>
> 参数：Type，类型：int
>
> 返回值：java.lang.String
## DeleteRingtone方法
**DeleteRingtone(Uri)**

?> 说明：删除给定的条目。
>
> 参数：Uri，类型：java.lang.String
>
> 返回值：void
## AddToMediaStore方法
**AddToMediaStore(Dir,FileName,Title,IsAlarm,IsNotification,IsRingtone,IsMusic)**

?> 说明：由于安卓系统中的限制，此方法不再有效。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：Title，类型：java.lang.String
>
> 参数：IsAlarm，类型：boolean
>
> 参数：IsNotification，类型：boolean
>
> 参数：IsRingtone，类型：boolean
>
> 参数：IsMusic，类型：boolean
>
> 返回值：java.lang.String
## SetDefault方法
**SetDefault(Type,Uri)**

?> 说明：设置给定类型的默认铃声。
>
> 参数：Type，类型：int
>
> 参数：Uri，类型：java.lang.String
>
> 返回值：void
## ShowRingtonePicker方法
**ShowRingtonePicker(ba,EventName,Type,IncludeSilence,ChosenRingtone)**

?> 说明：显示铃声选取器活动。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Type，类型：int
>
> 参数：IncludeSilence，类型：boolean
>
> 参数：ChosenRingtone，类型：java.lang.String
>
> 返回值：void
## GetContentDir方法
**GetContentDir()**

?> 说明：返回表示虚拟内容文件夹的字符串。这可用于使用MediaPlayer播放铃声。
>
> 返回值：java.lang.String
## TYPE_NOTIFICATION字段
>
> 返回值：int
## TYPE_RINGTONE字段
>
> 返回值：int
## TYPE_ALARM字段
>
> 返回值：int

# PhoneEvents
完整类名：anywheresoftware.b4a.phone.PhoneEvents
> 所有者：process

?> 说明：安卓操作系统会发送各种消息，通知应用程序系统中的更改。
> 事件：
>
> AirplaneModeChanged (State As Boolean, Intent As Intent)
>
> BatteryChanged (Level As Int, Scale As Int, Plugged As Boolean, Intent As Intent)
>
> ConnectivityChanged (NetworkType As String, State As String, Intent As Intent)
>
> DeviceStorageLow (Intent As Intent)
>
> DeviceStorageOk (Intent As Intent)
>
> PackageAdded (Package As String, Intent As Intent)
>
> PackageRemoved (Package As String, Intent As Intent)
>
> PhoneStateChanged (State As String, IncomingNumber As String, Intent As Intent)
>
> ScreenOff (Intent As Intent)
>
> ScreenOn (Intent As Intent)
>
> SmsDelivered (PhoneNumber As String, Intent As Intent)
>
> SmsSentStatus (Success As Boolean, ErrorMessage As String, PhoneNumber As String, Intent As Intent)
>
> Shutdown (Intent As Intent)
>
> TextToSpeechFinish (Intent As Intent)
>
> UserPresent (Intent As Intent)
## InitializeWithPhoneState方法
**InitializeWithPhoneState(ba,EventName,PhoneId)**

?> 说明：初始化对象并开始侦听事件。
```vbnet

Dim PhoneId As PhoneId
Dim PE As PhoneEvents
PE.InitializeWithPhoneState("PE", PhoneId)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：PhoneId，类型：anywheresoftware.b4a.phone.Phone.PhoneId
>
> 返回值：void
## StopListening方法
**StopListening()**

?> 说明：停止侦听事件。您可以稍后调用Initialize以再次开始侦听事件。
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象并开始侦听事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void

# SmsInterceptor
完整类名：anywheresoftware.b4a.phone.PhoneEvents.SMSInterceptor
> 所有者：process

?> 说明：收听传入的短信息。
> 事件：
>
> MessageReceived (From As String, Body As String) As Boolean
>
> MessageSent (MessageId As Int)

> 所需权限：
android.permission.RECEIVE_SMS
## Initialize2方法
**Initialize2(EventName,ba,Priority)**

?> 说明：初始化对象并开始侦听新消息。
>
> 参数：EventName，类型：java.lang.String
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Priority，类型：int
>
> 返回值：void
## ListenToOutgoingMessages方法
**ListenToOutgoingMessages()**

?> 说明：收听传出消息。发送消息时将引发MessageSent事件。
>
> 返回值：void
## StopListening方法
**StopListening()**

?> 说明：停止侦听事件。您可以稍后调用Initialize重新开始侦听。
>
> 返回值：void
## Initialize方法
**Initialize(EventName,ba)**

?> 说明：初始化对象并开始侦听新消息。
>
> 参数：EventName，类型：java.lang.String
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void

# Phone
完整类名：anywheresoftware.b4a.phone.Phone
> 所有者：process
## GetMaxVolume方法
**GetMaxVolume(Channel)**

?> 说明：获取给定频道的最大音量索引（值）。
>
> 参数：Channel，类型：int
>
> 返回值：int
## SetScreenOrientation方法
**SetScreenOrientation(ba,Orientation)**

?> 说明：更改当前活动方向。无法从服务模块调用此方法。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Orientation，类型：int
>
> 返回值：void
## GetNetworkType方法
**GetNetworkType()**

?> 说明：返回当前使用的蜂窝网络类型。
>
> 返回值：java.lang.String
## GetVolume方法
**GetVolume(Channel)**

?> 说明：返回指定通道的音量。
>
> 参数：Channel，类型：int
>
> 返回值：int
## ShellAsync方法
**ShellAsync(ba,Command,Args)**

?> 说明：Shell的异步版本。应与“等待”一起使用：
```vbnet

Dim p As Phone
Wait For (p.ShellAsync("ping", Array As String("-c", "1", "b4x.com"))) Complete (Success As Boolean, ExitValue As Int, StdOut As String, StdErr As String)
If Success Then
	Log(ExitValue)
	Log("Out: " & StdOut)
	Log("Err: "&  StdErr)
Else
	Log("Error: " & LastException)
End If
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Command，类型：java.lang.String
>
> 参数：Args，类型：java.lang.String[]
>
> 返回值：java.lang.Object
## GetSimOperator方法
**GetSimOperator()**

?> 说明：返回SIM卡提供商的代码。
>
> 返回值：java.lang.String
## SendBroadcastIntent方法
**SendBroadcastIntent(Intent)**

?> 说明：向所有侦听此类型意图的BroadcastReceiver发送意图。
```vbnet

Dim i As Intent
i.Initialize("android.intent.action.MEDIA_SCANNER_SCAN_FILE", _
	"file://" & File.Combine(File.DirRootExternal, "pictures/1.jpg"))
Dim p As Phone
p.SendBroadcastIntent(i)
```

>
> 参数：Intent，类型：android.content.Intent
>
> 返回值：void
## GetResourceDrawable方法
**GetResourceDrawable(ResourceId)**

?> 说明：返回一个内部可绘制对象。
```vbnet

Dim p As Phone
Dim bd As BitmapDrawable
bd = p.GetResourceDrawable(17301618)
Activity.AddMenuItem2("Menu1", "Menu1", bd.Bitmap)
```

>
> 参数：ResourceId，类型：int
>
> 返回值：android.graphics.drawable.Drawable
## IsNetworkRoaming方法
**IsNetworkRoaming()**

?> 说明：如果设备被认为在当前网络上漫游，则返回true。
>
> 返回值：boolean
## IsAirplaneModeOn方法
**IsAirplaneModeOn()**

?> 说明：测试手机“飞行模式”是否打开。
>
> 返回值：boolean
## GetPhoneType方法
**GetPhoneType()**

?> 说明：返回电话无线电类型。可能的值：CDMA、GSM、NONE。
>
> 返回值：java.lang.String
## Shell方法
**Shell(Command,Args,StdOut,StdErr)**

?> 说明：运行本机shell命令。由于操作系统的安全限制，许多命令无法访问。
```vbnet

Dim p As Phone
Dim sb As StringBuilder
sb.Initialize
p.Shell("df", Null, sb, Null)
Msgbox(sb.ToString, "Free space:")
```

>
> 参数：Command，类型：java.lang.String
>
> 参数：Args，类型：java.lang.String[]
>
> 参数：StdOut，类型：java.lang.StringBuilder
>
> 参数：StdErr，类型：java.lang.StringBuilder
>
> 返回值：int
## SetScreenBrightness方法
**SetScreenBrightness(ba,Value)**

?> 说明：设置当前活动的亮度。无法从服务模块调用此方法。
```vbnet

Sub Process_Globals
	Dim phone1 As Phone
End Sub

Sub Globals
	Dim sb As SeekBar
End Sub

Sub Activity_Create(FirstTime As Boolean)
	sb.Initialize("sb")
	sb.Max = 100
	sb.Value = 50
	Activity.AddView(sb, 10dip, 10dip, 90%x, 30dip)
End Sub
Sub sb_ValueChanged (Value As Int, UserChanged As Boolean)
	phone1.SetScreenBrightness(Max(Value, 5) / 100)
End Sub
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Value，类型：float
>
> 返回值：void
## SetRingerMode方法
**SetRingerMode(Mode)**

?> 说明：设置电话铃声模式。
```vbnet

Dim p As Phone
p.SetRingerMode(p.RINGER_VIBRATE)
```

>
> 参数：Mode，类型：int
>
> 返回值：void
## SetVolume方法
**SetVolume(Channel,VolumeIndex,ShowUI)**

?> 说明：设置指定通道的音量。
```vbnet

Dim p As Phone
p.SetVolume(p.VOLUME_MUSIC, 3, True)
```

>
> 参数：Channel，类型：int
>
> 参数：VolumeIndex，类型：int
>
> 参数：ShowUI，类型：boolean
>
> 返回值：void
## GetDataState方法
**GetDataState()**

?> 说明：返回当前蜂窝数据连接状态。
>
> 返回值：java.lang.String
## GetRingerMode方法
**GetRingerMode()**

?> 说明：返回电话振铃器模式。
>
> 返回值：int
## GetNetworkOperatorName方法
**GetNetworkOperatorName()**

?> 说明：返回当前注册操作员的名称。
>
> 返回值：java.lang.String
## HideKeyboard方法
**HideKeyboard(Activity)**

?> 说明：隐藏软键盘（如果显示）。
```vbnet

Dim p As Phone
p.HideKeyboard(Activity)
```

>
> 参数：Activity，类型：anywheresoftware.b4a.objects.ActivityWrapper
>
> 返回值：void
## SetMute方法
**SetMute(Channel,Mute)**

?> 说明：使给定频道静音或取消静音。
>
> 参数：Channel，类型：int
>
> 参数：Mute，类型：boolean
>
> 返回值：void
## GetSettings方法
**GetSettings(Settings)**

?> 说明：返回基于给定键的电话设置值。
```vbnet

Dim p As Phone
Log(p.GetSettings("android_id"))
```

>
> 参数：Settings，类型：java.lang.String
>
> 返回值：java.lang.String
## SdkVersion属性

?> 说明：返回一个描述SDK版本的整数。
>
> 返回值：int
## Model属性
>
> 返回值：java.lang.String
## Manufacturer属性
>
> 返回值：java.lang.String
## Product属性
>
> 返回值：java.lang.String
## VOLUME_MUSIC字段

?> 说明：音乐频道。
>
> 返回值：int
## RINGER_NORMAL字段

?> 说明：正常的电话铃声模式。
>
> 返回值：int
## RINGER_VIBRATE字段

?> 说明：手机铃声会振动并静音。
>
> 返回值：int
## VOLUME_RING字段

?> 说明：电话铃声频道。
>
> 返回值：int
## VOLUME_SYSTEM字段

?> 说明：系统声音通道。
>
> 返回值：int
## VOLUME_NOTIFICATION字段

?> 说明：通知频道。
>
> 返回值：int
## VOLUME_VOICE_CALL字段

?> 说明：语音呼叫频道。
>
> 返回值：int
## RINGER_SILENT字段

?> 说明：手机铃声将静音，不会振动。
>
> 返回值：int
## VOLUME_ALARM字段

?> 说明：报警通道。
>
> 返回值：int

# PhoneId
完整类名：anywheresoftware.b4a.phone.Phone.PhoneId
> 所有者：process

> 所需权限：
android.permission.READ_PHONE_STATE
## GetLine1Number方法
**GetLine1Number()**

?> 说明：返回SIM卡中配置的第1行的电话号码字符串。
>
> 返回值：java.lang.String
## GetSubscriberId方法
**GetSubscriberId()**

?> 说明：返回唯一的订阅者id。
>
> 返回值：java.lang.String
## GetDeviceId方法
**GetDeviceId()**

?> 说明：返回一个唯一的设备Id。如果设备Id不可用（通常在仅限wifi的设备上），则返回一个空字符串。
>
> 返回值：java.lang.String
## GetSimSerialNumber方法
**GetSimSerialNumber()**

?> 说明：返回SIM卡的序列号。
>
> 返回值：java.lang.String

# PhoneVibrate
完整类名：anywheresoftware.b4a.phone.Phone.PhoneVibrate
> 所有者：process

> 所需权限：
android.permission.VIBRATE
## Vibrate方法
**Vibrate(ba,TimeMs)**

?> 说明：在指定的持续时间内振动手机。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：TimeMs，类型：long
>
> 返回值：void

# PhoneWakeState
完整类名：anywheresoftware.b4a.phone.Phone.PhoneWakeState
> 所有者：process

?> 说明：PhoneWakeState对象允许您防止设备关闭屏幕。

> 所需权限：
android.permission.WAKE_LOCK
## ReleaseKeepAlive方法
**ReleaseKeepAlive()**

?> 说明：释放电源锁定并允许设备进入睡眠状态。
>
> 返回值：void
## PartialLock方法
**PartialLock(ba)**

?> 说明：获取部分锁定。这将防止CPU进入睡眠状态，即使用户按下电源按钮。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## KeepAlive方法
**KeepAlive(ba,BrightScreen)**

?> 说明：防止设备进入睡眠状态。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：BrightScreen，类型：boolean
>
> 返回值：void
## ReleasePartialLock方法
**ReleasePartialLock()**

?> 说明：释放以前通过调用PartialLock获取的部分锁。
>
> 返回值：void

# PhoneIntents
完整类名：anywheresoftware.b4a.phone.Phone.PhoneIntents
> 所有者：process

?> 说明：此对象包含创建intents对象的方法。在使用intent调用StartActivity之前，intent不会执行任何操作。
## PlayAudio方法
**PlayAudio(Dir,File)**

?> 说明：创建一个意图，该意图将开始使用默认播放器播放给定的音频文件。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：File，类型：java.lang.String
>
> 返回值：android.content.Intent
## PlayVideo方法
**PlayVideo(Dir,File)**

?> 说明：创建一个意图，该意图将开始使用默认播放器播放给定的视频文件。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：File，类型：java.lang.String
>
> 返回值：android.content.Intent
## OpenBrowser方法
**OpenBrowser(Uri)**

?> 说明：创建将打开指定URI的意图。
```vbnet

StartActivity (PhoneIntents.OpenBrowser("http://www.google.com"))
```

>
> 参数：Uri，类型：java.lang.String
>
> 返回值：android.content.Intent

# PhoneCalls
完整类名：anywheresoftware.b4a.phone.Phone.PhoneCalls
> 所有者：process

?> 说明：此对象创建启动电话应用程序的意图。

> 所需权限：
android.permission.CALL_PHONE
## Call方法
**Call(PhoneNumber)**

?> 说明：创建一个将呼叫电话号码的意图。
```vbnet

Dim p As PhoneCalls
StartActivity(p.Call("1234567890"))
```

>
> 参数：PhoneNumber，类型：java.lang.String
>
> 返回值：android.content.Intent

# PhoneSms
完整类名：anywheresoftware.b4a.phone.Phone.PhoneSms
> 所有者：process

> 所需权限：
android.permission.SEND_SMS
## Send2方法
**Send2(PhoneNumber,Text,ReceiveSentNotification,ReceiveDeliveredNotification)**

?> 说明：发送Sms消息。请注意，此方法实际上发送消息（与大多数其他方法不同
>
> 参数：PhoneNumber，类型：java.lang.String
>
> 参数：Text，类型：java.lang.String
>
> 参数：ReceiveSentNotification，类型：boolean
>
> 参数：ReceiveDeliveredNotification，类型：boolean
>
> 返回值：void
## Send方法
**Send(PhoneNumber,Text)**

?> 说明：发送Sms消息。请注意，此方法实际上发送消息（与大多数其他方法不同
>
> 参数：PhoneNumber，类型：java.lang.String
>
> 参数：Text，类型：java.lang.String
>
> 返回值：void

# Email
完整类名：anywheresoftware.b4a.phone.Phone.Email
> 所有者：process

?> 说明：使用电子邮件对象，您可以创建一个包含完整电子邮件的意向。
```vbnet

Dim Message As Email
Message.To.Add("SomeEmail@example.com")
Message.Attachments.Add(File.Combine(File.DirRootExternal, "SomeFile.txt"))
StartActivity(Message.GetIntent)
```

## GetHtmlIntent方法
**GetHtmlIntent()**

?> 说明：返回应该与StartActivity一起发送的意向。
>
> 返回值：android.content.Intent
## GetIntent方法
**GetIntent()**

?> 说明：返回应该与StartActivity一起发送的意向。
>
> 返回值：android.content.Intent
## CC字段
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## BCC字段
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## To字段
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## Body字段
>
> 返回值：java.lang.String
## Attachments字段
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## Subject字段
>
> 返回值：java.lang.String

# LogCat
完整类名：anywheresoftware.b4a.phone.Phone.LogCat
> 所有者：process

?> 说明：LogCat允许您读取内部电话日志。
> 事件：
>
> LogCatData (Buffer() As Byte, Length As Int)
## LogCatStop方法
**LogCatStop()**

?> 说明：停止跟踪日志。
>
> 返回值：void
## LogCatStart方法
**LogCatStart(ba,Args,EventName)**

?> 说明：开始跟踪日志。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Args，类型：java.lang.String[]
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void

# ContentChooser
完整类名：anywheresoftware.b4a.phone.Phone.ContentChooser
> 所有者：process

?> 说明：ContentChooser对象允许用户使用其他已安装的应用程序选择特定类型的内容。
> 事件：
>
> Result (Success As Boolean, Dir As String, FileName As String)
## Show方法
**Show(ba,Mime,Title)**

?> 说明：将请求发送到系统。如果有多个应用程序支持给定的Mime，则会向用户显示包含这些应用程序的列表。
```vbnet

CC.Show("image/*", "Choose image")
CC.Show("audio/*", "Choose audio file")
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Mime，类型：java.lang.String
>
> 参数：Title，类型：java.lang.String
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(EventName)**

?> 说明：初始化对象并设置将处理Result事件的Sub。
```vbnet

Dim CC As ContentChooser
CC.Initialize("CC")
```

>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void

# VoiceRecognition
完整类名：anywheresoftware.b4a.phone.Phone.VoiceRecognition
> 所有者：process

?> 说明：大多数安卓设备支持语音识别（语音转文本）。通常，该服务通过将音频流发送到某个外部服务器来工作
> 事件：
>
> Result (Success As Boolean, Texts As List)
## Listen方法
**Listen(ba)**

?> 说明：开始倾听。结果到达时将引发Result事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Listen2方法
**Listen2(ba,RecognizeIntent)**

?> 说明：类似于听。允许您自己构建意图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：RecognizeIntent，类型：android.content.Intent
>
> 返回值：void
## IsSupported方法
**IsSupported()**

?> 说明：测试此设备是否支持语音识别。
>
> 返回值：boolean
## Initialize方法
**Initialize(EventName)**

?> 说明：初始化对象并设置将捕获Result事件的Sub。
```vbnet

Dim VR As VoiceRecognition
VR.Initialize("VR")
```

>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Language属性

?> 说明：设置使用的语言。默认情况下，将使用设备默认语言。
```vbnet

VR.Language = "en"
```

>
> 参数：value，类型：java.lang.String
>
> 返回值：
## Prompt属性

?> 说明：设置除了“立即发言”消息之外，“立即发言“对话框中显示的提示。
>
> 参数：value，类型：java.lang.String
>
> 返回值：

# PhoneOrientation
完整类名：anywheresoftware.b4a.phone.Phone.PhoneOrientation
> 所有者：process

?> 说明：此对象可访问内部方位传感器。
> 事件：
>
> OrientationChanged (Azimuth As Float, Pitch As Float, Roll As Float)
## StartListening方法
**StartListening(ba,EventName)**

?> 说明：开始侦听OrientationChanged事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## StopListening方法
**StopListening(ba)**

?> 说明：停止侦听事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void

# PhoneAccelerometer
完整类名：anywheresoftware.b4a.phone.Phone.PhoneAccelerometer
> 所有者：process

?> 说明：此对象可访问内部加速计传感器。
> 事件：
>
> AccelerometerChanged (X As Float, Y As Float, Z As Float)
## StartListening方法
**StartListening(ba,EventName)**

?> 说明：开始侦听加速度计更改的事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## StopListening方法
**StopListening(ba)**

?> 说明：停止侦听事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void

# PhoneSensors
完整类名：anywheresoftware.b4a.phone.Phone.PhoneSensors
> 所有者：process

?> 说明：PhoneSensors对象允许您监听其中一个设备传感器的变化。
> 事件：
>
> SensorChanged (Values() As Float)
## Initialize2方法
**Initialize2(SensorType,SensorDelay)**

?> 说明：初始化对象并设置传感器类型和传感器事件率。
>
> 参数：SensorType，类型：int
>
> 参数：SensorDelay，类型：int
>
> 返回值：void
## StartListening方法
**StartListening(ba,EventName)**

?> 说明：开始侦听传感器事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：boolean
## StopListening方法
**StopListening(ba)**

?> 说明：停止侦听事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Initialize方法
**Initialize(SensorType)**

?> 说明：初始化对象并设置传感器类型（type_常量之一）。
>
> 参数：SensorType，类型：int
>
> 返回值：void
## Accuracy属性

?> 说明：返回事件精度，介于0（不可靠）到3（最大精度）之间。
>
> 返回值：int
## MaxValue属性

?> 说明：返回此传感器的最大值。
>
> 返回值：float
## Timestamp属性

?> 说明：返回以纳秒为单位测量的事件时间戳。请注意，实际值在不同的设备上具有不同的含义。
>
> 返回值：long
## TYPE_ACCELEROMETER字段

?> 说明：三个值-每个轴（X、Y和Z）的加速度测量单位为米/秒^2。
>
> 返回值：int
## TYPE_MAGNETIC_FIELD字段

?> 说明：三个值-X、Y和Z轴的环境磁场测量单位为微特斯拉。
>
> 返回值：int
## TYPE_PROXIMITY字段

?> 说明：单一值-以厘米为单位测量的接近度。大多数设备将只返回表示“近”和“远”的两个可能值。
>
> 返回值：int
## TYPE_PRESSURE字段

?> 说明：单一值-大气压力。
>
> 返回值：int
## TYPE_LIGHT字段

?> 说明：单一值-环境光照水平，单位为SI勒克斯。
>
> 返回值：int
## TYPE_ORIENTATION字段

?> 说明：三个值-方位角、俯仰和滚转的方向（以度为单位）。
>
> 返回值：int
## TYPE_TEMPERATURE字段

?> 说明：单一值-环境温度。
>
> 返回值：int
## TYPE_GYROSCOPE字段

?> 说明：三个值-围绕三个轴中的每一个测量的角速度，单位为弧度/秒。
>
> 返回值：int

# PackageManager
完整类名：anywheresoftware.b4a.phone.PackageManagerWrapper
> 所有者：process

?> 说明：PackageManager允许您查找有关已安装应用程序的信息。
## GetVersionName方法
**GetVersionName(Package)**

?> 说明：返回应用程序版本名称。
>
> 参数：Package，类型：java.lang.String
>
> 返回值：java.lang.String
## GetInstalledPackages方法
**GetInstalledPackages()**

?> 说明：返回已安装程序包的列表。
```vbnet

Dim pm As PackageManager
Dim packages As List
packages = pm.GetInstalledPackages
For i = 0 To packages.Size - 1
	Log(packages.Get(i))
Next
```

>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetVersionCode方法
**GetVersionCode(Package)**

?> 说明：返回应用程序版本代码。
>
> 参数：Package，类型：java.lang.String
>
> 返回值：int
## GetApplicationIntent方法
**GetApplicationIntent(Package)**

?> 说明：返回可用于启动给定应用程序的Intent对象。
```vbnet

Dim in As Intent
Dim pm As PackageManager
in = pm.GetApplicationIntent("com.google.android.youtube")
If in.IsInitialized Then StartActivity(in)
StartActivity(in)
```

>
> 参数：Package，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.IntentWrapper
## QueryIntentActivities方法
**QueryIntentActivities(Intent)**

?> 说明：返回一个列表，其中包含可以处理给定意图的已安装活动。
```vbnet

Dim pm As PackageManager
Dim Intent1 As Intent
Intent1.Initialize(Intent1.ACTION_VIEW, "file://")
Intent1.SetType("text/*")
For Each cn As String In pm.QueryIntentActivities(Intent1)
	Log(cn)
Next
```

>
> 参数：Intent，类型：android.content.Intent
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetApplicationLabel方法
**GetApplicationLabel(Package)**

?> 说明：返回应用程序标签。
>
> 参数：Package，类型：java.lang.String
>
> 返回值：java.lang.String
## GetApplicationIcon方法
**GetApplicationIcon(Package)**

?> 说明：返回应用程序图标。
```vbnet

Dim pm As PackageManager
Activity.Background = pm.GetApplicationIcon("com.google.android.youtube")
```

>
> 参数：Package，类型：java.lang.String
>
> 返回值：android.graphics.drawable.Drawable

# Contacts
完整类名：anywheresoftware.b4a.phone.ContactsWrapper
> 所有者：process

?> 说明：Contacts对象允许您访问设备存储的联系人。
```vbnet

Dim Contacts1 As Contacts
Dim listOfContacts As List
listOfContacts = Contacts1.FindByName("John", False)
For i = 0 To listOfContacts.Size - 1
	Dim Contact As Contact
	Contact = listOfContacts.Get(i)
	Log(Contact) 'will print the fields to the LogCat
	Dim photo As Bitmap
	photo = Contact.GetPhoto
	If photo <> Null Then Activity.SetBackgroundImage(photo)
	Dim emails As Map
	emails = Contact.GetEmails
	If emails.Size > 0 Then Log("Email addresses: " & emails)
	Dim phones As Map
	phones = Contact.GetPhones
	If phones.Size > 0 Then Log("Phone numbers: " & phones)
Next
```


> 所需权限：
android.permission.READ_CONTACTS
## FindByMail方法
**FindByMail(Email,Exact)**

?> 说明：返回联系人对象列表，其中包含与给定电子邮件匹配的所有联系人。
>
> 参数：Email，类型：java.lang.String
>
> 参数：Exact，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetAll方法
**GetAll()**

?> 说明：返回包含所有联系人的联系人对象列表。这个列表可能非常大。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetById方法
**GetById(Id)**

?> 说明：返回具有指定Id的联系人。
>
> 参数：Id，类型：int
>
> 返回值：anywheresoftware.b4a.phone.ContactsWrapper.Contact
## FindByName方法
**FindByName(Name,Exact)**

?> 说明：返回所有联系人与给定名称匹配的联系人对象列表。
>
> 参数：Name，类型：java.lang.String
>
> 参数：Exact，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.collections.List

# Contact
完整类名：anywheresoftware.b4a.phone.ContactsWrapper.Contact
> 所有者：process

?> 说明：表示单个联系人。
## GetEmails方法
**GetEmails()**

?> 说明：返回一个以联系人电子邮件地址为键、电子邮件类型为值的Map。
>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## GetPhones方法
**GetPhones()**

?> 说明：返回一张地图，其中所有联系人的电话号码为键，电话类型为值。
>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## GetPhoto方法
**GetPhoto()**

?> 说明：返回联系人照片，如果没有附加照片，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## PHONE_HOME字段
>
> 返回值：int
## EMAIL_HOME字段
>
> 返回值：int
## PHONE_CUSTOM字段
>
> 返回值：int
## TimesContacted字段

?> 说明：已联系此联系人的次数。
>
> 返回值：int
## EMAIL_OTHER字段
>
> 返回值：int
## PHONE_MOBILE字段
>
> 返回值：int
## PHONE_FAX_WORK字段
>
> 返回值：int
## Name字段

?> 说明：联系人姓名。
>
> 返回值：java.lang.String
## EMAIL_CUSTOM字段
>
> 返回值：int
## EMAIL_WORK字段
>
> 返回值：int
## LastTimeContacted字段

?> 说明：上次联系此联系人的时间。值是一个刻度值。
>
> 返回值：long
## PHONE_WORK字段
>
> 返回值：int
## DisplayName字段

?> 说明：显示的名称。如果Name不为空，则等于Name，否则等于联系人的第一个电子邮件地址。
>
> 返回值：java.lang.String
## PhoneNumber字段

?> 说明：主要电话号码。
>
> 返回值：java.lang.String
## PHONE_FAX_HOME字段
>
> 返回值：int
## PHONE_PAGER字段
>
> 返回值：int
## PHONE_OTHER字段
>
> 返回值：int
## Id字段

?> 说明：内部Id。
>
> 返回值：int
## Starred字段

?> 说明：此联系人是否为“常用”联系人。
>
> 返回值：boolean
## EMAIL_MOBILE字段
>
> 返回值：int
## Notes字段
>
> 返回值：java.lang.String

# Contacts2
完整类名：anywheresoftware.b4a.phone.Contacts2Wrapper
> 所有者：process

?> 说明：Contacts2对象允许您访问设备存储的联系人。此类型基于Android 2.0及更高版本支持的新API。
```vbnet

Dim Contacts2 As Contacts2
Dim listOfContacts As List
listOfContacts = Contacts2.FindByName("John", False, True, True)
For i = 0 To listOfContacts.Size - 1
    Dim Contact As Contact
    Contact = listOfContacts.Get(i)
    Log(Contact) 'will print the fields to the LogCat
    Dim photo As Bitmap
    photo = Contact.GetPhoto
    If photo <> Null Then Activity.SetBackgroundImage(photo)
    Dim emails As Map
    emails = Contact.GetEmails
    If emails.Size > 0 Then Log("Email addresses: " & emails)
    Dim phones As Map
    phones = Contact.GetPhones
    If phones.Size > 0 Then Log("Phone numbers: " & phones)
Next 
```

> 事件：
>
> Complete (ListOfContacts As List)

> 所需权限：
android.permission.READ_CONTACTS
## FindByMail方法
**FindByMail(Email,Exact,IncludePhoneNumber,IncludeNotes)**

?> 说明：返回联系人对象列表，其中包含与给定电子邮件匹配的所有联系人。
>
> 参数：Email，类型：java.lang.String
>
> 参数：Exact，类型：boolean
>
> 参数：IncludePhoneNumber，类型：boolean
>
> 参数：IncludeNotes，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetAll方法
**GetAll(IncludePhoneNumber,IncludeNotes)**

?> 说明：返回包含所有联系人的联系人对象列表。这个列表可能非常大。
>
> 参数：IncludePhoneNumber，类型：boolean
>
> 参数：IncludeNotes，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetContactsByQuery方法
**GetContactsByQuery(Query,Arguments,IncludePhoneNumber,IncludeNotes)**

?> 说明：返回基于指定查询和参数的联系人列表。
>
> 参数：Query，类型：java.lang.String
>
> 参数：Arguments，类型：java.lang.String[]
>
> 参数：IncludePhoneNumber，类型：boolean
>
> 参数：IncludeNotes，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetContactsAsync方法
**GetContactsAsync(ba,EventName,Query,Arguments,IncludePhoneNumber,IncludeNotes)**

?> 说明：此方法是GetContactsByQuery的异步版本。一旦列表准备就绪，将引发“完成”事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Query，类型：java.lang.String
>
> 参数：Arguments，类型：java.lang.String[]
>
> 参数：IncludePhoneNumber，类型：boolean
>
> 参数：IncludeNotes，类型：boolean
>
> 返回值：void
## GetById方法
**GetById(Id,IncludePhoneNumber,IncludeNotes)**

?> 说明：返回具有指定Id的联系人。
>
> 参数：Id，类型：int
>
> 参数：IncludePhoneNumber，类型：boolean
>
> 参数：IncludeNotes，类型：boolean
>
> 返回值：anywheresoftware.b4a.phone.ContactsWrapper.Contact
## FindByName方法
**FindByName(Name,Exact,IncludePhoneNumber,IncludeNotes)**

?> 说明：返回所有联系人与给定名称匹配的联系人对象列表。
>
> 参数：Name，类型：java.lang.String
>
> 参数：Exact，类型：boolean
>
> 参数：IncludePhoneNumber，类型：boolean
>
> 参数：IncludeNotes，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.collections.List

# CallLog
完整类名：anywheresoftware.b4a.phone.CallLogWrapper
> 所有者：process

?> 说明：CallLog允许您浏览呼叫日志。
```vbnet

Dim Calls As List
Dim CallLog As CallLog
calls = CallLog.GetAll(10) 'Get the last 10 calls
For i = 0 To calls.Size - 1
	Dim c As CallItem
	c = calls.Get(i)
	Dim callType, name As String
	Select c.CallType
		Case c.TYPE_INCOMING
			callType="Incoming"
		Case c.TYPE_MISSED
			callType = "Missed"
		Case c.TYPE_OUTGOING
			callType = "Outgoing"
	End Select
	name = c.CachedName
	If name = "" Then name = "N/A"
	Log("Number=" & c.Number & ", Name=" & name _
		& ", Type=" & callType & ", Date=" & DateTime.Date(c.Date))
Next
```


> 所需权限：
android.permission.READ_CONTACTS
android.permission.READ_CALL_LOG
## GetAll方法
**GetAll(Limit)**

?> 说明：以CallItems列表的形式返回按日期（降序）排序的所有调用。
>
> 参数：Limit，类型：int
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetSince方法
**GetSince(Date,Limit)**

?> 说明：返回日期值大于指定值的所有CallItems。
>
> 参数：Date，类型：long
>
> 参数：Limit，类型：int
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetById方法
**GetById(Id)**

?> 说明：返回具有指定Id的CallItem。
>
> 参数：Id，类型：int
>
> 返回值：anywheresoftware.b4a.phone.CallLogWrapper.CallItem

# CallItem
完整类名：anywheresoftware.b4a.phone.CallLogWrapper.CallItem
> 所有者：process

?> 说明：表示呼叫日志中的单个呼叫。有关详细信息，请参阅调用日志。
## Number字段

?> 说明：呼叫电话号码。
>
> 返回值：java.lang.String
## TYPE_MISSED字段
>
> 返回值：int
## CallType字段

?> 说明：呼叫类型。此值与其中一个TYPE常量匹配。
>
> 返回值：int
## Duration字段

?> 说明：呼叫持续时间（秒）。
>
> 返回值：long
## Id字段

?> 说明：调用内部id。
>
> 返回值：int
## TYPE_INCOMING字段
>
> 返回值：int
## TYPE_OUTGOING字段
>
> 返回值：int
## Date字段

?> 说明：以刻度衡量的呼叫日期。
>
> 返回值：long
## CachedName字段

?> 说明：返回呼叫时分配给此呼叫号码的缓存名称。
>
> 返回值：java.lang.String

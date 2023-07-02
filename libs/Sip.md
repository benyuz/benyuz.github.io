# Sip

版本:1.0
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Sip)

# Sip
完整类名：anywheresoftware.b4a.objects.SIP
> 所有者：process

?> 说明：提供对Voip/Sip服务的访问。仅支持Android 2.3（API 9）及以上版本。
> 事件：
>
> Registering
>
> RegistrationDone (ExpiryTime As Long)
>
> RegistrationFailed (ErrorCode As Int, ErrorMessage As String)
>
> CallEstablished
>
> CallEnded
>
> Calling
>
> CallError (ErrorCode As Int, ErrorMessage As String)
>
> CallRinging (IncomingCall As SipAudioCall)

> 所需权限：
android.permission.USE_SIP
android.permission.INTERNET
android.permission.RECORD_AUDIO
android.permission.ACCESS_WIFI_STATE
android.permission.WAKE_LOCK
android.permission.MODIFY_AUDIO_SETTINGS
## Initialize方法
**Initialize(EventName,User,Host,Password,ba)**

?> 说明：初始化对象。
>
> 参数：EventName，类型：java.lang.String
>
> 参数：User，类型：java.lang.String
>
> 参数：Host，类型：java.lang.String
>
> 参数：Password，类型：java.lang.String
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## MakeCall方法
**MakeCall(ba,TargetUri,TimeoutSeconds)**

?> 说明：进行音频通话。此方法只能在注册后调用。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：TargetUri，类型：java.lang.String
>
> 参数：TimeoutSeconds，类型：int
>
> 返回值：anywheresoftware.b4a.objects.SIP.SipAudioCallWrapper
## Close方法
**Close()**

?> 说明：关闭连接。
>
> 返回值：void
## Register方法
**Register(ba)**

?> 说明：向服务器发送注册请求。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Initialize2方法
**Initialize2(EventName,Uri,Password,ba)**

?> 说明：初始化对象。
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Uri，类型：java.lang.String
>
> 参数：Password，类型：java.lang.String
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Port属性

?> 说明：设置连接端口。
>
> 参数：p，类型：int
>
> 返回值：
## ProfileName属性

?> 说明：设置用户定义的配置文件名称。
>
> 参数：s，类型：java.lang.String
>
> 返回值：
## OutboundProxy属性

?> 说明：设置出站代理地址。
>
> 参数：v，类型：java.lang.String
>
> 返回值：
## SendKeepAlive属性

?> 说明：设置是否自动发送保持活动的消息。
>
> 参数：b，类型：boolean
>
> 返回值：
## IsVoipSupported属性

?> 说明：测试此设备是否支持Voip。
>
> 返回值：boolean
## AutoRegistration属性

?> 说明：设置Sip管理器是否会在需要时自动注册。
>
> 参数：b，类型：boolean
>
> 返回值：
## IsSipSupported属性

?> 说明：测试设备上是否支持Sip API。
>
> 返回值：boolean
## DisplayName属性

?> 说明：设置用户显示名称。
>
> 参数：s，类型：java.lang.String
>
> 返回值：
## Protocol属性

?> 说明：设置协议。“TCP”或“UDP”。
>
> 参数：s，类型：java.lang.String
>
> 返回值：
## IsInitialized属性

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean

# SipAudioCall
完整类名：anywheresoftware.b4a.objects.SIP.SipAudioCallWrapper
> 所有者：process

> 包装器：android.net.sip.SipAudioCall

?> 说明：表示音频呼叫。
## AnswerCall方法
**AnswerCall(TimeoutSeconds)**

?> 说明：接听来电。
>
> 参数：TimeoutSeconds，类型：int
>
> 返回值：void
## StartAudio方法
**StartAudio()**

?> 说明：启动通话的音频。应在CallEstablished事件中调用。
>
> 返回值：void
## ToggleMute方法
**ToggleMute()**

?> 说明：切换麦克风静音。
>
> 返回值：void
## SendDtmf方法
**SendDtmf(Code)**

?> 说明：发送Dtmf音调。值可以是0-15，其中0-9是数字，10是“*”，11是“#”，12-15是“A”-“D”。
>
> 参数：Code，类型：int
>
> 返回值：void
## EndCall方法
**EndCall()**

?> 说明：结束当前呼叫。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## IsInCall属性

?> 说明：测试呼叫是否已建立。
>
> 返回值：boolean
## IsMuted属性

?> 说明：测试麦克风是否静音。
>
> 返回值：boolean
## PeerUri属性

?> 说明：获取对等Uri。
>
> 返回值：java.lang.String
## SpeakerMode属性

?> 说明：设置扬声器模式。
>
> 参数：b，类型：boolean
>
> 返回值：

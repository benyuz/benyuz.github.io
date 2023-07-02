# TTS

版本:1.01
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=TTS)

# TTS
完整类名：anywheresoftware.b4a.obejcts.TTS
> 所有者：process

> 包装器：android.speech.tts.TextToSpeech

?> 说明：将文本合成语音并播放。
> 事件：
>
> Ready (Success As Boolean)
## Speak方法
**Speak(Text,ClearQueue)**

?> 说明：说出给定的文本。
>
> 参数：Text，类型：java.lang.String
>
> 参数：ClearQueue，类型：boolean
>
> 返回值：void
## SetLanguage方法
**SetLanguage(Language,Country)**

?> 说明：设置口语。
>
> 参数：Language，类型：java.lang.String
>
> 参数：Country，类型：java.lang.String
>
> 返回值：boolean
## Stop方法
**Stop()**

?> 说明：停止说出任何当前正在播放的文本（并取消队列中的文本）。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Release方法
**Release()**

?> 说明：释放与此对象相关的任何资源。在使用之前，您需要再次初始化该对象。
>
> 返回值：void
## Pitch属性

?> 说明：设置间距值。默认值为1。
```vbnet
TTS1.Pitch = 1.5
```

>
> 参数：value，类型：float
>
> 返回值：
## SpeechRate属性

?> 说明：设置语音速率。默认值为1。
```vbnet
TTS1.SpeechRate = 0.5
```

>
> 参数：value，类型：float
>
> 返回值：

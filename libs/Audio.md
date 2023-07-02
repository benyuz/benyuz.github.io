# Audio

版本:1.71
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=Audio)

# VideoView
完整类名：anywheresoftware.b4a.audio.VideoViewWrapper
> 所有者：activity

> 包装器：android.widget.VideoView

?> 说明：VideoView是一种允许您在应用程序中播放视频媒体的视图。
```vbnet

Sub Globals
	Dim vv As VideoView
End Sub
Sub Activity_Create(FirstTime As Boolean)
	vv.Initialize("vv")
	Activity.AddView(vv, 10dip, 10dip, 250dip, 250dip)
	vv.LoadVideo(File.DirRootExternal, "somefile.mp4")
	vv.Play
End Sub
Sub vv_Complete
	Log("Playing completed")
End Sub
```

> 事件：
>
> Complete
## Pause方法
**Pause()**

?> 说明：暂停播放。
>
> 返回值：void
## Stop方法
**Stop()**

?> 说明：停止播放。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象并设置将处理事件的子对象的名称。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## LoadVideo方法
**LoadVideo(Dir,FileName)**

?> 说明：加载视频文件并准备播放。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SetLayout方法
**SetLayout(arg0,arg1,arg2,arg3)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 参数：arg2，类型：int
>
> 参数：arg3，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(arg0,arg1,arg2,arg3)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 参数：arg2，类型：int
>
> 参数：arg3，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(arg0)**
>
> 参数：arg0，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(arg0,arg1,arg2)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 参数：arg2，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Play方法
**Play()**

?> 说明：开始或继续播放。
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## toString方法
**toString()**
>
> 返回值：java.lang.String
## IsPlaying方法
**IsPlaying()**

?> 说明：测试当前是否正在播放视频。
>
> 返回值：boolean
## SetLayoutAnimated方法
**SetLayoutAnimated(arg0,arg1,arg2,arg3,arg4)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 参数：arg2，类型：int
>
> 参数：arg3，类型：int
>
> 参数：arg4，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## Left属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Position属性

?> 说明：获取或设置播放位置（以毫秒为单位）。
>
> 参数：v，类型：int
>
> 返回值：int
## Parent属性
>
> 返回值：java.lang.Object
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Duration属性

?> 说明：获取视频持续时间（以毫秒为单位）。
>
> 返回值：int
## MediaControllerEnabled属性

?> 说明：设置是否启用媒体控制器。它在默认情况下处于启用状态。
>
> 参数：v，类型：boolean
>
> 返回值：
## Top属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## Visible属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Padding属性
>
> 参数：arg0，类型：int[]
>
> 返回值：int[]
## Height属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## Tag属性
>
> 参数：arg0，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性
>
> 参数：arg0，类型：int
>
> 返回值：int

# SoundPool
完整类名：anywheresoftware.b4a.audio.SoundPoolWrapper
> 所有者：process

> 包装器：android.media.SoundPool

?> 说明：SoundPool包含一组可以低延迟播放的短声音。
## Load方法
**Load(Dir,File)**

?> 说明：加载声音文件并返回声音LoadId。
```vbnet

Dim LoadId As Int
LoadId = SP.Load(File.DirAssets, "sound.wav")
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：File，类型：java.lang.String
>
> 返回值：int
## Pause方法
**Pause(PlayId)**

?> 说明：暂停具有给定播放ID的流。
>
> 参数：PlayId，类型：int
>
> 返回值：void
## Stop方法
**Stop(PlayId)**

?> 说明：停止具有给定播放ID的流。
>
> 参数：PlayId，类型：int
>
> 返回值：void
## SetRate方法
**SetRate(PlayId,Rate)**

?> 说明：设置具有给定PlayId的流的速率。值介于0到2之间。
>
> 参数：PlayId，类型：int
>
> 参数：Rate，类型：float
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(MaxStreams)**

?> 说明：初始化SoundPool并设置同时流的最大数量。
>
> 参数：MaxStreams，类型：int
>
> 返回值：void
## Play方法
**Play(LoadId,LeftVolume,RightVolume,Priority,Loop,Rate)**

?> 说明：播放具有匹配LoadId的声音并返回PlayId。如果出现错误，则返回0。
>
> 参数：LoadId，类型：int
>
> 参数：LeftVolume，类型：float
>
> 参数：RightVolume，类型：float
>
> 参数：Priority，类型：int
>
> 参数：Loop，类型：int
>
> 参数：Rate，类型：float
>
> 返回值：int
## Unload方法
**Unload(LoadId)**

?> 说明：卸载具有给定LoadId的流。
>
> 参数：LoadId，类型：int
>
> 返回值：void
## SetVolume方法
**SetVolume(PlayId,Left,Right)**

?> 说明：设置具有给定PlayId的流的音量。值介于0到1之间。
>
> 参数：PlayId，类型：int
>
> 参数：Left，类型：float
>
> 参数：Right，类型：float
>
> 返回值：void
## Release方法
**Release()**

?> 说明：释放分配给此对象的所有资源。
>
> 返回值：void
## Resume方法
**Resume(PlayId)**

?> 说明：恢复具有给定播放ID的流。
>
> 参数：PlayId，类型：int
>
> 返回值：void

# MediaPlayerStream
完整类名：anywheresoftware.b4a.audio.MediaPlayerStreamWrapper
> 所有者：process

?> 说明：MediaPlayerStream类似于MediaPlayer。与播放本地文件的MediaPlayer不同，MediaPlayerStream播放音频流
```vbnet

Sub Process_Globals
	Dim mp As MediaPlayerStream
End Sub

Sub Globals

End Sub

Sub Activity_Create(FirstTime As Boolean)
	If FirstTime Then
		mp.Initialize("mp")
	End If
	mp.Load("http://www...")
End Sub
Sub mp_StreamReady
	Log("starts playing")
	mp.Play
End Sub
Sub mp_StreamError (ErrorCode As String, ExtraData As Int)
	Log("Error: " & ErrorCode & ", " & ExtraData)
	ToastMessageShow("Error: " & ErrorCode & ", " & ExtraData, True)
End Sub
Sub mp_StreamBuffer(Percentage As Int)
	Log(Percentage)
End Sub
```

> 事件：
>
> StreamReady
>
> StreamError (ErrorCode As String, ExtraData As Int)
>
> StreamBuffer(Percentage As Int)
>
> Complete

> 所需权限：
android.permission.INTERNET
## Play方法
**Play()**
>
> 返回值：void
## Load方法
**Load(ba,URL)**

?> 说明：开始从给定的URL加载资源。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：URL，类型：java.lang.String
>
> 返回值：void
## Pause方法
**Pause()**
>
> 返回值：void
## SetVolume方法
**SetVolume(Right,Left)**

?> 说明：设置每个频道的播放音量。该值应介于0到1之间。
>
> 参数：Right，类型：float
>
> 参数：Left，类型：float
>
> 返回值：void
## Stop方法
**Stop()**
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## IsPlaying方法
**IsPlaying()**
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
>
> 返回值：void
## Looping属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Duration属性
>
> 返回值：int

# JetPlayer
完整类名：anywheresoftware.b4a.audio.JetPlayerWrapper
> 所有者：process

> 包装器：android.media.JetPlayer
> 事件：
>
> QueuedSegmentsCountChanged (Count As Int)
>
> CurrentUserIdChanged (UserId As Int, RepeatCount As Int)
## Pause方法
**Pause()**

?> 说明：暂停播放。
>
> 返回值：void
## SetTrackMute方法
**SetTrackMute(Track,Mute,Sync)**

?> 说明：类似于SetMute，但仅更改单个轨迹的状态。
>
> 参数：Track，类型：int
>
> 参数：Mute，类型：boolean
>
> 参数：Sync，类型：boolean
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象并设置将处理JetPlayer事件的Subs。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## QueueSegment方法
**QueueSegment(SegmentNum,LibNum,RepeatCount,Transpose,MuteArray,UserId)**

?> 说明：将段添加到队列中。不允许超过3个分段。
>
> 参数：SegmentNum，类型：int
>
> 参数：LibNum，类型：int
>
> 参数：RepeatCount，类型：int
>
> 参数：Transpose，类型：int
>
> 参数：MuteArray，类型：boolean[]
>
> 参数：UserId，类型：byte
>
> 返回值：void
## Play方法
**Play()**

?> 说明：开始播放分段队列。
>
> 返回值：void
## LoadFile方法
**LoadFile(Dir,File)**

?> 说明：加载一个jet文件。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：File，类型：java.lang.String
>
> 返回值：void
## ClearQueue方法
**ClearQueue()**

?> 说明：清除分段队列。
>
> 返回值：void
## CloseFile方法
**CloseFile()**

?> 说明：关闭与加载的文件相关的资源。
>
> 返回值：void
## SetMute方法
**SetMute(MuteArray,Sync)**

?> 说明：设置轨迹静音状态。
>
> 参数：MuteArray，类型：boolean[]
>
> 参数：Sync，类型：boolean
>
> 返回值：void
## Release方法
**Release()**

?> 说明：释放为JetPlayer分配的所有资源。
>
> 返回值：void
## MaxTracks属性

?> 说明：返回同时播放曲目的最大数目。
>
> 返回值：int

# Beeper
完整类名：anywheresoftware.b4a.audio.Beeper
> 所有者：process

?> 说明：以给定的持续时间和频率播放“嘟嘟”声。
```vbnet

Dim b As Beeper
b.Initialize(300, 500)
b.Beep
```

## Beep方法
**Beep()**

?> 说明：播放声音。
>
> 返回值：void
## Initialize2方法
**Initialize2(Duration,Frequency,VoiceChannel)**

?> 说明：类似于初始化。允许您设置音量通道。
>
> 参数：Duration，类型：int
>
> 参数：Frequency，类型：int
>
> 参数：VoiceChannel，类型：int
>
> 返回值：void
## Initialize方法
**Initialize(Duration,Frequency)**

?> 说明：使用以毫秒为单位的给定持续时间和以赫兹为单位的指定频率初始化对象。
>
> 参数：Duration，类型：int
>
> 参数：Frequency，类型：int
>
> 返回值：void
## Release方法
**Release()**

?> 说明：释放此蜂鸣器使用的资源。
>
> 返回值：void
## VOLUME_MUSIC字段

?> 说明：音乐频道。
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
## VOLUME_ALARM字段

?> 说明：报警通道。
>
> 返回值：int

# AudioStreamer
完整类名：anywheresoftware.b4a.audio.AudioStreamer
> 所有者：process
> 事件：
>
> RecordBuffer (Data() As Byte)
>
> PlaybackComplete
>
> Error

> 所需权限：
android.permission.RECORD_AUDIO
## StopRecording方法
**StopRecording()**

?> 说明：停止录制。
>
> 返回值：void
## StartPlaying方法
**StartPlaying()**

?> 说明：开始播放。您应该在播放过程中调用Write（写入）来写入PCM数据。
>
> 返回值：void
## Write方法
**Write(Data)**

?> 说明：将数据写入玩家队列。数组大小必须小于PlayerBufferSize。
>
> 参数：Data，类型：byte[]
>
> 返回值：boolean
## Initialize2方法
**Initialize2(ba,AudioSource,EventName,SampleRate,Mono,Encoding,VolumeChannel)**

?> 说明：类似于初始化。允许您设置音频源。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：AudioSource，类型：int
>
> 参数：EventName，类型：java.lang.String
>
> 参数：SampleRate，类型：int
>
> 参数：Mono，类型：boolean
>
> 参数：Encoding，类型：int
>
> 参数：VolumeChannel，类型：int
>
> 返回值：void
## StopPlaying方法
**StopPlaying()**

?> 说明：停止播放。
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName,SampleRate,Mono,Encoding,VolumeChannel)**

?> 说明：初始化对象。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：SampleRate，类型：int
>
> 参数：Mono，类型：boolean
>
> 参数：Encoding，类型：int
>
> 参数：VolumeChannel，类型：int
>
> 返回值：void
## StartRecording方法
**StartRecording()**

?> 说明：开始录制。RecordBuffer事件将在录制过程中引发。
>
> 返回值：void
## PlayerBufferSize属性

?> 说明：返回播放器缓冲区大小。这是一次可以写入的最大大小。
>
> 返回值：int
## VOLUME_MUSIC字段

?> 说明：音乐频道。
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
## VOLUME_ALARM字段

?> 说明：报警通道。
>
> 返回值：int

# AudioRecordApp
完整类名：anywheresoftware.b4a.audio.AudioRecordApp
> 所有者：process

?> 说明：AudioRecordApp允许您使用默认的录音机应用程序录制音频。
```vbnet

Sub Process_Globals
	Dim audioRecorder As AudioRecordApp
	Dim videoRecorder As VideoRecordApp
End Sub

Sub Globals
	Dim vv As VideoView
End Sub

Sub Activity_Create(FirstTime As Boolean)
   If FirstTime Then
   		audioRecorder.Initialize("audioRecorder")
		videoRecorder.Initialize("videoRecorder")
	End If
	vv.Initialize("vv")
	Activity.AddView(vv, 0, 0, 100%x, 100%y)
	Activity.AddMenuItem("Record Video", "RecordVideo")
	Activity.AddMenuItem("Record Audio", "RecordAudio")
	ToastMessageShow("Press on Menu button...", True)
End Sub

Sub RecordVideo_Click
	videoRecorder.Record(File.DirRootExternal, "1.mp4")
End Sub
Sub RecordAudio_Click
	audioRecorder.Record(File.DirRootExternal, "1.3gpp")
End Sub
Sub videoRecorder_RecordComplete (Success As Boolean)
	Log(Success)
	If Success Then
		vv.LoadVideo(File.DirRootExternal, "1.mp4")
		vv.Play
	End If
End Sub
Sub audioRecorder_RecordComplete (Success As Boolean)
	Log(Success)
	If Success Then
		vv.LoadVideo(File.DirRootExternal, "1.3gpp")
		vv.Play
	End If
End Sub

Sub Activity_Resume

End Sub

Sub Activity_Pause (UserClosed As Boolean)

End Sub
```

> 事件：
>
> RecordComplete (Success As Boolean)

> 所需权限：
android.permission.WRITE_EXTERNAL_STORAGE
## Record方法
**Record(ba,Dir,FileName)**

?> 说明：调用录制应用程序。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：void
## Initialize方法
**Initialize(EventName)**

?> 说明：初始化对象并设置将处理该事件的子。
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void

# VideoRecordApp
完整类名：anywheresoftware.b4a.audio.AudioRecordApp.VideoRecordApp
> 所有者：process

?> 说明：VideoRecordApp允许您使用默认的录像机应用程序录制视频。
> 事件：
>
> RecordComplete (Success As Boolean)
## Record方法
**Record(ba,Dir,FileName)**

?> 说明：<b>不会在Android 7+设备上工作</b> 请改用Record3。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：void
## Initialize方法
**Initialize(EventName)**

?> 说明：初始化对象并设置将处理该事件的子。
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Record3方法
**Record3(ba,Dir,FileName,MaxLengthSeconds,Uri)**

?> 说明：调用录制应用程序。将引发RecordComplete事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：MaxLengthSeconds，类型：int
>
> 参数：Uri，类型：android.net.Uri
>
> 返回值：void
## Record2方法
**Record2(ba,Dir,FileName,MaxLengthSeconds)**

?> 说明：<b>不会在Android 7+设备上工作</b> 请改用Record3。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：MaxLengthSeconds，类型：int
>
> 返回值：void

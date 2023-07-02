# NFC

版本:2.02
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=NFC)

# NFC
完整类名：anywheresoftware.b4a.objects.NFC
> 所有者：activity

?> 说明：支持读取和写入NFC标签，并支持在两个Android设备之间发送消息。
> 事件：
>
> CreateMessage As List

> 所需权限：
android.permission.NFC
## EnableForegroundDispatch方法
**EnableForegroundDispatch(ba)**

?> 说明：强制将所有NFC意图发送到当前活动。应从Activity_Resme调用。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## IsNdefIntent方法
**IsNdefIntent(Intent)**

?> 说明：测试Intent是否包含从NDef标记读取的数据。
>
> 参数：Intent，类型：android.content.Intent
>
> 返回值：boolean
## GetTechList方法
**GetTechList(Intent)**

?> 说明：返回一个包含NFC标签支持的技术的数组。
>
> 参数：Intent，类型：android.content.Intent
>
> 返回值：java.lang.String[]
## PreparePushMessage方法
**PreparePushMessage(ba,EventName)**

?> 说明：设置将处理CreateMessage事件的子。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## CreateUriRecord方法
**CreateUriRecord(Uri)**

?> 说明：使用Uri负载创建NdefMessage。
>
> 参数：Uri，类型：java.lang.String
>
> 返回值：java.lang.Object
## CreateMimeRecord方法
**CreateMimeRecord(Mime,Data)**

?> 说明：使用给定的mime类型和数据创建NdefMessage。
>
> 参数：Mime，类型：java.lang.String
>
> 参数：Data，类型：byte[]
>
> 返回值：java.lang.Object
## GetNdefRecords方法
**GetNdefRecords(Intent)**

?> 说明：检索Intent对象中存储的NdefRecords。
>
> 参数：Intent，类型：android.content.Intent
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## DisableForegroundDispatch方法
**DisableForegroundDispatch(ba)**

?> 说明：请参阅EnableForegroundDispatch。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## IsEnabled属性

?> 说明：如果支持并启用NFC，则返回true。
```vbnet

Dim in As Intent
in.Initialize("android.settings.NFC_SETTINGS", "")
StartActivity(in)
```

>
> 返回值：boolean
## IsSupported属性

?> 说明：如果NFC适配器可用，则返回true。
>
> 返回值：boolean

# NdefRecord
完整类名：anywheresoftware.b4a.objects.NFC.NdefRecordWrapper
> 所有者：process

> 包装器：android.nfc.NdefRecord
## GetPayload方法
**GetPayload()**

?> 说明：返回整个有效负载。
>
> 返回值：byte[]
## GetAsTextType方法
**GetAsTextType()**

?> 说明：读取有效负载并返回存储的文本。
>
> 返回值：java.lang.String
## GetAsUriType方法
**GetAsUriType()**

?> 说明：读取负载并返回存储的Uri。
>
> 返回值：java.lang.String
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean

# TagTechnology
完整类名：anywheresoftware.b4a.objects.NFC.TagTechnologyWrapper
> 所有者：process

> 包装器：android.nfc.tech.TagTechnology

?> 说明：提供对扫描标记的访问权限。
> 事件：
>
> Connected (Success As Boolean)
>
> RunAsync (Flag As Int, Success As Boolean, Result As Object)
## Connect方法
**Connect(ba)**

?> 说明：连接到标记。将引发Connected事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## RunAsync方法
**RunAsync(ba,EventName,Method,Params,Flag)**

?> 说明：异步运行给定的方法。这可用于访问本机I/O方法。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Method，类型：java.lang.String
>
> 参数：Params，类型：java.lang.Object[]
>
> 参数：Flag，类型：int
>
> 返回值：void
## Close方法
**Close()**

?> 说明：关闭连接。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(EventName,Tech,Intent)**

?> 说明：初始化对象。
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Tech，类型：java.lang.String
>
> 参数：Intent，类型：android.content.Intent
>
> 返回值：void
## Connected属性

?> 说明：如果存在活动连接，则返回true。
>
> 返回值：boolean

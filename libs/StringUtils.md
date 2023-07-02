# StringUtils

版本:1.12
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=StringUtils)

# StringUtils
完整类名：anywheresoftware.b4a.objects.StringUtils
> 所有者：process

?> 说明：字符串相关函数的集合。
## DecodeBase64方法
**DecodeBase64(Data)**

?> 说明：从Base64表示法解码数据。
>
> 参数：Data，类型：java.lang.String
>
> 返回值：byte[]
## EncodeBase64方法
**EncodeBase64(Data)**

?> 说明：将给定的字节数组编码为Base64表示法。
```vbnet

Dim su As StringUtils
Dim encoded As String
encoded = su.EncodeBase64(data) 'data is a bytes array
```

>
> 参数：Data，类型：byte[]
>
> 返回值：java.lang.String
## SaveCSV方法
**SaveCSV(Dir,FileName,SeparatorChar,Table)**

?> 说明：将表格另存为CSV文件。
```vbnet

Dim su As StringUtils
su.SaveCSV(File.DirRootExternal, "1.csv", ",", table)
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：SeparatorChar，类型：char
>
> 参数：Table，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## DecodeUrl方法
**DecodeUrl(Url,CharSet)**

?> 说明：对应用程序/x-www-form-urlencoded字符串进行解码。
>
> 参数：Url，类型：java.lang.String
>
> 参数：CharSet，类型：java.lang.String
>
> 返回值：java.lang.String
## SaveCSV2方法
**SaveCSV2(Dir,FileName,SeparatorChar,Table,Headers)**

?> 说明：类似于SaveCSV。将标题列表保存为第一行。这应该是一个字符串列表（或数组）。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：SeparatorChar，类型：char
>
> 参数：Table，类型：anywheresoftware.b4a.objects.collections.List
>
> 参数：Headers，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## EncodeUrl方法
**EncodeUrl(Url,CharSet)**

?> 说明：将字符串编码为application/x-www-form-urlencoded格式。
```vbnet

Dim su As StringUtils
Dim url, encodedUrl As String
encodedUrl = su.EncodeUrl(url, "UTF8")
```

>
> 参数：Url，类型：java.lang.String
>
> 参数：CharSet，类型：java.lang.String
>
> 返回值：java.lang.String
## MeasureMultilineTextHeight方法
**MeasureMultilineTextHeight(TextView,Text)**

?> 说明：返回所需的高度，以便在标签中显示给定的文本。
```vbnet

Dim Label1 As Label
Label1.Initialize("")
Label1.Text = "this is a long sentence, and we need to " _ 
	& "know the height required in order To show it completely."
Label1.TextSize = 20
Activity.AddView(Label1, 10dip, 10dip, 200dip, 30dip)
Dim su As StringUtils
Label1.Height = su.MeasureMultilineTextHeight(Label1, Label1.Text)
```

>
> 参数：TextView，类型：android.widget.TextView
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：int
## LoadCSV2方法
**LoadCSV2(Dir,FileName,SeparatorChar,Headers)**

?> 说明：类似于LoadCSV。将第一行加载到标题列表中。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：SeparatorChar，类型：char
>
> 参数：Headers，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## LoadCSV方法
**LoadCSV(Dir,FileName,SeparatorChar)**

?> 说明：加载CSV文件并将其存储在字符串数组列表中。
```vbnet

Dim su As StringUtils
Dim Table As List
Table = su.LoadCSV(File.DirAssets, "1.csv", ",")
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：SeparatorChar，类型：char
>
> 返回值：anywheresoftware.b4a.objects.collections.List

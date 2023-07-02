# OkHttp

版本:1.5
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=OkHttp)

# OkHttpClient
完整类名：anywheresoftware.b4h.okhttp.OkHttpClientWrapper
> 所有者：process

> 依赖：okhttp-4.9.0 | okio-2.8.0 | okhttp-urlconnection-4.9.3 | kotlin-stdlib-1.6.10

?> 说明：OkHttpClient允许您发出Http请求。建议使用[OkHttpUtil2](https://www.b4x.com/android/forum/threads/b4x-okhttputils2-with-wait-for.79345/)，而不是直接使用OkHttpClient
> 事件：
>
> ResponseSuccess (Response As OkHttpResponse, TaskId As Int)
>
> ResponseError (Response As OkHttpResponse, Reason As String, StatusCode As Int, TaskId As Int)

> 所需权限：
android.permission.INTERNET
## Execute方法
**Execute(ba,HttpRequest,TaskId)**

?> 说明：异步执行OkHttpRequest。稍后将触发ResponseSuccess或ResponseError事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：HttpRequest，类型：anywheresoftware.b4h.okhttp.OkHttpClientWrapper.OkHttpRequest
>
> 参数：TaskId，类型：int
>
> 返回值：boolean
## ExecuteCredentials方法
**ExecuteCredentials(ba,Request,TaskId,UserName,Password)**

?> 说明：与执行行为相同。用户名和密码将用于基本身份验证和摘要式身份验证。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Request，类型：anywheresoftware.b4h.okhttp.OkHttpClientWrapper.OkHttpRequest
>
> 参数：TaskId，类型：int
>
> 参数：UserName，类型：java.lang.String
>
> 参数：Password，类型：java.lang.String
>
> 返回值：boolean
## InitializeAcceptAll方法
**InitializeAcceptAll(EventName)**

?> 说明：类似于Initialize，但有一个重要区别。所有SSL证书都将被自动接受。
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(EventName)**

?> 说明：初始化此对象。
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void

# OkHttpRequest
完整类名：anywheresoftware.b4h.okhttp.OkHttpClientWrapper.OkHttpRequest
> 所有者：process

> 依赖：okhttp-4.9.0 | okio-2.8.0 | okhttp-urlconnection-4.9.3 | kotlin-stdlib-1.6.10
## InitializePost2方法
**InitializePost2(URL,Data)**

?> 说明：初始化请求并将其设置为HttpPost方法。
>
> 参数：URL，类型：java.lang.String
>
> 参数：Data，类型：byte[]
>
> 返回值：void
## InitializePut方法
**InitializePut(URL,InputStream,Length)**

?> 说明：初始化请求并将其设置为Http-Put方法。
>
> 参数：URL，类型：java.lang.String
>
> 参数：InputStream，类型：java.io.InputStream
>
> 参数：Length，类型：int
>
> 返回值：void
## SetContentType方法
**SetContentType(ContentType)**

?> 说明：设置请求的Mime标头。
>
> 参数：ContentType，类型：java.lang.String
>
> 返回值：void
## InitializeDelete方法
**InitializeDelete(URL)**

?> 说明：初始化请求并将其设置为Http-Delete方法。
>
> 参数：URL，类型：java.lang.String
>
> 返回值：void
## InitializePatch方法
**InitializePatch(URL,InputStream,Length)**

?> 说明：初始化请求并将其设置为Http Patch方法。
>
> 参数：URL，类型：java.lang.String
>
> 参数：InputStream，类型：java.io.InputStream
>
> 参数：Length，类型：int
>
> 返回值：void
## InitializePatch2方法
**InitializePatch2(URL,Data)**

?> 说明：初始化请求并将其设置为Http Patch方法。
>
> 参数：URL，类型：java.lang.String
>
> 参数：Data，类型：byte[]
>
> 返回值：void
## RemoveHeaders方法
**RemoveHeaders(Name)**

?> 说明：删除具有给定名称的所有标头。
>
> 参数：Name，类型：java.lang.String
>
> 返回值：void
## InitializeDelete2方法
**InitializeDelete2(URL,Data)**

?> 说明：初始化请求并将其设置为具有给定负载的Http-Delete方法。
>
> 参数：URL，类型：java.lang.String
>
> 参数：Data，类型：byte[]
>
> 返回值：void
## InitializeHead方法
**InitializeHead(URL)**

?> 说明：初始化请求并将其设置为Http-Head方法。
>
> 参数：URL，类型：java.lang.String
>
> 返回值：void
## InitializeGet方法
**InitializeGet(URL)**

?> 说明：初始化请求并将其设置为Http-Get方法。
>
> 参数：URL，类型：java.lang.String
>
> 返回值：void
## InitializePost方法
**InitializePost(URL,InputStream,Length)**

?> 说明：初始化请求并将其设置为HttpPost方法。
>
> 参数：URL，类型：java.lang.String
>
> 参数：InputStream，类型：java.io.InputStream
>
> 参数：Length，类型：int
>
> 返回值：void
## InitializePut2方法
**InitializePut2(URL,Data)**

?> 说明：初始化请求并将其设置为Http-Put方法。
>
> 参数：URL，类型：java.lang.String
>
> 参数：Data，类型：byte[]
>
> 返回值：void
## SetContentEncoding方法
**SetContentEncoding(Encoding)**

?> 说明：设置请求的编码标头。
>
> 参数：Encoding，类型：java.lang.String
>
> 返回值：void
## SetHeader方法
**SetHeader(Name,Value)**

?> 说明：设置具有给定名称的标头的值。如果不存在这样的标头，则将添加一个新标头。
>
> 参数：Name，类型：java.lang.String
>
> 参数：Value，类型：java.lang.String
>
> 返回值：void
## Timeout属性

?> 说明：获取或设置请求超时，以毫秒为单位。默认值为30000（30秒）。
>
> 参数：t，类型：int
>
> 返回值：int

# OkHttpResponse
完整类名：anywheresoftware.b4h.okhttp.OkHttpClientWrapper.OkHttpResponse
> 所有者：process

> 依赖：okhttp-4.9.0 | okio-2.8.0 | okhttp-urlconnection-4.9.3 | kotlin-stdlib-1.6.10

?> 说明：保存从服务器返回的响应的对象。
> 事件：
>
> StreamFinish (Success As Boolean, TaskId As Int)
## GetHeaders方法
**GetHeaders()**

?> 说明：返回一个带有响应标头的Map对象。
```vbnet

Dim list1 As List
list1 = response.GetHeaders.Get("Set-Cookie")
For i = 0 To list1.Size - 1
	Log(list1.Get(i))
Next
```

>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## GetAsynchronously方法
**GetAsynchronously(ba,EventName,Output,CloseOutput,TaskId)**

?> 说明：异步读取响应并将其写入给定的OutputStream。
```vbnet

Sub Http_ResponseSuccess (Response As OkHttpResponse, TaskId As Int)
	Response.GetAsynchronously("ImageResponse", _ 
		File.OpenOutput(File.DirInternalCache, "image.jpg", False), True, TaskId)
End Sub

Sub ImageResponse_StreamFinish (Success As Boolean, TaskId As Int)
	If Success = False Then
		Msgbox(LastException.Message, "Error")
		Return
	End If
	ImageView1.Bitmap = LoadBitmap(File.DirInternalCache, "image.jpg")
End Sub
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Output，类型：java.io.OutputStream
>
> 参数：CloseOutput，类型：boolean
>
> 参数：TaskId，类型：int
>
> 返回值：boolean
## Release方法
**Release()**

?> 说明：释放为此对象分配的资源。
>
> 返回值：void
## ContentType属性

?> 说明：返回“内容类型”标头。
>
> 返回值：java.lang.String
## ContentEncoding属性

?> 说明：返回内容编码标头。
>
> 返回值：java.lang.String
## ContentLength属性

?> 说明：返回响应正文长度。
>
> 返回值：long
## StatusCode属性

?> 说明：返回响应Http代码。
>
> 返回值：int
## ErrorResponse属性

?> 说明：以字符串形式返回服务器响应（仅适用于失败的响应）。
>
> 返回值：java.lang.String

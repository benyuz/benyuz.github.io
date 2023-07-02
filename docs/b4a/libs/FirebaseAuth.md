# FirebaseAuth

版本:3.0
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=FirebaseAuth)

# FirebaseAuth
完整类名：anywheresoftware.b4a.objects.FirebaseAuthWrapper
> 所有者：process

> 依赖：com.google.firebase:firebase-auth | com.google.android.gms:play-services-auth | com.google.firebase:firebase-core
> 事件：
>
> SignedIn (User As FirebaseUser)
>
> TokenAvailable (User As FirebaseUser, Success As Boolean, TokenId As String)
>
> SignError (Error As Exception)
## SignOutFromGoogle方法
**SignOutFromGoogle()**

?> 说明：从Firebase和Google注销。
>
> 返回值：void
## GetUserTokenId方法
**GetUserTokenId(ba,User,ForceRefresh)**

?> 说明：检索令牌id。此令牌可以发送到后端服务器。服务器可以使用它来验证用户。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：User，类型：anywheresoftware.b4a.objects.FirebaseAuthWrapper.FirebaseUserWrapper
>
> 参数：ForceRefresh，类型：boolean
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象。如果已经有登录用户，将引发SignedIn事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SignInWithGoogle方法
**SignInWithGoogle(ba)**

?> 说明：启动登录过程。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## CurrentUser属性

?> 说明：返回当前登录的用户。如果没有用户，则返回未初始化的对象。
>
> 返回值：anywheresoftware.b4a.objects.FirebaseAuthWrapper.FirebaseUserWrapper

# FirebaseUser
完整类名：anywheresoftware.b4a.objects.FirebaseAuthWrapper.FirebaseUserWrapper
> 所有者：process

> 包装器：com.google.firebase.auth.FirebaseUser

> 依赖：com.google.firebase:firebase-auth | com.google.android.gms:play-services-auth | com.google.firebase:firebase-core
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Uid属性
>
> 返回值：java.lang.String
## Email属性
>
> 返回值：java.lang.String
## DisplayName属性
>
> 返回值：java.lang.String
## PhotoUrl属性
>
> 返回值：java.lang.String

# FirebaseAdMob2

版本:3.0
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=FirebaseAdMob2)

# AdView
完整类名：anywheresoftware.b4a.admobwrapper.AdViewWrapper
> 所有者：activity

> 包装器：com.google.android.gms.ads.AdView

> 依赖：com.google.firebase:firebase-ads | gson-2.8.5 | GoogleConsent.aar
> 事件：
>
> ReceiveAd
>
> FailedToReceiveAd (ErrorCode As String)
>
> AdScreenDismissed
>
> PresentScreen

> 所需权限：
android.permission.INTERNET
android.permission.ACCESS_NETWORK_STATE
com.google.android.gms.permission.AD_ID
## LoadAdWithBuilder方法
**LoadAdWithBuilder(Builder)**

?> 说明：请求使用AdRequestBuilder配置的广告。
>
> 参数：Builder，类型：anywheresoftware.b4a.admobwrapper.AdViewWrapper.AdRequestBuilderWrapper
>
> 返回值：void
## Pause方法
**Pause()**

?> 说明：应该从Activity_Pause调用。
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName,PublisherId)**

?> 说明：使用默认的320dip x 50dip大小初始化AdView。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：PublisherId，类型：java.lang.String
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
## LoadAd方法
**LoadAd()**

?> 说明：向AdMob发送请求，请求广告。
>
> 返回值：void
## Initialize2方法
**Initialize2(ba,EventName,AdUnitId,Size)**

?> 说明：初始化AdView。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：AdUnitId，类型：java.lang.String
>
> 参数：Size，类型：java.lang.Object
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
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
## Resume方法
**Resume()**

?> 说明：应从Activity_Resme调用。
>
> 返回值：void
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
## SIZE_IAB_LEADERBOARD字段

?> 说明：728dip x 90dip-仅限片剂
>
> 返回值：java.lang.Object
## SIZE_SMART_BANNER字段

?> 说明：广告将自动使用全部可用宽度。
```vbnet

Adview1.Initialize2("Ad", "xxxxxxxx", AdView1.SIZE_SMART_BANNER)
Dim height As Int
If GetDeviceLayoutValues.ApproximateScreenSize < 6 Then
    'phones
    If 100%x > 100%y Then height = 32dip Else height = 50dip
Else
    'tablets
    height = 90dip
End If
Activity.AddView(AdView1, 0dip, 100%y - height, 100%x, height)
```

>
> 返回值：java.lang.Object
## SIZE_BANNER字段

?> 说明：320英寸x 50英寸（默认尺寸）
>
> 返回值：java.lang.Object
## SIZE_IAB_BANNER字段

?> 说明：468dip x 60dip-仅限片剂
>
> 返回值：java.lang.Object
## SIZE_IAB_MRECT字段

?> 说明：300dip x 250dip-仅限片剂
>
> 返回值：java.lang.Object

# InterstitialAd
完整类名：anywheresoftware.b4a.admobwrapper.AdViewWrapper.InterstitialAdWrapper
> 所有者：activity

> 依赖：com.google.firebase:firebase-ads | gson-2.8.5 | GoogleConsent.aar
> 事件：
>
> ReceiveAd
>
> FailedToReceiveAd (ErrorCode As String)
>
> AdClosed
>
> AdOpened
## LoadAdWithBuilder方法
**LoadAdWithBuilder(ba,AdRequestBuilder)**

?> 说明：请求使用AdRequestBuilder配置的广告。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：AdRequestBuilder，类型：com.google.android.gms.ads.AdRequest.Builder
>
> 返回值：void
## LoadAd方法
**LoadAd(ba)**

?> 说明：请求广告。将引发AdLoaded事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Show方法
**Show(ba)**

?> 说明：显示加载的广告。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName,AdUnitId)**

?> 说明：初始化对象。
```vbnet
ca-app-pub-3940256099942544/1033173712
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：AdUnitId，类型：java.lang.String
>
> 返回值：void
## Ready属性

?> 说明：测试是否有准备好播放的广告。
>
> 返回值：boolean

# MobileAds
完整类名：anywheresoftware.b4a.admobwrapper.AdViewWrapper.MobileAdsWrapper
> 所有者：process

> 依赖：com.google.firebase:firebase-ads | gson-2.8.5 | GoogleConsent.aar
## CreateRequestConfigurationBuilder方法
**CreateRequestConfigurationBuilder(TestDeviceIds)**
>
> 参数：TestDeviceIds，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：java.lang.Object
## SetConfiguration方法
**SetConfiguration(ConfigurationBuilder)**
>
> 参数：ConfigurationBuilder，类型：java.lang.Object
>
> 返回值：void
## Initialize方法
**Initialize(ba)**

?> 说明：应该在请求广告之前调用。可以像这样与Wait For一起使用：
```vbnet
Wait For (MobileAds.Initialize) MobileAds_Ready
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：java.lang.Object

# AdRequestBuilder
完整类名：anywheresoftware.b4a.admobwrapper.AdViewWrapper.AdRequestBuilderWrapper
> 所有者：process

> 包装器：com.google.android.gms.ads.AdRequest.Builder

> 依赖：com.google.firebase:firebase-ads | gson-2.8.5 | GoogleConsent.aar
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## NonPersonalizedAds方法
**NonPersonalizedAds()**

?> 说明：请求非个性化广告。
>
> 返回值：anywheresoftware.b4a.admobwrapper.AdViewWrapper.AdRequestBuilderWrapper
## Initialize方法
**Initialize()**
>
> 返回值：anywheresoftware.b4a.admobwrapper.AdViewWrapper.AdRequestBuilderWrapper

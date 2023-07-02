# AppCompat

版本:4.02
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=AppCompat)

# AppCompat
完整类名：de.amberhome.objects.appcompat.AppCompatBase
> 所有者：activity

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
## SetElevation方法
**SetElevation(View,Elevation)**

?> 说明：设置视图的高程
>
> 参数：View，类型：android.view.View
>
> 参数：Elevation，类型：float
>
> 返回值：void
## GetElevation方法
**GetElevation(View)**

?> 说明：获取视图的高程
>
> 参数：View，类型：android.view.View
>
> 返回值：float
## UnWrapDrawable方法
**UnWrapDrawable(drawable)**
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## GetStdActionBarHeight方法
**GetStdActionBarHeight(ba)**

?> 说明：获取标准ActionBar Height。由于Gingerbread没有ActionBar，它将在Android＜3.0时返回0。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：int
## GetNavigationBarHeight方法
**GetNavigationBarHeight(ba)**

?> 说明：获取导航栏高度
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：int
## GetThemeAttribute方法
**GetThemeAttribute(ba,AttributeName)**

?> 说明：尝试获取主题属性的值，如colorPrimary，
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：AttributeName，类型：java.lang.String
>
> 返回值：int
## GetMaterialActionBarHeight方法
**GetMaterialActionBarHeight(ba)**

?> 说明：获取“材质设计”样式指南中定义的ActionBar Height
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：int
## GetStatusBarHeight方法
**GetStatusBarHeight(ba)**

?> 说明：获取状态栏高度
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：int
## SetClickEffect方法
**SetClickEffect(ba,View,Borderless)**

?> 说明：设置视图的单击效果。将在棒棒糖或以后使用波纹效果
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：View，类型：android.view.View
>
> 参数：Borderless，类型：boolean
>
> 返回值：void
## SetDrawableTint方法
**SetDrawableTint(drawable,Color)**
>
> 参数：drawable，类型：android.graphics.drawable.Drawable
>
> 参数：Color，类型：int
>
> 返回值：void

# ACToolBarLight
完整类名：de.amberhome.objects.appcompat.ACToolbarLightWrapper
> 所有者：activity

> 包装器：de.amberhome.objects.appcompat.internal.InternalToolbar

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> NavigationItemClick
>
> MenuItemClick (Item as ACMenuItem)
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## GetView方法
**GetView(Index)**

?> 说明：获取给定索引的视图
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.ConcreteViewWrapper
## AddView方法
**AddView(View,Width,Height,Gravity)**

?> 说明：将视图添加到工具栏。宽度是
>
> 参数：View，类型：android.view.View
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 参数：Gravity，类型：int
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
## GetAllViewsRecursive方法
**GetAllViewsRecursive()**

?> 说明：获取添加到工具栏的所有视图。
>
> 返回值：anywheresoftware.b4a.BA.IterableList
## InitMenuListener方法
**InitMenuListener()**

?> 说明：重新初始化Menu侦听器。如果设置工具栏，这是必要的
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## RemoveViewAt方法
**RemoveViewAt(Index)**

?> 说明：删除具有给定索引的视图
>
> 参数：Index，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## AddCustomView方法
**AddCustomView(ba)**

?> 说明：添加自定义视图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## SetAsActionBar方法
**SetAsActionBar(ba)**

?> 说明：将此工具栏设置为活动主ActionBar
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## SetElevationAnimated方法
**SetElevationAnimated(Duration,Elevation)**
>
> 参数：Duration，类型：int
>
> 参数：Elevation，类型：float
>
> 返回值：void
## RemoveAllViews方法
**RemoveAllViews()**

?> 说明：从工具栏中删除所有视图
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，动画将
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## MinHeight属性

?> 说明：设置或获取工具栏的最小高度。MinHeight属性为
>
> 参数：MinHeight，类型：int
>
> 返回值：int
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Parent属性
>
> 返回值：java.lang.Object
## NumberOfViews属性

?> 说明：返回此工具栏中的视图数
>
> 返回值：int
## Elevation属性
>
> 参数：e，类型：float
>
> 返回值：float
## PopupTheme属性

?> 说明：设置弹出式菜单主题。
>
> 参数：Theme，类型：int
>
> 返回值：
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## Menu属性

?> 说明：获取工具栏的菜单
>
> 返回值：de.amberhome.objects.appcompat.ACMenuWrapper
## TitleTextColor属性

?> 说明：设置标题文本颜色
>
> 参数：Color，类型：int
>
> 返回值：
## Width属性

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## SubTitle属性

?> 说明：设置或获取工具栏的子标题
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## LogoBitmap属性

?> 说明：将位图设置为徽标。工具栏中的徽标无法单击。
>
> 参数：Icon，类型：android.graphics.Bitmap
>
> 返回值：
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## NavigationIconBitmap属性

?> 说明：设置工具栏的导航项。此图标是可单击的。
>
> 参数：Icon，类型：android.graphics.Bitmap
>
> 返回值：
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## Title属性

?> 说明：设置或获取工具栏的标题
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
>
> 返回值：int
## NavigationIconDrawable属性

?> 说明：设置或获取工具栏的导航图标。此图标是可单击的。
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Tag属性
>
> 参数：arg0，类型：java.lang.Object
>
> 返回值：java.lang.Object
## SubTitleTextColor属性

?> 说明：设置字幕文本颜色
>
> 参数：Color，类型：int
>
> 返回值：
## LogoDrawable属性

?> 说明：设置或获取工具栏的徽标。徽标不可点击
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## THEME_LIGHT字段
>
> 返回值：int
## THEME_DARK字段
>
> 返回值：int

# ACToolBarDark
完整类名：de.amberhome.objects.appcompat.ACToolbarDarkWrapper
> 所有者：activity

> 包装器：de.amberhome.objects.appcompat.internal.InternalToolbar

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> NavigationItemClick
>
> MenuItemClick (Item as ACMenuItem)
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## GetView方法
**GetView(Index)**

?> 说明：获取给定索引的视图
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.ConcreteViewWrapper
## AddView方法
**AddView(View,Width,Height,Gravity)**

?> 说明：将视图添加到工具栏。宽度是
>
> 参数：View，类型：android.view.View
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 参数：Gravity，类型：int
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
## GetAllViewsRecursive方法
**GetAllViewsRecursive()**

?> 说明：获取添加到工具栏的所有视图。
>
> 返回值：anywheresoftware.b4a.BA.IterableList
## InitMenuListener方法
**InitMenuListener()**

?> 说明：重新初始化Menu侦听器。如果设置工具栏，这是必要的
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## RemoveViewAt方法
**RemoveViewAt(Index)**

?> 说明：删除具有给定索引的视图
>
> 参数：Index，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## AddCustomView方法
**AddCustomView(ba)**

?> 说明：添加自定义视图。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## SetAsActionBar方法
**SetAsActionBar(ba)**

?> 说明：将此工具栏设置为活动主ActionBar
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## SetElevationAnimated方法
**SetElevationAnimated(Duration,Elevation)**
>
> 参数：Duration，类型：int
>
> 参数：Elevation，类型：float
>
> 返回值：void
## RemoveAllViews方法
**RemoveAllViews()**

?> 说明：从工具栏中删除所有视图
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，动画将
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## MinHeight属性

?> 说明：设置或获取工具栏的最小高度。MinHeight属性为
>
> 参数：MinHeight，类型：int
>
> 返回值：int
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Parent属性
>
> 返回值：java.lang.Object
## NumberOfViews属性

?> 说明：返回此工具栏中的视图数
>
> 返回值：int
## Elevation属性
>
> 参数：e，类型：float
>
> 返回值：float
## PopupTheme属性

?> 说明：设置弹出式菜单主题。
>
> 参数：Theme，类型：int
>
> 返回值：
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## Menu属性

?> 说明：获取工具栏的菜单
>
> 返回值：de.amberhome.objects.appcompat.ACMenuWrapper
## TitleTextColor属性

?> 说明：设置标题文本颜色
>
> 参数：Color，类型：int
>
> 返回值：
## Width属性

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## SubTitle属性

?> 说明：设置或获取工具栏的子标题
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## LogoBitmap属性

?> 说明：将位图设置为徽标。工具栏中的徽标无法单击。
>
> 参数：Icon，类型：android.graphics.Bitmap
>
> 返回值：
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## NavigationIconBitmap属性

?> 说明：设置工具栏的导航项。此图标是可单击的。
>
> 参数：Icon，类型：android.graphics.Bitmap
>
> 返回值：
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## Title属性

?> 说明：设置或获取工具栏的标题
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
>
> 返回值：int
## NavigationIconDrawable属性

?> 说明：设置或获取工具栏的导航图标。此图标是可单击的。
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Tag属性
>
> 参数：arg0，类型：java.lang.Object
>
> 返回值：java.lang.Object
## SubTitleTextColor属性

?> 说明：设置字幕文本颜色
>
> 参数：Color，类型：int
>
> 返回值：
## LogoDrawable属性

?> 说明：设置或获取工具栏的徽标。徽标不可点击
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## THEME_LIGHT字段
>
> 返回值：int
## THEME_DARK字段
>
> 返回值：int

# ACSwitch
完整类名：de.amberhome.objects.appcompat.ACSwitchCompatWrapper
> 所有者：activity

> 包装器：android.support.v7.widget.SwitchCompat

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> CheckedChange(Checked As Boolean)
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：float
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Initialize2方法
**Initialize2(ba,EventName,Style)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Style，类型：java.lang.String
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## ShowText属性

?> 说明：设置或获取是否应显示打开/关闭文本。
>
> 参数：Flag，类型：boolean
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：arg0，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性
>
> 返回值：java.lang.Object
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## TextSize属性
>
> 参数：arg0，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：arg0，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Checked属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## TextOn属性

?> 说明：设置或获取按钮处于选中状态时显示的文本。
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Ellipsize属性
>
> 参数：arg0，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
>
> 返回值：int
## TextOff属性

?> 说明：设置或获取按钮处于未选中状态时显示的文本。
>
> 参数：Text，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## TextColor属性
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

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## SingleLine属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：arg0，类型：int
>
> 返回值：int

# ACSubMenu
完整类名：de.amberhome.objects.appcompat.ACSubMenuWrapper
> 所有者：process

> 包装器：android.view.SubMenu

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
## Add方法
**Add(ItemId,SortOrder,Title,Icon)**

?> 说明：将菜单项添加到菜单
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.Bitmap
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## AddWithGroup2方法
**AddWithGroup2(GroupId,ItemId,SortOrder,Title,Icon)**

?> 说明：将菜单项添加到菜单中，并将此项放入一个组中。
>
> 参数：GroupId，类型：int
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## Size方法
**Size()**

?> 说明：返回菜单中的项数
>
> 返回值：int
## SetGroupCheckable方法
**SetGroupCheckable(GroupId,Checkable,Exclusive)**

?> 说明：使组中的所有项目都可检查
>
> 参数：GroupId，类型：int
>
> 参数：Checkable，类型：boolean
>
> 参数：Exclusive，类型：boolean
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## RemoveGroup方法
**RemoveGroup(GroupId)**

?> 说明：从菜单中删除组
>
> 参数：GroupId，类型：int
>
> 返回值：void
## SetGroupEnabled方法
**SetGroupEnabled(GroupId,Enable)**

?> 说明：启用/禁用给定的组
>
> 参数：GroupId，类型：int
>
> 参数：Enable，类型：boolean
>
> 返回值：void
## Add2方法
**Add2(ItemId,SortOrder,Title,Icon)**

?> 说明：将菜单项添加到菜单
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## Clear方法
**Clear()**

?> 说明：清除菜单中的所有菜单项。
>
> 返回值：void
## GetItem方法
**GetItem(Index)**

?> 说明：返回具有给定索引的项。
>
> 参数：Index，类型：int
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## RemoveItem方法
**RemoveItem(ItemId)**

?> 说明：从菜单中删除项目
>
> 参数：ItemId，类型：int
>
> 返回值：void
## ClearHeader方法
**ClearHeader()**
>
> 返回值：void
## AddSubMenu方法
**AddSubMenu(GroupId,ItemId,SortOrder,Title)**

?> 说明：将子菜单添加到菜单中。
>
> 参数：GroupId，类型：int
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：de.amberhome.objects.appcompat.ACSubMenuWrapper
## FindItem方法
**FindItem(ItemId)**

?> 说明：返回具有给定Id的项。如果找不到该项，则返回null。
>
> 参数：ItemId，类型：int
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## SetGroupVisible方法
**SetGroupVisible(GroupId,Visible)**

?> 说明：使给定的组可见/不可见
>
> 参数：GroupId，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## Close方法
**Close()**

?> 说明：如果菜单处于打开状态，请将其关闭。
>
> 返回值：void
## AddWithGroup方法
**AddWithGroup(GroupId,ItemId,SortOrder,Title,Icon)**

?> 说明：将菜单项添加到菜单中，并将此项放入一个组中
>
> 参数：GroupId，类型：int
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.Bitmap
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## HeaderTitle属性
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：
## Icon属性
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：
## HeaderIcon属性
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：

# ACSpinner
完整类名：de.amberhome.objects.appcompat.ACSpinnerWrapper
> 所有者：activity

> 包装器：de.amberhome.objects.appcompat.ACSpinnerWrapper.ACB4ASpinner

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> ItemClick (Position As Int, Value As Object)
>
> Closed
## Add方法
**Add(Item)**
>
> 参数：Item，类型：java.lang.CharSequence
>
> 返回值：void
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Add2方法
**Add2(Item,Icon)**
>
> 参数：Item，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：void
## Clear方法
**Clear()**
>
> 返回值：void
## GetItem方法
**GetItem(Index)**
>
> 参数：Index，类型：int
>
> 返回值：java.lang.String
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## IndexOf方法
**IndexOf(value)**
>
> 参数：value，类型：java.lang.CharSequence
>
> 返回值：int
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Initialize2方法
**Initialize2(ba,EventName,Theme)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Theme，类型：int
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## AddAll方法
**AddAll(List)**
>
> 参数：List，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## RemoveAt方法
**RemoveAt(Index)**
>
> 参数：Index，类型：int
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## SelectedIndex属性

?> 说明：获取或设置所选项的索引。如果没有项目，则返回-1
>
> 参数：value，类型：int
>
> 返回值：int
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
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
## Size属性

?> 说明：返回项目数
>
> 返回值：int
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## TextSize属性
>
> 参数：TextSize，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## DropdownBackgroundColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
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
## Prompt属性

?> 说明：设置或获取打开微调器时将显示的标题。
>
> 参数：title，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## DropdownTextColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Height属性

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## TextColor属性
>
> 参数：Color，类型：int
>
> 返回值：int
## Tag属性
>
> 参数：arg0，类型：java.lang.Object
>
> 返回值：java.lang.Object
## SelectedItem属性

?> 说明：返回所选项目的值
>
> 返回值：java.lang.String
## Width属性

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## THEME_LIGHT字段
>
> 返回值：int
## THEME_DARK字段
>
> 返回值：int

# ACSeekBar
完整类名：de.amberhome.objects.appcompat.ACSeekBarWrapper
> 所有者：activity

> 包装器：android.widget.SeekBar

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> ValueChanged (Value As Int, UserChanged As Boolean)
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Initialize2方法
**Initialize2(ba,EventName,Style)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Style，类型：java.lang.String
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Max属性
>
> 参数：arg0，类型：int
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
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
>
> 返回值：int
## Value属性
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## Tag属性
>
> 参数：arg0，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int

# ACSearchView
完整类名：de.amberhome.objects.appcompat.ACSearchViewWrapper
> 所有者：activity

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> QuerySubmitted (Query as String)
>
> QueryChanged (Query as String)
>
> Closed
## Initialize2方法
**Initialize2(ba,EventName,Theme)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Theme，类型：int
>
> 返回值：void
## Submit方法
**Submit()**

?> 说明：按程序提交搜索短语。
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Query属性

?> 说明：设置/获取查询文本
>
> 参数：Query，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## QueryHint属性

?> 说明：设置/获取查询提示
>
> 参数：Hint，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## SubmitButtonEnabled属性

?> 说明：如果启用了提交按钮，则设置/获取
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## IconifiedByDefault属性

?> 说明：如果默认情况下SearchView已图标化，则设置/获取
>
> 参数：Iconified，类型：boolean
>
> 返回值：boolean
## Iconfied属性

?> 说明：如果SerachView已图标化，则设置/获取
>
> 参数：Iconified，类型：boolean
>
> 返回值：boolean
## mSearchView字段
>
> 返回值：android.support.v7.widget.SearchView
## THEME_LIGHT字段
>
> 返回值：int
## THEME_DARK字段
>
> 返回值：int

# ACRadioButton
完整类名：de.amberhome.objects.appcompat.ACRadioButtonWrapper
> 所有者：activity

> 包装器：android.widget.RadioButton

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> CheckedChange(Checked As Boolean)
## innerInitialize2方法
**innerInitialize2(ba,eventName,keepOldObject,style)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：eventName，类型：java.lang.String
>
> 参数：keepOldObject，类型：boolean
>
> 参数：style，类型：java.lang.String
>
> 返回值：void
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：float
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Initialize2方法
**Initialize2(ba,EventName,Style)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Style，类型：java.lang.String
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：arg0，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性
>
> 返回值：java.lang.Object
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## TextSize属性
>
> 参数：arg0，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：arg0，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Checked属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Ellipsize属性
>
> 参数：arg0，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## TextColor属性
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

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## SingleLine属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：arg0，类型：int
>
> 返回值：int

# ACPopupMenu
完整类名：de.amberhome.objects.appcompat.ACPopupMenuWrapper
> 所有者：activity

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> ItemClicked (Item As ACMenuItem)
>
> Closed
## GetItem方法
**GetItem(ItemId)**

?> 说明：获取给定Id的菜单项对象
>
> 参数：ItemId，类型：int
>
> 返回值：android.view.MenuItem
## Initialize2方法
**Initialize2(ba,EventName,View,style)**

?> 说明：初始化弹出菜单
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：View，类型：android.view.View
>
> 参数：style，类型：java.lang.String
>
> 返回值：void
## AddMenuItem方法
**AddMenuItem(ItemId,Title,Icon)**

?> 说明：添加新的菜单项，然后返回。
>
> 参数：ItemId，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## Show方法
**Show()**

?> 说明：显示弹出菜单。
>
> 返回值：void
## Close方法
**Close()**

?> 说明：关闭弹出菜单
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName,View)**

?> 说明：初始化弹出菜单
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：View，类型：android.view.View
>
> 返回值：void
## RemoveMenuItem方法
**RemoveMenuItem(ItemId)**

?> 说明：删除菜单项
>
> 参数：ItemId，类型：int
>
> 返回值：void
## GetMenu方法
**GetMenu()**

?> 说明：获取菜单对象
>
> 返回值：de.amberhome.objects.appcompat.ACMenuWrapper

# ACMenu
完整类名：de.amberhome.objects.appcompat.ACMenuWrapper
> 所有者：process

> 包装器：android.view.Menu

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
## Add方法
**Add(ItemId,SortOrder,Title,Icon)**

?> 说明：将菜单项添加到菜单
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.Bitmap
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## AddWithGroup2方法
**AddWithGroup2(GroupId,ItemId,SortOrder,Title,Icon)**

?> 说明：将菜单项添加到菜单中，并将此项放入一个组中。
>
> 参数：GroupId，类型：int
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## Size方法
**Size()**

?> 说明：返回菜单中的项数
>
> 返回值：int
## SetGroupCheckable方法
**SetGroupCheckable(GroupId,Checkable,Exclusive)**

?> 说明：使组中的所有项目都可检查
>
> 参数：GroupId，类型：int
>
> 参数：Checkable，类型：boolean
>
> 参数：Exclusive，类型：boolean
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## RemoveGroup方法
**RemoveGroup(GroupId)**

?> 说明：从菜单中删除组
>
> 参数：GroupId，类型：int
>
> 返回值：void
## SetGroupEnabled方法
**SetGroupEnabled(GroupId,Enable)**

?> 说明：启用/禁用给定的组
>
> 参数：GroupId，类型：int
>
> 参数：Enable，类型：boolean
>
> 返回值：void
## Add2方法
**Add2(ItemId,SortOrder,Title,Icon)**

?> 说明：将菜单项添加到菜单
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## Clear方法
**Clear()**

?> 说明：清除菜单中的所有菜单项。
>
> 返回值：void
## GetItem方法
**GetItem(Index)**

?> 说明：返回具有给定索引的项。
>
> 参数：Index，类型：int
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## RemoveItem方法
**RemoveItem(ItemId)**

?> 说明：从菜单中删除项目
>
> 参数：ItemId，类型：int
>
> 返回值：void
## AddSubMenu方法
**AddSubMenu(GroupId,ItemId,SortOrder,Title)**

?> 说明：将子菜单添加到菜单中。
>
> 参数：GroupId，类型：int
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：de.amberhome.objects.appcompat.ACSubMenuWrapper
## FindItem方法
**FindItem(ItemId)**

?> 说明：返回具有给定Id的项。如果找不到该项，则返回null。
>
> 参数：ItemId，类型：int
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper
## SetGroupVisible方法
**SetGroupVisible(GroupId,Visible)**

?> 说明：使给定的组可见/不可见
>
> 参数：GroupId，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## Close方法
**Close()**

?> 说明：如果菜单处于打开状态，请将其关闭。
>
> 返回值：void
## AddWithGroup方法
**AddWithGroup(GroupId,ItemId,SortOrder,Title,Icon)**

?> 说明：将菜单项添加到菜单中，并将此项放入一个组中
>
> 参数：GroupId，类型：int
>
> 参数：ItemId，类型：int
>
> 参数：SortOrder，类型：int
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Icon，类型：android.graphics.Bitmap
>
> 返回值：de.amberhome.objects.appcompat.ACMenuItemWrapper

# ACMenuItem
完整类名：de.amberhome.objects.appcompat.ACMenuItemWrapper
> 所有者：process

> 包装器：android.view.MenuItem

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## ActionView属性

?> 说明：为此菜单项设置ActionView。
>
> 参数：View，类型：android.view.View
>
> 返回值：
## Enabled属性

?> 说明：启用/禁用项目
>
> 参数：Enabled，类型：boolean
>
> 返回值：boolean
## Title属性

?> 说明：设置/获取菜单的标题
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## SubMenu属性

?> 说明：获取此项的子菜单（如果有）。
>
> 返回值：de.amberhome.objects.appcompat.ACSubMenuWrapper
## GroupId属性

?> 说明：获取项的组id。
>
> 返回值：int
## Checked属性

?> 说明：检查项目
>
> 参数：Checked，类型：boolean
>
> 返回值：boolean
## ShowAsAction属性

?> 说明：如果可能，将菜单项显示为操作。
>
> 参数：ActionType，类型：int
>
> 返回值：
## SearchView属性

?> 说明：将搜索视图连接到此MenuItem。
>
> 参数：SearchView，类型：de.amberhome.objects.appcompat.ACSearchViewWrapper
>
> 返回值：
## Visible属性

?> 说明：显示/隐藏项目
>
> 参数：Visible，类型：boolean
>
> 返回值：boolean
## ItemCollapsed属性

?> 说明：将项目设置/设置为折叠模式。（例如，对于SearchView）
>
> 参数：Flag，类型：boolean
>
> 返回值：boolean
## Icon属性

?> 说明：设置或获取菜单项的图标。
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Checkable属性

?> 说明：使项目可检查
>
> 参数：Cheackable，类型：boolean
>
> 返回值：boolean
## Id属性

?> 说明：获取项目id
>
> 返回值：int
## SHOW_AS_ACTION_IF_ROOM字段
>
> 返回值：int
## SHOW_AS_ACTION_NEVER字段
>
> 返回值：int
## SHOW_AS_ACTION_ALWAYS字段
>
> 返回值：int
## SHOW_AS_ACTION_WITH_TEXT字段
>
> 返回值：int

# ACFlatButton
完整类名：de.amberhome.objects.appcompat.ACFlatButtonWrapper
> 所有者：activity

> 包装器：android.widget.Button

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> Click
>
> Down
>
> LongClick
>
> Up
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：float
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Initialize2方法
**Initialize2(ba,EventName,Style)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Style，类型：java.lang.String
>
> 返回值：void
## SetButtonColors方法
**SetButtonColors(PressedColor,EnabledColor,DisabledColor)**

?> 说明：更改按钮颜色
>
> 参数：PressedColor，类型：int
>
> 参数：EnabledColor，类型：int
>
> 参数：DisabledColor，类型：int
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，动画将
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：arg0，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性
>
> 返回值：java.lang.Object
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## TextSize属性
>
> 参数：arg0，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：arg0，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## ButtonColor属性

?> 说明：更改按钮颜色
>
> 参数：Color，类型：int
>
> 返回值：
## Ellipsize属性
>
> 参数：arg0，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## TextColor属性
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

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## SingleLine属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：arg0，类型：int
>
> 返回值：int

# ACEditText
完整类名：de.amberhome.objects.appcompat.ACEditTextWrapper
> 所有者：activity

> 包装器：android.widget.EditText

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> EnterPressed
>
> FocusChanged (HasFocus As Boolean)
>
> TextChanged (Old As String, New As String)
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## setTintColor方法
**setTintColor(DefaultColor,FocusedColor,DisabledColor)**
>
> 参数：DefaultColor，类型：int
>
> 参数：FocusedColor，类型：int
>
> 参数：DisabledColor，类型：int
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## SelectAll方法
**SelectAll()**
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：float
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## SetSelection方法
**SetSelection(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 返回值：void
## Initialize2方法
**Initialize2(ba,EventName,Style)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Style，类型：java.lang.String
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Wrap属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## ForceDoneButton属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## Hint属性
>
> 参数：arg0，类型：java.lang.String
>
> 返回值：java.lang.String
## Parent属性
>
> 返回值：java.lang.Object
## SelectionStart属性
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## TextColor属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## Width属性

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## Gravity属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## HintColor属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：arg0，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## TextSize属性
>
> 参数：arg0，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## PasswordMode属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## Text属性
>
> 参数：arg0，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Ellipsize属性
>
> 参数：arg0，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
>
> 返回值：int
## InputType属性
>
> 参数：arg0，类型：int
>
> 返回值：int
## Tag属性
>
> 参数：arg0，类型：java.lang.Object
>
> 返回值：java.lang.Object
## SingleLine属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## SelectionLength属性
>
> 返回值：int
## INPUT_TYPE_NONE字段
>
> 返回值：int
## INPUT_TYPE_TEXT字段
>
> 返回值：int
## INPUT_TYPE_NUMBERS字段
>
> 返回值：int
## INPUT_TYPE_DECIMAL_NUMBERS字段
>
> 返回值：int
## INPUT_TYPE_PHONE字段
>
> 返回值：int

# ACColoredButton
完整类名：de.amberhome.objects.appcompat.ACColoredButtonWrapper
> 所有者：activity

> 包装器：android.widget.Button

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> Up
>
> Down
>
> Click
>
> LongClick
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：float
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Initialize2方法
**Initialize2(ba,EventName,Style)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Style，类型：java.lang.String
>
> 返回值：void
## SetButtonColors方法
**SetButtonColors(PressedColor,EnabledColor,DisabledColor)**

?> 说明：更改按钮颜色
>
> 参数：PressedColor，类型：int
>
> 参数：EnabledColor，类型：int
>
> 参数：DisabledColor，类型：int
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，动画将
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：arg0，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性
>
> 返回值：java.lang.Object
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## TextSize属性
>
> 参数：arg0，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：arg0，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## ButtonColor属性

?> 说明：更改按钮颜色
>
> 参数：Color，类型：int
>
> 返回值：
## Ellipsize属性
>
> 参数：arg0，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## TextColor属性
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

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## SingleLine属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：arg0，类型：int
>
> 返回值：int

# ACCheckBox
完整类名：de.amberhome.objects.appcompat.ACCheckBoxWrapper
> 所有者：activity

> 包装器：android.widget.CheckBox

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> CheckedChange(Checked As Boolean)
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：float
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Initialize2方法
**Initialize2(ba,EventName,Style)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Style，类型：java.lang.String
>
> 返回值：void
## SetCheckBoxColors方法
**SetCheckBoxColors(EnabledColor,CheckedColor,DisabledColor)**

?> 说明：设置复选框的颜色
>
> 参数：EnabledColor，类型：int
>
> 参数：CheckedColor，类型：int
>
> 参数：DisabledColor，类型：int
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：arg0，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性
>
> 返回值：java.lang.Object
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## TextSize属性
>
> 参数：arg0，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：arg0，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Checked属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Ellipsize属性
>
> 参数：arg0，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## TextColor属性
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

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## SingleLine属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：arg0，类型：int
>
> 返回值：int

# ACButton
完整类名：de.amberhome.objects.appcompat.ACButtonWrapper
> 所有者：activity

> 包装器：android.widget.Button

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> Up
>
> Down
>
> Click
>
> LongClick
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## SetTextSizeAnimated方法
**SetTextSizeAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：float
>
> 返回值：void
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SetTextColorAnimated方法
**SetTextColorAnimated(arg0,arg1)**
>
> 参数：arg0，类型：int
>
> 参数：arg1，类型：int
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Initialize2方法
**Initialize2(ba,EventName,Style)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Style，类型：java.lang.String
>
> 返回值：void
## SetButtonColors方法
**SetButtonColors(PressedColor,EnabledColor,DisabledColor)**

?> 说明：更改按钮颜色
>
> 参数：PressedColor，类型：int
>
> 参数：EnabledColor，类型：int
>
> 参数：DisabledColor，类型：int
>
> 返回值：void
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，动画将
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
>
> 返回值：int
## Background属性
>
> 参数：arg0，类型：android.graphics.drawable.Drawable
>
> 返回值：android.graphics.drawable.Drawable
## Typeface属性
>
> 参数：arg0，类型：android.graphics.Typeface
>
> 返回值：android.graphics.Typeface
## Parent属性
>
> 返回值：java.lang.Object
## Color属性
>
> 参数：arg0，类型：int
>
> 返回值：
## TextSize属性
>
> 参数：arg0，类型：float
>
> 返回值：float
## Enabled属性
>
> 参数：arg0，类型：boolean
>
> 返回值：boolean
## Text属性
>
> 参数：arg0，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## ButtonColor属性

?> 说明：更改按钮颜色
>
> 参数：Color，类型：int
>
> 返回值：
## Ellipsize属性
>
> 参数：arg0，类型：java.lang.String
>
> 返回值：java.lang.String
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## TextColor属性
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

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## SingleLine属性
>
> 参数：arg0，类型：boolean
>
> 返回值：
## Gravity属性
>
> 参数：arg0，类型：int
>
> 返回值：int

# ACActionMode
完整类名：de.amberhome.objects.appcompat.ACActionModeWrapper
> 所有者：activity

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> ItemClicked (Item As ACMenuItem)
>
> Created (Menu as ACMenu)
>
> Prepared (Menu as ACMenu)
>
> Closed
## Start方法
**Start()**

?> 说明：启动ActionMode
>
> 返回值：void
## IsActive方法
**IsActive()**

?> 说明：如果ActionMode当前处于活动状态，则返回true
>
> 返回值：boolean
## Invalidate方法
**Invalidate()**

?> 说明：使ActionMode无效并重新创建菜单。如果调用此方法，则会再次调用_Prepared事件，其中可以修改菜单。
>
> 返回值：void
## Initialize方法
**Initialize(ba,EventName)**

?> 说明：初始化ActionMode对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Finish方法
**Finish()**

?> 说明：结束ActionMode并关闭上下文ActionBar
>
> 返回值：void
## Title属性

?> 说明：设置或获取标题
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## SubTitle属性

?> 说明：设置或获取子标题
>
> 参数：SubTitle，类型：java.lang.CharSequence
>
> 返回值：java.lang.String

# ACActionMenu
完整类名：de.amberhome.objects.appcompat.ACActionMenuWrapper
> 所有者：activity

> 包装器：android.support.v7.widget.ActionMenuView

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
> 事件：
>
> MenuItemClick (Item as ACMenuItem)
## DesignerCreateView方法
**DesignerCreateView(base,label,props)**

?> 说明：此方法仅适用于B4A设计师。不要直呼
>
> 参数：base，类型：anywheresoftware.b4a.objects.PanelWrapper
>
> 参数：label，类型：anywheresoftware.b4a.objects.LabelWrapper
>
> 参数：props，类型：anywheresoftware.b4a.objects.collections.Map
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
## SetLayout方法
**SetLayout(Left,Top,Width,Height)**

?> 说明：更改视图的位置和大小。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## BringToFront方法
**BringToFront()**
>
> 返回值：void
## SendToBack方法
**SendToBack()**
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## RemoveView方法
**RemoveView()**
>
> 返回值：void
## Invalidate3方法
**Invalidate3(Left,Top,Right,Bottom)**

?> 说明：使部分对象无效
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Right，类型：int
>
> 参数：Bottom，类型：int
>
> 返回值：void
## Invalidate2方法
**Invalidate2(Rect)**

?> 说明：使对象的矩形部分无效
>
> 参数：Rect，类型：android.graphics.Rect
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：将颜色设置为新值的动画
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetBackgroundImageNew方法
**SetBackgroundImageNew(arg0)**
>
> 参数：arg0，类型：android.graphics.Bitmap
>
> 返回值：anywheresoftware.b4a.objects.drawable.BitmapDrawable
## Invalidate方法
**Invalidate()**
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：类似于SetLayout。设置更改的动画。请注意，只有在Android 3+设备上运行时才会应用动画。
>
> 参数：Duration，类型：int
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：void
## RequestFocus方法
**RequestFocus()**
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置视图的左侧位置
>
> 参数：Left，类型：int
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
## OverflowMenuOpen属性

?> 说明：显示/隐藏溢出菜单，如果当前正在显示溢出菜单，则返回。
>
> 参数：Show，类型：boolean
>
> 返回值：boolean
## Top属性

?> 说明：获取或设置视图的顶部位置
>
> 参数：Top，类型：int
>
> 返回值：int
## PopupTheme属性

?> 说明：设置弹出式菜单主题。
>
> 参数：Theme，类型：int
>
> 返回值：
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

?> 说明：获取或设置视图的高度
>
> 参数：Height，类型：int
>
> 返回值：int
## Menu属性

?> 说明：获取ActionMenu的菜单。
>
> 返回值：de.amberhome.objects.appcompat.ACMenuWrapper
## Tag属性
>
> 参数：arg0，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Width属性

?> 说明：获取或设置视图的宽度
>
> 参数：Width，类型：int
>
> 返回值：int
## THEME_LIGHT字段
>
> 返回值：int
## THEME_DARK字段
>
> 返回值：int

# ACActionBar
完整类名：de.amberhome.objects.appcompat.ACActionBar
> 所有者：activity

> 依赖：com.android.support:appcompat-v7 | androidx.emoji2:emoji2-views | androidx.emoji2:emoji2-views-helper | androidx.arch.core:core-common | androidx.arch.core:core-runtime | kotlin-stdlib-1.6.10 | AppCompat.aar
## Hide方法
**Hide()**

?> 说明：隐藏操作栏
>
> 返回值：void
## IsShowing方法
**IsShowing()**

?> 说明：返回ActionBar当前是否隐藏。
>
> 返回值：boolean
## Show方法
**Show()**

?> 说明：显示操作栏
>
> 返回值：void
## Initialize方法
**Initialize(ba)**

?> 说明：初始化对象
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Subtitle属性

?> 说明：设置或获取ActionBar的副标题
>
> 参数：cs，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Elevation属性

?> 说明：设置或获取ActionBar的高程。只对Android 5.0及以上版本有影响。
>
> 参数：Elevation，类型：int
>
> 返回值：float
## TitleVisible属性

?> 说明：显示/隐藏标题
>
> 参数：Value，类型：boolean
>
> 返回值：
## ShowUpIndicator属性
>
> 参数：b，类型：boolean
>
> 返回值：
## UpIndicatorDrawable属性

?> 说明：将上指示灯设置为可抽出式。有助于实现
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：
## Title属性

?> 说明：设置或获取ActionBar的标题
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Icon属性

?> 说明：设置ActionBar的图标
>
> 参数：Icon，类型：android.graphics.drawable.Drawable
>
> 返回值：
## UpIndicatorBitmap属性

?> 说明：设置指示器位图。有助于实现
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：
## HomeVisible属性

?> 说明：显示/隐藏主页图标
>
> 参数：Value，类型：boolean
>
> 返回值：
## Logo属性

?> 说明：将徽标设置为图标
>
> 参数：Logo，类型：android.graphics.drawable.Drawable
>
> 返回值：

# XUI

版本:2.3
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=XUI)

# B4XView
完整类名：anywheresoftware.b4a.objects.B4XViewWrapper
> 所有者：activity

> 包装器：java.lang.Object
## GetView方法
**GetView(Index)**

?> 说明：返回给定索引处的视图。
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper
## AddView方法
**AddView(View,Left,Top,Width,Height)**

?> 说明：添加视图。
>
> 参数：View，类型：android.view.View
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
## GetBitmap方法
**GetBitmap()**

?> 说明：获取视图的位图。
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## SelectAll方法
**SelectAll()**

?> 说明：选择所有文本。
>
> 返回值：void
## GetAllViewsRecursive方法
**GetAllViewsRecursive()**

?> 说明：返回一个迭代器，该迭代器遍历所有子视图，包括添加到其他子视图的视图。
```vbnet

For Each v As B4XView In Panel1.GetAllViewsRecursive
	...
Next
```

>
> 返回值：anywheresoftware.b4a.BA.IterableList
## SetTextSizeAnimated方法
**SetTextSizeAnimated(Duration,TextSize)**

?> 说明：设置文本大小。
>
> 参数：Duration，类型：int
>
> 参数：TextSize，类型：float
>
> 返回值：void
## BringToFront方法
**BringToFront()**

?> 说明：更改此视图的Z顺序并将其置于前面。
>
> 返回值：void
## SendToBack方法
**SendToBack()**

?> 说明：更改此视图的Z顺序并将其发送到后面。
>
> 返回值：void
## SetColorAndBorder方法
**SetColorAndBorder(BackgroundColor,BorderWidth,BorderColor,BorderCornerRadius)**

?> 说明：设置背景颜色和边框。
>
> 参数：BackgroundColor，类型：int
>
> 参数：BorderWidth，类型：int
>
> 参数：BorderColor，类型：int
>
> 参数：BorderCornerRadius，类型：int
>
> 返回值：void
## SetVisibleAnimated方法
**SetVisibleAnimated(Duration,Visible)**

?> 说明：淡入或淡出视图。
>
> 参数：Duration，类型：int
>
> 参数：Visible，类型：boolean
>
> 返回值：void
## SetRotationAnimated方法
**SetRotationAnimated(Duration,Degree)**

?> 说明：使用动画旋转视图。
>
> 参数：Duration，类型：int
>
> 参数：Degree，类型：float
>
> 返回值：void
## SetBitmap方法
**SetBitmap(Bitmap)**

?> 说明：设置视图的位图。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 返回值：void
## SetAlphaAnimated方法
**SetAlphaAnimated(Duration,Alpha)**

?> 说明：为视图的alpha级别设置动画。
>
> 参数：Duration，类型：int
>
> 参数：Alpha，类型：float
>
> 返回值：void
## SetTextAlignment方法
**SetTextAlignment(Vertical,Horizontal)**

?> 说明：设置文本对齐方式。
>
> 参数：Vertical，类型：java.lang.String
>
> 参数：Horizontal，类型：java.lang.String
>
> 返回值：void
## LoadLayout方法
**LoadLayout(LayoutFile,ba)**

?> 说明：加载布局文件。
>
> 参数：LayoutFile，类型：java.lang.String
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## SetColorAnimated方法
**SetColorAnimated(Duration,FromColor,ToColor)**

?> 说明：使用“FromColor”和“ToColor”颜色之间的过渡动画更改背景颜色。
>
> 参数：Duration，类型：int
>
> 参数：FromColor，类型：int
>
> 参数：ToColor，类型：int
>
> 返回值：void
## SetSelection方法
**SetSelection(Start,Length)**

?> 说明：设置选择。
>
> 参数：Start，类型：int
>
> 参数：Length，类型：int
>
> 返回值：void
## RemoveViewFromParent方法
**RemoveViewFromParent()**

?> 说明：从其父视图中删除视图。
>
> 返回值：void
## Snapshot方法
**Snapshot()**

?> 说明：捕捉视图外观。
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## RemoveAllViews方法
**RemoveAllViews()**

?> 说明：删除所有视图。
>
> 返回值：void
## SetLayoutAnimated方法
**SetLayoutAnimated(Duration,Left,Top,Width,Height)**

?> 说明：设置视图的大小和位置。
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

?> 说明：请求将焦点设置为此视图。如果焦点发生偏移，则返回True。
>
> 返回值：boolean
## Left属性

?> 说明：获取或设置左侧位置。
>
> 参数：d，类型：int
>
> 返回值：int
## Parent属性

?> 说明：返回父级。如果没有父对象，则返回的对象将被取消初始化。
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper
## EditTextHint属性

?> 说明：获取或设置提示或提示文本。支持的类型：
>
> 参数：s，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## NumberOfViews属性

?> 说明：返回直接子视图的数目。
>
> 返回值：int
## SelectionStart属性

?> 说明：获取或设置选择开始索引。
>
> 参数：s，类型：int
>
> 返回值：int
## Font属性

?> 说明：获取或设置字体（字体和文本大小）。
>
> 参数：f，类型：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
## Visible属性

?> 说明：获取或设置视图是否可见。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## Height属性

?> 说明：获取或设置视图的高度。
>
> 参数：d，类型：int
>
> 返回值：int
## TextColor属性

?> 说明：获取或设置文本颜色。支持的类型：
>
> 参数：c，类型：int
>
> 返回值：int
## Width属性

?> 说明：获取或设置视图的宽度。
>
> 参数：d，类型：int
>
> 返回值：int
## Progress属性

?> 说明：获取或设置进度值。进度值在0到100之间缩放（这与B4J和B4i中的原生视图范围不同）。
>
> 参数：i，类型：int
>
> 返回值：int
## ScrollViewContentWidth属性

?> 说明：获取或设置滚动视图内部面板宽度。
>
> 参数：d，类型：int
>
> 返回值：int
## ScrollViewInnerPanel属性

?> 说明：获取或设置滚动视图内部面板。
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper
## Color属性

?> 说明：获取或设置背景颜色。如果颜色不可用，则返回0。
>
> 参数：Color，类型：int
>
> 返回值：int
## Enabled属性

?> 说明：获取或设置视图是否已启用。如果视图不支持此属性，则不执行任何操作。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## TextSize属性

?> 说明：获取或设置文本大小。
>
> 参数：d，类型：float
>
> 返回值：float
## Text属性

?> 说明：获取或设置文本。支持的类型：
>
> 参数：s，类型：java.lang.CharSequence
>
> 返回值：java.lang.String
## Rotation属性

?> 说明：获取或设置视图的旋转变换（以度为单位）。
>
> 参数：f，类型：float
>
> 返回值：float
## Checked属性

?> 说明：获取或设置选中状态（也称为选定状态或值）。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## ScrollViewContentHeight属性

?> 说明：获取或设置滚动视图内部面板的高度。
>
> 参数：d，类型：int
>
> 返回值：int
## ScrollViewOffsetX属性

?> 说明：获取或设置水平滚动位置。
>
> 参数：d，类型：int
>
> 返回值：int
## Top属性

?> 说明：获取或设置顶部位置。
>
> 参数：d，类型：int
>
> 返回值：int
## ScrollViewOffsetY属性

?> 说明：获取或设置垂直滚动位置。
>
> 参数：d，类型：int
>
> 返回值：int
## Alpha属性

?> 说明：获取或设置视图的alpha级别：0-透明，1（默认）完全不透明。
>
> 参数：alpha，类型：float
>
> 返回值：float
## Tag属性

?> 说明：获取或设置视图的标记对象。
>
> 参数：o，类型：java.lang.Object
>
> 返回值：java.lang.Object
## SelectionLength属性

?> 说明：获取选择长度。
>
> 返回值：int
## TOUCH_ACTION_UP字段
>
> 返回值：int
## TOUCH_ACTION_DOWN字段
>
> 返回值：int
## TOUCH_ACTION_MOVE_NOTOUCH字段

?> 说明：相当于B4J中的MouseMoved（永远不会在B4A或B4i中饲养）。
>
> 返回值：int
## TOUCH_ACTION_MOVE字段

?> 说明：相当于B4J中的鼠标碎片。
>
> 返回值：int

# B4XBitmap
完整类名：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
> 所有者：process

> 包装器：android.graphics.Bitmap

?> 说明：表示已加载的图像。类似于B4A位图、B4i位图和B4J图像。
## Crop方法
**Crop(Left,Top,Width,Height)**

?> 说明：返回<b>新的</b>裁剪位图。
>
> 参数：Left，类型：int
>
> 参数：Top，类型：int
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## Rotate方法
**Rotate(Degrees)**

?> 说明：返回<b>新的</b>旋转位图。位图将顺时针旋转。
>
> 参数：Degrees，类型：int
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## Resize方法
**Resize(Width,Height,KeepAspectRatio)**

?> 说明：返回具有给定宽度和高度的<b>新</b>位图。
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 参数：KeepAspectRatio，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## WriteToStream方法
**WriteToStream(Out,Quality,Format)**

?> 说明：将位图写入输出流。
```vbnet

Dim Out As OutputStream
Out = File.OpenOutput(XUI.DefaultFolder, "Test.png", False)
Bitmap1.WriteToStream(out, 100, "PNG")
Out.Close
```

>
> 参数：Out，类型：java.io.OutputStream
>
> 参数：Quality，类型：int
>
> 参数：Format，类型：android.graphics.Bitmap.CompressFormat
>
> 返回值：void
## Height属性

?> 说明：返回位图的高度。
>
> 返回值：double
## Scale属性

?> 说明：返回位图比例。在B4J和B4i中永远是1。
>
> 返回值：float
## Width属性

?> 说明：返回位图的宽度。
>
> 返回值：double

# B4XFont
完整类名：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
> 所有者：process

?> 说明：有字体和大小的物体。
## ToNativeFont方法
**ToNativeFont()**

?> 说明：返回表示相同字体的本机字体对象。
>
> 返回值：anywheresoftware.b4a.keywords.constants.TypefaceWrapper
## Size属性
>
> 返回值：float
## IsInitialized属性
>
> 返回值：boolean

# XUI
完整类名：anywheresoftware.b4a.objects.B4XViewWrapper.XUI
> 所有者：process

?> 说明：XUI对象包括各种方法和实用程序。
## Msgbox2Async方法
**Msgbox2Async(ba,Message,Title,Positive,Cancel,Negative,Icon)**

?> 说明：显示非模态消息框。
```vbnet

Dim sf As Object = xui.Msgbox2Async("Delete file?", "Title", "Yes", "Cancel", "No", Null)
Wait For (sf) Msgbox_Result (Result As Int)
If Result = xui.DialogResponse_Positive Then
	Log("Deleted!!!")
End If
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Message，类型：java.lang.CharSequence
>
> 参数：Title，类型：java.lang.CharSequence
>
> 参数：Positive，类型：java.lang.String
>
> 参数：Cancel，类型：java.lang.String
>
> 参数：Negative，类型：java.lang.String
>
> 参数：Icon，类型：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
>
> 返回值：java.lang.Object
## LoadBitmapResize方法
**LoadBitmapResize(Dir,FileName,Width,Height,KeepAspectRatio)**

?> 说明：加载位图并调整其大小。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 参数：KeepAspectRatio，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## PaintOrColorToColor方法
**PaintOrColorToColor(Color)**

?> 说明：B4A，B4i——什么都不做。
>
> 参数：Color，类型：java.lang.Object
>
> 返回值：int
## CreateFont方法
**CreateFont(Typeface,Size)**

?> 说明：根据给定的字体和大小创建一个新的B4X字体。
>
> 参数：Typeface，类型：android.graphics.Typeface
>
> 参数：Size，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
## GetRegisteredDesignerClass方法
**GetRegisteredDesignerClass(Module)**

?> 说明：获取已注册的设计器类实例。如果不存在，则返回Null。
>
> 参数：Module，类型：java.lang.String
>
> 返回值：java.lang.Object
## CreateDefaultFont方法
**CreateDefaultFont(Size)**

?> 说明：使用默认字体创建一个新的B4XFont。
>
> 参数：Size，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
## CreateDefaultBoldFont方法
**CreateDefaultBoldFont(Size)**

?> 说明：使用默认的粗体创建一个新的B4XFont。
>
> 参数：Size，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
## CreatePanel方法
**CreatePanel(ba,EventName)**

?> 说明：创建面板（或B4J中的窗格）。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper
## RegisterDesignerClass方法
**RegisterDesignerClass(ClassInstance)**

?> 说明：注册设计器脚本类。
>
> 参数：ClassInstance，类型：java.lang.Object
>
> 返回值：void
## LoadBitmap方法
**LoadBitmap(Dir,FileName)**

?> 说明：加载位图。在大多数情况下，您应该使用LoadBitmapResize。
>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## CreateFontAwesome方法
**CreateFontAwesome(Size)**

?> 说明：基于FontAwesome字体创建新的B4XFont。
>
> 参数：Size，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
## CreateMaterialIcons方法
**CreateMaterialIcons(Size)**

?> 说明：基于材质图标字体创建新的B4X字体。
>
> 参数：Size，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
## Color_ARGB方法
**Color_ARGB(Alpha,R,G,B)**

?> 说明：返回组件的颜色值。值应介于0到255之间。
>
> 参数：Alpha，类型：int
>
> 参数：R，类型：int
>
> 参数：G，类型：int
>
> 参数：B，类型：int
>
> 返回值：int
## FileUri方法
**FileUri(Dir,FileName)**

?> 说明：返回一个文件uri。这可以与WebView一起使用以访问本地资源。
```vbnet

WebView1.LoadHtml($"<img src="${xui.FileUri(File.DirAssets, "smiley.png")}" />"$)
'or:
WebView1.LoadUrl($"${xui.FileUri(File.DirAssets, "smiley.png")}"$)

```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 返回值：java.lang.String
## SetDataFolder方法
**SetDataFolder(AppName)**

?> 说明：B4A，B4i——什么都不做。
>
> 参数：AppName，类型：java.lang.String
>
> 返回值：void
## MsgboxAsync方法
**MsgboxAsync(ba,Message,Title)**

?> 说明：显示非模态消息框。
```vbnet
xui.MsgboxAsync("Hello", "World")
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Message，类型：java.lang.CharSequence
>
> 参数：Title，类型：java.lang.CharSequence
>
> 返回值：java.lang.Object
## Color_RGB方法
**Color_RGB(R,G,B)**

?> 说明：返回组件的颜色值。值应介于0到255之间。
>
> 参数：R，类型：int
>
> 参数：G，类型：int
>
> 参数：B，类型：int
>
> 返回值：int
## SubExists方法
**SubExists(ba,Component,Sub,NotUsed)**

?> 说明：与SubExists关键字相同。添加B4i中所需的附加参数（参数数量）。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Component，类型：java.lang.Object
>
> 参数：Sub，类型：java.lang.String
>
> 参数：NotUsed，类型：int
>
> 返回值：boolean
## CreateFont2方法
**CreateFont2(B4XFont,Size)**

?> 说明：根据给定的B4X字体和大小创建新的B4X样式。
>
> 参数：B4XFont，类型：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
>
> 参数：Size，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
## IsB4i属性

?> 说明：在B4i中返回True。
>
> 返回值：boolean
## IsB4J属性

?> 说明：在B4J中返回True。
>
> 返回值：boolean
## Scale属性

?> 说明：返回屏幕标准化比例。
>
> 返回值：float
## IsB4A属性

?> 说明：在B4A中返回True。
>
> 返回值：boolean
## DefaultFolder属性

?> 说明：B4A-与File.DirInternal相同。
>
> 返回值：java.lang.String
## DialogResponse_Positive字段
>
> 返回值：int
## Color_Gray字段
>
> 返回值：int
## Color_Magenta字段
>
> 返回值：int
## Color_Cyan字段
>
> 返回值：int
## Color_Black字段
>
> 返回值：int
## Color_Blue字段
>
> 返回值：int
## Color_Transparent字段
>
> 返回值：int
## DialogResponse_Negative字段
>
> 返回值：int
## Color_Green字段
>
> 返回值：int
## Color_LightGray字段
>
> 返回值：int
## Color_Yellow字段
>
> 返回值：int
## Color_White字段
>
> 返回值：int
## Color_Red字段
>
> 返回值：int
## DialogResponse_Cancel字段
>
> 返回值：int
## Color_DarkGray字段
>
> 返回值：int

# B4XCanvas
完整类名：anywheresoftware.b4a.objects.B4XCanvas
> 所有者：process

?> 说明：跨平台画布。
## DrawText方法
**DrawText(ba,Text,x,y,Font,Color,Alignment)**

?> 说明：绘制文本。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Text，类型：java.lang.String
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 参数：Font，类型：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
>
> 参数：Color，类型：int
>
> 参数：Alignment，类型：android.graphics.Paint.Align
>
> 返回值：void
## ClearRect方法
**ClearRect(Rect)**

?> 说明：清除给定的矩形。在具有剪切路径的B4J中不起作用。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 返回值：void
## DrawBitmap方法
**DrawBitmap(Bitmap,Destination)**

?> 说明：在给定的目标中绘制位图。使用B4XBitmap.Crop绘制位图的一部分。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 参数：Destination，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 返回值：void
## Resize方法
**Resize(Width,Height)**

?> 说明：调整画布的大小。
>
> 参数：Width，类型：float
>
> 参数：Height，类型：float
>
> 返回值：void
## DrawPath方法
**DrawPath(Path,Color,Filled,StrokeWidth)**

?> 说明：绘制给定的路径。
>
> 参数：Path，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XPath
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 返回值：void
## DrawPathRotated方法
**DrawPathRotated(Path,Color,Filled,StrokeWidth,Degrees,CenterX,CenterY)**

?> 说明：类似于DrawPath。基于度数和中心参数旋转路径。
>
> 参数：Path，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XPath
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 参数：Degrees，类型：float
>
> 参数：CenterX，类型：float
>
> 参数：CenterY，类型：float
>
> 返回值：void
## DrawTextRotated方法
**DrawTextRotated(ba,Text,x,y,Font,Color,Alignment,Degree)**

?> 说明：类似于DrawText。在绘制文本之前旋转文本。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Text，类型：java.lang.String
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 参数：Font，类型：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
>
> 参数：Color，类型：int
>
> 参数：Alignment，类型：android.graphics.Paint.Align
>
> 参数：Degree，类型：float
>
> 返回值：void
## Initialize方法
**Initialize(View)**

?> 说明：初始化画布。
>
> 参数：View，类型：anywheresoftware.b4a.objects.B4XViewWrapper
>
> 返回值：void
## DrawCircle方法
**DrawCircle(x,y,Radius,Color,Filled,StrokeWidth)**

?> 说明：画一个圆。
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 参数：Radius，类型：float
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 返回值：void
## RemoveClip方法
**RemoveClip()**

?> 说明：删除以前设置的片段区域。
>
> 返回值：void
## CreateBitmap方法
**CreateBitmap()**

?> 说明：返回画布位图的副本。在B4A中，它返回画布位图本身（而不是副本）。
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## DrawBitmapRotated方法
**DrawBitmapRotated(Bitmap,Destination,Degrees)**

?> 说明：类似于DrawBitmap。绘制旋转位图。
>
> 参数：Bitmap，类型：android.graphics.Bitmap
>
> 参数：Destination，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Degrees，类型：float
>
> 返回值：void
## DrawLine方法
**DrawLine(x1,y1,x2,y2,Color,StrokeWidth)**

?> 说明：在x1，y1到x2，y2之间绘制一条线。
>
> 参数：x1，类型：float
>
> 参数：y1，类型：float
>
> 参数：x2，类型：float
>
> 参数：y2，类型：float
>
> 参数：Color，类型：int
>
> 参数：StrokeWidth，类型：float
>
> 返回值：void
## DrawRect方法
**DrawRect(Rect,Color,Filled,StrokeWidth)**

?> 说明：绘制一个矩形。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：float
>
> 返回值：void
## Invalidate方法
**Invalidate()**

?> 说明：提交图纸。必须调用才能更新图形。
>
> 返回值：void
## ClipPath方法
**ClipPath(Path)**

?> 说明：将图形剪裁到闭合路径。
>
> 参数：Path，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XPath
>
> 返回值：void
## MeasureText方法
**MeasureText(Text,Font)**

?> 说明：测量单行文本并返回其宽度、高度和基线以上的高度。
```vbnet

Dim r As B4XRect = cvs1.MeasureText(Text, Fnt)
Dim BaseLine As Int = CenterY - r.Height / 2 - r.Top
cvs1.DrawText(Text, CenterX, BaseLine, Fnt, Clr, "CENTER")
```

>
> 参数：Text，类型：java.lang.String
>
> 参数：Font，类型：anywheresoftware.b4a.objects.B4XViewWrapper.B4XFont
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
## Release方法
**Release()**

?> 说明：释放与画布相关的本机资源。在B4A和B4J中不执行任何操作。
>
> 返回值：void
## TargetRect属性

?> 说明：返回尺寸与目标视图相同的B4XRect。
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
## TargetView属性

?> 说明：返回目标视图。
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper

# B4XRect
完整类名：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
> 所有者：process
## Initialize方法
**Initialize(Left,Top,Right,Bottom)**
>
> 参数：Left，类型：float
>
> 参数：Top，类型：float
>
> 参数：Right，类型：float
>
> 参数：Bottom，类型：float
>
> 返回值：void
## Left属性
>
> 参数：Left，类型：float
>
> 返回值：float
## Top属性
>
> 参数：Top，类型：float
>
> 返回值：float
## Right属性
>
> 参数：Right，类型：float
>
> 返回值：float
## Bottom属性
>
> 参数：Bottom，类型：float
>
> 返回值：float
## Height属性

?> 说明：获取或设置矩形高度。
>
> 参数：h，类型：float
>
> 返回值：float
## CenterY属性

?> 说明：返回垂直中心。
>
> 返回值：float
## CenterX属性

?> 说明：返回水平中心。
>
> 返回值：float
## Width属性

?> 说明：获取或设置矩形宽度。
>
> 参数：w，类型：int
>
> 返回值：float

# B4XPath
完整类名：anywheresoftware.b4a.objects.B4XCanvas.B4XPath
> 所有者：process

> 包装器：android.graphics.Path
## LineTo方法
**LineTo(x,y)**

?> 说明：添加从最后一个点到指定点的直线。
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XPath
## InitializeRoundedRect方法
**InitializeRoundedRect(Rect,CornersRadius)**

?> 说明：初始化路径并将当前路径形状设置为圆角矩形。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：CornersRadius，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XPath
## InitializeOval方法
**InitializeOval(Rect)**

?> 说明：初始化路径并将当前路径形状设置为椭圆形。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XPath
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(x,y)**

?> 说明：初始化路径并设置第一个点的值。
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XPath
## InitializeArc方法
**InitializeArc(x,y,Radius,StartingAngle,SweepAngle)**

?> 说明：初始化路径并将当前路径形状设置为圆弧。
>
> 参数：x，类型：float
>
> 参数：y，类型：float
>
> 参数：Radius，类型：float
>
> 参数：StartingAngle，类型：float
>
> 参数：SweepAngle，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XPath

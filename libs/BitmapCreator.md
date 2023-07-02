# BitmapCreator

版本:4.73
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=BitmapCreator)

# PremultipliedColor
完整类名：b4a.example.bitmapcreator._premultipliedcolor
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## a字段
>
> 返回值：int
## r字段
>
> 返回值：int
## g字段
>
> 返回值：int
## b字段
>
> 返回值：int

# ARGBColor
完整类名：b4a.example.bitmapcreator._argbcolor
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## a字段
>
> 返回值：int
## r字段
>
> 返回值：int
## g字段
>
> 返回值：int
## b字段
>
> 返回值：int

# DrawTask
完整类名：b4a.example.bitmapcreator._drawtask
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Source字段
>
> 返回值：Object
## SrcRect字段
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
## TargetX字段
>
> 返回值：int
## TargetY字段
>
> 返回值：int
## SkipBlending字段
>
> 返回值：boolean
## SrcScaleX字段
>
> 返回值：float
## SrcScaleY字段
>
> 返回值：float
## Degrees字段
>
> 返回值：int
## Transform字段
>
> 返回值：boolean
## IsCompressedSource字段
>
> 返回值：boolean
## TargetBC字段
>
> 返回值：b4a.example.bitmapcreator
## IsCanvasTask字段
>
> 返回值：boolean
## CanvasTask字段
>
> 返回值：b4a.example.bcpath._internalcanvasdrawtask

# CompressedBC
完整类名：b4a.example.bitmapcreator._compressedbc
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Rows字段
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## mBuffer字段
>
> 返回值：byte[]
## mWidth字段
>
> 返回值：int
## mHeight字段
>
> 返回值：int
## TargetRect字段
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
## Cache字段
>
> 返回值：b4a.example.bitmapcreator._internalcompressedbccache

# InternalCompressedBCCache
完整类名：b4a.example.bitmapcreator._internalcompressedbccache
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## ColorsMap字段
>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## mBuffer字段
>
> 返回值：byte[]

# InternalAntiAliasingBuffer
完整类名：b4a.example.bitmapcreator._internalantialiasingbuffer
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## IntsArray字段
>
> 返回值：int[]

# InternalBCColumn
完整类名：b4a.example.bitmapcreator._internalbccolumn
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Values字段
>
> 返回值：float[]
## StartY字段
>
> 返回值：int
## EndY字段
>
> 返回值：int
## LeftSide字段
>
> 返回值：boolean

# BitmapCreator
完整类名：b4a.example.bitmapcreator
> 所有者：process

> 依赖：javaobject | xui
> 事件：
>
> BitmapReady (bmp As B4XBitmap)
## IsInitialized方法
**IsInitialized()**

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## _argbtocolor方法
**_argbtocolor(ARGB)**

?> 说明：将ARGB值转换为color int值。
>
> 参数：ARGB，类型：b4a.example.bitmapcreator._argbcolor
>
> 返回值：int
## _argbtopremultipliedcolor方法
**_argbtopremultipliedcolor(ARGB,PM)**

?> 说明：将ARGB颜色转换为PremultipliedColor。
>
> 参数：ARGB，类型：b4a.example.bitmapcreator._argbcolor
>
> 参数：PM，类型：b4a.example.bitmapcreator._premultipliedcolor
>
> 返回值：b4a.example.bitmapcreator._premultipliedcolor
## _asyncdrawarc方法
**_asyncdrawarc(X,Y,Radius,Brush,Filled,StrokeWidth,StartingAngle,EndAngle)**

?> 说明：异步绘制圆弧。返回应添加到绘图任务列表中的DrawTask。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 参数：Radius，类型：float
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 参数：StartingAngle，类型：float
>
> 参数：EndAngle，类型：float
>
> 返回值：b4a.example.bitmapcreator._drawtask
## _asyncdrawcircle方法
**_asyncdrawcircle(X,Y,Radius,Brush,Filled,StrokeWidth)**

?> 说明：异步地画一个圆。返回应添加到绘图任务列表中的DrawTask。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 参数：Radius，类型：float
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bitmapcreator._drawtask
## _asyncdrawline方法
**_asyncdrawline(X0,Y0,X1,Y1,Brush,StrokeWidth)**

?> 说明：异步地画一条线。返回应添加到绘图任务列表中的DrawTask。
>
> 参数：X0，类型：float
>
> 参数：Y0，类型：float
>
> 参数：X1，类型：float
>
> 参数：Y1，类型：float
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bitmapcreator._drawtask
## _asyncdrawpath方法
**_asyncdrawpath(Path,Brush,Filled,StrokeWidth)**

?> 说明：异步绘制路径。返回应添加到绘图任务列表中的DrawTask。
>
> 参数：Path，类型：b4a.example.bcpath
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bitmapcreator._drawtask
## _asyncdrawrect方法
**_asyncdrawrect(Rect,Brush,Filled,StrokeWidth)**

?> 说明：异步绘制矩形。返回应添加到绘图任务列表中的DrawTask。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bitmapcreator._drawtask
## _asyncdrawrectrounded方法
**_asyncdrawrectrounded(Rect,Brush,Filled,StrokeWidth,CornersRadius)**

?> 说明：异步绘制带有圆角的矩形。返回应添加到绘图任务列表中的DrawTask。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 参数：CornersRadius，类型：int
>
> 返回值：b4a.example.bitmapcreator._drawtask
## _blendpixel方法
**_blendpixel(Source,SrcX,SrcY,TargetX,TargetY)**

?> 说明：将单个像素从Source复制到此BC。如果像素是非不透明的，那么它将与当前像素混合。
>
> 参数：Source，类型：b4a.example.bitmapcreator
>
> 参数：SrcX，类型：int
>
> 参数：SrcY，类型：int
>
> 参数：TargetX，类型：int
>
> 参数：TargetY，类型：int
>
> 返回值：String
## _blendpixel2方法
**_blendpixel2(SrcPM,TargetX,TargetY)**
>
> 参数：SrcPM，类型：b4a.example.bitmapcreator._premultipliedcolor
>
> 参数：TargetX，类型：int
>
> 参数：TargetY，类型：int
>
> 返回值：String
## _class_globals方法
**_class_globals()**
>
> 返回值：String
## _colortoargb方法
**_colortoargb(Clr,Result)**

?> 说明：将color int转换为ARGBColor对象。
>
> 参数：Clr，类型：int
>
> 参数：Result，类型：b4a.example.bitmapcreator._argbcolor
>
> 返回值：b4a.example.bitmapcreator._argbcolor
## _copypixel方法
**_copypixel(Source,SrcX,SrcY,TargetX,TargetY)**

?> 说明：将单个像素从Source复制到此BC。
>
> 参数：Source，类型：b4a.example.bitmapcreator
>
> 参数：SrcX，类型：int
>
> 参数：SrcY，类型：int
>
> 参数：TargetX，类型：int
>
> 参数：TargetY，类型：int
>
> 返回值：String
## _copypixelignoresemitransparent方法
**_copypixelignoresemitransparent(Source,SrcX,SrcY,TargetX,TargetY,SkipBlending)**
>
> 参数：Source，类型：b4a.example.bitmapcreator
>
> 参数：SrcX，类型：int
>
> 参数：SrcY，类型：int
>
> 参数：TargetX，类型：int
>
> 参数：TargetY，类型：int
>
> 参数：SkipBlending，类型：boolean
>
> 返回值：String
## _copypixelsfrombitmap方法
**_copypixelsfrombitmap(SourceBitmap)**

?> 说明：从SourceBitmap中提取像素并进行复制。
>
> 参数：SourceBitmap，类型：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
>
> 返回值：String
## _createbrushfrombitmap方法
**_createbrushfrombitmap(Bmp)**

?> 说明：从给定位图创建BCBrush。您可以重复使用笔刷。
>
> 参数：Bmp，类型：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
>
> 返回值：b4a.example.bcpath._bcbrush
## _createbrushfrombitmapcreator方法
**_createbrushfrombitmapcreator(BC)**

?> 说明：从给定的BitmapCreator创建BCBrush。您可以重复使用笔刷。
>
> 参数：BC，类型：b4a.example.bitmapcreator
>
> 返回值：b4a.example.bcpath._bcbrush
## _createbrushfromcolor方法
**_createbrushfromcolor(Color)**

?> 说明：根据给定的颜色创建BCBrush。您可以重复使用笔刷。
>
> 参数：Color，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _createdrawtask方法
**_createdrawtask(Source,SrcRect,TargetX,TargetY,SkipBlending)**

?> 说明：创建DrawTask对象。
>
> 参数：Source，类型：Object
>
> 参数：SrcRect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：TargetX，类型：int
>
> 参数：TargetY，类型：int
>
> 参数：SkipBlending，类型：boolean
>
> 返回值：b4a.example.bitmapcreator._drawtask
## _drawarc方法
**_drawarc(X,Y,Radius,Color,Filled,StrokeWidth,StartingAngle,SweepAngle)**

?> 说明：绘制圆弧并返回创建的笔刷。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 参数：Radius，类型：float
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 参数：StartingAngle，类型：float
>
> 参数：SweepAngle，类型：float
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawarc2方法
**_drawarc2(X,Y,Radius,Brush,Filled,StrokeWidth,StartingAngle,SweepAngle)**

?> 说明：类似于DrawArc。应为BCBrush，而不是颜色值。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 参数：Radius，类型：float
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 参数：StartingAngle，类型：float
>
> 参数：SweepAngle，类型：float
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawbitmap方法
**_drawbitmap(Bmp,TargetRect1,SkipBlending)**

?> 说明：在缓冲区中绘制位图。
>
> 参数：Bmp，类型：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
>
> 参数：TargetRect1，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：SkipBlending，类型：boolean
>
> 返回值：String
## _drawbitmapcreator方法
**_drawbitmapcreator(Source,SrcRect,TargetX,TargetY,SkipBlending)**

?> 说明：将存储在源BitmapCreator中的图像绘制到此BitmapCreator。
>
> 参数：Source，类型：b4a.example.bitmapcreator
>
> 参数：SrcRect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：TargetX，类型：int
>
> 参数：TargetY，类型：int
>
> 参数：SkipBlending，类型：boolean
>
> 返回值：String
## _drawbitmapcreatorsasync方法
**_drawbitmapcreatorsasync(Target,EventName,DrawTasks)**

?> 说明：异步绘制所有绘制任务。请注意，在引发BitmapReady事件之前，不应绘制其他图形。
```vbnet
bc1.DrawBitmapCreatorsAsync(Me, "BC", Tasks)
Wait For BC_BitmapReady (bmp As B4XBitmap)

```

>
> 参数：Target，类型：Object
>
> 参数：EventName，类型：String
>
> 参数：DrawTasks，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：String
## _drawbitmapcreatortransformed方法
**_drawbitmapcreatortransformed(Task)**

?> 说明：绘制缩放和/或旋转的BitmapCreator。
>
> 参数：Task，类型：b4a.example.bitmapcreator._drawtask
>
> 返回值：String
## _drawcircle方法
**_drawcircle(X,Y,Radius,Color,Filled,StrokeWidth)**

?> 说明：画一个圆。返回颜色笔刷。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 参数：Radius，类型：float
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawcircle2方法
**_drawcircle2(X,Y,Radius,Brush,Filled,StrokeWidth)**

?> 说明：画一个圆。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 参数：Radius，类型：float
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawcompressedbitmap方法
**_drawcompressedbitmap(Source,SrcRect,TargetX,TargetY)**

?> 说明：绘制使用BitmapCreator.ExtractCompressBC创建的CompressedBC对象。
>
> 参数：Source，类型：b4a.example.bitmapcreator._compressedbc
>
> 参数：SrcRect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：TargetX，类型：int
>
> 参数：TargetY，类型：int
>
> 返回值：String
## _drawline方法
**_drawline(X0,Y0,X1,Y1,Color,StrokeWidth)**

?> 说明：画一条线。返回颜色笔刷。
>
> 参数：X0，类型：float
>
> 参数：Y0，类型：float
>
> 参数：X1，类型：float
>
> 参数：Y1，类型：float
>
> 参数：Color，类型：int
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawline2方法
**_drawline2(X0,Y0,X1,Y1,Brush,StrokeWidth)**

?> 说明：画一条线。
>
> 参数：X0，类型：float
>
> 参数：Y0，类型：float
>
> 参数：X1，类型：float
>
> 参数：Y1，类型：float
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawpath方法
**_drawpath(Path,Color,Filled,StrokeWidth)**

?> 说明：绘制BCPath。不要与B4XPath或Path混淆。
>
> 参数：Path，类型：b4a.example.bcpath
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawpath2方法
**_drawpath2(Path,Brush,Filled,StrokeWidth)**

?> 说明：绘制BCPath。不要与B4XPath或Path混淆。
>
> 参数：Path，类型：b4a.example.bcpath
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawrect方法
**_drawrect(Rect,Color,Filled,StrokeWidth)**

?> 说明：绘制一个矩形。返回颜色笔刷。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawrect2方法
**_drawrect2(Rect,Brush,Filled,StrokeWidth)**

?> 说明：绘制一个矩形。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawrectrounded方法
**_drawrectrounded(Rect,Color,Filled,StrokeWidth,CornersRadius)**

?> 说明：绘制带有圆角的矩形。返回颜色笔刷。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Color，类型：int
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 参数：CornersRadius，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawrectrounded2方法
**_drawrectrounded2(Rect,Brush,Filled,StrokeWidth,CornersRadius)**

?> 说明：绘制带有圆角的矩形。
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Brush，类型：b4a.example.bcpath._bcbrush
>
> 参数：Filled，类型：boolean
>
> 参数：StrokeWidth，类型：int
>
> 参数：CornersRadius，类型：int
>
> 返回值：b4a.example.bcpath._bcbrush
## _drawrotatedcbc方法
**_drawrotatedcbc(cbc,Degrees,Width,Height,AABuffer)**

?> 说明：使用抗锯齿进行旋转。
>
> 参数：cbc，类型：b4a.example.bitmapcreator._compressedbc
>
> 参数：Degrees，类型：float
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 参数：AABuffer，类型：b4a.example.bitmapcreator._internalantialiasingbuffer
>
> 返回值：String
## _extractcompressedbc方法
**_extractcompressedbc(Rect,Cache)**
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Cache，类型：b4a.example.bitmapcreator._internalcompressedbccache
>
> 返回值：b4a.example.bitmapcreator._compressedbc
## _fillgradient方法
**_fillgradient(GradColors,Rect,Orientation)**

?> 说明：用渐变填充矩形。跳过混合。
>
> 参数：GradColors，类型：int[]
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 参数：Orientation，类型：String
>
> 返回值：String
## _fillradialgradient方法
**_fillradialgradient(GradColors,Rect)**

?> 说明：使用径向渐变填充矩形。跳过混合。
>
> 参数：GradColors，类型：int[]
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 返回值：String
## _fillrect方法
**_fillrect(Color,Rect)**

?> 说明：已弃用：请改用DrawRect。
>
> 参数：Color，类型：int
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 返回值：String
## _flipcompressedbitmap方法
**_flipcompressedbitmap(Source,Horizontal,Vertical)**
>
> 参数：Source，类型：b4a.example.bitmapcreator._compressedbc
>
> 参数：Horizontal，类型：boolean
>
> 参数：Vertical，类型：boolean
>
> 返回值：b4a.example.bitmapcreator._compressedbc
## _getargb方法
**_getargb(x,y,Result)**

?> 说明：获取给定点的颜色作为ARGB颜色。
>
> 参数：x，类型：int
>
> 参数：y，类型：int
>
> 参数：Result，类型：b4a.example.bitmapcreator._argbcolor
>
> 返回值：b4a.example.bitmapcreator._argbcolor
## _getbitmap方法
**_getbitmap()**

?> 说明：将字节缓冲区转换为位图。
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## _getbuffer方法
**_getbuffer()**

?> 说明：获取内部缓冲区。
>
> 返回值：byte[]
## _getcolor方法
**_getcolor(x,y)**

?> 说明：获取给定点的颜色作为int值。
>
> 参数：x，类型：int
>
> 参数：y，类型：int
>
> 返回值：int
## _getpremultipliedcolor方法
**_getpremultipliedcolor(x,y,Result)**

?> 说明：获取给定点的颜色作为预乘颜色。此格式不需要转换。
>
> 参数：x，类型：int
>
> 参数：y，类型：int
>
> 参数：Result，类型：b4a.example.bitmapcreator._premultipliedcolor
>
> 返回值：b4a.example.bitmapcreator._premultipliedcolor
## _initialize方法
**_initialize(ba,Width,Height)**

?> 说明：初始化对象并设置位图尺寸。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Width，类型：int
>
> 参数：Height，类型：int
>
> 返回值：String
## _istransparent方法
**_istransparent(x,y)**

?> 说明：测试给定的点是否完全透明。
>
> 参数：x，类型：int
>
> 参数：y，类型：int
>
> 返回值：boolean
## _replacesemitransparentpixels方法
**_replacesemitransparentpixels(NewColor,Rect)**

?> 说明：用NewColor替换Rect中的所有半透明像素。
>
> 参数：NewColor，类型：int
>
> 参数：Rect，类型：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
>
> 返回值：String
## _setargb方法
**_setargb(x,y,ARGB)**

?> 说明：设置指定点的颜色。
>
> 参数：x，类型：int
>
> 参数：y，类型：int
>
> 参数：ARGB，类型：b4a.example.bitmapcreator._argbcolor
>
> 返回值：String
## _setbitmaptoimageview方法
**_setbitmaptoimageview(Bitmap,ImageView)**

?> 说明：类似于B4XView.SetBitmap。不同之处在于B4A中“重力”设置为FILL而不是CENTER。
>
> 参数：Bitmap，类型：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
>
> 参数：ImageView，类型：anywheresoftware.b4a.objects.B4XViewWrapper
>
> 返回值：String
## _setcolor方法
**_setcolor(x,y,Clr)**

?> 说明：设置给定像素的颜色。
>
> 参数：x，类型：int
>
> 参数：y，类型：int
>
> 参数：Clr，类型：int
>
> 返回值：String
## _sethsv方法
**_sethsv(x,y,alpha,h,s,v)**

?> 说明：设置指定点的颜色。
>
> 参数：x，类型：int
>
> 参数：y，类型：int
>
> 参数：alpha，类型：int
>
> 参数：h，类型：int
>
> 参数：s，类型：float
>
> 参数：v，类型：float
>
> 返回值：String
## _setpremultipliedcolor方法
**_setpremultipliedcolor(x,y,Premultiplied)**

?> 说明：设置指定点的颜色。
>
> 参数：x，类型：int
>
> 参数：y，类型：int
>
> 参数：Premultiplied，类型：b4a.example.bitmapcreator._premultipliedcolor
>
> 返回值：String
## _bitmap属性

?> 说明：将字节缓冲区转换为位图。
>
> 返回值：anywheresoftware.b4a.objects.B4XViewWrapper.B4XBitmapWrapper
## _buffer属性

?> 说明：获取内部缓冲区。
>
> 返回值：byte[]
## _mwidth字段
>
> 返回值：int
## _mheight字段
>
> 返回值：int
## _targetrect字段
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
## _same_color_length_for_cache字段
>
> 返回值：int
## _max_same_color_size字段
>
> 返回值：int
## _alphathresholdforcbcextraction字段
>
> 返回值：int

# InternalBCPathColumnData
完整类名：b4a.example.bcpath._internalbcpathcolumndata
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## MinY字段
>
> 返回值：float
## MaxY字段
>
> 返回值：float
## StartPoint字段
>
> 返回值：float
## EndPoint字段
>
> 返回值：float
## SignY字段
>
> 返回值：float
## LastY字段
>
> 返回值：float

# InternalBCPathPointData
完整类名：b4a.example.bcpath._internalbcpathpointdata
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## X字段
>
> 返回值：float
## Y字段
>
> 返回值：float
## ColumnData字段
>
> 返回值：b4a.example.bcpath._internalbcpathcolumndata

# BCBrush
完整类名：b4a.example.bcpath._bcbrush
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Source字段
>
> 返回值：b4a.example.bitmapcreator
## SrcOffsetX字段
>
> 返回值：int
## SrcOffsetY字段
>
> 返回值：int
## IsColorSource字段
>
> 返回值：boolean
## BlendAll字段
>
> 返回值：boolean
## BlendBorders字段
>
> 返回值：boolean
## ColorPM字段
>
> 返回值：b4a.example.bitmapcreator._premultipliedcolor

# InternalCanvasDrawTask
完整类名：b4a.example.bcpath._internalcanvasdrawtask
> 所有者：process

> 依赖：javaobject | xui
## Initialize方法
**Initialize()**

?> 说明：将字段初始化为其默认值。
>
> 返回值：void
## IsInitialized字段

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## Brush字段
>
> 返回值：b4a.example.bcpath._bcbrush
## Code字段
>
> 返回值：int
## Values字段
>
> 返回值：float[]
## Filled字段
>
> 返回值：boolean

# BCPath
完整类名：b4a.example.bcpath
> 所有者：process

> 依赖：javaobject | xui
## IsInitialized方法
**IsInitialized()**

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## _class_globals方法
**_class_globals()**
>
> 返回值：String
## _clone方法
**_clone()**

?> 说明：创建路径的副本。这是由BitmapCreator.AsyncDrawPath使用的。
>
> 返回值：b4a.example.bcpath
## _findboundingrect方法
**_findboundingrect()**

?> 说明：返回路径边界矩形。
>
> 返回值：anywheresoftware.b4a.objects.B4XCanvas.B4XRect
## _initialize方法
**_initialize(ba,X,Y)**

?> 说明：初始化路径并设置第一个点。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 返回值：b4a.example.bcpath
## _invalidate方法
**_invalidate()**

?> 说明：如果直接修改了“点”列表，则调用Invalidate。
>
> 返回值：String
## _lineto方法
**_lineto(X,Y)**

?> 说明：在给定点上添加一条线。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 返回值：b4a.example.bcpath
## _prepareforfilling方法
**_prepareforfilling()**

?> 说明：内部接头。
>
> 返回值：String
## _removelastpoint方法
**_removelastpoint()**

?> 说明：删除最后一个点。
>
> 返回值：String
## _reset方法
**_reset(X,Y)**

?> 说明：重置路径。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 返回值：b4a.example.bcpath
## _points字段
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## _internalcounterclockwise字段
>
> 返回值：boolean
## _drawconnectionsegments字段
>
> 返回值：boolean

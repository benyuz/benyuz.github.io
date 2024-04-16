# rLiquidCrystal

版本:1
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rLiquidCrystal)

# LiquidCrystal
完整类名：B4R::B4RLiquidCrystal
## Initialize方法
**Initialize(RS,RW,Enable,DataPins)**

?> 说明：初始化对象。请注意，您还应该调用Begin。
```vbnet

lcd.Initialize(8, 255, 9, Array As Byte(4, 5, 6, 7))
```

>
> 参数：RS，类型：Byte
>
> 参数：RW，类型：Byte
>
> 参数：Enable，类型：Byte
>
> 参数：DataPins，类型：Byte[]
>
> 返回值：B4R::void
## Begin方法
**Begin(NumberOfColumns,NumberOfRows)**

?> 说明：设置列数和行数。
>
> 参数：NumberOfColumns，类型：Byte
>
> 参数：NumberOfRows，类型：Byte
>
> 返回值：B4R::void
## Write方法
**Write(Message)**

?> 说明：写入消息。消息可以是字符串、数字或字节数组。
>
> 参数：Message，类型：B4R::Object*
>
> 返回值：B4R::void
## SetCursor方法
**SetCursor(Column,Row)**

?> 说明：设置光标位置。
>
> 参数：Column，类型：Byte
>
> 参数：Row，类型：Byte
>
> 返回值：B4R::void
## Clear方法
**Clear()**

?> 说明：清除屏幕并将光标设置为（0,0）。
>
> 返回值：B4R::void
## Blink属性

?> 说明：设置光标是否应闪烁。
>
> 参数：b，类型：bool
>
> 返回值：
## CursorOn属性

?> 说明：设置光标状态。
>
> 参数：b，类型：bool
>
> 返回值：
## DisplayOn属性

?> 说明：设置显示状态。
>
> 参数：b，类型：bool
>
> 返回值：

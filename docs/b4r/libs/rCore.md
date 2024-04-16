# rCore

版本:3.9
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rCore)

# Timer
完整类名：B4R::Timer
> 事件：
>
> Tick
## Initialize方法
**Initialize(TickSub,Interval)**

?> 说明：初始化计时器。请注意，必须将“启用”设置为True，计时器才能开始运行。
>
> 参数：TickSub，类型：SubVoidVoid
>
> 参数：Interval，类型：ULong
>
> 返回值：B4R::void
## Enabled属性

?> 说明：启用或禁用计时器。
>
> 参数：e，类型：bool
>
> 返回值：bool
## Interval字段

?> 说明：获取或设置计时器间隔，以毫秒为单位。
>
> 返回值：ULong

# Bit
完整类名：B4R::BitClass
## BitClass_And方法
**BitClass_And(X,Y)**

?> 说明：返回这两个值的按位“与”。
>
> 参数：X，类型：UInt
>
> 参数：Y，类型：UInt
>
> 返回值：UInt
## BitClass_Or方法
**BitClass_Or(X,Y)**

?> 说明：返回这两个值的按位“或”。
>
> 参数：X，类型：UInt
>
> 参数：Y，类型：UInt
>
> 返回值：UInt
## BitClass_Xor方法
**BitClass_Xor(X,Y)**

?> 说明：返回两个值的逐位异或。
>
> 参数：X，类型：UInt
>
> 参数：Y，类型：UInt
>
> 返回值：UInt
## BitClass_Not方法
**BitClass_Not(N)**

?> 说明：返回给定值的按位补码。
>
> 参数：N，类型：UInt
>
> 返回值：UInt
## BitClass_ShiftLeft方法
**BitClass_ShiftLeft(N,Shift)**

?> 说明：向左移动N。
>
> 参数：N，类型：UInt
>
> 参数：Shift，类型：Byte
>
> 返回值：UInt
## BitClass_ShiftRight方法
**BitClass_ShiftRight(N,Shift)**

?> 说明：向右移动N。
>
> 参数：N，类型：UInt
>
> 参数：Shift，类型：Byte
>
> 返回值：UInt
## ToBinaryString方法
**ToBinaryString(N)**

?> 说明：返回以2为底的N的字符串表示形式。
>
> 参数：N，类型：UInt
>
> 返回值：B4R::B4RString*
## BitClass_ParseInt方法
**BitClass_ParseInt(Value,Radix)**

?> 说明：使用指定的基数将值解析为整数。如果无法分析值，则返回0。
>
> 参数：Value，类型：B4R::B4RString*
>
> 参数：Radix，类型：Byte
>
> 返回值：Int
## BitClass_LowByte方法
**BitClass_LowByte(N)**

?> 说明：返回给定数字的低字节值。
>
> 参数：N，类型：UInt
>
> 返回值：Byte
## BitClass_HighByte方法
**BitClass_HighByte(N)**

?> 说明：返回给定数字的高位字节值。
>
> 参数：N，类型：UInt
>
> 返回值：Byte
## BitClass_Set方法
**BitClass_Set(B,Bit)**

?> 说明：返回基于给定数字的字节，并设置指定的位。
```vbnet

Dim b As Byte = 0
b = Bit.Set(b, 0)
Log(b) '1
```

>
> 参数：B，类型：Byte
>
> 参数：Bit，类型：Byte
>
> 返回值：Byte
## BitClass_Clear方法
**BitClass_Clear(B,Bit)**

?> 说明：返回基于给定数字的字节，并清除指定的位。
>
> 参数：B，类型：Byte
>
> 参数：Bit，类型：Byte
>
> 返回值：Byte
## BitClass_Get方法
**BitClass_Get(B,Bit)**

?> 说明：返回给定数字中指定位的值。
>
> 参数：B，类型：Byte
>
> 参数：Bit，类型：Byte
>
> 返回值：Byte

# 
完整类名：B4R::Common
## Log方法
**Log(OneOrMoreMessages)**

?> 说明：记录一条或多条消息。
```vbnet

Log("x = ", x)
```

>
> 参数：OneOrMoreMessages，类型：B4R::Object*
>
> 返回值：B4R::void
## AvailableRAM方法
**AvailableRAM()**

?> 说明：返回可用内存。
>
> 返回值：ULong
## StackBufferUsage方法
**StackBufferUsage()**

?> 说明：返回堆栈内存缓冲区的使用情况（使用#StackMemoryBuffer属性设置）。
>
> 返回值：UInt
## Common_Sub方法
**Common_Sub()**

?> 说明：声明具有参数和返回类型的子。
```vbnet

Sub MySub (FirstName As String, LastName As String, Age As Int, OtherValues() As Double) As Boolean
...
End Sub
```

>
> 返回值：B4R::void
## Array方法
**Array()**

?> 说明：创建指定类型的一维数组，如果未指定类型，则创建对象。
```vbnet

Dim Days() As String = Array As String("Sunday", "Monday", ...)
```

>
> 返回值：B4R::void
## If方法
**If()**

?> 说明：单线：
>
> 返回值：B4R::void
## Dim方法
**Dim()**

?> 说明：声明一个变量。
```vbnet
Dim a = 1, b = 2, c = 3 As Int
```

>
> 返回值：B4R::void
## While方法
**While()**

?> 说明：条件为true时循环。
>
> 返回值：B4R::void
## Until方法
**Until()**

?> 说明：循环直到条件为true。
>
> 返回值：B4R::void
## For方法
**For()**

?> 说明：语法：
```vbnet

For i = 1 To 10
Log(i) 'Will print 1 to 10 (inclusive).
Next
For Each n As Int In Numbers 'an array
Sum = Sum + n
Next

```

>
> 返回值：B4R::void
## Type方法
**Type()**

?> 说明：声明一个结构。
```vbnet

Type MyType (Name As String, Value As Int)
Dim a, b As MyType
a.Value = 123
```

>
> 返回值：B4R::void
## Exit方法
**Exit()**

?> 说明：退出最内部的循环。
>
> 返回值：B4R::void
## Continue方法
**Continue()**

?> 说明：停止执行当前迭代并继续执行下一个迭代。
>
> 返回值：B4R::void
## Return方法
**Return()**

?> 说明：从当前子中返回，并可选择返回给定值。
>
> 返回值：B4R::void
## Select方法
**Select()**

?> 说明：将单个值与多个值进行比较。
```vbnet

Dim value As Int = 7
Select value
	Case 1
		Log("One")
	Case 2, 4, 6, 8
		Log("Even")
	Case 3, 5, 7, 9
		Log("Odd larger than one")
	Case Else
		Log("Larger than 9")
End Select
```

>
> 返回值：B4R::void
## IIf方法
**IIf(Condition,TrueValue,FalseValue)**

?> 说明：Inline If-如果Condition为True则返回TrueValue，否则返回False。仅计算相关表达式。
```vbnet
Dim x As Int = IIf(y > 10, 17, 7).As(Int)
```

>
> 参数：Condition，类型：B4R::boolean
>
> 参数：TrueValue，类型：B4R::Object
>
> 参数：FalseValue，类型：B4R::Object
>
> 返回值：B4R::Object
## SizeOf方法
**SizeOf(Object)**

?> 说明：返回给定对象的大小（字节数）。在编译过程中，对象类型必须是已知的。
>
> 参数：Object，类型：B4R::Object*
>
> 返回值：UInt
## Common_Delay方法
**Common_Delay(DelayMs)**

?> 说明：暂停执行指定的延迟（以毫秒为单位）。
>
> 参数：DelayMs，类型：ULong
>
> 返回值：B4R::void
## Common_DelayMicroseconds方法
**Common_DelayMicroseconds(Delay)**

?> 说明：暂停执行指定的延迟（以微秒为单位）。
>
> 参数：Delay，类型：UInt
>
> 返回值：B4R::void
## Common_Not方法
**Common_Not(Value)**

?> 说明：反转给定布尔值的值。
>
> 参数：Value，类型：Bool
>
> 返回值：bool
## CallSubPlus方法
**CallSubPlus(SubName,DelayMs,Tag)**

?> 说明：在指定时间过后运行给定的子。请注意，此调用不会阻塞线程。
```vbnet

CallSubPlus("DoSomething", 1000, 5)
'...

Sub DoSomething(Tag as Byte)

End Sub
```

>
> 参数：SubName，类型：SubVoidByte
>
> 参数：DelayMs，类型：ULong
>
> 参数：Tag，类型：Byte
>
> 返回值：B4R::void
## Common_RunNative方法
**Common_RunNative(Method,Arg)**

?> 说明：运行内联C函数。
```vbnet

RunNative("testc", Null)

#If C
void testc(B4R::Object* o) {
	Serial.println(b4r_main::_i); //print a global variable named i
}
#End If
```

>
> 参数：Method，类型：FunctionObjectObject
>
> 参数：Arg，类型：B4R::Object*
>
> 返回值：B4R::Object*
## AddLooper方法
**AddLooper(SubName)**

?> 说明：添加一个活套子。活套类似于具有尽可能低的间隔的计时器。
```vbnet

AddLooper("Looper1")
'...
Sub Looper1

End Sub
```

>
> 参数：SubName，类型：SubVoidVoid
>
> 返回值：B4R::void
## Sender方法
**Sender()**

?> 说明：返回引发事件的对象（如果已设置）。
>
> 返回值：B4R::Object*
## NumberFormat方法
**NumberFormat(Number,MinimumIntegers,MaximumFractions)**

?> 说明：将数字转换为具有指定的最小整数数和最大分数数的字符串。
>
> 参数：Number，类型：Double
>
> 参数：MinimumIntegers，类型：Byte
>
> 参数：MaximumFractions，类型：Byte
>
> 返回值：B4R::B4RString*
## Common_RndSeed方法
**Common_RndSeed(Seed)**

?> 说明：设置该随机种子值。
```vbnet

dim p as Pin
p.Initialize(0, p.MODE_INPUT)
RndSeed(p.AnalogRead)
```

>
> 参数：Seed，类型：ULong
>
> 返回值：B4R::void
## Common_Rnd方法
**Common_Rnd(Mininum,Maximum)**

?> 说明：返回一个介于最小值（包括最小值）和最大值（不包括最大值）之间的随机数。
>
> 参数：Mininum，类型：Long
>
> 参数：Maximum，类型：Long
>
> 返回值：Long
## Common_Millis方法
**Common_Millis()**

?> 说明：返回自上次重新启动以来的毫秒数。
>
> 返回值：ULong
## Common_Micros方法
**Common_Micros()**

?> 说明：返回自上次重新启动以来的微秒数。
>
> 返回值：ULong
## Common_Abs方法
**Common_Abs(Number)**

?> 说明：返回绝对值。
>
> 参数：Number，类型：Double
>
> 返回值：Double
## Common_Max方法
**Common_Max(Number1,Number2)**

?> 说明：返回两个数字之间较大的数字。
>
> 参数：Number1，类型：Double
>
> 参数：Number2，类型：Double
>
> 返回值：Double
## Common_Min方法
**Common_Min(Number1,Number2)**

?> 说明：返回两个数字之间的较小数字。
>
> 参数：Number1，类型：Double
>
> 参数：Number2，类型：Double
>
> 返回值：Double
## Common_Sin方法
**Common_Sin(Radians)**

?> 说明：计算三角正弦函数。以弧度为单位测量的角度。
>
> 参数：Radians，类型：Double
>
> 返回值：Double
## Common_SinD方法
**Common_SinD(Degrees)**

?> 说明：计算三角正弦函数。以度为单位测量的角度。
>
> 参数：Degrees，类型：Double
>
> 返回值：Double
## Common_Cos方法
**Common_Cos(Radians)**

?> 说明：计算三角余弦函数。以弧度为单位测量的角度。
>
> 参数：Radians，类型：Double
>
> 返回值：Double
## Common_CosD方法
**Common_CosD(Degrees)**

?> 说明：计算三角余弦函数。以度为单位测量的角度。
>
> 参数：Degrees，类型：Double
>
> 返回值：Double
## Common_Tan方法
**Common_Tan(Radians)**

?> 说明：计算三角正切函数。以弧度为单位测量的角度。
>
> 参数：Radians，类型：Double
>
> 返回值：Double
## Common_TanD方法
**Common_TanD(Degrees)**

?> 说明：计算三角正切函数。以度为单位测量的角度。
>
> 参数：Degrees，类型：Double
>
> 返回值：Double
## Common_Power方法
**Common_Power(Base,Exponent)**

?> 说明：返回提升到Exponent幂的基数。
>
> 参数：Base，类型：Double
>
> 参数：Exponent，类型：Double
>
> 返回值：Double
## Common_Sqrt方法
**Common_Sqrt(Value)**

?> 说明：返回正平方根。
>
> 参数：Value，类型：Double
>
> 返回值：Double
## Common_ASin方法
**Common_ASin(Value)**

?> 说明：返回以弧度测量的角度。
>
> 参数：Value，类型：Double
>
> 返回值：Double
## Common_ASinD方法
**Common_ASinD(Value)**

?> 说明：返回以度为单位测量的角度。
>
> 参数：Value，类型：Double
>
> 返回值：Double
## Common_ACos方法
**Common_ACos(Value)**

?> 说明：返回以弧度测量的角度。
>
> 参数：Value，类型：Double
>
> 返回值：Double
## Common_ACosD方法
**Common_ACosD(Value)**

?> 说明：返回以度为单位测量的角度。
>
> 参数：Value，类型：Double
>
> 返回值：Double
## Common_ATan方法
**Common_ATan(Value)**

?> 说明：返回以弧度测量的角度。
>
> 参数：Value，类型：Double
>
> 返回值：Double
## Common_ATanD方法
**Common_ATanD(Value)**

?> 说明：返回以度为单位测量的角度。
>
> 参数：Value，类型：Double
>
> 返回值：Double
## Common_ATan2方法
**Common_ATan2(Y,X)**

?> 说明：返回以弧度测量的角度。
>
> 参数：Y，类型：Double
>
> 参数：X，类型：Double
>
> 返回值：Double
## Common_ATan2D方法
**Common_ATan2D(Y,X)**

?> 说明：返回以度为单位测量的角度。
>
> 参数：Y，类型：Double
>
> 参数：X，类型：Double
>
> 返回值：Double
## Common_Logarithm方法
**Common_Logarithm(Number,Base)**
>
> 参数：Number，类型：Double
>
> 参数：Base，类型：Double
>
> 返回值：Double
## Common_Round方法
**Common_Round(Number)**

?> 说明：返回最接近给定数字的整数。
>
> 参数：Number，类型：Double
>
> 返回值：Long
## Common_Ceil方法
**Common_Ceil(Number)**

?> 说明：返回大于或等于指定数字且等于整数的最小双精度。
>
> 参数：Number，类型：Double
>
> 返回值：Double
## Common_Floor方法
**Common_Floor(Number)**

?> 说明：返回小于或等于指定数字且等于整数的最大双精度。
>
> 参数：Number，类型：Double
>
> 返回值：Double
## IsNumber方法
**IsNumber(Text)**

?> 说明：测试给定字符串是否可以安全地解析为数字。
>
> 参数：Text，类型：B4R::B4RString*
>
> 返回值：bool
## Constrain方法
**Constrain(Value,MinValue,MaxValue)**

?> 说明：等效于最小值（MaxValue，Max（Value，MinValue））
>
> 参数：Value，类型：Double
>
> 参数：MinValue，类型：Double
>
> 参数：MaxValue，类型：Double
>
> 返回值：Double
## Common_Asc方法
**Common_Asc(Character)**

?> 说明：返回字符串中第一个字符的字节（ASCII）值。
>
> 参数：Character，类型：B4R::B4RString*
>
> 返回值：Byte
## Common_MapRange方法
**Common_MapRange(Value,FromLow,FromHigh,ToLow,ToHigh)**

?> 说明：将值从“from”范围映射到“to”范围。
```vbnet

Dim v as int = MapRange(p.AnalogRead, 0, 1023, 0, 255)
```

>
> 参数：Value，类型：Long
>
> 参数：FromLow，类型：Long
>
> 参数：FromHigh，类型：Long
>
> 参数：ToLow，类型：Long
>
> 参数：ToHigh，类型：Long
>
> 返回值：Long
## JoinStrings方法
**JoinStrings(Strings)**

?> 说明：将字符串连接为单个字符串。
```vbnet

Dim s As String  = JoinStrings(Array As String("Pi = ", cPI))
```

>
> 参数：Strings，类型：String[]
>
> 返回值：B4R::B4RString*
## JoinBytes方法
**JoinBytes(ArraysOfObjects)**

?> 说明：将字节数组连接到单个数组。
```vbnet

Dim b() as byte = JoinBytes(Array("abc".GetBytes, Array as Byte(13, 10)))
```

>
> 参数：ArraysOfObjects，类型：Object[]
>
> 返回值：Byte[]
## Bit字段

?> 说明：比特相关方法。
>
> 返回值：B4R::BitClass*
## Common_True字段
>
> 返回值：bool
## Common_False字段
>
> 返回值：bool
## Common_Null字段
>
> 返回值：B4R::Object*
## Common_CRLF字段

?> 说明：换行符。Chr（13）和Chr（10）的值。请注意，在其他B4X产品中，该值为Chr（10）。
>
> 返回值：B4R::StringLiteral
## Common_TAB字段

?> 说明：制表符。
>
> 返回值：B4R::StringLiteral
## Common_QUOTE字段

?> 说明：引号字符。
>
> 返回值：B4R::StringLiteral
## Common_cPI字段

?> 说明：PI常数。
>
> 返回值：Double
## Common_cE字段

?> 说明：e（自然对数底）常数。
>
> 返回值：Double

# 
完整类名：B4R::B4RString
## GetBytes方法
**GetBytes()**

?> 说明：以字节数组的形式返回字符串内容。
>
> 返回值：Byte[]
## Length属性

?> 说明：返回字符串长度。
>
> 返回值：Int

# Pin
完整类名：B4R::Pin
> 事件：
>
> StateChanged (State As Boolean)
## Initialize方法
**Initialize(Pin,Mode)**

?> 说明：初始化引脚并设置模式。
>
> 参数：Pin，类型：Byte
>
> 参数：Mode，类型：Byte
>
> 返回值：B4R::void
## AddListener方法
**AddListener(StateChangedSub)**

?> 说明：添加侦听器。当引脚的状态发生变化时，将引发StateChanged事件。
>
> 参数：StateChangedSub，类型：SubVoidBool
>
> 返回值：B4R::void
## DigitalRead方法
**DigitalRead()**

?> 说明：读取引脚值并返回true或false。
>
> 返回值：bool
## AnalogRead方法
**AnalogRead()**

?> 说明：读取引脚值并返回0到1023之间的值。
>
> 返回值：UInt
## DigitalWrite方法
**DigitalWrite(Value)**

?> 说明：写入给定的值。
>
> 参数：Value，类型：bool
>
> 返回值：B4R::void
## AnalogWrite方法
**AnalogWrite(Value)**

?> 说明：写入给定的模拟值。值应介于0到255之间。
>
> 参数：Value，类型：UInt
>
> 返回值：B4R::void
## Mode属性

?> 说明：设置接点的模式（mode常量之一）。
>
> 参数：Mode，类型：Byte
>
> 返回值：
## PinNumber字段

?> 说明：返回引脚的编号。
>
> 返回值：Byte
## Pin_MODE_INPUT字段

?> 说明：输入模式。
>
> 返回值：Byte
## Pin_MODE_OUTPUT字段

?> 说明：输出模式。
>
> 返回值：Byte
## Pin_MODE_INPUT_PULLUP字段

?> 说明：具有内部上拉电阻器的输入模式。
>
> 返回值：Byte
## Pin_A0字段
>
> 返回值：Byte
## Pin_A1字段
>
> 返回值：Byte
## Pin_A2字段
>
> 返回值：Byte
## Pin_A3字段
>
> 返回值：Byte
## Pin_A4字段
>
> 返回值：Byte
## Pin_A5字段
>
> 返回值：Byte
## Pin_A6字段
>
> 返回值：Byte
## Pin_A7字段
>
> 返回值：Byte

# Stream
完整类名：B4R::B4RStream
## Flush方法
**Flush()**

?> 说明：冲洗溪流。
>
> 返回值：B4R::void
## WriteBytes方法
**WriteBytes(Buffer,StartOffset,Length)**

?> 说明：将数据写入流。返回写入的字节数。
>
> 参数：Buffer，类型：Byte[]
>
> 参数：StartOffset，类型：UInt
>
> 参数：Length，类型：UInt
>
> 返回值：UInt
## BytesAvailable方法
**BytesAvailable()**

?> 说明：返回可供读取的字节数。
>
> 返回值：Int
## ReadBytes方法
**ReadBytes(Buffer,StartOffset,Length)**

?> 说明：从流中读取数据并将其存储在缓冲区中。
>
> 参数：Buffer，类型：Byte[]
>
> 参数：StartOffset，类型：UInt
>
> 参数：Length，类型：UInt
>
> 返回值：UInt

# Serial
完整类名：B4R::Serial
## Initialize方法
**Initialize(BaudRate)**

?> 说明：初始化串行对象并设置波特率。使用默认的8N1配置。
>
> 参数：BaudRate，类型：ULong
>
> 返回值：B4R::void
## Close方法
**Close()**

?> 说明：关闭串行端口。
>
> 返回值：B4R::void
## Stream属性

?> 说明：返回内部流。这可以与AsyncStreams一起用于从串行中读取或写入。
>
> 返回值：B4R::B4RStream*

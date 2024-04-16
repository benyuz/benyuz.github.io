# rServo

版本:0.9
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=rServo)

# Servo
完整类名：B4R::B4RServo
## Attach方法
**Attach(Pin)**

?> 说明：将伺服连接到指定的引脚。
>
> 参数：Pin，类型：Int
>
> 返回值：Byte
## Attach2方法
**Attach2(Pin,MinValue,MaxValue)**

?> 说明：将伺服连接到指定的引脚。
>
> 参数：Pin，类型：Int
>
> 参数：MinValue，类型：Int
>
> 参数：MaxValue，类型：Int
>
> 返回值：Byte
## Detach方法
**Detach()**

?> 说明：拆下销。
>
> 返回值：B4R::void
## Write方法
**Write(Value)**

?> 说明：如果该值小于200，则将其视为角度。
>
> 参数：Value，类型：Int
>
> 返回值：B4R::void
## WriteMicroseconds方法
**WriteMicroseconds(Value)**

?> 说明：以微秒为单位写入脉冲宽度。
>
> 参数：Value，类型：Int
>
> 返回值：B4R::void
## Read方法
**Read()**

?> 说明：以0到180度之间的角度返回当前脉冲宽度。
>
> 返回值：Int
## ReadMicroseconds方法
**ReadMicroseconds()**

?> 说明：以微秒为单位返回当前脉冲宽度。
>
> 返回值：Int
## Attached属性

?> 说明：如果连接了伺服，则返回true。
>
> 返回值：bool

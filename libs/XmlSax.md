# XmlSax

版本:1.11
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=XmlSax)

# SaxParser
完整类名：anywheresoftware.b4a.objects.SaxParser
> 所有者：process

?> 说明：一种解析器，按顺序读取流，并在每个元素的开头和结尾引发事件。
> 事件：
>
> StartElement (Uri As String, Name As String, Attributes As Attributes)
>
> EndElement (Uri As String, Name As String, Text As StringBuilder)
## Initialize方法
**Initialize(ba)**

?> 说明：初始化对象。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 返回值：void
## Parse2方法
**Parse2(TextReader,EventName)**

?> 说明：分析给定的TextReader。
>
> 参数：TextReader，类型：java.io.Reader
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Parse方法
**Parse(InputStream,EventName)**

?> 说明：分析给定的InputStream。
>
> 参数：InputStream，类型：java.io.InputStream
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## Parents字段

?> 说明：包含父元素名称的列表。
>
> 返回值：anywheresoftware.b4a.objects.collections.List

# Attributes
完整类名：anywheresoftware.b4a.objects.SaxParser.AttributesWrapper
> 所有者：process

> 包装器：org.xml.sax.Attributes

?> 说明：此对象是在StartElement事件中传递的。
## GetValue2方法
**GetValue2(Uri,Name)**

?> 说明：返回具有以下Uri和名称的属性的值。
>
> 参数：Uri，类型：java.lang.String
>
> 参数：Name，类型：java.lang.String
>
> 返回值：java.lang.String
## GetValue方法
**GetValue(Index)**

?> 说明：返回指定索引处的属性值。
>
> 参数：Index，类型：int
>
> 返回值：java.lang.String
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## GetName方法
**GetName(Index)**

?> 说明：返回指定索引处的属性的名称。
>
> 参数：Index，类型：int
>
> 返回值：java.lang.String
## Size属性

?> 说明：返回此元素中的属性数。
>
> 返回值：int

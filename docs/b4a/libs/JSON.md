# JSON

版本:1.21
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=JSON)

# JSONParser
完整类名：anywheresoftware.b4a.objects.collections.JSONParser
> 所有者：process

> 包装器：org.json.JSONTokener

?> 说明：解析JSON格式的字符串：JSON的描述。
```vbnet

Dim JSON As JSONParser
Dim Map1 As Map
JSON.Initialize(File.ReadString(File.DirAssets, "example.json")) 'Read the text from a file.
Map1 = JSON.NextObject
```

## NextArray方法
**NextArray()**

?> 说明：分析文本，假设顶级值是一个数组。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## NextValue方法
**NextValue()**

?> 说明：分析文本，假设顶级值是一个简单值。
>
> 返回值：java.lang.Object
## NextObject方法
**NextObject()**

?> 说明：分析文本，假设顶级值是一个对象。
>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Text)**

?> 说明：初始化对象并设置将要分析的文本。
>
> 参数：Text，类型：java.lang.String
>
> 返回值：void

# JSONGenerator
完整类名：anywheresoftware.b4a.objects.collections.JSONParser.JSONGenerator
> 所有者：process

?> 说明：此对象生成JSON字符串。
## ToPrettyString方法
**ToPrettyString(Indent)**

?> 说明：从初始化的对象创建一个JSON字符串。
>
> 参数：Indent，类型：int
>
> 返回值：java.lang.String
## Initialize2方法
**Initialize2(List)**

?> 说明：使用给定的列表初始化对象。
>
> 参数：List，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## ToString方法
**ToString()**

?> 说明：从初始化的对象创建一个JSON字符串。
>
> 返回值：java.lang.String
## Initialize方法
**Initialize(Map)**

?> 说明：使用给定的Map初始化对象。
>
> 参数：Map，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：void

# JSON
完整类名：anywheresoftware.b4a.objects.collections.JSONParser.JSONConverter
> 所有者：process

> 包装器：java.lang.Object

?> 说明：使用As方法将字符串转换为对象，反之亦然。
```vbnet

Dim m As Map = CreateMap("Key1": "Value1")
Dim s As String = m.As(JSON).ToString
```

## ToCompactString方法
**ToCompactString()**

?> 说明：将Map或List转换为不带空格的JSON字符串。与JsonGenerator.ToString相同。
>
> 返回值：java.lang.String
## ToMap方法
**ToMap()**

?> 说明：将字符串转换为Map。
>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## ToString方法
**ToString()**

?> 说明：将Map或List转换为JSON字符串。与JsonGenerator.ToPrettyString（4）相同。
>
> 返回值：java.lang.String
## ToList方法
**ToList()**

?> 说明：将字符串转换为列表。
>
> 返回值：anywheresoftware.b4a.objects.collections.List

# KeyValueStore2

版本:2.21
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=KeyValueStore2)

# KeyValueStore
完整类名：b4a.example3.keyvaluestore
> 所有者：process

> 依赖：randomaccessfile | sql | b4xencryption

?> 说明：KeyValueStore:v2.21版本
## IsInitialized方法
**IsInitialized()**

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## _class_globals方法
**_class_globals()**
>
> 返回值：String
## _close方法
**_close()**

?> 说明：关闭商店。
>
> 返回值：String
## _containskey方法
**_containskey(Key)**

?> 说明：测试密钥在存储中是否可用。
>
> 参数：Key，类型：String
>
> 返回值：boolean
## _deleteall方法
**_deleteall()**

?> 说明：从存储中删除所有数据。
>
> 返回值：String
## _get方法
**_get(Key)**
>
> 参数：Key，类型：String
>
> 返回值：Object
## _getbitmap方法
**_getbitmap(Key)**
>
> 参数：Key，类型：String
>
> 返回值：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
## _getdefault方法
**_getdefault(Key,DefaultValue)**
>
> 参数：Key，类型：String
>
> 参数：DefaultValue，类型：Object
>
> 返回值：Object
## _getencrypted方法
**_getencrypted(Key,Password)**
>
> 参数：Key，类型：String
>
> 参数：Password，类型：String
>
> 返回值：Object
## _getmapasync方法
**_getmapasync(Keys)**

?> 说明：以异步方式从存储中检索值。
```vbnet

Wait For (Starter.kvs.GetMapAsync(Array("2 custom types", "time"))) Complete (Result As Map)

```

>
> 参数：Keys，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：anywheresoftware.b4a.keywords.Common.ResumableSubWrapper
## _initialize方法
**_initialize(ba,Dir,FileName)**

?> 说明：初始化存储并设置存储文件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Dir，类型：String
>
> 参数：FileName，类型：String
>
> 返回值：String
## _listkeys方法
**_listkeys()**

?> 说明：返回包含所有键的列表。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## _put方法
**_put(Key,Value)**
>
> 参数：Key，类型：String
>
> 参数：Value，类型：Object
>
> 返回值：String
## _putbitmap方法
**_putbitmap(Key,Value)**
>
> 参数：Key，类型：String
>
> 参数：Value，类型：anywheresoftware.b4a.objects.drawable.CanvasWrapper.BitmapWrapper
>
> 返回值：String
## _putencrypted方法
**_putencrypted(Key,Value,Password)**
>
> 参数：Key，类型：String
>
> 参数：Value，类型：Object
>
> 参数：Password，类型：String
>
> 返回值：String
## _putmapasync方法
**_putmapasync(Map)**

?> 说明：异步插入映射中的键和值。
>
> 参数：Map，类型：anywheresoftware.b4a.objects.collections.Map
>
> 返回值：anywheresoftware.b4a.keywords.Common.ResumableSubWrapper
## _remove方法
**_remove(Key)**

?> 说明：删除映射到此键的键和值。
>
> 参数：Key，类型：String
>
> 返回值：String

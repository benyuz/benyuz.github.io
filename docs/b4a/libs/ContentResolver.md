# ContentResolver

版本:1.5
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=ContentResolver)

# ContentResolver
完整类名：anywheresoftware.b4a.objects.ContentResolverWrapper
> 所有者：process

?> 说明：ContentResolver允许您与其他内容提供商进行交互。
> 事件：
>
> QueryCompleted (Success As Boolean, Crsr As Cursor)
>
> InsertCompleted (Success As Boolean, Uri As Uri)
>
> UpdateCompleted (Success As Boolean, RowsAffected As Int)
>
> DeleteCompleted (Success As Boolean, RowsAffected As Int)
>
> ObserverChange (Uri As Uri)
## Initialize方法
**Initialize(EventName)**

?> 说明：初始化对象并设置将处理异步操作的子。
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## UnregisterObserver方法
**UnregisterObserver(Uri)**
>
> 参数：Uri，类型：anywheresoftware.b4a.objects.ContentResolverWrapper.UriWrapper
>
> 返回值：void
## UpdateAsync方法
**UpdateAsync(ba,Uri,Values,Where,SelectionArgs)**

?> 说明：启动异步更新。操作完成时将引发UpdateCompleted事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Uri，类型：android.net.Uri
>
> 参数：Values，类型：android.content.ContentValues
>
> 参数：Where，类型：java.lang.String
>
> 参数：SelectionArgs，类型：java.lang.String[]
>
> 返回值：void
## Insert方法
**Insert(Uri,Values)**

?> 说明：插入一行。
>
> 参数：Uri，类型：anywheresoftware.b4a.objects.ContentResolverWrapper.UriWrapper
>
> 参数：Values，类型：android.content.ContentValues
>
> 返回值：anywheresoftware.b4a.objects.ContentResolverWrapper.UriWrapper
## Update方法
**Update(Uri,Values,Where,SelectionArgs)**

?> 说明：使用给定的值更新行。
>
> 参数：Uri，类型：android.net.Uri
>
> 参数：Values，类型：android.content.ContentValues
>
> 参数：Where，类型：java.lang.String
>
> 参数：SelectionArgs，类型：java.lang.String[]
>
> 返回值：int
## Query方法
**Query(Uri,Projection,Selection,SelectionArgs,SortOrder)**

?> 说明：查询内容提供商。
>
> 参数：Uri，类型：anywheresoftware.b4a.objects.ContentResolverWrapper.UriWrapper
>
> 参数：Projection，类型：java.lang.String[]
>
> 参数：Selection，类型：java.lang.String
>
> 参数：SelectionArgs，类型：java.lang.String[]
>
> 参数：SortOrder，类型：java.lang.String
>
> 返回值：anywheresoftware.b4a.sql.SQL.CursorWrapper
## UpdateDelete方法
**UpdateDelete(ba,Uri,Where,SelectionArgs)**

?> 说明：启动异步删除。操作完成时将引发DeleteCompleted事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Uri，类型：android.net.Uri
>
> 参数：Where，类型：java.lang.String
>
> 参数：SelectionArgs，类型：java.lang.String[]
>
> 返回值：void
## Delete方法
**Delete(Uri,Where,SelectionArgs)**

?> 说明：根据给定条件删除行。
>
> 参数：Uri，类型：android.net.Uri
>
> 参数：Where，类型：java.lang.String
>
> 参数：SelectionArgs，类型：java.lang.String[]
>
> 返回值：int
## InsertAsync方法
**InsertAsync(ba,Uri,Values)**

?> 说明：启动异步插入。操作完成时将引发InsertCompleted事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Uri，类型：anywheresoftware.b4a.objects.ContentResolverWrapper.UriWrapper
>
> 参数：Values，类型：android.content.ContentValues
>
> 返回值：void
## RegisterObserver方法
**RegisterObserver(ba,Uri,NotifyForDescendents)**

?> 说明：注册一个内容观察器。只要存在与给定Uri相关的更改，就会引发ObserverChange事件。
```vbnet

Sub Process_Globals
	Private cr As ContentResolver
End Sub

Sub Service_Create
	Dim uri As Uri
	uri.Parse("content://com.android.contacts/contacts")
	cr.Initialize("cr")
	cr.RegisterObserver(uri, True)
End Sub

Sub cr_ObserverChange (Uri As Uri)
	Log("Contacts provider has reported a change...")
End Sub
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Uri，类型：anywheresoftware.b4a.objects.ContentResolverWrapper.UriWrapper
>
> 参数：NotifyForDescendents，类型：boolean
>
> 返回值：void
## QueryAsync方法
**QueryAsync(ba,Uri,Projection,Selection,SelectionArgs,SortOrder)**
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：Uri，类型：anywheresoftware.b4a.objects.ContentResolverWrapper.UriWrapper
>
> 参数：Projection，类型：java.lang.String[]
>
> 参数：Selection，类型：java.lang.String
>
> 参数：SelectionArgs，类型：java.lang.String[]
>
> 参数：SortOrder，类型：java.lang.String
>
> 返回值：void

# Uri
完整类名：anywheresoftware.b4a.objects.ContentResolverWrapper.UriWrapper
> 所有者：process

> 包装器：android.net.Uri
## FromParts方法
**FromParts(Scheme,SSP,Fragment)**

?> 说明：根据给定的部分创建新的Uri。
>
> 参数：Scheme，类型：java.lang.String
>
> 参数：SSP，类型：java.lang.String
>
> 参数：Fragment，类型：java.lang.String
>
> 返回值：void
## ParseId方法
**ParseId()**

?> 说明：返回当前Uri的Id部分。
>
> 返回值：long
## Parse方法
**Parse(UriString)**

?> 说明：根据给定字符串创建新的Uri。
>
> 参数：UriString，类型：java.lang.String
>
> 返回值：void
## WithAppendedId方法
**WithAppendedId(BaseUri,Id)**

?> 说明：通过将Id附加到给定的Uri来创建新的Uri。
>
> 参数：BaseUri，类型：android.net.Uri
>
> 参数：Id，类型：long
>
> 返回值：void
## WithAppendedPath方法
**WithAppendedPath(BaseUri,PathSegment)**

?> 说明：通过将路径附加到给定的Uri来创建新的Uri。
>
> 参数：BaseUri，类型：android.net.Uri
>
> 参数：PathSegment，类型：java.lang.String
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean

# ContentValues
完整类名：anywheresoftware.b4a.objects.ContentResolverWrapper.ContentValuesWrapper
> 所有者：process

> 包装器：android.content.ContentValues

?> 说明：保存成对的键和值。
## Initialize方法
**Initialize()**
>
> 返回值：void
## PutNull方法
**PutNull(Key)**
>
> 参数：Key，类型：java.lang.String
>
> 返回值：void
## PutInteger方法
**PutInteger(Key,Value)**
>
> 参数：Key，类型：java.lang.String
>
> 参数：Value，类型：int
>
> 返回值：void
## PutBoolean方法
**PutBoolean(Key,Value)**
>
> 参数：Key，类型：java.lang.String
>
> 参数：Value，类型：boolean
>
> 返回值：void
## PutString方法
**PutString(Key,Value)**
>
> 参数：Key，类型：java.lang.String
>
> 参数：Value，类型：java.lang.String
>
> 返回值：void
## PutBytes方法
**PutBytes(Key,Value)**
>
> 参数：Key，类型：java.lang.String
>
> 参数：Value，类型：byte[]
>
> 返回值：void
## PutShort方法
**PutShort(Key,Value)**
>
> 参数：Key，类型：java.lang.String
>
> 参数：Value，类型：java.lang.Short
>
> 返回值：void
## PutFloat方法
**PutFloat(Key,Value)**
>
> 参数：Key，类型：java.lang.String
>
> 参数：Value，类型：java.lang.Float
>
> 返回值：void
## PutDouble方法
**PutDouble(Key,Value)**
>
> 参数：Key，类型：java.lang.String
>
> 参数：Value，类型：java.lang.Double
>
> 返回值：void
## Remove方法
**Remove(Key)**
>
> 参数：Key，类型：java.lang.String
>
> 返回值：void
## PutLong方法
**PutLong(Key,Value)**
>
> 参数：Key，类型：java.lang.String
>
> 参数：Value，类型：java.lang.Long
>
> 返回值：void
## PutByte方法
**PutByte(Key,Value)**
>
> 参数：Key，类型：java.lang.String
>
> 参数：Value，类型：java.lang.Byte
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean

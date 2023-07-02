# SQL

版本:1.5
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=SQL)

# SQL
完整类名：anywheresoftware.b4a.sql.SQL
> 所有者：process

?> 说明：访问数据库的主要对象。
> 事件：
>
> QueryComplete (Success As Boolean, Result As ResultSet)
>
> NonQueryComplete (Success As Boolean)
## EndTransaction方法
**EndTransaction()**

?> 说明：结束交易。
>
> 返回值：void
## ExecQuery2方法
**ExecQuery2(Query,StringArgs)**

?> 说明：执行查询并返回用于遍历结果的光标。
```vbnet

Dim Cursor As Cursor
Cursor = sql1.ExecQuery2("SELECT col1 FROM table1 WHERE col3 = ?", Array As String(22))
```

>
> 参数：Query，类型：java.lang.String
>
> 参数：StringArgs，类型：java.lang.String[]
>
> 返回值：android.database.Cursor
## ExecQuery方法
**ExecQuery(Query)**

?> 说明：执行查询并返回用于遍历结果的光标。
```vbnet

Dim Cursor As Cursor
Cursor = SQL1.ExecQuery("SELECT col1, col2 FROM table1")
For i = 0 To Cursor.RowCount - 1
	Cursor.Position = i
	Log(Cursor.GetString("col1"))
	Log(Cursor.GetInt("col2"))
Next
```

>
> 参数：Query，类型：java.lang.String
>
> 返回值：android.database.Cursor
## ExecQuerySingleResult2方法
**ExecQuerySingleResult2(Query,StringArgs)**

?> 说明：执行查询并返回（结果集中）第一列和第一行中的值。
```vbnet

Dim NumberOfMatches As Int
NumberOfMatches = SQL1.ExecQuerySingleResult2("SELECT count(*) FROM table1 WHERE col2 > ?", Array As String(300))
```

>
> 参数：Query，类型：java.lang.String
>
> 参数：StringArgs，类型：java.lang.String[]
>
> 返回值：java.lang.String
## IsInitialized方法
**IsInitialized()**

?> 说明：测试数据库是否已初始化和打开。
>
> 返回值：boolean
## Initialize方法
**Initialize(Dir,FileName,CreateIfNecessary)**

?> 说明：打开数据库文件。如果新数据库不存在并且CreateIfNenecessary为true，则将创建该数据库。
```vbnet

Dim SQL1 As SQL
SQL1.Initialize(File.DirInternal, "MyDb.db", True)
```

>
> 参数：Dir，类型：java.lang.String
>
> 参数：FileName，类型：java.lang.String
>
> 参数：CreateIfNecessary，类型：boolean
>
> 返回值：void
## ExecNonQueryBatch方法
**ExecNonQueryBatch(ba,EventName)**

?> 说明：异步执行一批非查询语句（如INSERT）。
```vbnet

For i = 1 To 1000
	sql.AddNonQueryToBatch("INSERT INTO table1 VALUES (?)", Array(Rnd(0, 100000)))
Next
Dim SenderFilter As Object = sql.ExecNonQueryBatch("SQL")
Wait For (SenderFilter) SQL_NonQueryComplete (Success As Boolean)
Log("NonQuery: " & Success)
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：java.lang.Object
## BeginTransaction方法
**BeginTransaction()**

?> 说明：开始交易。事务是一组以原子方式提交的多个“写入”语句，
```vbnet

SQL1.BeginTransaction
Try
	'block of statements like:
	For i = 1 to 1000
		SQL1.ExecNonQuery("INSERT INTO table1 VALUES(...)
	Next
	SQL1.TransactionSuccessful
Catch
	Log(LastException.Message) 'no changes will be made
End Try
SQL1.EndTransaction
```

>
> 返回值：void
## AddNonQueryToBatch方法
**AddNonQueryToBatch(Statement,Args)**

?> 说明：将非查询语句添加到语句批中。
```vbnet

For i = 1 To 1000
	sql.AddNonQueryToBatch("INSERT INTO table1 VALUES (?)", Array(Rnd(0, 100000)))
Next
Dim SenderFilter As Object = sql.ExecNonQueryBatch("SQL")
Wait For (SenderFilter) SQL_NonQueryComplete (Success As Boolean)
Log("NonQuery: " & Success)
```

>
> 参数：Statement，类型：java.lang.String
>
> 参数：Args，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## ExecQuerySingleResult方法
**ExecQuerySingleResult(Query)**

?> 说明：执行查询并返回（结果集中）第一列和第一行中的值。
```vbnet

Dim NumberOfMatches As Int
NumberOfMatches = SQL1.ExecQuerySingleResult("SELECT count(*) FROM table1 WHERE col2 > 300")
```

>
> 参数：Query，类型：java.lang.String
>
> 返回值：java.lang.String
## TransactionSuccessful方法
**TransactionSuccessful()**

?> 说明：将交易标记为成功交易。在调用EndTransaction之前，不应再执行任何语句。
>
> 返回值：void
## ExecNonQuery方法
**ExecNonQuery(Statement)**

?> 说明：执行单个非查询SQL语句。
```vbnet

SQL1.ExecNonQuery("CREATE TABLE table1 (col1 TEXT , col2 INTEGER, col3 INTEGER)")
```

>
> 参数：Statement，类型：java.lang.String
>
> 返回值：void
## Close方法
**Close()**

?> 说明：关闭数据库。
>
> 返回值：void
## ExecQueryAsync方法
**ExecQueryAsync(ba,EventName,Query,Args)**

?> 说明：异步执行给定的查询。当结果准备就绪时，将引发QueryComplete事件。
```vbnet

Dim SenderFilter As Object = sql.ExecQueryAsync("SQL", "SELECT * FROM table1", Null)
Wait For (SenderFilter) SQL_QueryComplete (Success As Boolean, rs As ResultSet)
If Success Then
	Do While rs.NextRow
		Log(rs.GetInt2(0))
	Loop
	rs.Close
Else
	Log(LastException)
End If
```

>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Query，类型：java.lang.String
>
> 参数：Args，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：java.lang.Object
## ExecNonQuery2方法
**ExecNonQuery2(Statement,Args)**

?> 说明：执行单个非查询SQL语句。
```vbnet

SQL1.ExecNonQuery2("INSERT INTO table1 VALUES (?, ?, 0)", Array As Object("some text", 2))
```

>
> 参数：Statement，类型：java.lang.String
>
> 参数：Args，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void

# Cursor
完整类名：anywheresoftware.b4a.sql.SQL.CursorWrapper
> 所有者：process

> 包装器：android.database.Cursor
## GetInt2方法
**GetInt2(Index)**

?> 说明：返回按给定序号存储在列中的Int值。
```vbnet

Log(Cursor.GetInt2(0))
```

>
> 参数：Index，类型：int
>
> 返回值：int
## GetBlob方法
**GetBlob(ColumnName)**

?> 说明：返回存储在给定列中的blob。
```vbnet

Dim Buffer() As Byte
Buffer = Cursor.GetBlob("col1")
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：byte[]
## GetDouble方法
**GetDouble(ColumnName)**

?> 说明：返回存储在给定列中的Double值。
```vbnet

Log(Cursor.GetDouble("col2"))
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：java.lang.Double
## GetLong方法
**GetLong(ColumnName)**

?> 说明：返回存储在给定列中的长值。
```vbnet

Log(Cursor.GetLong("col2"))
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：java.lang.Long
## GetColumnName方法
**GetColumnName(Index)**

?> 说明：返回指定索引处的列的名称。
>
> 参数：Index，类型：int
>
> 返回值：java.lang.String
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## GetBlob2方法
**GetBlob2(Index)**

?> 说明：返回按给定序号存储在列中的blob。
```vbnet

Dim Buffer() As Byte
Buffer = Cursor.GetBlob2(0)
```

>
> 参数：Index，类型：int
>
> 返回值：byte[]
## GetInt方法
**GetInt(ColumnName)**

?> 说明：返回存储在给定列中的Int值。
```vbnet

Log(Cursor.GetInt("col2"))
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：int
## GetString方法
**GetString(ColumnName)**

?> 说明：返回存储在给定列中的字符串值。
```vbnet

Log(Cursor.GetString("col2"))
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：java.lang.String
## Close方法
**Close()**

?> 说明：关闭光标并释放资源。
>
> 返回值：void
## GetDouble2方法
**GetDouble2(Index)**

?> 说明：返回按给定序号存储在列中的Double值。
```vbnet

Log(Cursor.GetDouble2(0))
```

>
> 参数：Index，类型：int
>
> 返回值：java.lang.Double
## GetString2方法
**GetString2(Index)**

?> 说明：返回存储在列中给定序号的字符串值。
```vbnet

Log(Cursor.GetString2(0))
```

>
> 参数：Index，类型：int
>
> 返回值：java.lang.String
## GetLong2方法
**GetLong2(Index)**

?> 说明：返回按给定序号存储在列中的长值。
```vbnet

Log(Cursor.GetLong2(0))
```

>
> 参数：Index，类型：int
>
> 返回值：java.lang.Long
## ColumnCount属性

?> 说明：获取结果集中可用的列数。
>
> 返回值：int
## Position属性

?> 说明：获取或设置当前位置（行）。
```vbnet

Dim Cursor As Cursor
Cursor = SQL1.ExecQuery("SELECT col1, col2 FROM table1")
For i = 0 To Cursor.RowCount - 1
	Cursor.Position = i
	Log(Cursor.GetString("col1"))
	Log(Cursor.GetInt("col2"))
Next
Cursor.Close
```

>
> 参数：Value，类型：int
>
> 返回值：int
## RowCount属性

?> 说明：获取结果集中可用的行数。
>
> 返回值：int

# ResultSet
完整类名：anywheresoftware.b4a.sql.SQL.ResultSetWrapper
> 所有者：process

> 包装器：android.database.Cursor

?> 说明：此类型是Cursor类型的扩展。
## GetInt2方法
**GetInt2(Index)**

?> 说明：返回按给定序号存储在列中的Int值。
```vbnet

Log(Cursor.GetInt2(0))
```

>
> 参数：Index，类型：int
>
> 返回值：int
## GetBlob方法
**GetBlob(ColumnName)**

?> 说明：返回存储在给定列中的blob。
```vbnet

Dim Buffer() As Byte
Buffer = Cursor.GetBlob("col1")
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：byte[]
## GetDouble方法
**GetDouble(ColumnName)**

?> 说明：返回存储在给定列中的Double值。
```vbnet

Log(Cursor.GetDouble("col2"))
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：java.lang.Double
## GetLong方法
**GetLong(ColumnName)**

?> 说明：返回存储在给定列中的长值。
```vbnet

Log(Cursor.GetLong("col2"))
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：java.lang.Long
## GetColumnName方法
**GetColumnName(Index)**

?> 说明：返回指定索引处的列的名称。
>
> 参数：Index，类型：int
>
> 返回值：java.lang.String
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## GetBlob2方法
**GetBlob2(Index)**

?> 说明：返回按给定序号存储在列中的blob。
```vbnet

Dim Buffer() As Byte
Buffer = Cursor.GetBlob2(0)
```

>
> 参数：Index，类型：int
>
> 返回值：byte[]
## GetInt方法
**GetInt(ColumnName)**

?> 说明：返回存储在给定列中的Int值。
```vbnet

Log(Cursor.GetInt("col2"))
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：int
## NextRow方法
**NextRow()**

?> 说明：将光标移动到下一个结果。当光标到达末尾时返回false。
```vbnet

Do While ResultSet1.NextRow
 'Work with Row
Loop
```

>
> 返回值：boolean
## GetString方法
**GetString(ColumnName)**

?> 说明：返回存储在给定列中的字符串值。
```vbnet

Log(Cursor.GetString("col2"))
```

>
> 参数：ColumnName，类型：java.lang.String
>
> 返回值：java.lang.String
## Close方法
**Close()**

?> 说明：关闭光标并释放资源。
>
> 返回值：void
## GetDouble2方法
**GetDouble2(Index)**

?> 说明：返回按给定序号存储在列中的Double值。
```vbnet

Log(Cursor.GetDouble2(0))
```

>
> 参数：Index，类型：int
>
> 返回值：java.lang.Double
## GetString2方法
**GetString2(Index)**

?> 说明：返回存储在列中给定序号的字符串值。
```vbnet

Log(Cursor.GetString2(0))
```

>
> 参数：Index，类型：int
>
> 返回值：java.lang.String
## GetLong2方法
**GetLong2(Index)**

?> 说明：返回按给定序号存储在列中的长值。
```vbnet

Log(Cursor.GetLong2(0))
```

>
> 参数：Index，类型：int
>
> 返回值：java.lang.Long
## ColumnCount属性

?> 说明：获取结果集中可用的列数。
>
> 返回值：int
## Position属性

?> 说明：获取或设置当前位置（行）。
```vbnet

Dim Cursor As Cursor
Cursor = SQL1.ExecQuery("SELECT col1, col2 FROM table1")
For i = 0 To Cursor.RowCount - 1
	Cursor.Position = i
	Log(Cursor.GetString("col1"))
	Log(Cursor.GetInt("col2"))
Next
Cursor.Close
```

>
> 参数：Value，类型：int
>
> 返回值：int
## RowCount属性

?> 说明：获取结果集中可用的行数。
>
> 返回值：int

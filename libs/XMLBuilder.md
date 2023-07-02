# XMLBuilder

版本:1.0
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=XMLBuilder)

# XMLBuilder
完整类名：com.jamesmurty.utils.XMLBuilder
> 所有者：process

?> 说明：这是javaxmlbuilder库的包装器。
## cdata方法
**cdata(data)**

?> 说明：将具有String内容的CDATA节点添加到由以下元素表示的元素中
>
> 参数：data，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## ns方法
**ns(namespaceURI)**

?> 说明：{@link#命名空间（字符串）}的同义词。
>
> 参数：namespaceURI，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## xpathQuery方法
**xpathQuery(xpath,type)**

?> 说明：返回在构建器的DOM上评估XPath查询的结果。
>
> 参数：xpath，类型：java.lang.String
>
> 参数：type，类型：javax.xml.namespace.QName
>
> 返回值：java.lang.Object
## elementAsString方法
**elementAsString(outputProperties)**

?> 说明：通过将当前XML元素及其子元素序列化为字符串
>
> 参数：outputProperties，类型：java.util.Map
>
> 返回值：java.lang.String
## toWriter2方法
**toWriter2(writer,outputProperties)**

?> 说明：使用默认值将XML文档序列化到给定的编写器
>
> 参数：writer，类型：java.io.Writer
>
> 参数：outputProperties，类型：java.util.Map
>
> 返回值：void
## toWriter方法
**toWriter(wholeDocument,writer,outputProperties)**

?> 说明：序列化此XMLBuilder包装的特定元素或其整个
>
> 参数：wholeDocument，类型：boolean
>
> 参数：writer，类型：java.io.Writer
>
> 参数：outputProperties，类型：java.util.Map
>
> 返回值：void
## root方法
**root()**

?> 说明：返回类型：@Return：表示XML文档根元素的构建器节点。
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## cmnt方法
**cmnt(comment)**

?> 说明：{@link#comment（String）}的同义词。
>
> 参数：comment，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## data方法
**data(data)**

?> 说明：{@link#cdata（字符串）}的同义词。
>
> 参数：data，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## attribute方法
**attribute(name,value)**

?> 说明：将命名属性值添加到此生成器表示的元素
>
> 参数：name，类型：java.lang.String
>
> 参数：value，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## elementBefore方法
**elementBefore(name)**

?> 说明：将命名的XML元素作为同级元素添加到文档中
>
> 参数：name，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## asString方法
**asString()**

?> 说明：将XML文档序列化为不包括XML声明的字符串。
>
> 返回值：java.lang.String
## inst方法
**inst(target,data)**

?> 说明：{@link#指令（字符串，字符串）}的同义词。
>
> 参数：target，类型：java.lang.String
>
> 参数：data，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## elementBefore2方法
**elementBefore2(name,namespaceURI)**

?> 说明：将命名和命名空间的XML元素作为同级元素添加到文档中
>
> 参数：name，类型：java.lang.String
>
> 参数：namespaceURI，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## create2方法
**create2(name,namespaceURI)**

?> 说明：为具有默认名称空间的新XML文档构造生成器。
>
> 参数：name，类型：java.lang.String
>
> 参数：namespaceURI，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## namespace方法
**namespace(namespaceURI)**

?> 说明：将XML命名空间属性添加到此生成器的元素节点
>
> 参数：namespaceURI，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## element2方法
**element2(name,namespaceURI)**

?> 说明：将命名和命名空间的XML元素作为的子元素添加到文档中
>
> 参数：name，类型：java.lang.String
>
> 参数：namespaceURI，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## instruction方法
**instruction(target,data)**

?> 说明：将指令添加到此生成器节点表示的元素，然后
>
> 参数：target，类型：java.lang.String
>
> 参数：data，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## parse方法
**parse(inputSource)**

?> 说明：从现有的XML文档构造生成器。提供的XML
>
> 参数：inputSource，类型：org.xml.sax.InputSource
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## element方法
**element(name)**

?> 说明：将命名的XML元素作为该构建器节点的子元素添加到文档中，
>
> 参数：name，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## text方法
**text(value)**

?> 说明：将文本值添加到此生成器节点表示的元素，然后
>
> 参数：value，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## d方法
**d(data)**

?> 说明：{@link#cdata（字符串）}的同义词。
>
> 参数：data，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## e方法
**e(name)**

?> 说明：{@link#元素（字符串）}的同义词。
>
> 参数：name，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## c方法
**c(comment)**

?> 说明：{@link#comment（String）}的同义词。
>
> 参数：comment，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## equals方法
**equals(obj)**

?> 说明：返回类型：@Return：true如果XML文档和元素对象被
>
> 参数：obj，类型：java.lang.Object
>
> 返回值：boolean
## importXMLBuilder方法
**importXMLBuilder(builder)**

?> 说明：将另一个XMLBuilder文档导入到该文档中，位于
>
> 参数：builder，类型：com.jamesmurty.utils.XMLBuilder
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## namespace2方法
**namespace2(prefix,namespaceURI)**

?> 说明：将XML命名空间属性添加到此生成器的元素节点。
>
> 参数：prefix，类型：java.lang.String
>
> 参数：namespaceURI，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## a方法
**a(name,value)**

?> 说明：{@link#属性（字符串，字符串）}的同义词。
>
> 参数：name，类型：java.lang.String
>
> 参数：value，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## xpathQuery2方法
**xpathQuery2(xpath,type,nsContext)**

?> 说明：返回在构建器的DOM上评估XPath查询的结果
>
> 参数：xpath，类型：java.lang.String
>
> 参数：type，类型：javax.xml.namespace.QName
>
> 参数：nsContext，类型：javax.xml.namespace.NamespaceContext
>
> 返回值：java.lang.Object
## attr方法
**attr(name,value)**

?> 说明：{@link#属性（字符串，字符串）}的同义词。
>
> 参数：name，类型：java.lang.String
>
> 参数：value，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## xpathFind2方法
**xpathFind2(xpath,nsContext)**

?> 说明：在生成器的DOM中查找与给定的匹配的第一个元素
>
> 参数：xpath，类型：java.lang.String
>
> 参数：nsContext，类型：javax.xml.namespace.NamespaceContext
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## buildDocumentNamespaceContext方法
**buildDocumentNamespaceContext()**

?> 说明：返回类型：@Return：包含所使用的前缀和命名空间URI的命名空间上下文
>
> 返回值：com.jamesmurty.utils.NamespaceContextImpl
## up2方法
**up2(steps)**

?> 说明：返回表示第n个</em>祖先元素的生成器节点
>
> 参数：steps，类型：int
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## create方法
**create(name)**

?> 说明：为新的XML文档构造生成器。将创建文档
>
> 参数：name，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## reference方法
**reference(name)**

?> 说明：添加对此构建器节点表示的元素的引用，然后
>
> 参数：name，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## up方法
**up()**

?> 说明：返回表示当前节点的父节点的生成器节点。
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## i方法
**i(target,data)**

?> 说明：{@link#指令（字符串，字符串）}的同义词。
>
> 参数：target，类型：java.lang.String
>
> 参数：data，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## ns2方法
**ns2(prefix,namespaceURI)**

?> 说明：{@link#命名空间（String，String）}的同义词。
>
> 参数：prefix，类型：java.lang.String
>
> 参数：namespaceURI，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## elem方法
**elem(name)**

?> 说明：{@link#元素（字符串）}的同义词。
>
> 参数：name，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## asString2方法
**asString2(outputProperties)**

?> 说明：通过委托给
>
> 参数：outputProperties，类型：java.util.Map
>
> 返回值：java.lang.String
## ref方法
**ref(name)**

?> 说明：{@link#reference（String）}的同义词。
>
> 参数：name，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## xpathFind方法
**xpathFind(xpath)**

?> 说明：在生成器的DOM中查找与给定的匹配的第一个元素
>
> 参数：xpath，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## t方法
**t(value)**

?> 说明：{@link#text（String）}的同义词。
>
> 参数：value，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## r方法
**r(name)**

?> 说明：{@link#reference（String）}的同义词。
>
> 参数：name，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## GetElement方法
**GetElement()**

?> 说明：返回类型：@Return：这个构建器节点包装的XML元素。
>
> 返回值：org.w3c.dom.Element
## comment方法
**comment(comment)**

?> 说明：将注释添加到此生成器节点表示的元素，然后
>
> 参数：comment，类型：java.lang.String
>
> 返回值：com.jamesmurty.utils.XMLBuilder
## Document属性
>
> 返回值：org.w3c.dom.Document

# XUI2D

版本:1.02
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=XUI2D)

# B2WorldManifold
完整类名：anywheresoftware.b4a.objects.B2WorldManifold
> 所有者：process
## GetPoint方法
**GetPoint(Index)**

?> 说明：世界接触点（交叉点）
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## Normal属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## PointCount字段
>
> 返回值：int

# B2Manifold
完整类名：anywheresoftware.b4a.objects.B2WorldManifold.B2Manifold
> 所有者：process
## GetManifoldPoint方法
**GetManifoldPoint(Index)**
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.B2WorldManifold.B2ManifoldPoint
## PointCount属性
>
> 返回值：int

# B2ManifoldPoint
完整类名：anywheresoftware.b4a.objects.B2WorldManifold.B2ManifoldPoint
> 所有者：process
## LocalPoint属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## TangentImpulse属性
>
> 返回值：float
## NormalImpulse属性
>
> 返回值：float

# B2ContactImpulse
完整类名：anywheresoftware.b4a.objects.B2WorldManifold.B2ContactImpulse
> 所有者：process
## GetNormalImpulse方法
**GetNormalImpulse(Index)**
>
> 参数：Index，类型：int
>
> 返回值：float
## GetTangentImpulse方法
**GetTangentImpulse(Index)**
>
> 参数：Index，类型：int
>
> 返回值：float
## PointCount属性
>
> 返回值：int

# B2World
完整类名：anywheresoftware.b4a.objects.B2World
> 所有者：process
> 事件：
>
> BeginContact (Contact As B2Contact)
>
> EndContact (Contact As B2Contact)
>
> PreSolve (Contact As B2Contact, OldManifold As B2Manifold)
>
> PostSolve (Contact As B2Contact, Impulse As B2ContactImpulse)
>
> RayCastCallback (Fixture As B2Fixture, Point As B2Vec2, Normal As B2Vec2, Fraction As Float) As Float
## DestroyBody方法
**DestroyBody(Body)**

?> 说明：这将自动删除所有关联的形状和关节。
>
> 参数：Body，类型：anywheresoftware.b4a.objects.B2Body
>
> 返回值：void
## RayCast方法
**RayCast(FromVec,ToVec)**

?> 说明：光线投射了光线路径上所有固定装置的世界，从FromVec到ToVec。您的回调控制您是否
>
> 参数：FromVec，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：ToVec，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## FirstJoint方法
**FirstJoint()**
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## Initialize方法
**Initialize(ba,EventName,Gravity)**

?> 说明：初始化世界并设置其重力。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 参数：Gravity，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## sayGoodbye方法
**sayGoodbye(joint)**
>
> 参数：joint，类型：org.jbox2d.dynamics.joints.Joint
>
> 返回值：void
## TimeStep方法
**TimeStep(TimeStep,VelocityIterations,PositionIterations)**

?> 说明：迈出一步。这将执行碰撞检测、集成和约束解决方案。
>
> 参数：TimeStep，类型：float
>
> 参数：VelocityIterations，类型：int
>
> 参数：PositionIterations，类型：int
>
> 返回值：void
## CreateVec2方法
**CreateVec2(X,Y)**

?> 说明：创建了一个B2Vec2载体。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## DestroyJoint方法
**DestroyJoint(Joint)**
>
> 参数：Joint，类型：anywheresoftware.b4a.objects.joints.B2Joint
>
> 返回值：void
## QueryAABBToMapOfBodies方法
**QueryAABBToMapOfBodies(AABB)**

?> 说明：查询世界上可能与给定AABB重叠的所有固定装置。
>
> 参数：AABB，类型：anywheresoftware.b4a.objects.B2AABB
>
> 返回值：anywheresoftware.b4a.objects.collections.Map
## CreateBody方法
**CreateBody(BodyDef)**

?> 说明：在给定定义的情况下创建刚体。
>
> 参数：BodyDef，类型：anywheresoftware.b4a.objects.B2Body.B2BodyDef
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## CreateJoint方法
**CreateJoint(JointDef)**
>
> 参数：JointDef，类型：anywheresoftware.b4a.objects.joints.B2Joint.B2JointDef
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## FirstContact方法
**FirstContact()**

?> 说明：返回第一个联系人。请注意，联系人列表包括非接触联系人。
```vbnet

Dim contact As B2Contact = world.FirstContact
Do While contact <> Null
	If contact.IsTouching Then
		'...
	End If
	contact = contact.NextContact
Loop
```

>
> 返回值：anywheresoftware.b4a.objects.B2Contact
## QueryAABBToListOfFixtures方法
**QueryAABBToListOfFixtures(AABB)**

?> 说明：查询世界上可能与给定AABB重叠的所有固定装置。
>
> 参数：AABB，类型：anywheresoftware.b4a.objects.B2AABB
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## Locked属性

?> 说明：如果当前世界已锁定以进行更改，则返回True。
>
> 返回值：boolean
## AllBodies属性

?> 说明：返回包含所有实体的列表。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## DynamicBodies属性

?> 说明：返回一个包含所有具有动态实体类型的实体的列表。
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## Gravity属性

?> 说明：获取或设置世界重力。
>
> 参数：v，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2

# B2Vec2
完整类名：anywheresoftware.b4a.objects.B2Vec2
> 所有者：process
## Equals方法
**Equals(Other)**

?> 说明：测试两个向量是否相等。
>
> 参数：Other，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：boolean
## Set方法
**Set(X,Y)**

?> 说明：按分量设置矢量。
>
> 参数：X，类型：float
>
> 参数：Y，类型：float
>
> 返回值：void
## SubtractFromThis方法
**SubtractFromThis(Other)**

?> 说明：从这个向量中减去另一个向量，返回结果-改变这个向量。
>
> 参数：Other，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## AddToThis方法
**AddToThis(Other)**

?> 说明：将另一个向量加到这个向量上，并返回结果-更改这个向量。
>
> 参数：Other，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## MultiplyThis方法
**MultiplyThis(Scalar)**

?> 说明：将这个向量乘以一个数字并返回结果-改变这个向量。
>
> 参数：Scalar，类型：float
>
> 返回值：void
## CreateCopy方法
**CreateCopy()**

?> 说明：创建当前矢量的副本。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## NormalizeThis方法
**NormalizeThis()**

?> 说明：规格化此向量并返回规格化前的长度。更改此矢量。
>
> 返回值：float
## Negate方法
**Negate()**

?> 说明：返回该向量的否定；不会改变这个矢量。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## LengthSquared属性

?> 说明：返回此向量的平方长度。
>
> 返回值：float
## Length属性

?> 说明：返回此矢量的长度。
>
> 返回值：float
## X属性
>
> 参数：x，类型：float
>
> 返回值：float
## Y属性
>
> 参数：y，类型：float
>
> 返回值：float

# B2Transform
完整类名：anywheresoftware.b4a.objects.B2Transform
> 所有者：process
## MultiplyRot方法
**MultiplyRot(v)**

?> 说明：将向量与变换旋转矩阵相乘。
>
> 参数：v，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## Initialize方法
**Initialize()**

?> 说明：创建新的标识变换。
>
> 返回值：void
## Translation属性

?> 说明：获取或设置由转换引起的转换
>
> 参数：v，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## Angle属性

?> 说明：获取或设置由转换引起的旋转
>
> 参数：f，类型：float
>
> 返回值：float

# 
完整类名：anywheresoftware.b4a.objects.B2Shape
> 所有者：process

> 包装器：T
## ComputeAABB方法
**ComputeAABB(Output,Transform)**

?> 说明：基于传递的变换计算形状AABB。结果存储在Output对象中。
>
> 参数：Output，类型：anywheresoftware.b4a.objects.B2AABB
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 返回值：void
## TestPoint方法
**TestPoint(Transform,Point)**

?> 说明：测试此形状中的某个点是否包含。这只适用于凸面形状。
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 参数：Point，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：boolean
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Radius属性

?> 说明：获取或设置基础形状的半径。根据
>
> 参数：radius，类型：float
>
> 返回值：float
## ShapeType属性

?> 说明：返回作为shape常量之一的形状类型。
>
> 返回值：java.lang.Object
## SHAPE_CIRCLE字段
>
> 返回值：java.lang.Object
## SHAPE_CHAIN字段
>
> 返回值：java.lang.Object
## SHAPE_EDGE字段
>
> 返回值：java.lang.Object
## SHAPE_POLYGON字段
>
> 返回值：java.lang.Object

# B2Shape
完整类名：anywheresoftware.b4a.objects.B2Shape.ConcreteB2Shape
> 所有者：process

> 包装器：org.jbox2d.collision.shapes.Shape
## ComputeAABB方法
**ComputeAABB(Output,Transform)**

?> 说明：基于传递的变换计算形状AABB。结果存储在Output对象中。
>
> 参数：Output，类型：anywheresoftware.b4a.objects.B2AABB
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 返回值：void
## TestPoint方法
**TestPoint(Transform,Point)**

?> 说明：测试此形状中的某个点是否包含。这只适用于凸面形状。
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 参数：Point，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：boolean
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Radius属性

?> 说明：获取或设置基础形状的半径。根据
>
> 参数：radius，类型：float
>
> 返回值：float
## ShapeType属性

?> 说明：返回作为shape常量之一的形状类型。
>
> 返回值：java.lang.Object
## SHAPE_CIRCLE字段
>
> 返回值：java.lang.Object
## SHAPE_CHAIN字段
>
> 返回值：java.lang.Object
## SHAPE_EDGE字段
>
> 返回值：java.lang.Object
## SHAPE_POLYGON字段
>
> 返回值：java.lang.Object

# B2CircleShape
完整类名：anywheresoftware.b4a.objects.B2Shape.B2CircleShape
> 所有者：process

> 包装器：org.jbox2d.collision.shapes.CircleShape

?> 说明：圆形。
## ComputeAABB方法
**ComputeAABB(Output,Transform)**

?> 说明：基于传递的变换计算形状AABB。结果存储在Output对象中。
>
> 参数：Output，类型：anywheresoftware.b4a.objects.B2AABB
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 返回值：void
## TestPoint方法
**TestPoint(Transform,Point)**

?> 说明：测试此形状中的某个点是否包含。这只适用于凸面形状。
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 参数：Point，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：boolean
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Radius)**
>
> 参数：Radius，类型：float
>
> 返回值：void
## Radius属性

?> 说明：获取或设置基础形状的半径。根据
>
> 参数：radius，类型：float
>
> 返回值：float
## SupportVertex属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## ShapeType属性

?> 说明：返回作为shape常量之一的形状类型。
>
> 返回值：java.lang.Object
## SHAPE_CIRCLE字段
>
> 返回值：java.lang.Object
## SHAPE_CHAIN字段
>
> 返回值：java.lang.Object
## SHAPE_EDGE字段
>
> 返回值：java.lang.Object
## SHAPE_POLYGON字段
>
> 返回值：java.lang.Object

# B2EdgeShape
完整类名：anywheresoftware.b4a.objects.B2Shape.B2EdgeShape
> 所有者：process

> 包装器：org.jbox2d.collision.shapes.EdgeShape

?> 说明：线段（边）形状。这些可以以链或环的形式连接到其他边缘形状。这个
## Set方法
**Set(FromVec,ToVec)**
>
> 参数：FromVec，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：ToVec，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## ComputeAABB方法
**ComputeAABB(Output,Transform)**

?> 说明：基于传递的变换计算形状AABB。结果存储在Output对象中。
>
> 参数：Output，类型：anywheresoftware.b4a.objects.B2AABB
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 返回值：void
## TestPoint方法
**TestPoint(Transform,Point)**

?> 说明：测试此形状中的某个点是否包含。这只适用于凸面形状。
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 参数：Point，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：boolean
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(FromVec,ToVec)**
>
> 参数：FromVec，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：ToVec，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## Vertex2属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## Radius属性

?> 说明：获取或设置基础形状的半径。根据
>
> 参数：radius，类型：float
>
> 返回值：float
## Vertex1属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## ShapeType属性

?> 说明：返回作为shape常量之一的形状类型。
>
> 返回值：java.lang.Object
## SHAPE_CIRCLE字段
>
> 返回值：java.lang.Object
## SHAPE_CHAIN字段
>
> 返回值：java.lang.Object
## SHAPE_EDGE字段
>
> 返回值：java.lang.Object
## SHAPE_POLYGON字段
>
> 返回值：java.lang.Object

# B2ChainShape
完整类名：anywheresoftware.b4a.objects.B2Shape.B2ChainShape
> 所有者：process

> 包装器：org.jbox2d.collision.shapes.ChainShape

?> 说明：链形是线段的自由形式序列。链条有双边碰撞，所以你
## GetEdge方法
**GetEdge(Index,OutShape)**

?> 说明：将边复制到OutShape。
>
> 参数：Index，类型：int
>
> 参数：OutShape，类型：anywheresoftware.b4a.objects.B2Shape.B2EdgeShape
>
> 返回值：void
## ComputeAABB方法
**ComputeAABB(Output,Transform)**

?> 说明：基于传递的变换计算形状AABB。结果存储在Output对象中。
>
> 参数：Output，类型：anywheresoftware.b4a.objects.B2AABB
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 返回值：void
## CreateLoop方法
**CreateLoop(Vertices)**

?> 说明：创建一个循环。这会自动调整连接。
>
> 参数：Vertices，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## CreateChain方法
**CreateChain(Vertices)**

?> 说明：创建具有孤立端点的链。
>
> 参数：Vertices，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize()**
>
> 返回值：void
## TestPoint方法
**TestPoint(Transform,Point)**

?> 说明：测试此形状中的某个点是否包含。这只适用于凸面形状。
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 参数：Point，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：boolean
## Radius属性

?> 说明：获取或设置基础形状的半径。根据
>
> 参数：radius，类型：float
>
> 返回值：float
## EdgeCount属性

?> 说明：返回边的数目。
>
> 返回值：int
## ShapeType属性

?> 说明：返回作为shape常量之一的形状类型。
>
> 返回值：java.lang.Object
## SHAPE_CIRCLE字段
>
> 返回值：java.lang.Object
## SHAPE_CHAIN字段
>
> 返回值：java.lang.Object
## SHAPE_EDGE字段
>
> 返回值：java.lang.Object
## SHAPE_POLYGON字段
>
> 返回值：java.lang.Object

# B2PolygonShape
完整类名：anywheresoftware.b4a.objects.B2Shape.B2PolygonShape
> 所有者：process

> 包装器：org.jbox2d.collision.shapes.PolygonShape

?> 说明：一种凸多边形。多边形的最大顶点数等于8。
## SetAsBox2方法
**SetAsBox2(HalfWidth,HalfHeight,Center,Angle)**

?> 说明：创建长方体多边形。
>
> 参数：HalfWidth，类型：float
>
> 参数：HalfHeight，类型：float
>
> 参数：Center，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：Angle，类型：float
>
> 返回值：void
## Set方法
**Set(B2Vecs)**

?> 说明：创建凸多边形。最大顶点数为8。
>
> 参数：B2Vecs，类型：anywheresoftware.b4a.objects.collections.List
>
> 返回值：void
## SetAsBox方法
**SetAsBox(HalfWidth,HalfHeight)**

?> 说明：创建长方体多边形。
>
> 参数：HalfWidth，类型：float
>
> 参数：HalfHeight，类型：float
>
> 返回值：void
## ComputeAABB方法
**ComputeAABB(Output,Transform)**

?> 说明：基于传递的变换计算形状AABB。结果存储在Output对象中。
>
> 参数：Output，类型：anywheresoftware.b4a.objects.B2AABB
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize()**
>
> 返回值：void
## GetVertex方法
**GetVertex(Index)**

?> 说明：获取给定索引处的顶点。
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## TestPoint方法
**TestPoint(Transform,Point)**

?> 说明：测试此形状中的某个点是否包含。这只适用于凸面形状。
>
> 参数：Transform，类型：anywheresoftware.b4a.objects.B2Transform
>
> 参数：Point，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：boolean
## Radius属性

?> 说明：获取或设置基础形状的半径。根据
>
> 参数：radius，类型：float
>
> 返回值：float
## VertexCount属性

?> 说明：返回顶点的数目。
>
> 返回值：int
## ShapeType属性

?> 说明：返回作为shape常量之一的形状类型。
>
> 返回值：java.lang.Object
## SHAPE_CIRCLE字段
>
> 返回值：java.lang.Object
## SHAPE_CHAIN字段
>
> 返回值：java.lang.Object
## SHAPE_EDGE字段
>
> 返回值：java.lang.Object
## SHAPE_POLYGON字段
>
> 返回值：java.lang.Object

# B2Fixture
完整类名：anywheresoftware.b4a.objects.B2Fixture
> 所有者：process
## NextFixture方法
**NextFixture()**

?> 说明：返回下一个固定装置。如果这是最后一个固定装置，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.B2Fixture
## SetFilterBits方法
**SetFilterBits(CategoryBits,MaskBits)**

?> 说明：限制为低16位。
>
> 参数：CategoryBits，类型：int
>
> 参数：MaskBits，类型：int
>
> 返回值：void
## Restitution属性

?> 说明：恢复（弹性）通常在[0,1]的范围内。
>
> 参数：f，类型：float
>
> 返回值：float
## Shape属性

?> 说明：获取儿童形状。您可以修改子图形，但不应更改数字
>
> 返回值：anywheresoftware.b4a.objects.B2Shape.ConcreteB2Shape
## IsSensor属性

?> 说明：传感器形状收集接触信息，但从不产生碰撞响应。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## Friction属性

?> 说明：摩擦系数，通常在[0,1]的范围内。
>
> 参数：f，类型：float
>
> 返回值：float
## IsInitialized属性
>
> 返回值：boolean
## Body属性

?> 说明：获取此固定装置所连接的实体。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## Density属性

?> 说明：密度，通常以kg/m^2为单位
>
> 参数：f，类型：float
>
> 返回值：float
## Tag字段
>
> 返回值：java.lang.Object

# B2FixtureDef
完整类名：anywheresoftware.b4a.objects.B2Fixture.B2FixtureDef
> 所有者：process
## SetFilterBits方法
**SetFilterBits(CategoryBits,MaskBits)**

?> 说明：限制为低16位。
>
> 参数：CategoryBits，类型：int
>
> 参数：MaskBits，类型：int
>
> 返回值：void
## Restitution属性

?> 说明：恢复（弹性）通常在[0,1]的范围内。
>
> 参数：f，类型：float
>
> 返回值：float
## Shape属性

?> 说明：形状，这必须设置。创建设备时将克隆造型。
>
> 参数：Shape，类型：org.jbox2d.collision.shapes.Shape
>
> 返回值：anywheresoftware.b4a.objects.B2Shape.ConcreteB2Shape
## IsSensor属性

?> 说明：传感器形状收集接触信息，但从不产生碰撞响应。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## Friction属性

?> 说明：摩擦系数，通常在[0,1]的范围内。
>
> 参数：f，类型：float
>
> 返回值：float
## Density属性

?> 说明：密度，通常以kg/m^2为单位
>
> 参数：f，类型：float
>
> 返回值：float

# B2Contact
完整类名：anywheresoftware.b4a.objects.B2Contact
> 所有者：process

?> 说明：两个身体之间的接触。请注意，只要主体AABB重叠，就会创建一个接触。
## NextContact方法
**NextContact()**

?> 说明：返回下一个联系人，如果没有，则返回Null。应仅用于通过World.FirstContact访问的联系人。
>
> 返回值：anywheresoftware.b4a.objects.B2Contact
## GetWorldManifold方法
**GetWorldManifold(OutManifold)**

?> 说明：获取世界流形。
>
> 参数：OutManifold，类型：anywheresoftware.b4a.objects.B2WorldManifold
>
> 返回值：void
## GetManifold方法
**GetManifold()**

?> 说明：获取接触歧管。
>
> 返回值：anywheresoftware.b4a.objects.B2WorldManifold.B2Manifold
## IsEnabled属性

?> 说明：启用/禁用此联系人。这可以在预解决联系人侦听器中使用。这个
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## FixtureB属性

?> 说明：返回第二个固定装置。
>
> 返回值：anywheresoftware.b4a.objects.B2Fixture
## FixtureA属性

?> 说明：返回第一个固定装置。请注意，固定装置的顺序不一致。
>
> 返回值：anywheresoftware.b4a.objects.B2Fixture
## IsTouching属性

?> 说明：如果两个实体实际接触，则返回true。
>
> 返回值：boolean

# B2Body
完整类名：anywheresoftware.b4a.objects.B2Body
> 所有者：process
## SetTransform方法
**SetTransform(Position,Angle)**

?> 说明：设置实体原点和旋转的位置。这会断开所有联系人并唤醒
>
> 参数：Position，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：Angle，类型：float
>
> 返回值：void
## GetLocalVector方法
**GetLocalVector(WorldVector)**

?> 说明：获取给定世界向量的局部向量。
>
> 参数：WorldVector，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## GetContactList方法
**GetContactList(TouchingOnly)**

?> 说明：返回包含正文联系人的列表。
>
> 参数：TouchingOnly，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.collections.List
## GetWorldPoint方法
**GetWorldPoint(LocalPoint)**

?> 说明：在给定局部坐标的情况下，获取一个点的世界坐标。
>
> 参数：LocalPoint，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## GetLocalPoint方法
**GetLocalPoint(WorldPoint)**

?> 说明：在给定世界点的情况下，获取相对于身体原点的局部点。
>
> 参数：WorldPoint，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## ApplyTorque方法
**ApplyTorque(Torque)**

?> 说明：施加扭矩。这会影响角速度，而不会影响
>
> 参数：Torque，类型：float
>
> 返回值：void
## DestroyFixture方法
**DestroyFixture(Fixture)**

?> 说明：销毁固定装置。这将夹具从宽相位移除，并破坏所有触点
>
> 参数：Fixture，类型：anywheresoftware.b4a.objects.B2Fixture
>
> 返回值：void
## CreateFixture2方法
**CreateFixture2(Shape,Density)**

?> 说明：从造型创建固定装置并将其附着到此实体。这是一个方便功能。使用
>
> 参数：Shape，类型：org.jbox2d.collision.shapes.Shape
>
> 参数：Density，类型：float
>
> 返回值：anywheresoftware.b4a.objects.B2Fixture
## ApplyLinearImpulse方法
**ApplyLinearImpulse(Impulse,Point)**

?> 说明：在一点上施加脉冲。这会立即修改速度。它还修改了
>
> 参数：Impulse，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：Point，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## CreateFixture方法
**CreateFixture(FixtureDef)**

?> 说明：创建固定装置并将其附着到此实体。如果您需要设置一些固定装置，请使用此功能
>
> 参数：FixtureDef，类型：anywheresoftware.b4a.objects.B2Fixture.B2FixtureDef
>
> 返回值：anywheresoftware.b4a.objects.B2Fixture
## ApplyForceToCenter方法
**ApplyForceToCenter(Force)**

?> 说明：对重心施加一个力，这会唤醒身体。
>
> 参数：Force，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## GetWorldVector方法
**GetWorldVector(LocalVector)**

?> 说明：在给定局部坐标的情况下，获取向量的世界坐标。
>
> 参数：LocalVector，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## ApplyAngularImpulse方法
**ApplyAngularImpulse(Impulse)**

?> 说明：施加角度脉冲。
>
> 参数：Impulse，类型：float
>
> 返回值：void
## ApplyForce方法
**ApplyForce(Force,Point)**

?> 说明：在世界点上施加力。如果力没有施加在质心上
>
> 参数：Force，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：Point，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## LinearVelocity属性

?> 说明：获取或设置质心的线速度。不要修改返回的矢量。
>
> 参数：vec，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## Bullet属性
>
> 参数：b，类型：boolean
>
> 返回值：
## Position属性

?> 说明：获取世界身体原点位置。请勿修改。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## IsBullet属性

?> 说明：这具尸体是否被当作子弹进行连续碰撞检测？
>
> 返回值：boolean
## LinearDamping属性

?> 说明：获取或设置身体的线性阻尼。
>
> 参数：f，类型：float
>
> 返回值：float
## IsInitialized属性
>
> 返回值：boolean
## BodyType属性

?> 说明：获取或设置正文类型。
>
> 参数：o，类型：java.lang.Object
>
> 返回值：java.lang.Object
## SleepingAllowed属性

?> 说明：获取或设置是否允许睡眠。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## AngularDamping属性

?> 说明：获取或设置身体的角度阻尼。
>
> 参数：f，类型：float
>
> 返回值：float
## Awake属性

?> 说明：获取或设置此身体的睡眠状态。睡眠身体的CPU成本非常低。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## Mass属性

?> 说明：求出身体的总质量。通常以千克为单位。
>
> 返回值：float
## IsColliding属性

?> 说明：如果联系人列表不为空，则返回true。请注意，该列表包括非接触式联系人。
>
> 返回值：boolean
## Angle属性

?> 说明：以弧度为单位获取角度。
>
> 返回值：float
## FirstFixture属性

?> 说明：返回第一个固定装置。
>
> 返回值：anywheresoftware.b4a.objects.B2Fixture
## WorldCenter属性

?> 说明：获取质心的世界位置。不要修改。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## GravityScale属性

?> 说明：获取或设置重力刻度。
>
> 参数：f，类型：float
>
> 返回值：float
## Inertia属性

?> 说明：求出物体的中心转动惯量。通常以kg-m^2为单位
>
> 返回值：float
## AngularVelocity属性

?> 说明：获取或设置角速度。以弧度/秒为单位测量。
>
> 参数：f，类型：float
>
> 返回值：float
## Tag属性
>
> 参数：o，类型：java.lang.Object
>
> 返回值：java.lang.Object
## Transform属性

?> 说明：获取正文转换。
>
> 返回值：anywheresoftware.b4a.objects.B2Transform
## LocalCenter属性

?> 说明：获取质心的局部位置。不要修改。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## FixedRotation属性

?> 说明：获取或设置此实体是否具有固定旋转。设置会使质量重置。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## TYPE_STATIC字段
>
> 返回值：java.lang.Object
## TYPE_DYNAMIC字段
>
> 返回值：java.lang.Object
## TYPE_KINEMATIC字段
>
> 返回值：java.lang.Object

# B2BodyDef
完整类名：anywheresoftware.b4a.objects.B2Body.B2BodyDef
> 所有者：process
## LinearVelocity属性

?> 说明：物体在世界坐标系中的线速度。
>
> 参数：b，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## Bullet属性

?> 说明：这是一个快速移动的物体吗？应该防止它穿过其他移动的物体？
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## AllowSleep属性

?> 说明：如果这个身体永远不应该睡着，请将此标志设置为false。请注意，这会增加CPU
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## Position属性

?> 说明：身体的世界位置。避免在原点创建实体，因为这可能会导致许多
>
> 参数：b，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## LinearDamping属性

?> 说明：线性阻尼用于降低线性速度。阻尼参数可以大于
>
> 参数：f，类型：float
>
> 返回值：float
## BodyType属性

?> 说明：获取或设置身体类型。
>
> 参数：o，类型：java.lang.Object
>
> 返回值：java.lang.Object
## AngularDamping属性

?> 说明：角阻尼用于降低角速度。阻尼参数可以大于
>
> 参数：f，类型：float
>
> 返回值：float
## Awake属性

?> 说明：这具尸体最初是在睡觉吗？
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## Active属性

?> 说明：这个身体开始活跃吗？
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## Angle属性

?> 说明：身体的世界角度（以弧度为单位）。
>
> 参数：a，类型：float
>
> 返回值：float
## GravityScale属性

?> 说明：实验：缩放惯性张量。
>
> 参数：f，类型：float
>
> 返回值：float
## AngularVelocity属性

?> 说明：物体的角速度。
>
> 参数：f，类型：float
>
> 返回值：float
## FixedRotation属性

?> 说明：应该防止这个物体旋转吗？对字符有用。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## TYPE_STATIC字段
>
> 返回值：java.lang.Object
## TYPE_DYNAMIC字段
>
> 返回值：java.lang.Object
## TYPE_KINEMATIC字段
>
> 返回值：java.lang.Object

# B2AABB
完整类名：anywheresoftware.b4a.objects.B2AABB
> 所有者：process
## TestOverlap方法
**TestOverlap(Other)**

?> 说明：如果此AABB与其他AABB重叠，则返回true。
>
> 参数：Other，类型：anywheresoftware.b4a.objects.B2AABB
>
> 返回值：boolean
## Initialize2方法
**Initialize2(BottomLeft,TopRight)**
>
> 参数：BottomLeft，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：TopRight，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## Combine方法
**Combine(Other)**

?> 说明：将此AABB与其他AABB合并。
>
> 参数：Other，类型：anywheresoftware.b4a.objects.B2AABB
>
> 返回值：void
## Contains方法
**Contains(Other)**

?> 说明：如果此AABB包含其他AABB，则返回true。
>
> 参数：Other，类型：anywheresoftware.b4a.objects.B2AABB
>
> 返回值：boolean
## Initialize方法
**Initialize()**
>
> 返回值：void
## Center属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## BottomLeft属性

?> 说明：返回左下角的点。您可以修改它。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## Height属性
>
> 返回值：float
## TopRight属性

?> 说明：返回右上角的点。您可以修改它。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## Width属性
>
> 返回值：float

# B2WheelJoint
完整类名：anywheresoftware.b4a.objects.joints.B2WheelJoint
> 所有者：process

?> 说明：车轮接合处定义。这需要使用轴和锚来定义运动线
## NextJoint方法
**NextJoint()**

?> 说明：返回下一个关节。如果这是最后一个关节，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## AnchorA属性

?> 说明：获取BodyA在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## DampingRatio属性
>
> 参数：f，类型：float
>
> 返回值：float
## AnchorB属性

?> 说明：获取BodyB在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## LocalAnchorA属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## LocalAnchorB属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## IsInitialized属性
>
> 返回值：boolean
## MaxMotorTorque属性

?> 说明：获取或设置最大电机扭矩，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float
## MotorEnabled属性

?> 说明：获取或设置是否启用电机。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## JointSpeed属性

?> 说明：获取当前关节速度（以弧度每秒为单位）。
>
> 返回值：float
## JointType属性
>
> 返回值：java.lang.Object
## MotorSpeed属性

?> 说明：获取或设置以弧度每秒为单位的电机速度。
>
> 参数：f，类型：float
>
> 返回值：float
## FrequencyHz属性
>
> 参数：f，类型：float
>
> 返回值：float
## JOINT_GEAR字段
>
> 返回值：java.lang.Object
## JOINT_ROPE字段
>
> 返回值：java.lang.Object
## JOINT_UNKNOWN字段
>
> 返回值：java.lang.Object
## JOINT_MOTOR字段
>
> 返回值：java.lang.Object
## JOINT_PULLEY字段
>
> 返回值：java.lang.Object
## JOINT_WELD字段
>
> 返回值：java.lang.Object
## JOINT_FRICTION字段
>
> 返回值：java.lang.Object
## JOINT_REVOLUTE字段
>
> 返回值：java.lang.Object
## JOINT_PRISMATIC字段
>
> 返回值：java.lang.Object
## Tag字段
>
> 返回值：java.lang.Object
## JOINT_DISTANCE字段
>
> 返回值：java.lang.Object
## JOINT_WHEEL字段
>
> 返回值：java.lang.Object
## JOINT_MOUSE字段
>
> 返回值：java.lang.Object

# B2WheelJointDef
完整类名：anywheresoftware.b4a.objects.joints.B2WheelJoint.B2WheelJointDef
> 所有者：process
## Initialize方法
**Initialize(BodyA,BodyB,AnchorPoint,Axis)**

?> 说明：基于当前位置设置实体和定位。
>
> 参数：BodyA，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：BodyB，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：AnchorPoint，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：Axis，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## DampingRatio属性

?> 说明：悬架阻尼比，1表示临界阻尼。
>
> 参数：f，类型：float
>
> 返回值：float
## MotorEnabled属性

?> 说明：获取或设置是否启用电机。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## CollideConnected属性

?> 说明：获取或设置附加的实体是否可以碰撞。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## MaxMotorTorque属性

?> 说明：获取或设置最大电机扭矩，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float
## MotorSpeed属性

?> 说明：获取或设置以弧度每秒为单位的电机速度。
>
> 参数：f，类型：float
>
> 返回值：float
## FrequencyHz属性

?> 说明：悬架频率为零表示没有悬架。
>
> 参数：f，类型：float
>
> 返回值：float

# B2WeldJoint
完整类名：anywheresoftware.b4a.objects.joints.B2WeldJoint
> 所有者：process

?> 说明：将两个物体严格连接在一起的关节。
## NextJoint方法
**NextJoint()**

?> 说明：返回下一个关节。如果这是最后一个关节，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## AnchorA属性

?> 说明：获取BodyA在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## AnchorB属性

?> 说明：获取BodyB在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## IsInitialized属性
>
> 返回值：boolean
## JointType属性
>
> 返回值：java.lang.Object
## JOINT_GEAR字段
>
> 返回值：java.lang.Object
## JOINT_ROPE字段
>
> 返回值：java.lang.Object
## JOINT_UNKNOWN字段
>
> 返回值：java.lang.Object
## JOINT_MOTOR字段
>
> 返回值：java.lang.Object
## JOINT_PULLEY字段
>
> 返回值：java.lang.Object
## JOINT_WELD字段
>
> 返回值：java.lang.Object
## JOINT_FRICTION字段
>
> 返回值：java.lang.Object
## JOINT_REVOLUTE字段
>
> 返回值：java.lang.Object
## JOINT_PRISMATIC字段
>
> 返回值：java.lang.Object
## Tag字段
>
> 返回值：java.lang.Object
## JOINT_DISTANCE字段
>
> 返回值：java.lang.Object
## JOINT_WHEEL字段
>
> 返回值：java.lang.Object
## JOINT_MOUSE字段
>
> 返回值：java.lang.Object

# B2WeldJointDef
完整类名：anywheresoftware.b4a.objects.joints.B2WeldJoint.B2WeldJointDef
> 所有者：process
## Initialize方法
**Initialize(BodyA,BodyB,AnchorPoint)**

?> 说明：基于当前位置设置实体和定位。
>
> 参数：BodyA，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：BodyB，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：AnchorPoint，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## CollideConnected属性

?> 说明：获取或设置附加的实体是否可以碰撞。
>
> 参数：b，类型：boolean
>
> 返回值：boolean

# B2RopeJoint
完整类名：anywheresoftware.b4a.objects.joints.B2RopeJoint
> 所有者：process

?> 说明：绳索连接强制两个实体上的两个点之间的最大距离。它没有其他
## NextJoint方法
**NextJoint()**

?> 说明：返回下一个关节。如果这是最后一个关节，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## AnchorA属性

?> 说明：获取BodyA在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## AnchorB属性

?> 说明：获取BodyB在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## IsInitialized属性
>
> 返回值：boolean
## MaxLength属性

?> 说明：获取或设置绳索的最大长度。
>
> 参数：f，类型：float
>
> 返回值：float
## JointType属性
>
> 返回值：java.lang.Object
## JOINT_GEAR字段
>
> 返回值：java.lang.Object
## JOINT_ROPE字段
>
> 返回值：java.lang.Object
## JOINT_UNKNOWN字段
>
> 返回值：java.lang.Object
## JOINT_MOTOR字段
>
> 返回值：java.lang.Object
## JOINT_PULLEY字段
>
> 返回值：java.lang.Object
## JOINT_WELD字段
>
> 返回值：java.lang.Object
## JOINT_FRICTION字段
>
> 返回值：java.lang.Object
## JOINT_REVOLUTE字段
>
> 返回值：java.lang.Object
## JOINT_PRISMATIC字段
>
> 返回值：java.lang.Object
## Tag字段
>
> 返回值：java.lang.Object
## JOINT_DISTANCE字段
>
> 返回值：java.lang.Object
## JOINT_WHEEL字段
>
> 返回值：java.lang.Object
## JOINT_MOUSE字段
>
> 返回值：java.lang.Object

# B2RopeJointDef
完整类名：anywheresoftware.b4a.objects.joints.B2RopeJoint.B2RopeJointDef
> 所有者：process
## Initialize方法
**Initialize(BodyA,BodyB,LocalPointA,LocalPointB,MaxLength)**

?> 说明：设置实体和局部连接点。
>
> 参数：BodyA，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：BodyB，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：LocalPointA，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：LocalPointB，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：MaxLength，类型：float
>
> 返回值：void
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## CollideConnected属性

?> 说明：获取或设置附加的实体是否可以碰撞。
>
> 参数：b，类型：boolean
>
> 返回值：boolean

# B2RevoluteJoint
完整类名：anywheresoftware.b4a.objects.joints.B2RevoluteJoint
> 所有者：process

?> 说明：旋转关节约束两个实体在自由旋转时共享一个公共点
## NextJoint方法
**NextJoint()**

?> 说明：返回下一个关节。如果这是最后一个关节，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## SetLimits方法
**SetLimits(LowerLimit,UpperLimit)**

?> 说明：设置以弧度为单位测量的下限和上限。
>
> 参数：LowerLimit，类型：float
>
> 参数：UpperLimit，类型：float
>
> 返回值：void
## JointAngle属性

?> 说明：获取当前关节角度（以弧度为单位）。
>
> 返回值：float
## AnchorA属性

?> 说明：获取BodyA在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## AnchorB属性

?> 说明：获取BodyB在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## LocalAnchorA属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## LocalAnchorB属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## IsInitialized属性
>
> 返回值：boolean
## MaxMotorTorque属性

?> 说明：获取或设置最大电机扭矩，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float
## UpperLimit属性

?> 说明：获取以弧度为单位的上限。
>
> 返回值：float
## MotorEnabled属性

?> 说明：获取或设置是否启用电机。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## LimitEnabled属性

?> 说明：获取或设置是否启用限制。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## LowerLimit属性

?> 说明：获取以弧度为单位的下限。
>
> 返回值：float
## JointSpeed属性

?> 说明：获取当前关节速度（以弧度每秒为单位）。
>
> 返回值：float
## JointType属性
>
> 返回值：java.lang.Object
## MotorSpeed属性

?> 说明：获取或设置以弧度每秒为单位的电机速度。
>
> 参数：f，类型：float
>
> 返回值：float
## JOINT_GEAR字段
>
> 返回值：java.lang.Object
## JOINT_ROPE字段
>
> 返回值：java.lang.Object
## JOINT_UNKNOWN字段
>
> 返回值：java.lang.Object
## JOINT_MOTOR字段
>
> 返回值：java.lang.Object
## JOINT_PULLEY字段
>
> 返回值：java.lang.Object
## JOINT_WELD字段
>
> 返回值：java.lang.Object
## JOINT_FRICTION字段
>
> 返回值：java.lang.Object
## JOINT_REVOLUTE字段
>
> 返回值：java.lang.Object
## JOINT_PRISMATIC字段
>
> 返回值：java.lang.Object
## Tag字段
>
> 返回值：java.lang.Object
## JOINT_DISTANCE字段
>
> 返回值：java.lang.Object
## JOINT_WHEEL字段
>
> 返回值：java.lang.Object
## JOINT_MOUSE字段
>
> 返回值：java.lang.Object

# B2RevoluteJointDef
完整类名：anywheresoftware.b4a.objects.joints.B2RevoluteJoint.B2RevoluteJointDef
> 所有者：process
## Initialize方法
**Initialize(BodyA,BodyB,AnchorPoint)**

?> 说明：基于当前位置设置实体和定位。
>
> 参数：BodyA，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：BodyB，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：AnchorPoint，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## SetLimits方法
**SetLimits(LowerLimit,UpperLimit)**

?> 说明：设置以弧度为单位测量的下限和上限。
>
> 参数：LowerLimit，类型：float
>
> 参数：UpperLimit，类型：float
>
> 返回值：void
## MotorEnabled属性

?> 说明：获取或设置是否启用电机。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## LimitEnabled属性

?> 说明：获取或设置是否启用限制。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## LowerLimit属性

?> 说明：获取以弧度为单位的下限。
>
> 返回值：float
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## CollideConnected属性

?> 说明：获取或设置附加的实体是否可以碰撞。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## MaxMotorTorque属性

?> 说明：获取或设置最大电机扭矩，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float
## UpperLimit属性

?> 说明：获取以弧度为单位的上限。
>
> 返回值：float
## MotorSpeed属性

?> 说明：获取或设置以弧度每秒为单位的电机速度。
>
> 参数：f，类型：float
>
> 返回值：float

# B2PrismaticJoint
完整类名：anywheresoftware.b4a.objects.joints.B2PrismaticJoint
> 所有者：process

?> 说明：棱柱形接头。该关节提供一个自由度：沿固定在中的轴平移
## NextJoint方法
**NextJoint()**

?> 说明：返回下一个关节。如果这是最后一个关节，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## SetLimits方法
**SetLimits(LowerLimit,UpperLimit)**

?> 说明：设置以米为单位测量的下限和上限。
>
> 参数：LowerLimit，类型：float
>
> 参数：UpperLimit，类型：float
>
> 返回值：void
## AnchorA属性

?> 说明：获取BodyA在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## JointTranslation属性

?> 说明：获取当前关节平移（以米为单位）。
>
> 返回值：float
## AnchorB属性

?> 说明：获取BodyB在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## LocalAnchorA属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## LocalAnchorB属性
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## IsInitialized属性
>
> 返回值：boolean
## UpperLimit属性

?> 说明：获取以米为单位的上限。
>
> 返回值：float
## MotorEnabled属性

?> 说明：获取或设置是否启用电机。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## LimitEnabled属性

?> 说明：获取或设置是否启用限制。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## MaxMotorForce属性

?> 说明：获取或设置最大马达力，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float
## LowerLimit属性

?> 说明：获取以米为单位的下限。
>
> 返回值：float
## JointSpeed属性

?> 说明：获取当前关节速度（以米每秒为单位）。
>
> 返回值：float
## JointType属性
>
> 返回值：java.lang.Object
## MotorSpeed属性

?> 说明：获取或设置电机速度（以米/秒为单位）。
>
> 参数：f，类型：float
>
> 返回值：float
## JOINT_GEAR字段
>
> 返回值：java.lang.Object
## JOINT_ROPE字段
>
> 返回值：java.lang.Object
## JOINT_UNKNOWN字段
>
> 返回值：java.lang.Object
## JOINT_MOTOR字段
>
> 返回值：java.lang.Object
## JOINT_PULLEY字段
>
> 返回值：java.lang.Object
## JOINT_WELD字段
>
> 返回值：java.lang.Object
## JOINT_FRICTION字段
>
> 返回值：java.lang.Object
## JOINT_REVOLUTE字段
>
> 返回值：java.lang.Object
## JOINT_PRISMATIC字段
>
> 返回值：java.lang.Object
## Tag字段
>
> 返回值：java.lang.Object
## JOINT_DISTANCE字段
>
> 返回值：java.lang.Object
## JOINT_WHEEL字段
>
> 返回值：java.lang.Object
## JOINT_MOUSE字段
>
> 返回值：java.lang.Object

# B2PrismaticJointDef
完整类名：anywheresoftware.b4a.objects.joints.B2PrismaticJoint.B2PrismaticJointDef
> 所有者：process
## Initialize方法
**Initialize(BodyA,BodyB,AnchorPoint,Axis)**

?> 说明：基于当前位置设置实体和定位。
>
> 参数：BodyA，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：BodyB，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：AnchorPoint，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：Axis，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## SetLimits方法
**SetLimits(LowerLimit,UpperLimit)**

?> 说明：设置以米为单位测量的下限和上限。
>
> 参数：LowerLimit，类型：float
>
> 参数：UpperLimit，类型：float
>
> 返回值：void
## MotorEnabled属性

?> 说明：获取或设置是否启用电机。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## LimitEnabled属性

?> 说明：获取或设置是否启用限制。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## MaxMotorForce属性

?> 说明：获取或设置最大马达力，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float
## LowerLimit属性

?> 说明：获取以米为单位的下限。
>
> 返回值：float
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## CollideConnected属性

?> 说明：获取或设置附加的实体是否可以碰撞。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## UpperLimit属性

?> 说明：获取以米为单位的上限。
>
> 返回值：float
## MotorSpeed属性

?> 说明：获取或设置以弧度每秒为单位的电机速度。
>
> 参数：f，类型：float
>
> 返回值：float

# B2MotorJoint
完整类名：anywheresoftware.b4a.objects.joints.B2MotorJoint
> 所有者：process

?> 说明：棱柱形接头。该关节提供一个自由度：沿固定在中的轴平移
## NextJoint方法
**NextJoint()**

?> 说明：返回下一个关节。如果这是最后一个关节，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## AnchorA属性

?> 说明：获取BodyA在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## AnchorB属性

?> 说明：获取BodyB在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## AngularOffset属性

?> 说明：获取或设置BodyB相对于BodyA的目标角度偏移量。
>
> 参数：f，类型：float
>
> 返回值：float
## LinearOffset属性

?> 说明：获取或设置BodyB相对于BodyA的目标线性偏移量。
>
> 参数：b，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## MaxMotorForce属性

?> 说明：获取或设置最大马达力，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float
## CorrectionFactor属性

?> 说明：获取或设置位置校正因子[0，1]。
>
> 参数：f，类型：float
>
> 返回值：float
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## IsInitialized属性
>
> 返回值：boolean
## JointType属性
>
> 返回值：java.lang.Object
## MaxMotorTorque属性

?> 说明：获取或设置最大电机扭矩，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float
## JOINT_GEAR字段
>
> 返回值：java.lang.Object
## JOINT_ROPE字段
>
> 返回值：java.lang.Object
## JOINT_UNKNOWN字段
>
> 返回值：java.lang.Object
## JOINT_MOTOR字段
>
> 返回值：java.lang.Object
## JOINT_PULLEY字段
>
> 返回值：java.lang.Object
## JOINT_WELD字段
>
> 返回值：java.lang.Object
## JOINT_FRICTION字段
>
> 返回值：java.lang.Object
## JOINT_REVOLUTE字段
>
> 返回值：java.lang.Object
## JOINT_PRISMATIC字段
>
> 返回值：java.lang.Object
## Tag字段
>
> 返回值：java.lang.Object
## JOINT_DISTANCE字段
>
> 返回值：java.lang.Object
## JOINT_WHEEL字段
>
> 返回值：java.lang.Object
## JOINT_MOUSE字段
>
> 返回值：java.lang.Object

# B2MotorJointDef
完整类名：anywheresoftware.b4a.objects.joints.B2MotorJoint.B2MotorJointDef
> 所有者：process
## Initialize方法
**Initialize(BodyA,BodyB)**

?> 说明：设置实体。身体B相对于身体A移动。
>
> 参数：BodyA，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：BodyB，类型：anywheresoftware.b4a.objects.B2Body
>
> 返回值：void
## AngularOffset属性

?> 说明：获取或设置BodyB相对于BodyA的角度偏移。
>
> 参数：f，类型：float
>
> 返回值：float
## LinearOffset属性

?> 说明：获取或设置BodyB相对于BodyA的线性偏移量。
>
> 参数：b，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## MaxMotorForce属性

?> 说明：获取或设置最大马达力，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float
## CorrectionFactor属性

?> 说明：获取或设置位置校正因子[0，1]。
>
> 参数：f，类型：float
>
> 返回值：float
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## CollideConnected属性

?> 说明：获取或设置附加的实体是否可以碰撞。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## MaxMotorTorque属性

?> 说明：获取或设置最大电机扭矩，通常以N/m为单位。
>
> 参数：f，类型：float
>
> 返回值：float

# B2Joint
完整类名：anywheresoftware.b4a.objects.joints.B2Joint
> 所有者：process
## NextJoint方法
**NextJoint()**

?> 说明：返回下一个关节。如果这是最后一个关节，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## AnchorA属性

?> 说明：获取BodyA在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## AnchorB属性

?> 说明：获取BodyB在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## IsInitialized属性
>
> 返回值：boolean
## JointType属性
>
> 返回值：java.lang.Object
## JOINT_GEAR字段
>
> 返回值：java.lang.Object
## JOINT_ROPE字段
>
> 返回值：java.lang.Object
## JOINT_UNKNOWN字段
>
> 返回值：java.lang.Object
## JOINT_MOTOR字段
>
> 返回值：java.lang.Object
## JOINT_PULLEY字段
>
> 返回值：java.lang.Object
## JOINT_WELD字段
>
> 返回值：java.lang.Object
## JOINT_FRICTION字段
>
> 返回值：java.lang.Object
## JOINT_REVOLUTE字段
>
> 返回值：java.lang.Object
## JOINT_PRISMATIC字段
>
> 返回值：java.lang.Object
## Tag字段
>
> 返回值：java.lang.Object
## JOINT_DISTANCE字段
>
> 返回值：java.lang.Object
## JOINT_WHEEL字段
>
> 返回值：java.lang.Object
## JOINT_MOUSE字段
>
> 返回值：java.lang.Object

# B2JointDef
完整类名：anywheresoftware.b4a.objects.joints.B2Joint.B2JointDef
> 所有者：process
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## CollideConnected属性

?> 说明：获取或设置附加的实体是否可以碰撞。
>
> 参数：b，类型：boolean
>
> 返回值：boolean

# B2DistanceJoint
完整类名：anywheresoftware.b4a.objects.joints.B2DistanceJoint
> 所有者：process

?> 说明：距离关节约束两个实体上的两个点，使其保持固定距离
## NextJoint方法
**NextJoint()**

?> 说明：返回下一个关节。如果这是最后一个关节，则返回Null。
>
> 返回值：anywheresoftware.b4a.objects.joints.B2Joint
## AnchorA属性

?> 说明：获取BodyA在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## DampingRatio属性
>
> 参数：f，类型：float
>
> 返回值：float
## AnchorB属性

?> 说明：获取BodyB在世界坐标中的锚点。
>
> 返回值：anywheresoftware.b4a.objects.B2Vec2
## Length属性
>
> 参数：f，类型：float
>
> 返回值：float
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## IsInitialized属性
>
> 返回值：boolean
## JointType属性
>
> 返回值：java.lang.Object
## FrequencyHz属性
>
> 参数：f，类型：float
>
> 返回值：float
## JOINT_GEAR字段
>
> 返回值：java.lang.Object
## JOINT_ROPE字段
>
> 返回值：java.lang.Object
## JOINT_UNKNOWN字段
>
> 返回值：java.lang.Object
## JOINT_MOTOR字段
>
> 返回值：java.lang.Object
## JOINT_PULLEY字段
>
> 返回值：java.lang.Object
## JOINT_WELD字段
>
> 返回值：java.lang.Object
## JOINT_FRICTION字段
>
> 返回值：java.lang.Object
## JOINT_REVOLUTE字段
>
> 返回值：java.lang.Object
## JOINT_PRISMATIC字段
>
> 返回值：java.lang.Object
## Tag字段
>
> 返回值：java.lang.Object
## JOINT_DISTANCE字段
>
> 返回值：java.lang.Object
## JOINT_WHEEL字段
>
> 返回值：java.lang.Object
## JOINT_MOUSE字段
>
> 返回值：java.lang.Object

# B2DistanceJointDef
完整类名：anywheresoftware.b4a.objects.joints.B2DistanceJoint.B2DistanceJointDef
> 所有者：process
## Initialize方法
**Initialize(BodyA,BodyB,WorldPointA,WorldPointB)**

?> 说明：设置实体和连接点。
>
> 参数：BodyA，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：BodyB，类型：anywheresoftware.b4a.objects.B2Body
>
> 参数：WorldPointA，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 参数：WorldPointB，类型：anywheresoftware.b4a.objects.B2Vec2
>
> 返回值：void
## DampingRatio属性

?> 说明：弹簧阻尼比，1表示临界阻尼。
>
> 参数：f，类型：float
>
> 返回值：float
## Length属性
>
> 参数：f，类型：float
>
> 返回值：float
## BodyB属性

?> 说明：获取第二个附加正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## BodyA属性

?> 说明：获取第一个附加的正文。
>
> 返回值：anywheresoftware.b4a.objects.B2Body
## CollideConnected属性

?> 说明：获取或设置附加的实体是否可以碰撞。
>
> 参数：b，类型：boolean
>
> 返回值：boolean
## FrequencyHz属性

?> 说明：弹簧频率为零表示无悬架。
>
> 参数：f，类型：float
>
> 返回值：float

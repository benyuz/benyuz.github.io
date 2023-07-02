# USB

版本:1.01
[BBS View](https://www.b4x.com/android/forum/pages/results/?query=USB)

# UsbManager
完整类名：anywheresoftware.b4a.objects.usb.UsbManagerWrapper
> 所有者：process

?> 说明：UsbManager允许访问连接的Usb设备。它还保存相关的常量。
## GetDevices方法
**GetDevices()**

?> 说明：返回UsbDevice的数组以及所有连接的USB设备。
>
> 返回值：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbDeviceWrapper[]
## HasPermission方法
**HasPermission(Device)**

?> 说明：测试您的应用程序是否具有访问此设备的权限。
>
> 参数：Device，类型：android.hardware.usb.UsbDevice
>
> 返回值：boolean
## OpenAccessory方法
**OpenAccessory(Accessory)**

?> 说明：连接到给定的附件
>
> 参数：Accessory，类型：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbAccessoryWrapper
>
> 返回值：void
## RequestPermission方法
**RequestPermission(Device)**

?> 说明：显示一个对话框，要求用户允许您的应用程序访问USB设备。
>
> 参数：Device，类型：android.hardware.usb.UsbDevice
>
> 返回值：void
## HasAccessoryPermission方法
**HasAccessoryPermission(Accessory)**

?> 说明：测试您的应用程序是否具有访问此附件的权限。
>
> 参数：Accessory，类型：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbAccessoryWrapper
>
> 返回值：boolean
## Initialize方法
**Initialize()**

?> 说明：初始化对象。
>
> 返回值：void
## GetAccessories方法
**GetAccessories()**

?> 说明：返回一个UsbAccessories数组以及所有连接的USB附件。
>
> 返回值：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbAccessoryWrapper[]
## OpenDevice方法
**OpenDevice(Device,Interface,ForceClaim)**

?> 说明：连接到给定的设备并声明对给定接口的独占访问权。
>
> 参数：Device，类型：android.hardware.usb.UsbDevice
>
> 参数：Interface，类型：android.hardware.usb.UsbInterface
>
> 参数：ForceClaim，类型：boolean
>
> 返回值：anywheresoftware.b4a.objects.usb.UsbDeviceConnectionWrapper
## RequestAccessoryPermission方法
**RequestAccessoryPermission(Accessory)**

?> 说明：显示一个对话框，要求用户允许您的应用程序访问USB附件。
>
> 参数：Accessory，类型：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbAccessoryWrapper
>
> 返回值：void
## USB_CLASS_PHYSICA字段
>
> 返回值：int
## USB_TYPE_CLASS字段
>
> 返回值：int
## USB_CLASS_MISC字段
>
> 返回值：int
## USB_CLASS_HID字段
>
> 返回值：int
## USB_CLASS_AUDIO字段
>
> 返回值：int
## USB_ENDPOINT_XFER_INT字段
>
> 返回值：int
## USB_CLASS_APP_SPEC字段
>
> 返回值：int
## USB_INTERFACE_SUBCLASS_BOOT字段
>
> 返回值：int
## USB_TYPE_RESERVED字段
>
> 返回值：int
## USB_ENDPOINT_XFER_CONTROL字段
>
> 返回值：int
## USB_CLASS_STILL_IMAGE字段
>
> 返回值：int
## USB_CLASS_WIRELESS_CONTROLLER字段
>
> 返回值：int
## USB_CLASS_CONTENT_SEC字段
>
> 返回值：int
## USB_TYPE_STANDARD字段
>
> 返回值：int
## USB_CLASS_MASS_STORAGE字段
>
> 返回值：int
## USB_DIR_OUT字段
>
> 返回值：int
## USB_ENDPOINT_NUMBER_MASK字段
>
> 返回值：int
## USB_ENDPOINT_DIR_MASK字段
>
> 返回值：int
## USB_TYPE_MASK字段
>
> 返回值：int
## USB_CLASS_PER_INTERFACE字段
>
> 返回值：int
## USB_SUBCLASS_VENDOR_SPEC字段
>
> 返回值：int
## USB_TYPE_VENDOR字段
>
> 返回值：int
## USB_ENDPOINT_XFERTYPE_MASK字段
>
> 返回值：int
## USB_CLASS_COMM字段
>
> 返回值：int
## USB_CLASS_VENDOR_SPEC字段
>
> 返回值：int
## USB_CLASS_CDC_DATA字段
>
> 返回值：int
## USB_ENDPOINT_XFER_ISOC字段
>
> 返回值：int
## USB_CLASS_CSCID字段
>
> 返回值：int
## USB_DIR_IN字段
>
> 返回值：int
## USB_CLASS_VIDEO字段
>
> 返回值：int
## USB_CLASS_PRINTER字段
>
> 返回值：int
## USB_ENDPOINT_XFER_BULK字段
>
> 返回值：int
## USB_CLASS_HUB字段
>
> 返回值：int

# UsbDevice
完整类名：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbDeviceWrapper
> 所有者：process

> 包装器：android.hardware.usb.UsbDevice

?> 说明：表示Usb设备。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## GetInterface方法
**GetInterface(Index)**

?> 说明：获取给定索引处的接口。
>
> 参数：Index，类型：int
>
> 返回值：android.hardware.usb.UsbInterface
## InterfaceCount属性

?> 说明：获取接口的数目。
>
> 返回值：int
## DeviceSubclass属性

?> 说明：获取设备子类。
>
> 返回值：int
## DeviceId属性

?> 说明：获取设备id。
>
> 返回值：int
## DeviceClass属性

?> 说明：获取设备类。
>
> 返回值：int
## VendorId属性

?> 说明：获取供应商id。
>
> 返回值：int
## ProductId属性

?> 说明：获取产品id。
>
> 返回值：int
## DeviceName属性

?> 说明：获取设备名称。
>
> 返回值：java.lang.String

# UsbInterface
完整类名：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbInterfaceWrapper
> 所有者：process

> 包装器：android.hardware.usb.UsbInterface

?> 说明：表示特定设备上的Usb接口。
## GetEndpoint方法
**GetEndpoint(Index)**

?> 说明：获取给定索引处的终结点。
>
> 参数：Index，类型：int
>
> 返回值：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbEndpointWrapper
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## EndpointCount属性

?> 说明：获取此接口中可用的终结点数。
>
> 返回值：int
## InterfaceSubclass属性

?> 说明：获取接口子类。
>
> 返回值：int
## InterfaceClass属性

?> 说明：获取接口类。
>
> 返回值：int
## InterfaceProtocol属性

?> 说明：获取接口协议。
>
> 返回值：int

# UsbEndpoint
完整类名：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbEndpointWrapper
> 所有者：process

> 包装器：android.hardware.usb.UsbEndpoint

?> 说明：表示特定接口中的终结点。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Type属性

?> 说明：获取终结点类型。
>
> 返回值：int
## Address属性

?> 说明：获取终结点地址。
>
> 返回值：int
## Attributes属性

?> 说明：获取端点属性。
>
> 返回值：int
## EndpointNumber属性

?> 说明：获取终结点编号。
>
> 返回值：int
## Direction属性

?> 说明：获取端点方向。可以是UsbManager.USB_DIR_IN或UsbManager.USB_DIR_OUT。
>
> 返回值：int
## MaxPacketSize属性

?> 说明：获取最大数据包大小。
>
> 返回值：int
## Interval属性

?> 说明：获取间隔字段。
>
> 返回值：int

# UsbAccessory
完整类名：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbAccessoryWrapper
> 所有者：process

?> 说明：表示Usb附件。
## Close方法
**Close()**

?> 说明：关闭附件。
>
> 返回值：void
## Serial属性

?> 说明：获取附件的唯一序列号。
>
> 返回值：java.lang.String
## Description属性

?> 说明：获取附件的描述。
>
> 返回值：java.lang.String
## Version属性

?> 说明：获取附件的版本。
>
> 返回值：java.lang.String
## InputStream属性

?> 说明：获取附件的输入流。
>
> 返回值：anywheresoftware.b4a.objects.streams.File.InputStreamWrapper
## OutputStream属性

?> 说明：获取附件的输出流。
>
> 返回值：anywheresoftware.b4a.objects.streams.File.OutputStreamWrapper
## Manufacturer属性

?> 说明：获取配件的制造商。
>
> 返回值：java.lang.String
## Model属性

?> 说明：获取配件的型号名称。
>
> 返回值：java.lang.String
## Uri属性

?> 说明：获取附件的网站的URI。
>
> 返回值：java.lang.String

# UsbDeviceConnection
完整类名：anywheresoftware.b4a.objects.usb.UsbDeviceConnectionWrapper
> 所有者：process

?> 说明：表示主机和客户端之间的连接。
> 事件：
>
> NewData (Request As UsbRequest, InDirection As Boolean)
## CloseSynchronous方法
**CloseSynchronous()**

?> 说明：关闭连接。StopListening也会关闭连接。
>
> 返回值：void
## BulkTransfer方法
**BulkTransfer(Endpoint,Buffer,Length,Timeout)**

?> 说明：发送同步请求。
>
> 参数：Endpoint，类型：android.hardware.usb.UsbEndpoint
>
> 参数：Buffer，类型：byte[]
>
> 参数：Length，类型：int
>
> 参数：Timeout，类型：int
>
> 返回值：int
## StartListening方法
**StartListening(ba,EventName)**

?> 说明：开始侦听已完成的请求。当这些可用时，将引发NewData事件。
>
> 参数：ba，类型：anywheresoftware.b4a.BA
>
> 参数：EventName，类型：java.lang.String
>
> 返回值：void
## StopListening方法
**StopListening()**

?> 说明：停止侦听请求并关闭连接。
>
> 返回值：void
## GetRawDescriptors方法
**GetRawDescriptors()**

?> 说明：以字节数组的形式返回原始描述符。
>
> 返回值：byte[]
## IsInitialized方法
**IsInitialized()**

?> 说明：测试对象是否已初始化。
>
> 返回值：boolean
## ControlTransfer方法
**ControlTransfer(RequestType,Request,Value,Index,Buffer,Length,Timeout)**

?> 说明：对终结点0执行控制事务。返回传输的字节数。
>
> 参数：RequestType，类型：int
>
> 参数：Request，类型：int
>
> 参数：Value，类型：int
>
> 参数：Index，类型：int
>
> 参数：Buffer，类型：byte[]
>
> 参数：Length，类型：int
>
> 参数：Timeout，类型：int
>
> 返回值：int
## ContinueListening方法
**ContinueListening()**

?> 说明：通知侦听器继续侦听已完成的请求。
>
> 返回值：void
## Serial属性

?> 说明：返回连接的设备序列号。
>
> 返回值：java.lang.String

# UsbRequest
完整类名：anywheresoftware.b4a.objects.usb.UsbDeviceConnectionWrapper.UsbRequestWrapper
> 所有者：process

> 包装器：android.hardware.usb.UsbRequest

?> 说明：此对象表示USB请求数据包。
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(Connection,Endpoint)**

?> 说明：初始化请求。该请求将绑定到给定的连接和端点。
>
> 参数：Connection，类型：anywheresoftware.b4a.objects.usb.UsbDeviceConnectionWrapper
>
> 参数：Endpoint，类型：android.hardware.usb.UsbEndpoint
>
> 返回值：void
## Queue方法
**Queue(Buffer,Length)**

?> 说明：对发送请求进行排队。事务完成时将引发UsbDeviceConnection_NewData事件。
>
> 参数：Buffer，类型：byte[]
>
> 参数：Length，类型：int
>
> 返回值：void
## Buffer属性

?> 说明：返回与请求关联的缓冲区。
>
> 返回值：byte[]
## UsbEndpoint属性
>
> 返回值：anywheresoftware.b4a.objects.usb.UsbManagerWrapper.UsbEndpointWrapper
## Name属性

?> 说明：获取或设置可用于标识请求的任意字符串。
>
> 参数：n，类型：java.lang.String
>
> 返回值：java.lang.String

# MtpDevice
完整类名：anywheresoftware.b4a.objects.usb.MtpDeviceWrapper
> 所有者：process

> 包装器：android.mtp.MtpDevice
## Close方法
**Close()**
>
> 返回值：void
## IsInitialized方法
**IsInitialized()**
>
> 返回值：boolean
## Initialize方法
**Initialize(EventName,UsbDevice)**
>
> 参数：EventName，类型：java.lang.String
>
> 参数：UsbDevice，类型：android.hardware.usb.UsbDevice
>
> 返回值：void
## Open方法
**Open(Connection)**
>
> 参数：Connection，类型：anywheresoftware.b4a.objects.usb.UsbDeviceConnectionWrapper
>
> 返回值：void

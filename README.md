# work_2
<img width="600" alt="图片 4" src="https://github.com/nieting1997/work_2/assets/90097659/5c3b2bfd-7a60-4078-9b54-0116c9490908">

* 项目场景：
  * 云连接将客户的线上资源和线下IDC机房连接起来。 
  * 但客户线下IDC机房想要直接互通，产品缺乏该支持。
  * 该项目将专线接入的IDC机房之间相联，解决客户问题。  
* 备注：
  * 此处路由器可以理解为work 1的agent(np网关)。
  * DGW可以理解为虚拟网关。
 
* 本人负责工作：
  * 使用api-first原则，先对业务建模，定义对应api。
<img width="500" alt="图片 4" src="https://github.com/nieting1997/work_2/assets/90097659/6a1f6964-0684-4707-aa81-784878f883a1">

  * 使用公司框架生成相对应的类与server/client。
  * 使用java开发业务代码。其中，java使用spring-boot框架+reactor-core编程模型。
      * 以创建为例。
        * 创建一个分支网络
        * 创建P2P分支连接信息(一期只支持P2P)
        * 为分支网络分配VNI(租户隔离)
        * 为VTEP分配IP地址
        * 创建一条vxlan隧道
<img width="400" alt="图片 4" src=https://github.com/nieting1997/work_2/assets/90097659/57036188-cb75-406e-bca8-049e7d3d1022>


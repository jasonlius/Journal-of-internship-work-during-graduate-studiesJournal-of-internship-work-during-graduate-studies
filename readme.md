# 读研期间实习工作记录
**花有重开日，人无再少年。**  
  
![追逐](https://i1.nichengzhan.com/eec27964b3e4a90db27efe5f/ecdd/ab9d313deb/a8983337ecb4fc40e824a109bc993b556a.jpg)
## 2022年5月16日  
  
计划解决的问题：上位机GATT服务关闭后，GATT服务重连异常的问题，排除故障并且解决.
  
解决情况：对于Ble设备能够关闭GATT服务并且重连，对于经典蓝牙设备无法断开GATT服务。
  
## 2022年5月17-18日
计划解决的问题：学习blufi数据传输协议以及blufi的数据帧格式，手机app能够传输正确的数据帧并对esp32进行wifi网络配置。  
解决情况：已经解决！在esp官方的例程中，在数据帧上加入日志，利用官方的APP发送数据帧，然后查看运行日志，就能准确的知道每一个数据帧执行什么功能。
## 2022年5月19日
计划解决的问题：熟悉基本的网络通信Socket编程，学习利用UDP与TCP协议传输数据。  
完成情况：在学习了基本的socket编程之后，自己独立编写了一个基于TCP/IP协议的socket客户机，程序运行遇到了BUG 无法与serve建立连接。
## 2022年5月20日
计划解决的问题：  
1.在基于昨天的socket编程的基础上，解决本次socket客户机无法与server建立连接的问题；  
2.自己独立编写基于TCP/IP协议的Socket的server，要求能够实现收发功能。  
3.如果以上问题顺利解决，将TCP协议转换成UDP协议进行通信编程。  
完成情况：任务1的问题已经解决，任务2也已经解决,任务3基于udp的listener不知道如何开发，下周一解决。  
## 2022年5月23日
计划解决的问题:解决不知道用UDP协议实现server的功能。  
任务完成情况：计划已改变，使用BLEmesh组网控制灯带，昨日主要在其他人的协助下，对BLe mesh协议进行分析
## 2022年5月24日
计划解决的问题：BleMesh底层的数据接收的协议的找出，在我的上位机上传送对应的数据。  
任务完成的情况：blemesh的profile太复杂了，正在努力想办法！！！
## 2022年5月26日
计划解决的问题：同样的问题，如何在我的app中传输数据。  
任务完成的情况：实在是不会请教了朱总，提出利用xamarin中的Binding a Java Library功能，将android的blemesh库翻译成C#mesh库，参考了微软的官方文档，发现拓展名为.jar的BleMesh包无法翻译成c#，于是改用拓展名为.aar的ble Mesh包，发现该方法可行，发现11个报错，解决掉错误，生成了 一个拓展名为.dll的C#类库。至此我们获得了一个基于xamarin.andriod框架的C#BleMesh类库。
## 2022年5月27日
计划解决的问题：在昨天生成的C#Blemesh类库的基础上，要解决如何将xamarin.android框架的C#类库在xamarin.forms跨平台上使用。  
任务完成情况：请教了大佬，提出现在目前要搞清xamarin.andriod上的工作原理，所以昨天的工作主要学习了一下xamarin.andriod的入门app。
## 2022年5月28日
计划解决的问题，在xamarin.andriod上调用之前的类库争取能够实现 一个小功能。  
问题解决情况：说实话，我目前对安卓一窍不通😂，在YouTube上找了一个android的学习视频，了解了一下安卓的基本文件结构。然后使用了dependency injection technique 使得xamarin.forms能够借用xamarin.andriod的library.
## 2022年5月30日
计划解决的问题，当下能在xamarin.forms中使用BLE MESH binding library,当下的主要问题在于找出来示例项目的API，然后使APP能够实现对MESH节点的扫描这一个小功能。  
问题解决情况：正在全力分析已有的代码ing.......
## 2022年5月31日
计划解决的问题：使APP能够实现对MESH节点的扫描这一个小功能。  
问题解决情况：正在全力分析已有的代码ing....... ,太难了，搞不出，想放弃了!
## 2022年6月1日(儿童节)
计划解决的问题:我怀疑这个问题我还能不能解决。  
问题解决情况：正所谓穷则独善其身，我先去充充电再来，今天的退后是为了明天更好的前进。
## 2022年6月2日
计划解决的问题:重新学习Ble.net.sampleApp.要做到把APP的每一个文件夹的每一个文件的每一句代码都能看懂。加油肝！加油肝!  
问题解决情况:肝微软xamarin.forms官方文档. 冲他妈的！
## 2022年6月5日
计划解决的问题：项目真的好难啊，真的好难啊！我此刻代码的海洋里面遨游，前方突然遇到了一个巨大的漩涡，漩涡已经把我卷了进去，我用尽全力苦苦挣扎着，我知道漩涡不会散去，我只能拼命挣扎，直到我能游出这个漩涡。  
问题解决情况:水了一天，又困又倦，可能确实是有点疲倦了，或许是失掉自信心开始摆烂了，进展是不可能有的。
## 2022年6月6日
计划解决的问题：调整状态，防止摆烂！
## 2022年6月7日
忘记干啥了！！！
## 2022年6月8日
找了一天的东西，找到了蓝牙技术联盟的上位机开发文档。我重新看见了希望的光！！！！！
## 2022年6月9日
学习了blemesh上位机开发文档的理论部分。u1s1这东西真TMD难！！
## 2022年6月10日
开始学习BLemesh代码开发部分，不管了先把技术联盟文档先走一遍！
## 2022年6月13日
蓝牙技术联盟mesh开发文档，在一定程度上是正确的道路，但需要花些时间消化，今天先把后续的hand—code lab 部分代码复刻出来，再来解决原理的问题。
## 2022年6月14日
复刻了蓝牙mesh中code—lab后续的代码
## 2022年6月15日
将文档中第三部分的动手实验全部完成了，并且阅读了第四部的的开发范例
## 2022年6月16日
重新回顾了开发手册的第一部分的理论部分，继续加强蓝牙mesh代理协议跟加深层次的理解。争取明天将开发文档的逻辑代码写成c#。
## 2022年6月17日
今天的主要任务再次重新阅读开发文档第三部分的mesh proxy code-Lab中的代码，将JS的后端代码逻辑，用C#代码实现。  
任务主要分为两步走：  
1.实现mesh proxy protocol中的mesh PDUs加密部分的代码,首先基于AES_CMAC算法，实现加密需要用到的K2，K3，K4密钥生成方法，其次后续需要利用AES_CCM加密算法以及AES_EBC加密算法实现Mesh Pdu对应层的数据加密。  
2.第二步是建立在第一部分的加密功能完整无误的情况下，根据蓝牙Mesh PDUs的组成特点将各个层的发送的PDUs组装成一个完整的Mesh proxy PDUs，然后通过手机发送给树莓派下位机。 
任务完成情况：在对照JS范例程序，已经用c#写好了K1密钥生成方法，在下周的工作中需要对已经写好的K1密钥生成方法进行测试。  
（ps：加密算法的库使用开源的BouncyCastle）
## 2022年6月20日
今天的工作任务：对已经写好的K1密钥生成方法进行测试，具体的测试内容有如下几个，第一是AES_CAMC算法的加密测试，主要检测AES_CMAC加密算法是否正确,以及K1密钥能否生成对应encryption key，privacy Key以及NID。  
任务完成情况：经过调试，密钥能够完全生成，密码长度无误。算法无误。明天继续整K3，k4密钥生成函数。

## 2022年6月21日
今天的工作任务:写出K3密钥生成函数，测试写出的K3密钥 生成函数，如果顺利完成，继续写往下进行。  
任务完成情况:k3密钥生成函数顺利写出，在测试的时候发现与Java的k3函数运行的结果不一样，经过层层调试发现了2处问题：  
problem1：在调用完AES_CMAC算法后，原来传进来的参数发生被算法的值改变了，影响到了原来的变量。  
problem2:c# 高精度类型BIginteger将16进制数据转化为10进制时，他的转化会将一个16进制的正数，转化为10进制的负数，导致最后的结果出错。  
## 2022年6月22日
今天的工作任务：解决昨天遇到的问题，使K3密钥生成函数运行正确，同时写出K4密钥生成函数。  
任务完成情况：在深入分析之后，针对调用完AES_CMAC算法原来传入参数值发生改变的情况，发现，在c#的运行机制下，参数byte【】数组类型的变量属于引用类型的变量，传入参数属于shadow copy，因此会改变原来传入参数的值，所以需要在AES算法中在传入参数中加入Deep Copy。基于上述，问题1得到解决。  
问题2:问题2的原因是由于c#语言与Java语言对16进制字符串进行biginteger大数转化的机制不同，在C#中如果最高位是0-8则会转化为正数，如果是9-F则转化为负数，因此只需要在16进制的字符串最高位补上一个0即可解决该问题。  
k3，K4生成函数已经运行正确，目前已经开始进行第二部分的任务，开始Ble proxy protocol的PDUs的拼接部分，争取明天能够完成接入层paylaod PDU部分的拼接。  
## 2022年6月23日
工作任务：第二部分PDU的拼接，冲!!!  
任务完成情况：
1.为了更加深入了解蓝牙Mesh proxy PDUs 的组成，昨天继续深入学习了蓝牙mesh的协议栈，各个层之间的功能以及作用，对协议栈的各个层级有了更加深入的理解。  
2.昨天给原来的bleMesh上位机app添加了uuid过滤机制，当下ble.mesh app 只能扫描到代理节点的GAP广播包。  
![](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/4d72eb417adf4ab2b65573a13868872c~tplv-k3u1fbpfcp-zoom-in-crop-mark:3024:0:0:0.awebp?)
## 2022年6月24日
今日的任务计划：在昨天的基础上，完成Access layer、upper transport layer 、lower transport layer这三层Pdu的拼接。  
任务完成情况，已经对upper transport layer pdu完成，周一之后将继续完成所有pdu的完成。  
## 2022年6月27日
今日计划:对lower transport layer，network layer层pdu完成拼接。将其组装成proxy PDUS  
任务完成情况:已经完成了对mesh proxy pdus的组装，同时测试了 network layer pdu的正确性，发现网络层pdu传输正确，接着测试代理pdu传输，发现通过手机发送代理pdu，接收端存在着数据截断问题，考虑问题原因为GATT服务的MTU设置过小，导致一个mesh proxy pdus不能完整传输。明天任务为排除代理pdu所遇到的问题，使代理pdu能够顺利被下位机解析。
## 2022年6月28日
今日记录：上午测试了代理PDU的正确性，发现所拼接的代理PDU在加密与格式解析上完全正确。下午开始解决GATT传输数据的MTU设置过小的问题，google了一个下午的答案，发现我使用的xamarin.forms的包上面没有更改MTU的API。而安卓平台又没有自动协商MTU的机制，在GATT的技术规范中默认的ATT MTU为23Byte，我方发送端没有分包机制，对端也没有组包机制，ATT MTU的问题目前没有太大进展。
## 2022年6月29日
今日记录：基于昨天的情况继续解决MTU传输字节过小的问题，遇到了一个突如的BUG，测试机连接蓝牙之后无法扫描到代理节点的GATT services，最后测试发现换成android12的手机，这个bug没有了，昨天干的事情基本上就是使mesh上位机APP能够适配最新的android12，同时为了避免代码被改乱，学习了git的使用，如何新建本地仓库，如何推送到远端仓库，如何创建代码分枝，如何合并分枝。
## 2022年6月30日
今日记录：接到新任务，Ble GATT下位机profile的实现，上面ATT-MTU的问题也需要弄懂GATT与ATT 协议，在mesh协议的 ble core specification的那一层还没有更深入的理解，趁着这个任务顺便补一下蓝牙核心的知识。  
任务完成情况：学习BLE入门的理论知识。了解了BLE协议栈的大致结构
## 2022年7月1日
今日记录：完成了GATT，GAP理论部分的学习，完成了server端低功耗蓝牙开发基本环境的配置。预计下周开始配置GATT的各个profile。  
## 2022年7月4日
今日计划：完成server的GATT profile部分的代码。  
完成情况：使用zypherSDK配置编译蓝牙官方文档上的代码编译esp32不通过，研究了一天的报错，没能解决，遂决定使用树莓派来做sever。
## 2022年7月5日
今日记录：针对昨天的问题改用树莓派来做，树莓派的代码使用javascript来做的较为简单。完成了GATT部分，发现其是利用bleno内置的库来实现的gatt服务。
##2022年7月6日
今日计划：继续完成树莓派的代码

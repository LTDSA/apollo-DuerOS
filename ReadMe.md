# Apollo-DuerOS
Apollo-DuerOS 是一套与 Apollo 相关的远程信息处理产品，目前有几种开源产品。
 
## Android 车机的 CarLife  

[Android 车机的 CarLife](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/CarLife-Android-Vehicle) 是 CarLife 协议在 Android 平台上的实现。

[CarLife](http://carlife.baidu.com/) 是智能手机集成解决方案，通过多屏幕共享和交互技术，驾驶员可通过该解决方案与 MD（移动设备）到 HU（主机）共享适合安全驾驶条件的移动应用程序，并使用触摸屏，硬键，旋钮控制和麦克风控制 CarLife。 
![CarLife Screen](CarLife.jpeg)

所有业务逻辑都在移动电话端，车机端主要负责连接、协议解析、视频解码、音频播放和触摸事件的功能。

CarLife 手机终端支持 iOS 和 Android 平台，车机终端支持 Android、Linux、WINCE、QNX 等平台。

## CarLife 车机库
[CarLife 车机库](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/CarLife-Vehicle-Lib) is a C++ based cross platform dynamic library, which realizes the function of channel establishment, data sending and receiving, protocol parsing and packing in HU CarLife. Using this library can speed up the development of CarLife in HU.


## DuerOS 启动器
Lanucher is the interface of the first user graphical interaction of the Android terminal,is the start of the installation of other applications on the terminal entrance(Telephone, radio, and so on need to be connected to app).
![Launcher Screen](Launcher.jpeg)

### [DuerOS 启动器](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/DuerOS-Launcher)特性：
1. 适用于驾驶场景设计，采用轻巧、科学的 UI 设计感

2. 主页汇总语音、地图、音乐等入口，车内场景使用更方便

## Apollo DuerOS 的 DSP 解决方案
[DSP 解决方案](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/DSP-Solution-For-DuerOS) includes two parts: front-end signal acquisition and voice signal processing.
![DSPSolution](DSPDesign.png)
Front-end signal acquisition is completed through a set of MIC array (2~3 MIC), while the voice signal processing is achieved by DSP. The DSP chips embedded into the motherboard of the vehicle would work on echo’s noise cancellation and directional voice pick-up, and then convey the processed signal to the main CPU layer, and finally the signals would flow into the Baidu Voice ASR Engine.

## DuerOS 汽车规格
[DuerOS 汽车规格](https://github.com/ApolloAuto/apollo-DuerOS/tree/master/DuerOS-Auto-Spec) 是 DuerOS Auto 的集成指南，包括 DuerOS Auto 软件和硬件要求的集成，访问过程描述，功能和接口描述，测试和验收过程等。合作伙伴 OEM 可以根据此文档执行 DuerOS Auto。

# My-hackintool-Opencore

> **用前须知：**
> 笔记本型号：神舟z7-kp7sc
> 配置：i7-8750H+Nvidia GTX1060+Intel WiFi蓝牙+Realtek网卡9462+Realtek声卡ALC269
> 下载记得自行修改paltform参数
> 引导主题文件：个人自制主题

![](/1.png)
## OC-15.6.1 (24G90)
OC版本：1.0.5
适用版本：macOS Sequoia
功能完善：基本正常
- CPU核显 IntelUHD630 (正常)
- 独显Nvdia 1060（无解），可用：OCLP，BigSur和Monterey，不支持 Metal
- WiFi 蓝牙，需提前下载[OCLP](https://github.com/dortania/OpenCore-Legacy-Patcher/)/[小白推荐用OCLP-MOD](https://github.com/laobamac/OCLP-Mod)，进系统后注入补丁重启。[参考步骤](https://zzmac.com/sequoia-intel-wifi-bluetooth-driver-tutorial.html)
- 声卡，摄像头，睡眠，USB/Type-C (正常)，风扇（可运行，无数据暂无解）
- 电源 插电(正常)，单独电池使用会死机（可能是我的设备硬件故障）
- 外接显示器 HDMI/DP01（接在独显口，无解），DP02（此miniDP口接在核显，可用但不稳定），实测需要开机之前连接dp线，保证在引导阶段检测到外接屏并输出显示。问题：进入系统后内屏黑屏，外接屏30s左右不稳定闪屏，通过合盖关闭内屏几秒钟，再开盖解决（最好关闭macOS合盖睡眠，因为此方式只需内屏关闭重启无需睡眠）
- 外接显示器USB 通过：[Dell D6000设备](https://www.dell.com/support/product-details/zh-cn/product/dell-universal-dock-d6000/overview)+[DisplayLink Manager驱动](https://www.synaptics.com/products/displaylink-graphics/downloads/macos)解决
  
## opencore-OC-14.7.1 (23H222)
OC版本：1.0.2
适用版本：macOS14 Sonoma
功能完善：基本正常
- CPU核显 IntelUHD630 (正常)
- 独显Nvdia 1060（无解），可用OCLP补丁驱动，但不支持 Metal
- 声卡，摄像头，睡眠，USB/Type-C (正常)，风扇（可运行，无数据暂无解）
- 电源 插电(正常)，单独电池使用会死机（可能是我的设备硬件故障）
- 外接显示器 HDMI/DP01（接在独显口，无解），DP02（此miniDP口接在核显，可用但不稳定），实测需要开机之前连接dp线，保证在引导阶段检测到外接屏并输出显示。问题：进入系统后内屏黑屏，外接屏30s左右不稳定闪屏，通过合盖关闭内屏几秒钟，再开盖解决（最好关闭macOS合盖睡眠，因为此方式只需内屏关闭重启无需睡眠）
- 外接显示器USB 通过：[Dell D6000设备](https://www.dell.com/support/product-details/zh-cn/product/dell-universal-dock-d6000/overview)+[DisplayLink Manager驱动](https://www.synaptics.com/products/displaylink-graphics/downloads/macos)解决

## clover-10.13.6
适用版本：macOS10.13.6
功能完善：完美黑苹果
- 核显Intel UHD630(正常)
- WiFi 蓝牙 声卡 摄像头 睡眠 电池(正常)
- Nvdia独显1060（正常），需要安装WebDriver-387.10.10.10.40.139.pkg
- HDMI，USB/Type-C（正常）

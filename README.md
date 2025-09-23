# My-hackintool-Opencore

> **用前须知：**
> 笔记本型号：神舟z7-kp7sc

> 配置：i7-8750H+Nvidia GTX1060+HM370+Intel Wireless-AC 9462+Realtek RTL8411B+Realtek声卡ALC269(模具clevo N8XXEP6)

> 下载记得自行修改paltform参数

> 引导主题文件：个人自制主题

![](/1.png)
## OC-15.7 (24G222)
系统：macOS15 Sequoia
OC：1.0.5
功能：基本完美
- CPU睿频，核显IntelUHD630 (正常)
- 独显Nvdia 1060（无法驱动，可用OCLP补丁驱动，但不支持 Metal）
- WiFi、蓝牙（需提前下载[OCLP](https://github.com/dortania/OpenCore-Legacy-Patcher/)/[小白推荐用OCLP-MOD](https://github.com/laobamac/OCLP-Mod)，进系统后注入补丁重启。[参考步骤](https://zzmac.com/sequoia-intel-wifi-bluetooth-driver-tutorial.html)）
- 声卡，摄像头，睡眠，USB/Type-C (正常)
- 风扇（转动，正常监控数据，但无法控制转速，因EC控制非SuperIO暂无解）
- 电源 插电(正常)，不插电使用电池会死机（可能是我的设备硬件故障）
- 外接显示器：
  - HDMI/DP01（无法驱动，接在独显口无解）
  - DP02（正常，此miniDP接在核显，已知问题及解决办法：接入外接屏后开机，30s左右后可能会出现闪屏现象，可通过拔插DP线/盒盖关闭重开显示屏解决）
  - USB外接显示器：[Dell D6000设备](https://www.dell.com/support/product-details/zh-cn/product/dell-universal-dock-d6000/overview)+[DisplayLink Manager驱动](https://www.synaptics.com/products/displaylink-graphics/downloads/macos)解决
  
## OC-14.7.1 (23H222)
系统：macOS14 Sonoma
OC：1.0.2
功能：基本正常，部分功能修复可参考上方最新版本OC更改
- CPU睿频，核显IntelUHD630 (正常)
- 独显Nvdia 1060（无法驱动，可用OCLP补丁驱动，但不支持 Metal）
- WiFi、蓝牙，声卡，摄像头，睡眠，USB/Type-C (正常)
- 风扇（转动，无法监控数据，参考最新OC解决）
- 电源 插电(正常)，不插电使用电池会死机（可能是我的设备硬件故障）
- 外接显示器：
  - HDMI/DP01（接在独显口，无解）
  - DP02（正常，此miniDP接在核显，已知问题参考最新OC解决）
  - USB外接显示器：[Dell D6000设备](https://www.dell.com/support/product-details/zh-cn/product/dell-universal-dock-d6000/overview)+[DisplayLink Manager驱动](https://www.synaptics.com/products/displaylink-graphics/downloads/macos)解决

## Clover-10.13.6
系统：macOS10.13.6
功能：基本完美
- 核显Intel UHD630(正常)
- Nvdia独显1060（正常），需要安装WebDriver-387.10.10.10.40.139.pkg
- WiFi 蓝牙，声卡，摄像头，睡眠，USB/Type-C，风扇，电源（正常）
- 外接显示器：miniDP、HDMI（应该都正常）

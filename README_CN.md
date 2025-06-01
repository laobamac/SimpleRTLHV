# SimpleRTLHV
[English](README.md)
---------
一款用于为 Realtek RTL8125 2.5G 网卡注入驱动的 Lilu 插件。

## 功能特性

* 支持近期主板搭载的所有版本 Realtek RTL8125 2.5Gb 以太网控制器。</br>
* 支持多分段数据包处理，在组包传输时避免网络栈的不必要拷贝操作。
* 零拷贝接收与发送（小数据包接收时仍会拷贝，因分配新缓冲区效率更低）。
* TCP/UDP/IPv4 校验和卸载（接收与发送）。
* 支持 IPv4/IPv6 的 TCP 分段卸载 (TSO)。
* 支持 TCP/IPv4、UDP/IPv4、TCP/IPv6 和 UDP/IPv6 校验和卸载。
* 支持最高 4076 字节的巨帧传输。
* 已针对 macOS Catalina 深度优化（注：旧版 macOS 可能不支持 2.5Gb 以太网）。
* 支持网络唤醒 (WoL)（未经充分测试）。
* 支持 VLAN 功能。
* 支持节能以太网 (EEE)，可通过修改驱动 Info.plist 中的 `enableEEE` 为 `NO` 禁用（无需重新编译），默认启用。
* 兼容现代 macOS 系统：**Catalina** 至 **Sequoia**

## 支持型号
* Realtek RTL**8125A**
* Realtek RTL**8125B**
* Realtek RTL**8125KB**
* Realtek RTL**8125BP**
* Realtek RTL**8125D**

## 致谢
* 灵感来源于 [mieze](https://github.com/Mieze/RTL8111_driver_for_OS_X) 的 RTL8111_driver_for_OS_X
* 参考 [Realtek](https://github.com/notpeelz/r8125) 官方 r8125 Linux 驱动
* 感谢 [一个憨憨的电脑小白](https://github.com/fix221) 参与测试（截图 -> [hanhan_test](Images/hanhan_test.md)）
* 感谢 请叫我无名 参与测试（截图 -> [wuming_test](Images/wuming_test.md)）

## 交流社区
* [laobamac&win10Q 黑苹果交流群①](https://qm.qq.com/q/fCpQhYKwta) （已满员）
* [laobamac&win10Q 黑苹果交流群②](https://qm.qq.com/q/DA1XSDUaYw) （开放加入中）

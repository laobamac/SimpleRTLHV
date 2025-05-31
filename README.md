# SimpleRTLHV

A Lilu plugin to inject driver for Realtek RTL8125 2.5Gbit Ethernet cards.

## Features

* Supports all versions of Realtek's RTL8125 2.5GBit Ethernet Controllers found on recent boards.</br>
* Support for multisegment packets relieving the network stack of unnecessary copy operations when assembling packets for transmission. 
* No-copy receive and transmit. Only small packets are copied on reception because creating a copy is more efficient than allocating a new buffer. TCP, UDP and IPv4 checksum offload (receive and transmit).
* TCP segmentation offload over IPv4 and IPv6.
* Support for TCP/IPv4, UDP/IPv4, TCP/IPv6 and UDP/IPv6 checksum offload.
* Supports jumbo frames up to 4076 bytes.
* Fully optimized for Catalina. Note that older versions of macOS might not support 2.5GB Ethernet.
* Supports Wake on LAN (untested).
* Supports VLAN.
* Support for Energy Efficient Ethernet (EEE) which can be disabled by setting enableEEE to NO in the drivers Info.plist without rebuild. The default is YES.
* Support modern macOS **Catalina** to **Sequoia**

## Support
* Realtek RTL**8125A**
* Realtek RTL**8125B**
* Realtek RTL**8125KB**
* Realtek RTL**8125BP**
* Realtek RTL**8125D**

## Credits
* [mieze](https://github.com/Mieze/RTL8111_driver_for_OS_X)'s RTL8111_driver_for_OS_X
* [Realtek](https://github.com/notpeelz/r8125)'s r8125 Linux Driver
* [一个憨憨的电脑小白](https://github.com/fix221) helped tested process.

## Community
* [laobamac&win10Q的黑苹果交流群①](https://qm.qq.com/q/fCpQhYKwta) 此群已满员，请进二群
* [laobamac&win10Q的黑苹果交流群②](https://qm.qq.com/q/DA1XSDUaYw) 此群未满，可加入

# XiaomiRouter-R4AC-Firmware
This is the firmware for Xiaomi Router 4A 100Mbps version, which includes Breed, OpenWrt, Padavan  



这是一个自用的小米路由器4A百兆版本的固件仓库。由于为了满足ZJU学校内网，本仓库包含小米路由器相关固件和刷机包。
## 清单
+ OpenWRT(.bin)
  基于Lede的库构建，编译平台WSL-Ubuntu 22.04。干净简洁，仅编译zerotier和xl2tpd插件，**由于本路由器性能羸弱不推荐使用**，并且编译R4AC过程中需要更换写入内存位置以适应breed的刷写，或者逆向思路从修改breed公版内存布局入手。由于后者相对麻烦，本固件采用前者从lede源码进行修改，直接修改写入包的位置（见.dtsi文件）。
+ Breed及EEPROM(.bin)
+ Padavan（.trx）
  基于小鱼的库构建，简单清爽，没有任何多余的功能。

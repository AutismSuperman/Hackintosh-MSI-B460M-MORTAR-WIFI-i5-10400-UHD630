# 中文版

## 配置

**如果使用该EFI,切记请更换三码！！！**

macOS Sonoma 14.3.1 + OpenCore 0.9.8

| 组件 | 名称                      |
| ---- |-------------------------|
| CPU  | i5 10400                |
| 主板 | 微星MAG B460M MORTAR WIFI |
| iGPU | Intel UHD Graphics 630  |
| 显卡 | RX6600XT                |
| 机型 | iMac 20,1               |
| 网卡 | AX200                   |

## CPU支持
- [x] 支持所有10代核显为UHD630的CPU
- [x] 无核显带F的10代CPU，有以下免驱独显也可以（但无法使用核显加速）

## 显卡支持
- [x] 支持仅有CPU核显的UHD630显卡
- [x] 支持AMD独显 RX 470/480/570/570X/580/580X/590 系列显卡
- [x] 支持AMD独显 RX 5500/5600/5700 系列显卡(需使用在boot-args中加入agdpmod=pikera)

## BIOS设置

* USB设备从S3/S4/S5唤醒：允许
* PS/2鼠标从S3/S4/S5唤醒：允许
* USB键盘从S3/S4/S5唤醒：任意键
* 集成显卡多显示器：允许（否则核显硬件解码失效，只使用核显的可以忽略）
* OC -> CPU 特征 -> Intel 虚拟化技术：允许
* OC -> CPU 特征 -> Intel VT-D 技术：禁止
* OC -> CPU 特征 -> CFG锁定：禁止


# iStore OS 固件

[![iStore使用文档](https://img.shields.io/badge/使用文档-iStore%20OS-brightgreen?style=flat-square)](https://doc.linkease.com/zh/guide/istoreos)

![支持设备](https://img.shields.io/badge/支持设备:-blueviolet.svg?style=flat-square) ![H88K](https://img.shields.io/badge/H88K-blue.svg?style=flat-square) ![H66K](https://img.shields.io/badge/H66K-blue.svg?style=flat-square) ![H68K](https://img.shields.io/badge/H68K-blue.svg?style=flat-square) ![H69K](https://img.shields.io/badge/H69K-blue.svg?style=flat-square) ![R5S](https://img.shields.io/badge/R5S-blue.svg?style=flat-square) ![R6S](https://img.shields.io/badge/R6S-blue.svg?style=flat-square) ![R66S](https://img.shields.io/badge/R66S-blue.svg?style=flat-square) ![R68S](https://img.shields.io/badge/R68S-blue.svg?style=flat-square) ![STATION P2](https://img.shields.io/badge/STATION%20P2-blue.svg?style=flat-square) ![T68M](https://img.shields.io/badge/T68M-blue.svg?style=flat-square)

## 默认配置

- IP: `http://192.168.100.1` or `http://iStoreOS.lan/`
- 用户名: `root`
- 密码: `password`
- 如果设备只有一个网口，则此网口就是 `LAN` , 如果大于一个网口, 默认第一个网口是 `WAN` 口, 其它都是 `LAN`
- 如果要修改 `LAN` 口 `IP` , 首页有个内网设置，或者用命令 `quickstart` 修改
- 北京时间每天 `0:00` 定时编译, `Release` 中只保留不同架构的最新版本
- 历史版本在 `Actions` 中选择一个已经运行完成且成功的 `workflow` 在页面底部可以看到 `Artifacts`, `Artifacts` 需要登录 Github 才能下载

## 支持架构

### RK33xx 架构

| 设备       | 包名称                                                                    |
| ---------- | ------------------------------------------------------------------------- |
| R2S        | istoreos-rockchip-armv8-friendlyarm_nanopi-r2s-squashfs-sysupgrade.img.gz |
| R4S        | istoreos-rockchip-armv8-friendlyarm_nanopi-r4s-squashfs-sysupgrade.img.gz |
| R4SE       | istoreos-rockchip-armv8-friendlyarm_nanopi-r4se-squashfs-sysupgrade.img.gz |
| ROCK-PI-4A | istoreos-rockchip-armv8-radxa_rock-pi-squashfs-sysupgrade.img.gz           |
| ROCKPRO64  | istoreos-rockchip-armv8-pine64_rockpro64-squashfs-sysupgrade.img.gz        |

### RK35xx 架构

| 设备           | 包名称                                                                   |
| -------------- | ------------------------------------------------------------------------ |
| H66K/H68K/H69K | istoreos-rockchip-rk35xx-hinlink_opc-h6xk-squashfs-combined.img.gz       |
| H88K           | istoreos-rockchip-rk35xx-hinlink_h88k-squashfs-combined.img.gz           |
| NANOPI-R5S     | istoreos-rockchip-rk35xx-friendlyarm_nanopi-r5s-squashfs-combined.img.gz |
| NANOPI-R6S     | istoreos-rockchip-rk35xx-friendlyarm_nanopi-r6s-squashfs-combined.img.gz |
| R66S/R68S      | istoreos-rockchip-rk35xx-fastrhino_r6xs-squashfs-combined.img.gz         |
| STATION-P2     | istoreos-rockchip-rk35xx-firefly_station-p2-squashfs-combined.img.gz     |
| T68M           | istoreos-rockchip-rk35xx-lyt_t68m-squashfs-combined.img.gz               |

### x86 架构

| 设备       | 包名称                                              |
| ---------- | --------------------------------------------------- |
| X86-64     | istoreos-x86-64-generic-squashfs-combined.img.gz    |
| X86-64-EFI | storeos-x86-64-generic-squashfs-combined-efi.img.gz |

## 鸣谢

- [istoreos](https://github.com/istoreos/istoreos)
- [P3TERX/Actions-OpenWrt](https://github.com/P3TERX/Actions-OpenWrt)
- [OpenWrt](https://github.com/openwrt/openwrt)

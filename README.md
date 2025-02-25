##

本项目用于编译 `ImmortalWrt` 固件。

### 说明

- 由于仓库的代码大部分时间都处于不可用的状态，所以并不建议 fork 使用。除非能够自行排查和修复错误。
- ImmortalWrt-18.06 ImmortalWrt-23.05 OpenWrt-23.05 固件采用 [Flippy](https://github.com/unifreq) 大佬的方案由 Armbian 内核打包制作，LEDE iStoreOS 由于硬件原生支持，为直接编译。
- 固件不定时更新，更新通知可关注 Telegram 频道 [N1 Openwrt firmware](https://t.me/zhenzhushan)，下载前往 [Releases](https://github.com/ffuqiangg/build_openwrt/releases)
- 默认 IP：192.168.1.99， 默认密码：password
- 插件：PassWall，v2rayA，Homeproxy，OpenClash，Nikki，DAED，MosDNS，硬盘休眠，KMS，FileBrowser，Frpc，网络共享，FTP 服务器，DockerMan，DocKer-Compose，UPNP，VerySync
- 各固件包含的科学插件略有差别，具体区别见 release 说明。
- ImmortalWrt-23.05 以及 OpenWrt-23.05 固件经过特殊优化可避免安装 kmod 内核模块时出现 pkg_hash 错误。
- 固件对一些命令进行了简化，如 `ungz = tar -xvzf`，`777 = chmod -R 777`，`mkdirg = 创建并进入目录` 等，详情可查看仓库 files/init/etc/shinit 文件。
- 在终端里输入命令起始部分再通过键盘 `↑ ↓` 可以匹配执行过的历史命令快速输入。
- 固件刷机：具体方法请认真阅读 ⌈ [使用说明](doc/readme.md) ⌋

> [!IMPORTANT]
> iStoreOS 固件相对于其官方固件仅保留插件商店，可以看作包含 iStore 插件商店的原版 OpenWrt-22.03 固件。  
> 带 Pre-release 标签的是测试固件随时删除，且可能有各种问题请谨慎下载使用。

### 感谢

- 本项目源自于[ffuqiangg/build_openwrt](https://github.com/ffuqiangg/build_openwrt) 项目。

# Dell-7460-Hackintosh-OC

EFI使用有问题？请参考这篇文档[黑苹果安装指北手册](https://howiehye.top/post/9ff9620/)

## 说明

此 EFI 适用于戴尔燃 7000 系列第二代型号为 7460 的笔记本电脑。

此分支的`OpenCore`来自[OpenCore-Factory](https://github.com/williambj1/OpenCore-Factory) [![Release](https://img.shields.io/static/v1?label=Releases&message=2020-09-04&color=orange)](https://github.com/williambj1/OpenCore-Factory/releases)

目前已经测试过
- 安装
  - `macOS Catalina 10.15.6(19G2005)`
  - `macOS Big Sur Developer Beta3(20A5323I)`
  - `macOS Big Sur Public Beta1(20A5343j)`
- 升级
  - `macOS Catalina 10.15.6(19G2005)`OTA 直升`macOS Big Sur Public Beta1(20A5343j)`
  - `macOS Catalina 10.15.6(19G2005)`OTA 直升`macOS Big Sur Public Beta2(20A5354i)`
  - `macOS Big Sur Public Beta1(20A5343j)`OTA 直升`macOS Big Sur Public Beta2(20A5354i)`

## 电脑配置

| 规格     | 型号                                                                                        |
| -------- | ------------------------------------------------------------------------------------------- |
| 电脑型号 | `Dell Inspiron 7460`                                                                        |
| 操作系统 | `macOS Big Sur Public Beta2(20A5354i)` && `Windows 10` |
| 处理器   | `Intel Core i7-7500U @ 2.70GHz` 双核                                                        |
| 声卡     | `ALC256`                                                                                    |
| 网卡     | 已更换为 `DW1560`                                                                           |

## OC

- 支持安装、升级和日常使用（不能保证都可以顺利安装，安装或升级时请自行在`boot-args`里添加`-v`）
- 支持`macOS Catalina、macOS Big Sur Devloper Beta1~Beta5、macOS Big Sur Public Beta1~Beta2`,理论上支持`macOS High Sierra/macOS Mojave`
- CPU 原生支持，变频正常
- 显卡原生支持，`Lilu+WEG`
- 声卡正常
- 无线网卡更换为`DW1560`
- 显示器亮度调节正常

## Hidpi

仓库地址:[一键开启 HIDPI](https://github.com/xzhih/one-key-hidpi)

### 非Big Sur用户

> 在终端运行
>
> ```bash
> bash -c "$(curl -fsSL https://raw.githubusercontent.com/xzhih/one-key-hidpi/master/hidpi.sh)"
> ```
> 
> 网络不好的可以用这条
>
> ```bash
> bash -c "$(curl -fsSL https://gitee.com/howiehye/one-key-hidpi/raw/master/hidpi.sh)"
> ```

### Big Sur用户

> ```bash
> bash -c "$(curl -fsSL https://raw.githubusercontent.com/xzhih/one-key-hidpi/dev/hidpi.sh)"
> ```
> 
> 网络不好的可以用这条
> 
> ```bash
> bash -c "$(curl -fsSL https://gitee.com/howiehye/one-key-hidpi/raw/dev/hidpi.sh)"
> ```

## 系统截图

![更新截图](https://img.howiehye.top//img/20200807203611.png)

![关于本机](https://img.howiehye.top//img/20200807204722.png)

![控制中心](https://img.howiehye.top//img/20200807204844.png)

![Wi-Fi](https://img.howiehye.top//img/20200807204949.png)

![蓝牙](https://img.howiehye.top//img/20200807205020.png)

![Hacintool](https://img.howiehye.top//img/20200807205115.png)

## LOG

- 2020-08-05
  - 更新`OC0.6.0`
- 2020-08-06
  - 更新`config.plist` , 修复安装/进入`Recovery`时显示俄语的错误
  - 已经测试`Big Sur Beta3`全新引导安装
- 2020-08-07
  - `Big Sur Developer Beta4(20A5343i)`OTA 升级`Big Sur Public Beta1(20A5343j)`
- 2020-08-08
  - 测试安装`macOS Big Sur Developer Beta3(20A5323I)`
  - 测试安装`macOS Catalina 10.15.6(19G2005)`
  - `macOS Catalina 10.15.6(19G2005)`OTA 升级`Big Sur Public Beta1(20A5343j)`
- 2020-08-09
  - 测试安装`Big Sur Public Beta1(20A5343j)`
- 2020-08-21
  - 升级`macOS Big Sur Public Beta2(20A5354i)`

## 其他说明

- 安装`macOS Big Sur`的过程很漫长 , 请耐心等待 , 不一定是有错误
- 每次升级或替换新的`EFI`后 , 最好重置一下`NVRAM`

## 鸣谢

- [@黑果小兵](https://github.com/daliansky/)

- [@冰水加劲](https://github.com/xzhih/)

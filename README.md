## TB-X505F 刷机资源站

`产品描述:  高通骁龙429ARM 四核芯2.0GHz/10.1"英寸 1280x800 IPS 350nits /3GB DDR3内存/32GB SSD储存/Android 9/双频WIFI/WIFI/前置200万像素，后置800万像素/4850mAh/蓝牙4.0/GPS/北斗/USB/243.2x169.2x8.45mm/480g/塑料/人脸识别/护眼模式/双立体声扬声器+杜比`

笔者是一名学生 在小黄鱼被人强塞50得到了这个平板 结果开机是个学习系统 于是有了以下折腾的经历 据卖家说是学校1299买的 每学期300块 （这也太**坑爹了）

### 你一定需要的东西

[笔记本（防止突然断电）](https://item.jd.com/70239970489.html)

[Micro-USB数据线（别买一两块的就行）](https://s.taobao.com/search?q=Micro-USB)

[鼠标](https://s.taobao.com/search?q=%E9%BC%A0%E6%A0%87)

[键盘](https://s.taobao.com/search?q=%E9%94%AE%E7%9B%98)

[压缩软件](https://www.7-zip.org/)

[高通9008驱动](https://www.baidu.com/baidu?wd=%E9%AB%98%E9%80%9A9008%E9%A9%B1%E5%8A%A8%E5%AE%89%E8%A3%85%E6%95%99%E7%A8%8B)

[QFIL](https://qfiltool.com/)

[fh_loader（放入qfil目录下）](https://mega.nz/file/IolkFLqb#0RiKIfwDKeBTklICTpwKnLQ-kDMVL3LPHoB8fFxJHPQ) [百毒网盘 提取码6xqa](https://pan.baidu.com/s/14tCaBmtVVsjWP_Ym-d931g?pwd=6xqa)

[运行库](https://www.ghxi.com/yxkhj.html)

[Rescue and Smart Assistant (LMSA) 下载原厂系统](https://download.lenovo.com/lsa/Releases/Rescue_and_Smart_Assistant_v5.9.2.4_prod_setup.exe)/[TB-X505F_S001142_210804_ROW高速直链（请使用单线程下载）](https://service-jg4dbh40-1309432354.hk.apigw.tencentcs.com/release/SCFOnedriveIndex-1643191796/OD01/Firmware/Lenovo%20TB-X505F/TB-X505F_S001142_210804_ROW.zip)/[镜像站](https://mirrors.lolinet.com/)

**脑子（重要）**

### 可能需要的东西

[TWRP](https://forum.xda-developers.com/t/recovery-tb-x505f-unofficial-twrp-3-6-x-for-lenovo-tab-m10-hd.4211221/)

[Magisk](https://github.com/topjohnwu/Magisk/releases/)

[Android SDK Platform Tools（俗称adb&fastboot）](https://developer.android.google.cn/studio/releases/platform-tools?hl=zh-cn)

### 学习系统刷正常系统

如果你想在刷机后刷回到学习系统 请用qfil备份**boot system vendor vbmeta vbmetabak recovery(可选)**等分区

详情可见[YoungToday/Lenovotabunlock](YoungToday/Lenovotabunlock)

1.电脑安装好9008驱动 打开qfil

2.平板关机 数据线一端连接电脑

3.平板按住音量上键 数据线连接平板并等待

4.电脑发出usb连接提示音即可松手

5.qfil选择COM端口 Flat Build 右下角选emmc

6.Programmer Path选择你解压的系统包里的mbn文件

7.Load XML选择rawprogram_upgrade.xml patch0.xml

8.点击Download刷入系统

9.待进度条走完提示Success时 拔下数据线 长按电源键10s开机

### 正常系统oem解锁

设置-关于平板电脑-点四下系统版本打开开发者选项

开发者选项里打开oem解锁 重启时按住音量下键进入fastboot

连接电脑 输入 `fastboot oem unlock-go` 即可解bl锁

#### 刷入TWRP

`fastboot flash recovery ***.img`

重启时按住音量上下键即可进入recovery

#### 刷入Magisk

**不推荐卡刷面具**

用TWRP备份**Boot**分区

Magisk app内修补Boot分区文件

TWRP将Magisk修补的文件刷入Boot分区即可

#### 几个救砖操作

1.将Magisk的apk文件命名为`uninstall.zip`在TWRP卡刷

2.TWRP刷入[Riru](https://github.com/RikkaApps/Riru/releases)（会和Zygote冲突）

3.qfil重新刷机

### 正常系统刷回学习系统

如果你没有备份原系统分区 那么你可以**修改开机脚本**来卡第一屏 然后让学校管理员给你刷机

### 推荐使用的[GSI](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list)

已知TB-X505F为**A/B分区** 其他平板请自测

[LineageOS19.X 安卓12 构建:AndyYan](https://sourceforge.net/projects/andyyan-gsi/files/lineage-19.x/)

[dotOS 安卓11 官方构建](https://www.droidontime.com/devices/arm64)

[Resurrection Remix 安卓10 构建:RobotHanzo](https://sourceforge.net/projects/resurrection-remix-q-gsi/files/)

### 友情链接

[有问题欢迎在此提问](https://www.baidu.com/)

[领创获取设备密码](https://github.com/KuzeKumiko/Lenovo_tb_x505f_StudyNM/raw/main/getpwd.exe)

[勇士，欢迎你来到讯飞平板资源下载站](https://magisk-root.github.io/)

[LinspirerAppStoreEnumerator](https://github.com/F-Unction/LinspirerAppStoreEnumerator)

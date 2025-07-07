---
title: 重装 Win11 完整教程
description: 从镜像下载到软件安装 
date: 2025-07-07 
image: win11.jpg 
categories: 
    - 工具 

---

作为重装过我的和朋友两款天选的"experienced"用户，我决定写一篇教程。~~（因为朋友不小心初始化电脑搞得电脑混乱所以决定光速记录一下）~~
## 准备

### 拷贝你的重要文件

**重要提示**：如果你的电脑只有一个分盘C盘，并且没有多余的空间来分盘、没有多余的8G以上U盘，请先看第三点，然后把所有的重要文件（比如win11默认放图片、视频的文件夹，在C盘内建立的工作文件夹，尤其是“文档”里的Tencent Files，里面有所有qq和微信的文件，如果你需要，请把这个文件夹整个带走）拷到U盘等外部存储设备。不建议你带走软件，不过你可以记录一下自己下过哪些软件。  
  
如果你有D盘，或者你的电脑有其他的硬盘，你可以把它们放到D盘或其他硬盘里，因为一般的重装只会清空C盘。如果你“**电脑所有可用的存储空间**”是512G，我不建议以后分C和D盘。如果是1T及以上，建议C盘占512G，这样默认的图片、文档、软件和部分游戏都可以放C盘，其他盘空间足够富余。

### 下载 Windows 11 镜像

  * **进入网页：** 在**Bing**搜索“win11镜像”，选择官网，或[点击这里](https://www.microsoft.com/zh-cn/software-download/windows11)。

  * **选择方式：** 选择”下载磁盘映像（ISO）”下，选择”适用于多版本的ISO“（不建议在这选择简中版），经过一些验证和重新选择语言，就可以点击下载了。
  * **拷贝方式：** 如果你选择在该设备安装，请把它放在已安装win11的磁盘（一般是C盘）**之外的存储设备**，比如D盘、其他硬盘、U盘。
### 准备 WePE 启动盘

WePE 是一款完善的 Windows PE 工具，它集成了多种实用工具，方便我们进行系统安装、分区管理、数据恢复等操作。

  * **下载PE：** 在Bing搜索WePE，在官网小额赞助下载最新的 WePE 工具箱。[123云盘链接,exe](https://www.123912.com/s/JcaUjv-PUYo3)下载其他的PE工具箱也可以。
  * **安装PE：** 如果你就在该电脑上安装，那么不需要制作U盘。制作U盘工具要对U盘格式化。


## 重装系统

### 进 WePE

常规设置下，进入系统会自动跳出让你选择进入win11还是PE。赶紧敲击方向键并选择PE，回车

  * **打开DISM++：** 在上方一大行黑色空间里选中你的C盘，使它显蓝色，然后左上角文件→释放镜像/映像。
  * **选择位置：**
      * 第二行找到你下载好的ISO文件。记住不要是在C盘，否则你会在后面丢失它，你就得从别的设备重新下载ISO拷贝过去了。
      * 第一行版本，可以一步到位选择功能最多的“Windows 11 Pro WorkStation”（家庭--专业--专业工作站版的功能呈越来越多的趋势）。
      * 选择你要安装系统的硬盘分区（通常是 C 盘）。
      * 下方的五个勾勾，选择后三个，ToGo，含引导，格式化。然后安装。如果成功，黑色空间就会显示C盘有Win11专业工作站版了。

  * **修复引导：** 以防万一，在安装完毕后，在上方黑色空间选中C盘，左上角修复→修复引导。一般来说是好的，不过就要修复一下。
  * **重启电脑：** 修复完成后，重启到Win11。

### 设置 Windows 11

电脑重启后，会进入 Windows 11 的初次设置界面。开始是需要联网的，新系统并没有携带你网卡的驱动，如果你身边没有网线，那么请在需要你安装驱动的页面，按Shift + F10，在命令行界面输入`OOBE\BYPASSNRO`（这个斜杠一般在回车键上面），回车，此时会重启，重启后就出现能跳过联网的选项了。如果你不能正确执行这个命令，请在b站具体搜索方法。其他的就和正常进新系统一样。

### 安装厂家驱动

  * **最推荐方式：** 搜索你的电脑品牌官方支持网站，例如“华硕支持”，根据你的电脑型号，找到对应的驱动下载页面。如果你找不到，问淘宝/京东的官方店客服即可。如果没有网线，那得下到U盘或手机上再导给电脑。下好网卡的几个驱动就可以在电脑上自己下载了。  
如果官方有xx管家可以帮你下驱动，也是一种备选方案。下载所有必要的驱动程序，包括显卡驱动、声卡驱动、网卡驱动、性能设置软件等。极其不推荐第三方的驱动大师、驱动精灵等。

### Win11基本软件

在下载我直接给出的文件前，请阅读“本站文件须知”。

  * **激活工具：** 这个软件能给出最优方法。[123云盘链接.zip](https://www.123912.com/s/JcaUjv-GUYo3)
  * **Office：** 使用Office Tool Plus来激活使用Office。[官网](https://otp.landian.vip/zh-cn/download.html)，[教程](https://www.coolhub.top/archives/42)


### 下载常用软件

名字后带*的在[此123链接](https://www.123912.com/s/JcaUjv-OUYo3)有截至发稿日期还能正常用的软件版本，后续可自己更新；不带的给出官网链接。


  * **浏览器：** [Chrome](https://www.google.com/intl/zh-CN/chrome), Edge, [Firefox(推荐)](https://www.mozilla.org/zh-CN/firefox/new/)

  * **解压缩工具：** 7-Zip*
  * **影音处理：** [PotPlayer](https://potplayer.tv/), [VLC Media Player](https://www.videolan.org/vlc/index.zh_CN.html)，[网易云音乐](https://music.163.com/#/download)，[Spotify](https://open.spotify.com/download), [Fxsound(调音)](https://www.fxsound.com/download)，[剪映专业版](https://www.capcut.cn/)

  * **聊天工具：** [微信](https://pc.weixin.qq.com/)、[QQ](https://im.qq.com/pcqq/index.shtml)

  * **专业软件：** [Visual Studio](https://visualstudio.microsoft.com/zh-hans/), Git*, [Dev C++](https://sourceforge.net/projects/orwelldevcpp/), [Python](https://www.python.org/about/), PowerShell*

  * **网盘软件：** [123云盘](https://www.123pan.com/Downloadclient)，[天翼云盘](https://cloud.189.cn/web/static/download-client/index.html)，[百度网盘](https://pan.baidu.com/download#win)，[迅雷](https://www.xunlei.com/)

  * **游戏工具：** [Nvidia App](https://www.nvidia.cn/software/nvidia-app/), [Steam](https://store.steampowered.com/about/), [Epic Game](https://www.epicgames.com/site/zh-CN/home/), MSI Afterburner*(小飞机，性能监控)，[雷神加速器](https://www.leigod.com/)，[bilibili直播姬](https://link.bilibili.com/p/eden/download?hotRank=0#/web)，OBS*，[完美世界竞技平台](https://pvp.wanmei.com/)

  * **其他工具：** Everything*(搜文件), Traffic Monitor*(看网速), Wiztree*(文件空间大小可视化), 图吧工具箱*, [Clash Verge(翻墙)](https://github.com/clash-verge-rev/clash-verge-rev), HiBitUninstaller*(卸载工具), IDM*(快速下载插件), Quicklook*(空格键预览), StartAllBack*(**让win11回归win10部分人性化的界面**)，[火绒安全软件](https://www.huorong.cn/)，LocalSend*(局域网传文件)


## 后续维护

经反馈，可能会出现耳机麦克风没声等问题...不过似乎跟本人做法无关，请自行搜索合适的解决方案或联系我。

希望本文有帮助~

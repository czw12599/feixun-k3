固件管理地址：192.168.5.3（旁路由模式）

编译系统升级导致在线更新失败请下载升级包https://github.com/czw12599/OPENWRT/releases/tag/Update-x86 无需解压直接到固件升级/备份里手动升级可解决

首先需要打开 Openwrt 主页,点击系统-TTYD 命令窗,或者使用putty或者openwrt后台luci插件在线更新

输入openwrt即可进入固件升级菜单

输入tools即可打开工具箱

输入qinglong即可全自动安装青龙

================================================================

自行云编译固件姿势

ssh-actions改为ssh就可以启动插件选择

看到ssh链接会有一个web的链接，打开就是命令行，根据下面命令进入

开始 ctrl+c

进ssh选择插件

cd openwrt && make menuconfig
结束ctrl+d

REPO_TOKEN密匙制作教程：https://git.io/jm.md

云编译需要 在此 创建个token,勾选：repo, workflow，保存所得的key

然后在此仓库Settings->Secrets中添加个名字为REPO_TOKEN的Secret,填入token获得的key

TG通知Settings->Secrets中添加个名字为TELEGRAM_BOT_TOKEN和TELEGRAM_CHAT_ID

<details>
<summary>🆙点击查看更新说明</summary>
<br>

2022年7月28号，编译时候在diy-part.sh文件里面可以对OpenClash代码进行分支选择，可选master或者dev分支，选错或者不选就默认使用master分支


2022年7月6号16点，去除重复插件


2022年4月27号修改
  
1、把 build/openwrt_amlogic/diy-part.sh 里面的晶晨打包组合的路径修改过了，请及时更新

2、把编译的时候不想要的固件或者文件的删除方法修改过了，注意diy-part.sh的代码路径也修改过了，要及时更新，新删除方法请到《[`删除不想要的固件或者文件`](https://github.com/danshui-git/shuoming/blob/master/%E5%9B%BA%E4%BB%B6%E6%96%87%E4%BB%B6%E5%A4%B9%E6%95%B4%E7%90%86.md)》查看说明

<br />
</details>


---
<details>
<summary>🆘点击查看编译教程</summary>
<br>

## [`github编译教程`](https://github.com/danshui-git/shuoming#readme)

---
#### [`本地Ubuntu一键编译`](https://github.com/281677160/bendi)
#### [`本地一键提取.config然后在云编译脚本使用`](https://github.com/danshui-git/shuoming/blob/master/yijianconfig.md)

<br />
</details>


---
 ### 鸣谢！
 感谢以下各位大佬（排名无分先后）<br />
 
 [`coolsnowwolf`](https://github.com/coolsnowwolf/lede/tree/master)
 [`Lienol`](https://github.com/Lienol/openwrt/tree/22.03)
 [`immortalwrt`](https://github.com/immortalwrt/immortalwrt)
 [`P3TERX`](https://github.com/P3TERX/Actions-OpenWrt)
 [`Hyy2001X`](https://github.com/Hyy2001X/AutoBuild-Actions)
 [`dhxh`](https://github.com/dhxh/Openwrt-Build)
 [`ophub`](https://github.com/ophub/amlogic-s9xxx-openwrt)
 [`nicholas-opensource`](https://github.com/nicholas-opensource/OpenWrt-Autobuild)
 [`hx210`](#/README.md)
 [`hyird`](#/README.md)
 [`World Peace`](#/README.md)
 [`klever1988`](https://github.com/klever1988/cachewrtbuild)
 [`actions`](https://github.com/actions/upload-artifact)
 [`svenstaro`](https://github.com/svenstaro/upload-release-action)

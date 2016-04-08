##ChromeBook Crouton代理

####今天正好有空写个教程，通过crouton方式专门给arm架构带chrome系统的chrome本，平板电脑，树莓派使用上Ubuntu系统（chrome os 内部包含）。执行的下一步动作的话先下载crouton https://github.com/dnschneid/crouton
* 1.Unity：
Ubuntu 12.04 with Unity (2D)：
`sudo sh -e ~/Downloads/crouton -r precise -t unity -e`
（arm架构unity最多支持12.04）

* 2.Xfce：
Ubuntu 14.04 with Xfce：
`sudo sh -e ~/Downloads/crouton -r trusty -t xfce -e`

* 3.kubuntu: 
首选 `sudo sh -e ~/Downloads/crouton -t kde` 
触摸屏可以试`sudo sh -e ~/Downloads/crouton -t touch,kde`
类似的可以安装gnome (GNOME Shell), cinnamon, lxde等发行版本。。。

####参考：
* 1. http://www.linux.com/learn/tutorials/795730-how-to-easily-install-ubuntu-on-chromebook-with-crouton
* 2. http://www.webupd8.org/2013/12/install-ubuntu-on-your-chromebook-using.html
* 3.请务必使用国内源：mirrors.ustc.edu.cn/ubuntu/ubuntu
调出终端，在键盘上按ctrl+alt+T 参考下我的命令：比如安装Ubuntu14.04的话 `sudo sh -e ~/Downloads/crouton -r trusty -t xfce -e -m http://mirrors.ustc.edu.cn/ubuntu/ubuntu/
-m`的意思是指向源地址,
接着等待安装结束后在终端输入`sudo startxfce`就可以了
* 4.参考：http://tieba.baidu.com/p/3490991713?pid=62200356240&cid=62661091999#62661091999
* 5.参考原作者 url https://github.com/dnschneid/crouton/raw/releases/$INSTALLER
***
crouton.proxy 请用pac，我已经上传到百度云，可以下载下来用notepad++或者sublime修改。
在第84行的 sed -i '/Execute the main script inline/ased -i '\''s/wget -O /wget -e "https_proxy=http:\\/\\/pac.xxxx.com:25\\/" -O /g'\'' $SCRIPTDIR/targets/audio' "$CACHEFILE" “pac.xxx.com”指的是你代理地址，自己可以通过vps搭建，或者用ip地址也行。
百度云：http://pan.baidu.com/s/1bnIyMa7 密码：jdj6

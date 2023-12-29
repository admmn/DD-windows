# DD-windows

一键DD脚本

1keydd

1. wget -qO- inst.sh|bash -s - -t https://oss.sunpma.com/Windows/Win_Server2022_64_Administrator_nat.ee.gz

sunpma

说明

无限制全自动dd安装Windows；

突破没有VNC,没有救援模式,内存比dd包小的限制；

使用Debian Live CD中的busybox做中间媒介,经过复杂的处理使本机的网络参数传进Windows操作系统中；

即使没有DHCP能够让Windows获取网络参数,也能让Windows操作系统在开机的第一时间能够连通网络；

本站所提供的脚本及安装包均来源于网络并通过测试；

特别注意：脚本不适用于OpenVZ构架的服务器，请勿尝试；

安装依赖

更新系统

#Debian/Ubuntu:

1. apt-get update

#RedHat/CentOS:

1. yum update

必要依赖

#Debian/Ubuntu:

1. apt-get install -y xz-utils openssl gawk file

#RedHat/CentOS:

1. yum install -y xz openssl gawk file

一键脚本

示例脚本，补全DD包直连地址后运行即可；

wget --no-check-certificate -qO InstallNET.sh 'https://sunpma.com/other/oss/InstallNET.sh' && bash InstallNET.sh -dd '[Windows DD包直链地址]'

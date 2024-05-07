# BBR
BBR加速一键安装脚本汇总，总有一个适合你，轻松给自己的vps加速，服务器vps加速|bbr加速更换最新内核|bbr plus加速安装|bbr install script

方案一项目地址：https://github.com/Chikage0o0/Linux-NetSpeed

最常用的脚本（此脚本Ubuntu安装了会导致服务器失联，值得注意的是此脚本已停止更新）：

```
   wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh"

   chmod +x tcp.sh

   ./tcp.sh
```

菜单命令

```
./tcp.sh
```


方案二项目地址：https://github.com/cx9208/bbrplus

此脚本只能用于CentOS，Centos9目前测试了安装不了，Centos7.6能安装

```
wget "https://github.com/cx9208/bbrplus/raw/master/ok_bbrplus_centos.sh" && chmod +x ok_bbrplus_centos.sh && ./ok_bbrplus_centos.sh
```

查看内核版本

```
uname -r
```

查看BBR是否启动成功，输入下面代码，显示有bbrplus则启动成功

```
lsmod | grep bbr
```

方案三项目地址：https://teddysun.com/489.html

```
wget --no-check-certificate -O /opt/bbr.sh https://github.com/teddysun/across/raw/master/bbr.sh

chmod 755 /opt/bbr.sh

/opt/bbr.sh
```

查看内核版本

```
uname -r
```

查看BBR是否启动成功

```
lsmod | grep bbr
```

方案四项目地址（根据官方文档选择安装）：https://github.com/jinwyp/one_click_script

通过 bash安装脚本

```
bash <(curl -Lso- https://git.io/kernel.sh)
```

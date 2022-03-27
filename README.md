
```bash
git clone --depth=1 -b ky-branch https://github.com/beidongjiedeguang/Clash.git
```
对于图形界面的linux用户而言，clash for win是更好的选择：https://github.com/Fndroid/clash_for_windows_pkg/releases

# Linux 使用, Ubuntu 为例

~**使用本仓库**
```bash
./install.sh 

# root user:
. /etc/profile &> /dev/null

# non-root user: 
source ~/.bashrc &> /dev/null
```
跟着教程一步一步就好
bywave: https://bywave.art/clientarea.php



```Shell
clash #正常模式运行
clash -h #脚本帮助及说明
clash -u #卸载脚本
clash -t #测试模式运行
```

~**运行时的额外依赖**：<br>

`大部分的设备/系统都已经预装了以下的大部分依赖，使用时如无影响可以无视之`

```sh
bash/ash		必须		全部缺少时无法安装及运行脚本
curl/wget		必须		全部缺少时无法在线安装及更新，无法使用节点保存功能
iptables		重要		缺少时只能使用纯净模式
systemd/rc.common	一般		全部缺少时只能使用保守模式
iptables-mod-nat	一般		缺少时无法使用redir模式，混合模式
ip6tables-mod-nat	较低		缺少时影响redir模式，混合模式对ipv6的支持
crontab			较低		缺少时无法启用定时任务功能
net-tools		极低		缺少时无法正常检测端口占用
ubus/iproute-doc	极低		缺少时无法正常获取本机host地址
```




# OpenWrt
OpenWrt相关或者Linux脚本

进入 webshell 或者终端登录执行命令，在和DNS相关的操作时，需要重启DNSmasq和清除系统DNS缓存和浏览器缓存以便生效。

重启DNSmasq服务命令：
/etc/init.d/dnsmasq restart

mkdir /etc/dnsmasq.d
//新建一个dnsmasq.d的目录
//这里边存放dns规则
 
echo "conf-dir=/etc/dnsmasq.d" >> /etc/dnsmasq.conf
//使dnsmasq.d目录内的规则生效

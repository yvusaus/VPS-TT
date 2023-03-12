## VPS搭建代码
# 获取root权限
```
sudo -i
```
# 更新及安装组件
- Debian/Ubuntu 命令
```
apt update -y
```
```
apt install -y curl socat
```
- CentOS 命令
```
yum update -y
```
```
yum install -y curl socat
```
# 删除内部防火墙
```
- apt remove iptables -y
```
# 重启系统
```
reboot
```
# 开启bbr加速
```
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh"

chmod +x tcp.sh
./tcp.sh


## 甬哥xui的证书

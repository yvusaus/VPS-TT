
## VPS搭建代码
# 一键更改roo密码
```
  wget -N https://gitlab.com/rwkgyg/vpsroot/raw/main/root.sh && bash root.sh
```
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
  apt remove iptables -y
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
```
- 更改证书路径
```
~/.acme.sh/acme.sh --installcert -d 域 --key-file /root/private.key --fullchain-file /root/cert.crt
```
- 证书路径为
```
/root/cert.crt
```
```
/root/private.key
```
#   测奈飞
```
wget -O nf https://github.com/sjlleo/netflix-verify/releases/download/2.01/nf_2.01_linux_amd64 && chmod +x nf && clear && ./nf
```

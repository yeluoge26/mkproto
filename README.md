更新系统并安装基本依赖：
bash

复制
sudo apt update && sudo apt upgrade -y
sudo apt install wget curl -y
下载一键脚本： 
bash

复制
wget -N --no-check-certificate https://raw.githubusercontent.com/iiiiiii1/doubi/master/mtproxy_go.sh
chmod +x mtproxy_go.sh

一路下一步

管理服务： 脚本通常会自动配置 systemd 服务，可用以下命令管理：
bash

复制
systemctl start mtproxy
systemctl stop mtproxy
systemctl status mtproxy

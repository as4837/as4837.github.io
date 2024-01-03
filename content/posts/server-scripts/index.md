+++
title = '服务器一键脚本'
date = 2024-01-03T12:46:18+08:00
draft = false
+++

重装脚本

wget --no-check-certificate -qO InstallNET.sh 'https://raw.githubusercontent.com/leitbogioro/Tools/master/Linux_reinstall/InstallNET.sh' && chmod a+x InstallNET.sh && bash InstallNET.sh -debian 12 -pwd 'password' --cloudkernel 1 --bbr --ip-dns 9.9.9.9 --fail2ban



Xray VLESS Vision Reality

bash <(curl -L https://github.com/crazypeace/xray-vless-reality/raw/main/install.sh)



YABS

wget -qO- yabs.sh | bash


三网回程测试

wget -N --no-check-certificate https://raw.githubusercontent.com/Chennhaoo/Shell_Bash/master/AutoTrace.sh && chmod +x AutoTrace.sh && bash AutoTrace.sh



BBR

    echo "net.core.default_qdisc=fq" >> /etc/sysctl.conf
    echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.conf
    sysctl -p
    sysctl net.ipv4.tcp_available_congestion_control
    lsmod | grep bbr

# 内网IP邦定


第一步
cp ifcfg-eth0 ifcfg-eth1

第二步修改 ifcfg-eth1的内容如下

DEVICE=eth1
BOOTPROTO=static
IPADDR=10.52.55.2
MTU=1450
NETMASK=255.255.0.0
TYPE=Ethernet
NM_CONTROLLED=no
ONBOOT=yes

第三步
service network restart

第四步
ifconfig -a 去查看情况

MLS2#conf t
MLS2(config)#int vlan 10
MLS2(config-if)#ip address 10.10.10.3 255.255.255.0
MLS2(config-if)#no sh
MLS2(config-if)#int vlan 20
MLS2(config-if)#ip add 10.10.20.3 255.255.255.0
MLS2(config-if)#no sh
MLS2(config-if)#int vlan 30
MLS2(config-if)#ip add 10.10.30.3 255.255.255.0
MLS2(config-if)#no sh
MLS2(config-if)#int vlan 50
MLS2(config-if)#ip address 10.10.50.3 255.255.255.0
MLS2(config-if)#no sh

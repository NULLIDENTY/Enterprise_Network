MLS1#conf t
MLS1(config)#int vlan 10
MLS1(config-if)#ip address 10.10.10.2 255.255.255.0
MLS1(config-if)#no sh
MLS1(config-if)#int vlan 20
MLS1(config-if)#ip add 10.10.20.2 255.255.255.0
MLS1(config-if)#no sh
MLS1(config-if)#int vlan 30
MLS1(config-if)#ip add 10.10.30.2 255.255.255.0
MLS1(config-if)#no sh
MLS1(config-if)#int vlan 50
MLS1(config-if)#ip address 10.10.50.2 255.255.255.0
MLS1(config-if)#end
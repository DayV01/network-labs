# \# network-labs



##### \# basic-configs

all commands while in configure terminal mode:

&nbsp;	hostname (name) 		→ changes hostname

&nbsp;	no ip domain-lookup 		→ stops DNS resolving after misspeling command

&nbsp;	enable secret (password) 	→ sets password for entering privilaged mode

&nbsp;	banner motd (use special character at the beginning and at the end, ex. $) → sets a banner to be shown on login attempt



##### \# basic-telnet

line vty (0-15) 	→ choose virtual line to configure

password (password)	→ set password for login **!!! Password is stored in plain text**

login			→ enable logging



**Important:** telnet connection is not secure, everything goes by plain text.



##### \# vlan-config

vlan (number) 	→ creates VLAN

name (name)	→ changes vlan name



###### \# vlan-interface-config

&nbsp;	interface vlan (number) 		→ enters VLAN interface configuration

&nbsp;	ip address (ip: x.x.x.x) (mask: x.x.x.x)→ sets ip address for interface

&nbsp;	no shutdown				→ interface is shut down by default, you have turn it on



##### \# interface-config

interface (type of interface) (interface number) → enters interface configuration

switchport mode (access/trunk)			 → sets switchport mode, 'access' for device, 'trunk' for multiple vlans

switchport access vlan (num)			 → sets access for chosen vlan to switchport

switchport trunk allowed vlan (nums)		 → sets allowed vlans to be trunked



#### \# router-on-a-stick

interface (type of interface) (interface number).(subinterface number, ex. 10 for VLAN 10 but it's not mandatory to match) 
						→ enters subinterface configuration

encapsulation dot1Q (vlan number)		→ enables VLAN routing, you must choose vlan number on this specific subif

ip address (ip: x.x.x.x) (mask: x.x.x.x)	→ sets ip address for subif










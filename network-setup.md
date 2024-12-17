Router1 (ISR4331)


Switch1 (Cisco 2960) 168.90.0.1
Server1-PT
Laptop-PT Laptop1
PC-PT PC 1
PC-PT PC 2
PC-PT PC 4


Switch2 (Cisco 2960) 210.3.14.1
Server2-PT
Server3-PT
PC-PT PC3
PC-PT PC5


Switch1
enable config t interface GigabitEthernet 0/0/0 ip address 168.90.0.1 255.255.255.0 no shutdown exit ip dhcp pool FIRST-POOL network 168.90.0.0 255.255.255.0 default-router 168.90.0.1 dns-server 168.90.0.254 exit

Switch2
enable config t interface GigabitEthernet 0/0/1 ip address 210.3.14.1 255.255.255.0 no shutdown exit ip dhcp pool FIRST-POOL network 210.3.14.0 255.255.255.0 default-router 210.3.14.1 dns-server 210.3.14.254 exit

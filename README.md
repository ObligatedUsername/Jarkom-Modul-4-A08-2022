# Jarkom-Modul-4-A08-2022

| **No** | **Nama**                   | **NRP**    |
| ------ | -------------------------- | ---------- |
| 1      | Dhani Rizki A. C. T. P.    | 5025201226 |
| 2      | Khariza Azmi Alfajira H.   | 5025201044 |
| 3      | Farros Hilmi Syafei        | 5025201012 |


## Topologi
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/topologi_soal.jpg) <br>

## CPT Menggunakan VLSM
#### Topologi dengan pembagian subnet
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/topology_w_subnet_VLSM.png) <br>
#### Perhitungan Netmask
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/tabel_jml_IP_VLSM.png) <br>
#### VLSM Tree
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/VLSM_Tree.jpg) <br>
Pembagian IP Dari Tree akan mendapat pembagian IP sebagai berikut <br>
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/tabel%20subnet%20vlsm.jpg) <br>

## GNS3 Menggunakan CIDR
#### Topologi dengan pembagian Subnet
Dapat dilihat di link berikut
[Topologi pembagian subnet menggunakan CIDR](https://www.figma.com/file/lo5zmFVVrsZfndWpW3vkya/CIDR---Modul-4---Jarkom---A08?node-id=0%3A1&t=J80zNCHu2Xs32OIP-1) <br>
#### CIDR Tree
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/cidr_tree.png) <br>
Pembagian IP Dari Tree akan mendapat pembagian IP sebagai berikut <br>
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/tabel_subnet_cidr.png) <br>

**Konfigurasi: The Resonance**
```
auto eth0
iface eth0 inet dhcp
auto eth1
iface eth1 inet static
      address 
      netmask 
auto eth2
iface eth2 inet static
      address 
      netmask 
auto eth3
iface eth3 inet static
      address 
      netmask 
auto eth4
iface eth4 inet static
      address 
      netmask 
```

**Konfigurasi: The Order**
```
auto eth0
iface eth0 inet static
      address 
      netmask
      gateway 
auto eth1
iface eth1 inet static
      address 
      netmask 
auto eth2
iface eth2 inet static
      address 
      netmask 
```

**Konfigurasi: The Minister**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
auto eth1
iface eth1 inet static
      address 
      netmask 
auto eth2
iface eth2 inet static
      address 
      netmask 
```

**Konfigurasi: The Dauntless**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
auto eth1
iface eth1 inet static
      address 
      netmask 
```

**Konfigurasi: The Instrument**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      getaway 
auto eth1
iface eth1 inet static
      address 
      netmask 
auto eth2
iface eth2 inet static
      address
      netmask 
auto eth3
iface eth3 inet static
      address 
      netmask 
```

**Konfigurasi: The Profound**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway
auto eth1
iface eth1 inet static
      address 
      netmask 
auto eth2
iface eth2 inet static
      address 
      netmask 
```

**Konfigurasi: The Firefist**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
auto eth1
iface eth1 inet static
      address 
      netmask 
auto eth2
iface eth2 inet static
      address 
      netmask 
```

**Konfigurasi: The Queen**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway
auto eth1
iface eth1 inet static
      address 
      netmask 
```

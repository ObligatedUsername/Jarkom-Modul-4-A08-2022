# Jarkom-Modul-4-A08-2022

| **No** | **Nama**                   | **NRP**    |
| ------ | -------------------------- | ---------- |
| 1      | Dhani Rizki A. C. T. P.    | 5025201226 |
| 2      | Khariza Azmi Alfajira H.   | 5025201044 |
| 3      | Farros Hilmi Syafei        | 5025201012 |


## Topologi
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/topologi_soal.jpg) <br>

## CPT Menggunakan VLSM
#### Topologi Dengan Pembagian Subnet
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/topology_w_subnet_VLSM.png) <br>
#### Perhitungan Netmask
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/tabel_jml_IP_VLSM.png) <br>
#### VLSM Tree
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/VLSM_Tree.jpg) <br>
Pembagian IP Dari Tree akan mendapat pembagian IP sebagai berikut <br>
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/tabel%20subnet%20vlsm.jpg) <br>
#### Contoh Konfigurasi IP dan Routing Pada CPT
Setelah menentukan dan membuat tabel pembagian IP VLSM lengkap, kita kemudian mengisi konfigurasi IP dan routing pada setiap node di dalam CPT. Berikut contoh konfigurasi IP pada router The Resonance & server The Beast <br>
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/konfigurasi_ip_the_resonance.png) <br><br>
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/konfigurasi_ip_the_beast.png) <br><br>
Dan berikut contoh routing pada The Resonance & The Order <br>
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/routing_the_resonance.png) <br><br>
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/routing_the_order.png) <br><br>
#### Testing
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/testing_vlsm.gif?raw=true) <br><br>

## GNS3 Menggunakan CIDR
#### Topologi Dengan Pembagian Subnet
Dapat dilihat di link berikut
[Topologi pembagian subnet menggunakan CIDR](https://www.figma.com/file/lo5zmFVVrsZfndWpW3vkya/CIDR---Modul-4---Jarkom---A08?node-id=0%3A1&t=J80zNCHu2Xs32OIP-1) <br>
#### CIDR Tree
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/cidr_tree.png) <br>
Pembagian IP Dari Tree akan mendapat pembagian IP sebagai berikut <br>
![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/tabel_subnet_cidr.png) <br>

### CIDR Routing - Setting Network Configuration
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

### CIDR Routing - Setting Host Configuration

**Konfigurasi: Guideau (1000 Host)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
```

**Konfigurasi: Phanora (150 Host)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
```

**Konfigurasi: Johan (100 Host)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
```

**Konfigurasi: Ashaf (50 Host)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
```

**Konfigurasi: Matt Cugatt (120 Host)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway
```

**Konfigurasi: Keith (210 Host)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway
```

**Konfigurasi: Oakleave (500 Host)**
```
auto eth0
iface eth0 inet static
      address 
      netmask
      gateway 
```

**Konfigurasi: The Witch (Server)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
```

**Konfigurasi: The Beast (Server)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
```

**Konfigurasi: Haines (70 Host)**
```
auto eth0
iface eth0 inet static
      address
      netmask 
      gateway 
```
**Konfigurasi: Corvekt (200 Host)**\
```bash
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
```

**Konfigurasi: Spendrow (120 Host)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
```

**Konfigurasi: Helga (70 Host)**
```
auto eth0
iface eth0 inet static
      address 
      netmask 
      gateway 
```

### CIDR Routing - Routing
**The Resonance**
```

```

**The Order**
```

```

**The Minister**
```

```

**The Dauntless**
```

```

**The Magical**
```

```

**The Instrument**
```

```

**The Profound**
```

```

**The Firefist**
```

```

**The Queen**
```

```


### Koneksi Internet
Setiap node diminta agar dapat terhubung dengan internet, maka pada , jalankan command berikut.

```
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 
```

Untuk setiap node selain , jalankan command berikut.

```
echo nameserver  > /etc/resolv.conf
```

Terakhir, mencoba ping ke google.com dari salah satu node.



konfigurasi IP resonance:
```
auto eth1
iface eth1 inet static
 address 10.3.64.1
 netmask 255.255.255.252
auto eth2
iface eth2 inet static
 address 10.3.64.5
 netmask 255.255.255.252
auto eth3
iface eth3 inet static
 address 10.3.68.1
 netmask 255.255.255.252
auto eth3
iface eth3 inet static
 address 10.3.68.1
 netmask 255.255.255.252
 ```

konfigurasi IP beast:
```
auto eth0
iface eth0 inet static
 address 10.3.128.2
 netmask 255.255.255.252
 gateway 10.3.128.1
 ```

routing resonance:
```
route add -net 10.3.16.64 netmask 255.255.255.192 gw 10.3.64.2
route add -net 10.3.16.0 netmask 255.255.255.252 gw 10.3.64.2
route add -net 10.3.12.0 netmask 255.255.252.0 gw 10.3.64.2
route add -net 10.3.9.0 netmask 255.255.255.252 gw 10.3.64.2
route add -net 10.3.8.0 netmask 255.255.255.0 gw 10.3.64.2
route add -net 10.3.34.128 netmask 255.255.255.128 gw 10.3.64.6
route add -net 10.3.34.0 netmask 255.255.255.252 gw 10.3.64.6
route add -net 10.3.2.0 netmask 255.255.254.0 gw 10.3.64.6
route add -net 10.3.1.0 netmask 255.255.255.0 gw 10.3.64.6
route add -net 10.3.0.0 netmask 255.255.255.252 gw 10.3.64.6
route add -net 10.3.33.0 netmask 255.255.255.252 gw 10.3.64.6
route add -net 10.3.32.0 netmask 255.255.255.128 gw 10.3.64.6
route add -net 10.3.32.128 netmask 255.255.255.128 gw 10.3.64.6
route add -net 10.3.70.0 netmask 255.255.254.0 gw 10.3.68.2
```
routing order:
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.3.64.1
route add -net 10.3.12.0 netmask 255.255.252.0 gw 10.3.16.2
route add -net 10.3.9.0 netmask 255.255.255.252 gw 10.3.16.2
route add -net 10.3.8.0 netmask 255.255.255.0 gw 10.3.16.2
```

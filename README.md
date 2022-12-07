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




## Contoh Pengerjaan Soal


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

## Contoh Hasil

![alt text](https://github.com/ObligatedUsername/Jarkom-Modul-4-A08-2022/blob/master/assets/testing_cidr.gif) <br><br>

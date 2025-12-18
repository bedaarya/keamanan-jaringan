# Keamanan Jaringan

Berikut adalah hasil kerja saya:

## Setting up Honeypot (Cowrie)
## 1. Sudo apt update && sudo apt upgrade -y
![](./Honeypot%20VM/step1.png)

## 2. Install dependencies
![Installed Dependencies](./Honeypot%20VM/step2.png)

## 3. Create Cowrie User
![User Created](./Honeypot%20VM/step3.png)

## 4. Install Cowrie 
![Cowrie Installed](./Honeypot%20VM/step4.png)

## 5. Create && Activate Python Virtual Environment
![Environment created](./Honeypot%20VM/step5.png)

## 6. Install Dependencies
![Successfully Installed](./Honeypot%20VM/step6.png)

## 7. Copy Default Config & Start Cowrie Through Virtual Environment
![Start Success](./Honeypot%20VM/step7.png)

## 8. Create A Symlink To The Real Cowrie Script
![Symlink Created](./Honeypot%20VM/step8.png)

## 9. Verify If Symlink Exist & Start Cowrie From Bin/ Command
![bin/cowrie start Succeed](./Honeypot%20VM/step9.png)

## 10. Create A Systemd Service File For Automating Cowrie
![Service File Created](./Honeypot%20VM/step10.png)

## 11. Start Cowrie
![Cowrie Successfully Started](./Honeypot%20VM/step11.png)

## 12. SSH Succeed
![SSH Succeed](./Honeypot%20VM/step12.jpg)

## 13. Double Network Adapter (Nat && Host-Only) & Static IP Setting
![Double Network Adapter Succeed](./Honeypot%20VM/step13.png)

## Setting up Wazuh Manager (Dashboard Included with Manager)

## 1. Installing Wazuh Manager
![Wazuh Manager Installed](./WazuhManager/WazuhManager.png)
![](./WazuhManager/WazuhManager1.png)

## 2. Setting Static IP For Manager VM
![Static IP Done](./WazuhManager/WazuhManager3(1).png)
![Static IP Done](./WazuhManager/WazuhManager3(2).png)


## Wazuh Agent && Dashboard

## 1. Wazuh Agent Installed and running & Connecting To Dashboard
![Wazuh Agent Installed](./Honeypot%20VM/WazuhAgent&Dashboard.png)


## Attack Testing

## 1. Scanning
![Scanning](Screenshot%202025-11-16%20203657.png)
![Scanning](Screenshot%202025-11-16%20203030.png)

## 2. Brute Force
![Brute Force](WhatsApp%20Image%202025-11-17%20at%2007.03.37_93577a88.jpg)
![](Screenshot%202025-11-16%20235621.png)
![](Screenshot%202025-11-17%20082129.png)

## 3. DDOS
![Flooding](Screenshot%202025-11-17%20081324.png)
![](Screenshot%202025-11-17%20081653.png)
##
##

## Pengenalan Firewall di Linux
## Menggunakan iptables (Default di Kali)
## Lihat aturan saat ini:
![](LihatAturan.png)
## Izinkan koneksi dari localhost dan izinkan akses SSH (port 22):
![](IzinkanKoneksi.png)
## Simpan aturan agar tetap ada setelah reboot:
![](SimpanAturan.png)
![](SimpanAturan2.png)
##
## Gunakan iptables untuk Filter Lebih Detail
## Bersihkan aturan lama
![](BersihkanAturanLama.png)
## Menetapkan Kebijakan Default
![](aturandasar2.png)
## Izinkan loopback
![](izinLoopback.png)
## Izinkan koneksi established/related
![](izinEstablish.png)
## Izinkan SSH hanya dari host (192.168.56.1)
![](IzinkanSSH.png)
## Simpan aturan
![](SimpanSemuaAturan.png)
##
##
## Session 1 bidirectional ping
## Ping dari kali ke windows dan windows ke kali
![](PingSession1.png)
## Analisis wireshark
![](WiresharkSession1.png)
## Hasil tcpdump
![](tcpdumpSession1.png)
##
##
## Session 2 Flood Simulation
## lakukan flooding ke ip windows dan analisis menggunakan wireshark
![](WiresharkSession2.png)

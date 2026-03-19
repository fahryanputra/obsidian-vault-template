---
aliases: [Pengelolaan Teknologi Informasi, Pengelolaan TI]
date: 2026-02-03 00:00
tags: [Aplikasi, Infrastruktur, Keamanan, Notulensi]
lokasi: Jakarta
instansi: KLH/BPLH
satuan kerja: Sekretariat Utama
unit kerja: Pusat Data dan Informasi
updated: 2026-03-19 20:41
---

## Infrastruktur Jaringan

### Internet Bandwith

- Kebon Nanas
	- 5050 Mbps Main Link Server
	- 500 Mbps Backup Link dan User
	- Load Balancing 1 Gbps
- Colocation
	- 250 Mbps Server Farm: NIX Jatinegara, Gedung Cyber, Backup Cibinong
- Kuningan
	- 1Gbps user -> 2026 2Gbps

### Data Center

- Kebon Nanas
	- 7 Rak Server
- Colocation
	- 1 Rak Server

### Pengelolaan Server

- Server Pusdatin KLH/BPLH
- Server Satker sebagai penyimpanan dan hosting
- Spek on premise:
	- CPU 160 core
	- Memory 640GB
	- Storage 20TB
- Spek cloud -> DNS, mail:
	- CPU 512 core
	- Memory 4TB
	- Storage 20TB -> potensial 90TB
- Pemindahan aplikasi Bonas ke cloud pada migrasi data center 2026
- Prioritas opsi penyimpanan
	1. Fasilitas data center dan server pusdatin KLH
	2. Fasilitas data center KLH dan server milik satker
	3. PDN
	4. Cloud server/colocation

### Pengelolaan DNS

- Memfasilitasi DNS server klh dengan domain *.kemenlh.go.id
- Infrastruktur server menggunakan server KLH di BoNas

### Pengelolaan Mail Server

- Menggunakan Zimbra mail server on premise
- 771 akun email terdaftar
- Menggunakan multi server untuk kebutuhan email satker, ASN dan kebutuhan lain
	- Mail server
	- Mail border

## Pengamanan Sistem Informasi

### Layanan Secure Socket Layer

- Perpanjang di bulan Desember
- Share SSL kalau menggunakan server sendiri
- Otomatis install SSL pada DC Bonas dan DC NIX Jatinegara

### Firewall

- Fortigate, F5, FortiAnalyzer, Wazuh

### CSIRT

- Workshop
- Peningkatan SDM
	- Threat Hunting
	- Certified Ethical Hacker
	- Kesiapan Teknis Penanganan Insiden Keamanan Siber Sektor Pemerintah Pusat

### Pengamanan SPBE

- PERBAN No.4/2021 -> Tanggung jawab pengembang

## Pengembangan Aplikasi

### Kondisi Aplikasi

- 81% Aktif
- 19% belum aktif
- 0% tidak aktif
- Interoperability menggunakan Confluent
- Datin Hub mendokumentasikan API KLH/BPLH

### Bimtek Aplikasi

- Pembangunan/Pengembangan
- Keamanan Aplikasi
- UAT

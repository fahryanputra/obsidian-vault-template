---
aliases: []
date: 2025-08-06 00:00
tags: [Infrastruktur, Notulensi]
lokasi: Jakarta
instansi: KLH/BPLH
satuan kerja: Sekretariat Utama
unit kerja: Pusat Data dan Informasi
updated: 2026-03-19 20:40
---

## Paparan Teknis

- PT. Daya Kurnia Mandiri
- Melakukan pengadaan barang:
	- Core Switch
	- TOR switch
	- Rak 42U
	- Next Generation Firewall (100F -> 200G)
	- UPS & AC standing floor
- Jangka waktu 87 hari kalender dari Minggu 4 Juni - Minggu 4 September
- Pengiriman barang pada Minggu 1 September
- Item:
	- APC - Smart UPS
	- Cisco - catalyst 9500
	- Cisco catalyst c9200L
	- Daikin - AC Standing 5 PK
	- Dell - Poweredge R760 (2U)
	- Fortinet - Fortigate 200G
	- IndoRack - IR11542P
- Belum punya TOR Switch
- Mereduce serangan dari luar dan dalam dengan Fortigate 200G
- DHCP dari Fortigate dipisah untuk meringankan kinerja Core switch
- Core switch akan difokuskan untuk routing
- Di Kebon Nanas belum ada VLAN
- akan dilakukan pembuatan VLAN
	- VLAN ID - Network
	- 101 - Management 172.16.2.0/24
	- 102 - Farm 172.16.4.0/24
	- 201 - Gedung A
	- 302 - Gedung B
	- 401 - Gedung C
	- 501 - WLAN
- Penyamaan VLAN ID untuk tiap gedung untuk menghindari interferensi

## Kebutuhan Data

- Inventarisasi masing masing port yang digunakan sebagai Access Point
- Diperlukan akses dalam masing-masing perangkat
- Diperlukan file backup masing-masing perangkat
- Diperlukan mapping penempatan barang yang akan dideliver

## Resiko

- Downtime ketika proses penggantian firewall
- Downtime ketika proses pemasangan core switch dan perubahan gateway yang sebelum ada di firewall maka dipindah ke Core
- Ada perubahan besar pada semua interkoneksi switch distribusi yang dimiliki oleh Pusdatin karena sebelumnya hanya menggunakan VLAN default
- Diperlukan inventarisasi masing-masing port yang digunakan sebagai port Access Point

## Diskusi

- 1 AP 1 POE
- TOR Switch hanya ada di DMZ
- Eksisting infrastruktur di jaringan gedung A dan B
- Gedung B menjadi gedung konsultan ingkungan hidup
- Prioritas pekerjaan revitalisasi data center ada di gedung C
- Pemindahan data center utama ke NIX Jatinegara

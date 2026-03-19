---
aliases: []
date: 2026-02-17 00:00
tags: [Aplikasi, IBEQ, Integrasi, Notulensi]
lokasi: Online
instansi: KLH/BPLH
satuan kerja: Deputi Pengendalian Pencemaran dan Kerusakan Lingkungan
unit kerja: Perlindungan dan Pengelolaan Ekosistem Gambut
updated: 2026-03-19 20:29
---

- Sistem Informasi Gambut sudah dimigrasi dari KLHK ke KemenLH
- [SIMATAG](https://gambutindonesia.kemenlh.go.id/simpel/dashboard)
![[Integrasi Sistem Informasi Gambut-1.png]]
- SIMATAG sudah terintegrasi dengan SIMPEL
- Data perusahaan:
	- Tinggi permukaan air tanah
- Sudah develop data logger
- [SiPPEG](https://sippeg.menlhk.go.id/apps)
![[Integrasi Sistem Informasi Gambut-2.png]]
- SIPPEG -> Sistem Informasi Pengelolaan Ekosistem Gambut
- SIPPEG memiliki 8 aplikasi di dalamnya
- SIPALAGA -> Menggunakan data realtime dengan data eks-BRGM
- SIMATAG sudah terintegrasi dalam SiPPEG
- Menonaktifkan website perlu izin Biro Umum

---

## SIPALAGA & SIMATAG

- challenge:
	- backend sistem yang banyak dan dibuat oleh developer yang berbeda
	- backend disajikan dalam 8 aplikasi
- opsi:
	- direct service
	- data replication
- HLD: arsitektur menggunakan pendekatan federated GIS service
- Arsitektur
	- SIPALAGA dan SIMATAG tidak tergantung pada SiPPEG
	- Single visualization layer
	- Standarized GIS Service
	- Layer Registry
- data SIPALAGA merupakan bagian dari data SIMATAG
- SIPALAGA memantau 7 provinsi dengan data realtime
- SIMATAG data seluruh Indonesia
- SIPALAGA sebelumnya merupakan sistem nonaktif
- TMAT Dwi Mingguan merupakan data dari SIMATAG
	- datalogger otomatis 1 bulan 2 kali
	- datalogger 1 bulan sekali
- TIDAK ADA DOKUMENTASI SISTEM SIMATAG DENGAN SERVER WINDOWS
- SIPALAGA BELUM ADA TRANSFER KNOWLEDGE DARI PIHAK BRGM
- 3 domain utama sistem gambut
	- gambutindonesia
	- SiPPEG
	- PKEG KLHK
- Integrasi:
	- Air Gambut BRG -> SIPALAGA
	- Air Gambut KLHK -> SIMATAG
- Server SiPPEG -> H3C
- KLHK web -> Lenovo
- SIMATAG -> Rack Mount hitam di pojok ada yang nyala di tengah

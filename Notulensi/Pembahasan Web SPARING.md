---
aliases: []
date: 2025-07-28 00:00
tags: [Aplikasi, IBEQ, Integrasi, Notulensi]
lokasi: Jakarta
instansi: KLH/BPLH
satuan kerja: Deputi Bidang Pengendalian Pencemaran dan Kerusakan Lingkungan
unit kerja: Direktorat Perlindungan dan Pengelolaan Mutu Air
updated: 2026-03-19 20:39
---

- Pengembangan SPARING masih on progres
- Ada permintaan penambahan fitur dari Deputi Gakkum
- SPARING menjadi salah satu platform feeder data
- PSILH sedang mengembangkan standar untuk SPARING
- Perusahaan yang wajib SPARING namun tidak memasang SPARING terkena denda administratif (Rp10.000.000 - Rp15.000.000) dan wajib melakukan pemasangan SPARING

## Progres Web SPARING

- Dirancang sejak 2018-2019 dan sudah operasional hingga awal tahun 2025
- Mulai dilakukan migrasi sistem dan domain di awal tahun 2025
	1. Menyiapkan domain baru yang dikelola Pusdatin
	2. Mekanisme pengiriman data yang baru
	3. Penyesuaian pada format pengiriman laporan
- Uji konektivitas oleh KLH/BPLH:
	1. Pengajuan vendor
	2. Uji konektivitas
	3. Hasil lulus uji konektivitas

## Kebutuhan Fitur Denda Administratif Baku Mutu

### Melebihi Baku Mutu

[PERMEN LHK 14 2024](https://peraturan.bpk.go.id/Details/309107/permen-lhk-no-14-tahun-2024)

- Denda tidak memasang alat SPARING sebesar Rp15.000.000
- Tahapan SPARING
	1. Pemasangan Alat
	2. Pengoperasian SPARING
	3. Perhitungan beban pencemaran air
	4. Pelaporan data pemantauan kualitas air limbah
- Perhitungan laporan harian per 2 menit yang dikirim tiap jam
- Data per jam adalah data rata-rata konsenterasi aktual dan akumulasi debit
- Data harian sudah tersedia di SPARING
- Data baku mutu sedang on progres dan sudah tersedia di SPARING dan dapat diakses dari platform SIMPEL

## Pengembangan Web SPARING 2025

---

- Perusahaan
	- Pendaftaran alat
	- Pengiriman data
	- Laporan kondisi tidak normal
	- Uji konektivitas individual
	- Alert / teguran melebihi Baku Mutu
	- Perhitungan denda administratif (?)
- Dit PPMA / Admin
	- Periksa laporan SPARING
	- Info laporan melebihi BM
	- Download data
	- Validasi pendaftaran logger
	- Validasi uji konektivitas
- KLH/BPLH
	- Periksa laporan SPARING
	- Info laporan melebihi Baku Mutu
	- Download data
	- Perhitungan denda administratif
- Vendor
	- Pendaftaran vendor
	- Uji konektivitas
- Pemda / Instansi
	- Periksa laporan SPARING
	- Info laporan melebihi Baku Mutu
	- Download data

---

- Perubahan dashboard web SPARING agar memudahkan pengguna untuk memahami data yang ditampilkan (perkiraan kesiapan mock up pada tanggal 4 Agustus 2025)

## Ekosistem Pengendalian Pencemaran Dan Perusakan Lingkungan Hidup

## Kesiapan Arsitektur Server

- Web SPARING termasuk kedalam Integrasi Sistem Pemantauan Kualitas LH
- Pusdatin telah memfasilitasi pada 21 Maret 2025 dengan migrasi data SPARING ke NIX Jatinegara
	- sudah setting server
	- sudah setting backup
- SPARING sudah terintegrasi dengan SIMPEL
- Integrasi beberapa platform ke dalam satu DSS (Decision Support System)
- Pusdatin akan membuat 1 Data Center baru di gedung C lantai 2 (tahun ini)
- NIX Jatinegara akan menjadi backup server bagi server baru di gedung C lantai 2
- Kebutuhan server untuk volume data sangat besar
- Terdapat 3 rak server di NIX Jatinegara Data Center
- Kesiapan arsitektur server diperkirakan pada bulan November
- Beberapa opsi pengadaan server jika server SPARING sudah tidak layak
	- Membeli server baru
	- Sewa server
- Optimalisasi pengiriman data dari per 2 menit menjadi tiap 1 jam
- 3 server SPARING sudah operasional namun belum ada server backup

---

**Rapat lanjutan pada tanggal 14 Agustus 2025**

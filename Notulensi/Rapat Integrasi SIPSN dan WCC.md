---
aliases: []
date: 2026-01-20 00:00
tags: [Aplikasi, Integrasi, Notulensi, SIKPSN]
lokasi: Jakarta
instansi: KLH/BPLH
satuan kerja: Deputi Bidang Pengelolaan Sampah, Limbah, dan Bahan Berbahaya dan Beracun
unit kerja: Direktorat Penanganan Sampah
updated: 2026-03-19 20:45
---

## Pemaparan Hasil Analisa Integrasi SIPSN Dan WCC

### Pendahuluan

- Integrasi sistem SIPSN dan WCC difokuskan pada penyelarasan arsitektur sistem.

### High Level Diagram

- SIPSN dan WCC memiliki DB masing masing
	- SIPSN -> MySQL
	- WCC -> Google Sheet
- Pembentukan Data Warehouse dengan mengintegrasikan DB dari WCC dan SIPSN
	1. Filebase Integration + RClone (WCC)
	2. Backup database (SIPSN)
	3. ETL terjadwal dengan Python
	4. Penyajian dashboard integrasi
- Mekanisme Keamanan dan Kontrol
	1. Kredensial terbatas
	2. Loging
	3. Audit Trail
- Penyajian data pada WCC dan SIPSN tidak selaras

### Implementasi

- Instalasi Server
- Konfigurasi Sistem
- Backup Database SIPSN

## Diskusi

- Pembatasan akses data WCC berdasarkan instruksi dari Menteri KLH/Kepala BPLH
- Skema integrasi untuk jangka pendek
- rekaptpa343@gmail.com sebagai owner spreadsheet database WCC
- Berbagai upaya otomatisasi perhitungan dalam pengolahan data WCC untuk mengurangi perhitungan manual
- Tim Pusdatin KLH/BPLH akan diberikan akses ke spreadsheet WCC
- Usul untuk kedepannya pembuatan SIPSN daerah untuk mengurangi beban transaksi data pada SIPSN pusat
- Memfokuskan pada desentralisasi SIPSN
- Berfokus pada menampilkan data WCC dan SIPSN yang beririsan
- Integrasi dashboard WCC dan SIPSN dalam satu Dashboard Pengelolaan Sampah
- Todo List
	- Persiapkan akses database Persampahan
	- Setting Batch update, export sheet
	- Akses IP Publik database SIPSN
	- Menggunakan lookerstudio sebagai visualization tools

## Pain Point

- Belum bisa identifikasi data yang masuk ke dalam WCC
- Perbedaan istilah pada WCC dan SIPSN
- Belum ada akses pada DB WCC
- Sistem monitoring dan tracking sampah belum optimal
- Masih banyak data redundansi
- Kesulitan dalam pengumpulan data dari pengepul sampah

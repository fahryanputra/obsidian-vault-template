---
aliases: []
date: 2025-08-27 00:00
tags: [Aplikasi, Notulensi]
lokasi: Jakarta
instansi: KLH/BPLH
satuan kerja: Sekretariat Utama
unit kerja: Pusat Data dan Informasi
updated: 2026-03-19 20:48
---

- Sudah tersedia desain sistem Pengaduan dan Monitoring pada Website KLH/BPLH
- Sistem pengaduan internal dari GAKKUM, Inspektorat dan Humas yang tidak melalui SPAN Lapor
- Desain landing page sudah tersedia
- Data dari SPAN Lapor dan Aduan tindak lanjut secara manual

## Dashboard

- Desain Dashboard sudah tersedia
- Admin tidak perlu membuka SPAN Lapor untuk melihat summary data pengaduan
- Desain visualisasi data aduan dari SPAN Lapor dan manual sudah tersedia
- Transaksi monitoring dimana admin dapat menambahkan aduan baru
- Role:
	1. Admin (Pusdatin, Humas)
	2. PIC
- PIC dan admin dapat melampirkan file dan pesan aduan
- Desain detail data laporan pengaduan dari masyarakat sudah tersedia dalam bentuk read-only
- Mengambil data lapor secara otomatis menggunakan Cronjob dan Selenium

## Usulan Dan Masukan

- Tambahan menu pada tampilan depan yang mengarah ke SPAN Lapor, Pengaduan Gakkum dan Pengaduan Irtama
- Menu pengaduan internal akan diletakkan pada submenu pengaduan
- Hanya admin yang bisa merubah status pengaduan
- Terdapat CAPTCHA dan dilakukan pentest berkala untuk memastikan keamanan sistem
- Server akan berlokasi di Pusdatin

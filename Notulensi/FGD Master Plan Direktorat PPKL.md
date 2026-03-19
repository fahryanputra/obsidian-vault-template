---
aliases: [Master Plan PPKL]
date: 2025-08-28 00:00
tags: [Aplikasi, IBEQ, Integrasi, Notulensi]
lokasi: Bekasi
instansi: KLH/BPLH
satuan kerja: Deputi Bidang Pengendalian Pencemaran dan Kerusakan Lingkungan
unit kerja: Direktorat Perlindungan dan Pengelolaan Mutu Air
updated: 2026-03-19 20:29
---

## Arahan Deputi PPKL

	Rasio Ridho Sani
- Deputi PPKL KLH Ingin membangun sebuah sistem dengan ownership yang kuat
- Banyak sistem yang tidak sustain karena ownership yang kurang kuat
- Master plan ini adalah satu upaya pemantauan kualitas lingkungan
- Akan digunakan oleh publik dan harapannya dapat digunakan dengan baik
- Terdapat 35 aplikasi aktif yang sistemnya belum terintegrasi
- Pusdatin membantu integrasi berbagai sistem PPKL
- Setelah proses pengembangan selesai, PPKL akan memiliki ownership dari sistem tersebut

## Arahan Kapusdatin

	Ir. Hari Wibowo
- IBEQ AI merupakan bagian dari SPBE KLH/BPLH
- Merupakan salah satu program prioritas di Pusdatin
- Satu domain penting yaitu layanan SPBE
- SPBE akan migrasi ke PemDig pada tahun 2026
- Sudah terbentuk Integrated DSS pada tahun 2025
- Ada sekitar 38-39 aplikasi
- Akan ada 5 sistem besar:
	- SIMPEL
	- AMDALNET
	- SIPSN
	- SRN
	- E-Gakkum
- Fokus pada permasalahan keamanan dan layanan sistem terintegrasi
- Sistem integrasi akan menjadi alat bantu pengambilan keputusan dan sebagai informasi publik

## Integrated Big Data Environmental Quality (IBEQ) AI

- Merupakan integrasi sistem pemantauan kualitas lingkungan hidup
- Integrasi big data kualitas lingkungan melalui *Artificial Intelligence*
- Merupakan Datamart untuk penggunaan bersama data kualitas lingkungan hidup dengan stakeholder lainnya
- Digunakan untuk membantu proses pengambilan kebijakan
- Sebagai *Early Warning* pencemaran dan kerusakan lingkungan hidup

## Master Plan Teknologi Informasi (MPTI)

- Tujuan MPTI untuk mendukung fungsi inti deputi 2, meningkatkan keputusan berbasis data, meningkatkan pemantauan dan pengendalian lingkungan, serta mempercepat transformasi digital yang sejalan dengan tujuan pengelolaan lingkungan nasional
- MPTI merujuk pada peta rencana pemerintahan digital dari Pusdatin
- Banyak instansi yang belum mendefinisikan secara detail mengenai sistem PemDig
- Konsep pembuatan layanan digital berawal dari proses bisnis dan SOTK
- Nama layanan merupakan hal penting yang harus didefinisikan terlebih dahulu
- Menggunakan *framework* TOGAF

## Kondisi Existing Arsitektur PPKL

![[FGD Master Plan Direktorat PPKL-1.png]]

- Terlihat pada gambar bahwa sistem belum terintegrasi
- Fokus pada integrasi sistem
- Sistem existing PPKL masih oversize dengan jumlah sub domain (aplikasi) yang cukup banyak
- Ruangan monitoring PPKL tidak dirancang dan didesign sebagai sebuah pusat monitoring atau kontrol
- Infrastruktur tidak memadai sebagai sarana prasarana dalam pemantauan

## Harapan Arsitektur PPKL

![[FGD Master Plan Direktorat PPKL-2.png]]

- Diharapkan menggunakan Microservice kedepannya
- Diperlukan identifikasi dan validasi data dalam data warehouse PPKL
- Pembangunan Operation Room PPKL untuk pemantauan kualitas lingkungan secara real-time
- Penghapusan domain dan sub domain nonaktif
- Pengurangan 41 aplikasi menjadi 12 aplikasi yang akan dirangkum dalam 7 aplikasi IBEQ
	- Air Quality
	- River Quality
	- Biodiversity
	- Coastal and Marine
	- Forest
	- Industrial
	- IKLH
- IBEQ - HUB sebagai penghubung antar layanan PPKL
- Pusdatin memiliki Grand Design TI KLH/BPLH
- Data & Application Custodian (Pusdatin)
- Data ownership (PPKL)

## Indeks Kualitas Lingkungan Hidup (IKLH)

- IKLH merupakan hasil dari integrasi berbagai sistem
- Data geospasial harus ditingkatkan lagi
- Akan ada integrasi SITALA dan E-GIS
- E-GIS menggunakan ArcGis
- SITALA/IKLH tadinya hanya untuk mengumpulkan data kualitas lingkungan gabungan semua direktorat yang ada di PPKL
- IKLH merupakan komposit dari indeks kualitas air, udara, air laut dan lahan
- Indeks kualitas lahan terdiri dari:
	- Indeks kualitas tutupan lahan
	- Indeks kualitas gambut
- Butuh Sekretariat IKLH yang berfungsi mengatur tata kelola pelaksanaan perhitungan indeks
- Tahapan perhitungan indeks
	1. Pemantauan
	2. Pengujian
	3. Input Data
	4. Verifikasi
	5. Output nilai IKLH
- Sebagian besar merupakan data tabular
- Data titik pantau merupakan data spasial
- Menggunakan 8 parameter kunci karena 23 parameter membutuhkan resource yang besar
- SITALA/IKLH masih ada di server sharing dengan license yang out of date
- IKLH termasuk kedalam data prioritas Pusdatin tingat menengah 2025-2029
- Mengambil data prioritas tahun 2024 untuk diajukan sebagai data prioritas ke Bappenas
- Akses data menjadi fokus Pusdatin

## Perlindungan Dan Pengelolaan Mutu Udara

- ISPU sudah digunakan secara nasional
- Gap ISPU
	- Padat dengan overlay
	- Minim kontrol waktu
	- Keterbasan filter & pencarian
	- Informasi titik sensor minim
	- Keterbacaan legenda & UI
	- Tidak responsif dan aksesibilitas terbatas
	- Belum ada notifikasi
	- Kurangnya ekspor data dan API terbuka
![[FGD Master Plan Direktorat PPKL-3.png]]
- Perlu melakukan tambahan sistem atau sub sistem untuk melakukan prediksi pencemaran
- Rekomendasi pengembangan ISPU akan didefinisikan pada program kerja di MPTI

___

- Lokasi pada peta di aplikasi SISPEK tidak akurat
- Gap SISPEK
	- Keterlambatan data
	- Keterbatasan filter
	- Ketidakjelasan visualisasi
	- Panel informasi yang minim
	- Keterbatasan histori
	- Kurangnya aspek keamanan dan privasi
	- Skalabilitas dan performa
![[FGD Master Plan Direktorat PPKL-4.png]]

___

- SIMPEL sudah berjalan dengan AMDALNET menggunakan SSO
- SIMPEL akan menjadi salah satu layanan utama KLH/BPLH
- SIMPEL AIR, SIMPEL LAHAN dan SIMPEL UDARA akan tetap terpisah
- Sudah integrasi akun dengan AMDALNET
- Server SIMPEL berlokasi di Colocation Semut Data

## Diskusi Developer

- Pengujian aplikasi akan dilakukan di server Pusdatin
- Pusdatin akan membangun repository untuk aplikasi
- Usahakan jangan menggunakan framework yang monolitik
- Pengembangan menggunakan layanan bersifat *microservices*
- List repository prioritas yang akan migrasi ke Pusdatin
	- SIMPEL
	- Aplikasi berbasis sensor (SPARING, ONLIMO, SISPEK, ISPU)
	- SIUMI
- SiMATAG bersifat rahasia, khusus untuk perusahaan
- Akan ada 6000 device SiMATAG yang tersambung ke KLH/BPLH
- Jika perusahaan tidak punya server maka akan menggunakan server KLH/BPLH
- SiMATAG akan terintegrasi dengan SIMPEL sebagai penilaian PROPER
- SIMPEG memiliki license ArcGIS Enterprise
- SIMPEG terdiri dari 7 server dan 1 NAS
- Source Code akan masuk di GitHub
- Proses migrasi repository aplikasi ke Pusdatin akan mulai pada September 2025 dimulai dari sistem prioritas
- Pengisian spesifikasi teknis (<https://ppkl.link/SpekTeknisAplikasiPPKL>)

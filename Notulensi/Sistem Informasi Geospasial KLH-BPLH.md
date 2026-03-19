---
aliases: []
date: 2025-07-23 00:00
tags: [Aplikasi, EGIS, Integrasi, Notulensi]
lokasi: Jakarta
instansi: KLH/BPLH
satuan kerja: Sekretariat Utama
unit kerja: Pusat Data dan Informasi
updated: 2026-03-19 20:48
---

## WEBGIS: -EGIS KLH

<https://egis.kemenlh.go.id>

- Kedepannya menjadi salah satu fitur dalam grand design
- Menampilkan 31 bentuk data spasial existing di KLH/BPLH yang diambil dari [SIGAP](https://sigap.menlhk.go.id/)
- Pengusulan 28 bentuk data baru dalam KLH/BPLH
- Akan ditambah 200 data geospasial dari Inventarisasi Lingkungan Hidup: Mengkoleksi data lingkungan hidup, QC dan pengolahan data
- Rencana pembuatan Sistem Perencanaan RPPLH
- Kebutuhan berbagi pakai dari internal KLH/BPLH dan eksternal
- Untuk internal KLH/BPLH langsung dari database selama SI belum terbentuk (selama masa transisi) target Agustus 2025
- Pintu akses data spasial berada di PLSDAB
- Salah satu pengguna internal adalah PDLUK
- Launching di bulan Agustus 2025
- Sounding EA dan proses SI ke Pusdatin
- Arsitektur
	1. Database (Postgre database dengan extension PostGIS )
	2. Mapserver -> REST (WMS, Vector Tiles, KML, GeoJSON)
	3. Interface (WebGIS, StoryMap, Vue3, OpenLayers, PDF JS, Turn JS)
	4. Tile Map Service (OSM, ArcGIS Online, Here)
	5. Backend (Golang, Python)
- Kelemahan [SIGAP](https://sigap.menlhk.go.id/), orang dapat mengakses vector secara langsung diatasi dengan MBTiles Map Server
- Tenaga GIS existing untuk pengolahan peta
- Membutuhkan programmer GIS untuk pengolahan data

---

---

## Pengembangan Sistem Informasi Geospasial KLH/BPLH

Sebagai bagian dari implementasi *Grand Design* SPBE, KLH/BPLH tengah mengembangkan sistem informasi spasial (<https://egis.kemenlh.go.id>) yang direncanakan menjadi salah satu fitur utama. Sistem ini bertujuan untuk mendukung perencanaan, pengelolaan, serta kebutuhan berbagi pakai data spasial, baik untuk kepentingan internal KLH/BPLH maupun pihak eksternal.

Saat ini, telah tersedia 31 bentuk data spasial eksisting yang bersumber dari platform [SIGAP](https://sigap.menlhk.go.id/), dan telah diusulkan penambahan sebanyak 28 bentuk data baru. Selain itu, direncanakan penambahan kurang lebih 200 data geospasial yang akan diperoleh melalui bagian Inventarisasi Lingkungan Hidup, yang mencakup proses pengumpulan, pengolahan, dan *quality control* data.

Dalam masa transisi menuju sistem informasi yang utuh, akses internal KLH/BPLH terhadap data spasial akan difasilitasi langsung dari basis data, dengan target implementasi penuh pada bulan Agustus 2025. Pintu akses utama data spasial akan dikelola oleh PLSDAB, dan salah satu unit pengguna internal yang telah diidentifikasi adalah PDLUK.

Peluncuran awal sistem direncanakan pada bulan Agustus 2025, seiring dengan proses *sounding* arsitektur sistem dan koordinasi pengembangan sistem informasi ke Pusdatin.

Secara teknis, arsitektur sistem dirancang sebagai berikut:

1. **Basis Data**: Postgre dengan extension PostGIS sebagai sistem manajemen basis data spasial.
2. **Map Server**: Penyedia layanan REST (WMS, Vector Tiles, KML, GeoJSON).
3. **Antarmuka**: WebGIS berbasis Vue3 dan OpenLayers, dilengkapi dengan fitur StoryMap, PDF JS, dan Turn JS.
4. **Tile Map Service**: Menggunakan sumber peta dasar dari OSM, ArcGIS Online, dan HERE.
5. **Backend**: Menggunakan bahasa pemrograman Golang dan Python.

Sebagai catatan, salah satu kelemahan dari platform [SIGAP](https://sigap.menlhk.go.id/) adalah terbukanya akses langsung terhadap data vektor. Hal ini akan diantisipasi dengan penggunaan *MBTiles Map Server* untuk memastikan keamanan dan keterbatasan akses terhadap data spasial.

Dari sisi sumber daya, saat ini telah tersedia tenaga teknis GIS untuk pengolahan peta. Namun, dibutuhkan tambahan personel dengan kompetensi pemrograman GIS guna mendukung proses pengolahan data dan pengembangan sistem lebih lanjut.

![[Sistem Informasi Geospasial KLH-BPLH-1.jpeg]]![[Sistem Informasi Geospasial KLH-BPLH-2.jpeg]]![[Sistem Informasi Geospasial KLH-BPLH-3.jpeg]]![[Sistem Informasi Geospasial KLH-BPLH-4.jpeg]]

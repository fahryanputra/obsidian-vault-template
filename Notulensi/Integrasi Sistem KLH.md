---
aliases: []
date: 2025-06-16 00:00
tags: [Aplikasi, DSS, Integrasi, Notulensi]
lokasi: Jakarta
instansi: KLH/BPLH
satuan kerja: Sekretariat Utama
unit kerja: Pusat Data dan Informasi
updated: 2026-03-19 20:30
---

## Notulensi Integrasi System KLH - Senin, 16 Juni 2025

- Integrasi khusus urusan perusahaan
- Integrasi dari segala deputi
- [AMDAL NET](https://www.menlhk.go.id/public-service/amdal-klhk/) - [SIMPEL(deputi 2)](https://simpel.menlhk.go.id/2023/login) - [SIPSN](https://sipsn.menlhk.go.id/sipsn/) - [SRN](https://srn.menlhk.go.id/index.php?r=home%2Findex) - GAKKUM LH(seksi administratif, pidana, sengketa)
- Menteri request fokus di [SIPSN](https://sipsn.menlhk.go.id/sipsn/)

### Next Follow up

- Menunggu kebutuhan data dari Gakkum untuk pusdatin menyiapkan tools (perpindahan data dari manggala)
- Spec server existing gakkum (menunggu dari Pak Budi)
- Data existing infrastruktur (total rack server, ram, storage, vm alokasi & sisa, nas)

### Timeline

- Critical: Perencanaan (Juli 2025) - Proses administrasi pengadaan
- Development (fase 1, 2) - agustus-nov 2025
- implementasi - desember 2025

#### Issue

- implementasi superapps dgn 4 bulan tdk memungkinkan, solusinya menggunakan DSS integrasi sistem 3-5 sistem.
- Anggaran besar bisa didapatkan dengan e-catalog

### Flow DSS

1. Amdalnet pintu pertama utk kelayakan lingkungan RKL Rencana Pemulihan Lingkungan
2. Setelah dipenuhi oleh perusahaan maka ada UKL/UPL - sampah ([SIPSN](https://sipsn.menlhk.go.id/sipsn/)), karbon ( [SRN](https://srn.menlhk.go.id/index.php?r=home%2Findex)), [SIMPEL(deputi 2)](https://simpel.menlhk.go.id/2023/login) (reporting-blm ada integrasi dgn srn)
3. if perusahaan tidak cocok dgn ukl/upl, then masuk Gakkum

### Solusi

- Decision Support System Cleansing data oleh Pusdatin
- Memiliki seluruh keyword yg memungkinkan tampil data spasial termasuk status proper perusahaan dan detailnya

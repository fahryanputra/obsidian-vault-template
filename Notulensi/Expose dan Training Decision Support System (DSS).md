---
aliases: [Expose DSS, Training DSS]
date: 2026-01-29 00:00
tags: [Aplikasi, DSS, Integrasi, Notulensi]
lokasi: Jakarta
instansi: KLH/BPLH
satuan kerja: Sekretariat Utama
unit kerja: Pusat Data dan Informasi
updated: 2026-03-19 20:30
---

## Expose DSS

- AgentLH menggunakan Gemini yang terintegrasi dengan BigQuery
- Data local menggunakan PostgreSQL untuk user management
- Kafka belum terkoneksi dengan source DB, hanya dapat akses ke backup DB
- 3 juta record data perusahaan amdal
- DSS tidak melakukan update data
- AmdalNET terakhir update 6 Desember
- SIMPEL terakhir update 23 November
- Data live -> AMDAL, SIMPEL, PUSARPEDAL, GAKKUM
- Tidak ada tabel master NIB
- SKKL -> RKL & RPL
- PPKLH -> UKL & UPL (diterbitkan oleh pemda)
- 2 DB AMDAL -> amdalnet_ublic & amdalnet_perubahan_pl

## Training DSS

### Confluent

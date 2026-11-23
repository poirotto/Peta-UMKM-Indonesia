# Peta UMKM Indonesia 2025

Dashboard 3D interaktif yang memetakan sebaran usaha mikro, kecil, dan menengah (UMKM) di 38 provinsi Indonesia berdasarkan data Kementerian UMKM tahun 2025.

**Demo:** https://poirotto.github.io/Peta-UMKM-Indonesia/

## Fitur

- Peta isometrik 38 provinsi dengan tumpukan koin yang tingginya mengikuti indikator terpilih.
- Empat indikator: jumlah UMKM, naik kelas (proporsi usaha kecil dan menengah), formalitas (berbadan hukum atau berpembukuan lengkap), dan rasio buruh tetap.
- Kartu ringkasan nasional, tren jumlah UMKM 2020 sampai 2025, dan sorotan temuan per indikator.
- Bilah 38 provinsi yang terhubung dengan peta, serta pencarian provinsi.
- Klik provinsi untuk masuk ke diorama pasar berisi 200 usaha yang menggambarkan komposisi skala usaha dan formalitas provinsi tersebut, lengkap dengan perbandingan terhadap angka nasional.
- Tautan langsung ke provinsi tertentu, misalnya `#jawa-barat`.

## Sumber data

- Kementerian UMKM, Data Prioritas Capaian 2025 (Biro Data dan Teknologi Informasi).
- Kementerian UMKM, UMKM dalam Angka: Data Makro UMKM Indonesia 2020–2024.
- Batas provinsi: [Indonesia GeoJSON & TopoJSON Maps (38 Provinces)](https://github.com/denyherianto/indonesia-geojson-topojson-maps-with-38-provinces), lisensi [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), telah disederhanakan.

Beberapa provinsi mencatat angka 0 untuk usaha menengah atau besar. Angka ini kemungkinan muncul karena keterbatasan sampel survei, bukan karena usahanya tidak ada. Posisi lapak di diorama hanya ilustrasi.

## Teknologi

Satu file HTML statis tanpa proses build. Grafik 3D memakai [Three.js](https://threejs.org/) yang dimuat dari CDN jsDelivr, sehingga halaman membutuhkan koneksi internet.

## Menjalankan secara lokal

```sh
python3 -m http.server 8000
# lalu buka http://localhost:8000
```

## Publikasi lewat GitHub Pages

Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main`, folder `/ (root)` → Save.

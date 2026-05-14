# Sistem Fuzzy Logic - Seleksi 5 Restoran Terbaik

**Mata Kuliah:** Kecerdasan Buatan  
**Program Studi:** S1 Rekayasa Perangkat Lunak  
**Universitas:** Telkom  

## Deskripsi

Program ini menggunakan logika fuzzy untuk mengevaluasi dan memilih 5 restoran terbaik berdasarkan kriteria kualitas pelayanan dan harga. Sistem ini dibangun secara manual tanpa menggunakan library fuzzy eksternal seperti scikit-fuzzy.

### Fitur Utama
- **Fuzzifikasi**: Mengubah input crisp menjadi nilai fuzzy.
- **Inferensi**: Menggunakan metode Mamdani dengan operator MIN untuk AND dan MAX untuk agregasi.
- **Defuzzifikasi**: Menggunakan metode Centroid (Center of Area) untuk menghasilkan output crisp.

## Persyaratan Sistem

- Python 3.x
- Library: `openpyxl` (untuk membaca/menulis file Excel)

## Instalasi dan Setup

1. **Install Python 3.x** jika belum terinstall.
2. **Install dependensi**:
   ```
   pip install openpyxl
   ```
3. **Persiapkan file data**: Letakkan file `restoran.xlsx` di folder yang sama dengan `fuzzy_restoran.py`, atau sesuaikan path `input_file` di kode.

## Cara Menjalankan

Jalankan perintah berikut di terminal:
```
python fuzzy_restoran.py
```

## Output

- **Terminal**: Menampilkan 5 restoran terbaik beserta skor kelayakan.
- **File Excel**: `peringkat.xlsx` berisi daftar 5 restoran terbaik dengan kolom:
  - Peringkat
  - ID Restoran
  - Kualitas Pelayanan
  - Harga
  - Skor Kelayakan

## Catatan Teknis

- Program tidak menggunakan library fuzzy apapun; semua proses dibangun dari nol.
- Metode defuzzifikasi: Centroid.
- Metode inferensi: Mamdani.

## Kontribusi

Untuk pertanyaan atau kontribusi, silakan buat issue atau pull request di repository ini.
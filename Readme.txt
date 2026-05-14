============================================================
  SISTEM FUZZY LOGIC - SELEKSI 5 RESTORAN TERBAIK
  Mata Kuliah: Kecerdasan Buatan
  S1 Rekayasa Perangkat Lunak - Universitas Telkom
============================================================

CARA MENJALANKAN PROGRAM
--------------------------
1. Pastikan Python 3.x sudah terinstall.
2. Install dependensi (hanya openpyxl untuk baca/tulis xlsx):
       pip install openpyxl
3. Letakkan file restoran.xlsx di folder yang sama, ATAU
   sesuaikan path input_file di bagian bawah fuzzy_restoran.py.
4. Jalankan program:
       python fuzzy_restoran.py

OUTPUT
--------------------------
- Tampilan di terminal: 5 restoran terbaik beserta skor.
- File peringkat.xlsx: daftar 5 restoran terbaik dengan kolom
  Peringkat, ID Restoran, Kualitas Pelayanan, Harga, Skor Kelayakan.

CATATAN
--------------------------
- Program TIDAK menggunakan library fuzzy (scikit-fuzzy, dll).
- Semua proses (fuzzifikasi, inferensi, defuzzifikasi) dibangun manual.
- Metode defuzzifikasi: Centroid (Center of Area).
- Metode inferensi: Mamdani (operator MIN untuk AND, MAX untuk agregasi).

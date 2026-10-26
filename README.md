# Pertemuan 13 - Debugging dan Testing
Nama: RIKI AGIL SAPUTRA


NIM: 2225250026


Kelas:3A 
## Kasus
Program yang diuji merupakan sebuah program untuk mengetahui berapa rata-rata dari data nilai yang diberikan, status kelulusa untuk nilai 60, dan untuk mengetahui berapa nilai tertinggi dari data nilai yang diberikan.
## Test Case

| ID | Input | Expected | Actual Awal | Status |
| :--- | :--- | :--- | :--- | :--- |
| T1 | 75 | Lulus | Lulus | PASS |
| T2 | 60 | Lulus | Tidak lulus | FAIL |
| T3 | 59 | Tidak lulus | Tidak lulus | PASS |

## Bug Report

| gejala | lokasi | Akar penyebab | Perbaikan |
| :--- | :--- | :--- | :--- |
| Output aktual yang salah/error | Praktik_4_debugging/rata_rata/2 | Fungsi rata_rata yang membagi total tidak sesuai jumlah banyaknya data nilai yang diberikan | Mengubah pembagi total data pada fungsi data menjadi len (nilai) |
| Output aktual yang salah/error | Praktik_4_debugging/rata_rata/2 | Fungsi rata_rata yang membagi total tidak sesuai jumlah banyaknya data nilai yang diberikan | Mengubah pembagi total data pada fungsi data menjadi len (nilai) |
| Output aktual yang salah/error | Praktik_4_debugging/status/5 | Batas pengkondisian di dalam fungsi status yang tidak memasukkan nilai 60 ke dalam batas | Mengubah batas pengkondisian if di dalam fungsi status menjadi >= |

## Retest

| ID | INPUT | EXPECTED | ACTUAL PERBAIKAN | STATUS |
| :--- | :--- | :--- | :--- | :--- |
| T1 | [80, 60, 90, 70] | 75.0 | 75.0 | PASS |
| T2 | [100, 80] | 90.0 | 90.0 | PASS |
| T3 | 60 | Lulus | Lulus | PASS |
| T4 | 59 | Tidak lulus | Tidak lulus | PASS |
| T5 | [80, 60, 90, 70] | 90 | 90 | PASS |
.
## Cara Menjalankan
python3 praktik/praktik_4_debugging.py
## Refleksi
teknik debugging berdasarkan hipotesis dikarenakan teknik tersebut dilakukan secara runtut dan sistematis sehingga langkah-langkah yang dilakukan mempunyai urutan yang pasti dan tidak berantakan, sehingga bug yang ada dapat dengan mudah ditemui dikarenakan langkahnya yang sistematis.
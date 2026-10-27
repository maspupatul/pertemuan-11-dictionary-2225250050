# Pertemuan 11 - Dictionary/Map

**Nama:** Maspupatul Hasanah 
**NIM:** 2225250050
**Kelas:** 3A (Pendidikan Matematika)

## Tujuan
Mempelajari penggunaan dictionary dalam Python untuk menyimpan dan mengelola data pendidikan menggunakan pasangan key-value. Program ini juga menerapkan operasi pencarian, penambahan, perubahan, dan penelusuran data mahasiswa.

## Struktur Data
Program menggunakan dictionary dengan NIM sebagai key utama. Setiap NIM memiliki value berupa dictionary yang menyimpan nama, kelas, dan nilai mahasiswa.

Contoh struktur data:

```python
data_mahasiswa = {
    "A001": {"nama": "Ayu", "kelas": "A", "nilai": 85},
    "A002": {"nama": "Budi", "kelas": "A", "nilai": 78},
    "A003": {"nama": "Citra", "kelas": "B", "nilai": 92},
    "A004": {"nama": "Deni", "kelas": "B", "nilai": 74},
    "A005": {"nama": "Eka", "kelas": "A", "nilai": 88}
}
```

Dictionary digunakan agar data mahasiswa dapat dicari berdasarkan NIM tanpa harus mengetahui posisi indeksnya. Fungsi `get()` digunakan untuk mengakses data dengan lebih aman ketika NIM mungkin tidak tersedia.

## Fitur Program
1. Menyimpan data minimal lima mahasiswa.
2. Mencari data mahasiswa berdasarkan NIM.
3. Menampilkan pesan jika data mahasiswa tidak ditemukan.
4. Menambahkan data mahasiswa baru.
5. Mengubah nilai mahasiswa.
6. Menampilkan seluruh data menggunakan `items()`.
7. Menghitung rata-rata nilai mahasiswa.
8. Menggunakan fungsi untuk pencarian dan perhitungan rata-rata nilai.

## Cara Menjalankan
1. Buka folder proyek di Visual Studio Code.
2. Pastikan Python sudah terpasang.
3. Buka terminal pada folder utama proyek.
4. Jalankan perintah berikut:

```bash
python praktik/data_mahasiswa.py
```

Jika perintah tersebut tidak dapat digunakan, coba sesuaikan dengan konfigurasi Python di komputer.

## Test Case

| No. | Pengujian | Input/Aksi | Hasil yang Diharapkan |
|---|---|---|---|
| 1 | Pencarian data tersedia | NIM A003 | Data mahasiswa Citra ditampilkan |
| 2 | Pencarian data tidak tersedia | NIM A999 | Pesan "Data tidak ditemukan" ditampilkan |
| 3 | Pembaruan nilai | Nilai A002 diubah menjadi 82 | Nilai Budi berubah menjadi 82 |
| 4 | Penambahan mahasiswa | Menambahkan NIM A006 | Data A006 tersimpan dalam dictionary |
| 5 | Menampilkan seluruh data | Menggunakan `items()` | Semua NIM dan data mahasiswa ditampilkan |
| 6 | Menghitung rata-rata | Menggunakan fungsi rata-rata | Rata-rata nilai seluruh mahasiswa ditampilkan |

## Refleksi
Melalui praktikum ini, saya memahami bahwa dictionary dapat digunakan untuk menyimpan data dalam bentuk pasangan key-value. Penggunaan NIM sebagai key memudahkan pencarian data mahasiswa. Saya juga mempelajari perbedaan akses menggunakan tanda kurung siku dan fungsi `get()`. Jika key yang dicari tidak tersedia, akses menggunakan tanda kurung siku dapat menghasilkan `KeyError`, sedangkan `get()` dapat digunakan untuk menghindari kesalahan tersebut. Selain itu, saya memahami cara menambah, mengubah, dan menampilkan data menggunakan dictionary.

## Kesimpulan
Dictionary merupakan struktur data yang berguna untuk mengelola data berdasarkan key. Dengan menggabungkan dictionary, list, perulangan, dan fungsi, program pengelolaan data mahasiswa dapat dibuat lebih terstruktur dan mudah diuji.
# data_akuisisi_kebutuhan_storage
# Praktikum 6 – Klasifikasi Jenis Data

## Deskripsi
Praktikum ini bertujuan untuk memahami dan mengklasifikasikan berbagai jenis data berdasarkan struktur, cara membaca menggunakan Python, serta media penyimpanan yang sesuai.

Praktikum dikerjakan menggunakan Google Colab dengan bantuan library Pandas.

## Tujuan Praktikum
1. Memahami perbedaan Structured, Semi-structured, dan Unstructured Data.
2. Mengetahui cara membaca berbagai format berkas menggunakan Python.
3. Menentukan media penyimpanan yang sesuai untuk setiap jenis data.
4. Menyimpan hasil klasifikasi dalam format CSV.

## Tools yang Digunakan
- Google Colab
- Python
- Pandas
- Visual Studio Code
- GitHub

## Struktur Folder
```text
Praktikum_6/
├── docs/
│   └── klasifikasi_jenis_data.csv
├── praktikum_6_klasifikasi_data.ipynb
└── README.md
```

## Hasil Praktikum

Hasil klasifikasi terdiri dari 9 berkas dengan kategori Structured, Semi-structured, dan Unstructured Data.

| Berkas | Jenis Data | Cara Membaca |
|---|---|---|
| destinasi.csv | Structured | pd.read_csv() |
| destinasi.xlsx | Structured | pd.read_excel() |
| ulasan.json | Semi-structured | pd.read_json() |
| katalog.xml | Semi-structured | pd.read_xml() |
| contoh.png | Unstructured | PIL.Image.open() |
| Teks bebas | Unstructured | open().read() |
| anggota_sanggar.csv | Structured | pd.read_csv() |
| jadwal_latihan.json | Semi-structured | pd.read_json() |
| foto_tarian.jpg | Unstructured | PIL.Image.open() |

## Penyimpanan Hasil

Hasil klasifikasi disimpan dalam folder `docs` dengan nama file `klasifikasi_jenis_data.csv`.

Kode yang digunakan:

```python
import os

os.makedirs("docs", exist_ok=True)

df.to_csv("docs/klasifikasi_jenis_data.csv", index=False)
```

## Kesimpulan

Melalui praktikum ini, saya memahami bahwa setiap jenis data memiliki struktur dan cara pengolahan yang berbeda. Data Structured cocok disimpan dalam basis data relasional, data Semi-structured dapat menggunakan database dokumen atau NoSQL, sedangkan data Unstructured dapat disimpan menggunakan file storage atau object storage.

Hasil praktikum berhasil disimpan dalam format CSV untuk memudahkan pengelolaan dan dokumentasi data.

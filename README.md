# 🧩 Tugas Pertemuan 10 — Upload Data Menggunakan File CSV

Proyek ini merupakan lanjutan dari tugas sebelumnya (Pertemuan 9) dan berfokus pada **penerapan fitur upload file CSV** untuk memasukkan data ke dalam database secara otomatis menggunakan Java Swing dan JDBC.

---

## 🚀 Deskripsi Proyek

Dalam proyek ini, pengguna dapat:
- Mengunggah (upload) file **CSV** berisi data `mata_kuliah`.
- Sistem akan membaca isi file tersebut baris demi baris.
- Data dari file CSV akan langsung dimasukkan ke dalam tabel database menggunakan perintah `INSERT`.
- Jika file yang diunggah **bukan file CSV**, sistem akan menampilkan pesan error.

Fitur ini dibuat untuk memudahkan proses input data tanpa perlu mengetik manual di form, terutama saat jumlah data besar.

---

## 🛠️ Teknologi yang Digunakan

- **Java SE (Swing)** untuk antarmuka GUI.
- **JDBC (Java Database Connectivity)** untuk koneksi ke database.
- **MySQL / MariaDB** sebagai database.
- **JDK 17+** untuk menjalankan program.
- **NetBeans IDE** sebagai lingkungan pengembangan.

---

## 🧮 Struktur Database (Contoh)

Tabel: `mata_kuliah`

| Kolom           | Tipe Data     |
|-----------------|----------------|
| kode_matkul     | VARCHAR(10)    |
| nama_matkul     | VARCHAR(100)   |
| sks_matkul      | INT            |
| dosen_pengajar  | VARCHAR(100)   |

---

## 💻 Fitur Utama
✅ Validasi File

- Program hanya menerima file dengan ekstensi .csv.

- Jika pengguna memilih file lain (misalnya .txt, .xlsx, atau .pdf), sistem akan menampilkan pesan kesalahan.

✅ Proses Upload Otomatis

- Setelah file CSV dipilih, sistem akan membaca setiap baris.

- Setiap data akan dimasukkan otomatis ke dalam tabel database menggunakan PreparedStatement.

✅ Penanganan Error

- Menampilkan pesan jika file gagal dibaca.

- Menampilkan pesan jika terjadi kesalahan SQL (misalnya duplikasi data).

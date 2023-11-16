# UTS_BASIS_DATA
REZA DWI PUTRA (20220801472)

Repositori ini berisi skrip SQL untuk membuat skema basis data dan menyisipkan data contoh. Basis data ini dirancang untuk mengelola informasi tentang mata kuliah, mahasiswa, dan dosen. Terdapat tiga tabel utama: mata_kuliah, mahasiswa, dan dosen.

Skema Tabel
Tabel mata_kuliah
id (INT, PRIMARY KEY): Identifikasi unik untuk setiap mata kuliah.
kode_matkul (VARCHAR(50), NOT NULL): Kode mata kuliah.
nama_matkul (VARCHAR(50), NOT NULL): Nama mata kuliah.
sks (VARCHAR(50), NOT NULL): Jumlah jam kredit untuk mata kuliah.
Tabel mahasiswa
id (INT, PRIMARY KEY): Identifikasi unik untuk setiap mahasiswa.
nim (VARCHAR(50), NOT NULL): Nomor identifikasi mahasiswa.
first_name (VARCHAR(50), NOT NULL): Nama depan mahasiswa.
last_name (VARCHAR(50), NOT NULL): Nama belakang mahasiswa.
jurusan (VARCHAR(50), NOT NULL): Jurusan mahasiswa.
kode_matkul (VARCHAR(50), NOT NULL, FOREIGN KEY ke mata_kuliah(id)): Identifikasi untuk mata kuliah yang diikuti mahasiswa.
Tabel dosen
id (INT, PRIMARY KEY): Identifikasi unik untuk setiap dosen.
kode_dosen (VARCHAR(50), NOT NULL): Kode dosen.
first_name (VARCHAR(50), NOT NULL): Nama depan dosen.
last_name (VARCHAR(50), NOT NULL): Nama belakang dosen.
jurusan (VARCHAR(50), NOT NULL): Jurusan dosen.
kode_matkul (VARCHAR(50), NOT NULL, FOREIGN KEY ke mata_kuliah(id)): Identifikasi untuk mata kuliah yang diajar oleh dosen.
Data Contoh
Skrip ini menyertakan data contoh untuk setiap tabel agar dapat memberikan gambaran tentang struktur dan hubungan data.

Query
Berbagai query SELECT telah disertakan untuk menunjukkan cara mengambil informasi dari basis data, termasuk penggabungan tabel untuk mendapatkan data yang lebih lengkap.

Penggunaan
1. Jalankan skrip SQL di dalam sistem manajemen basis data (DBMS) yang mendukung untuk membuat skema basis data dan menyisipkan data contoh.
2. Gunakan query yang telah disediakan sebagai referensi untuk mengambil informasi dari basis data.

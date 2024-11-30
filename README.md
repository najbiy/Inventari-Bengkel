# Inventari-Bengkel
Berikut adalah tata cara untuk menggunakan program aplikasi inventaris bengkel ini:

### 1. **Clone Repositori**
   - Pertama, clone repositori ini ke komputer Anda menggunakan perintah Git berikut:
     ```bash
     git clone https://github.com/najbiy/Inventari-Bengkel.git
     ```
### 2. **Membuat Database di XAMPP**
   - Buka aplikasi XAMPP dan pastikan Apache serta MySQL sudah berjalan.
   - Akses phpMyAdmin melalui browser dengan alamat: `http://localhost/phpmyadmin/`.
   - Buatlah database baru untuk aplikasi ini dengan cara klik "New" dan beri nama sesuai keinginan Anda (misalnya, `inventaris_bengkel`).

### 3. **Mengubah Nama Database di File `hibernate.cfg.xml`**
   - Masuk ke folder proyek yang sudah Anda clone.
   - Temukan file `hibernate.cfg.xml` di dalam folder `src/main/resources/`.
   - Buka file tersebut dengan editor teks dan cari bagian berikut:
     ```xml
     <property name="hibernate.connection.url">jdbc:mysql://localhost:3306/nama_database</property>
     ```
   - Gantilah `nama_database` dengan nama database yang sudah Anda buat di langkah sebelumnya, misalnya `inventaris_bengkel`:
     ```xml
     <property name="hibernate.connection.url">jdbc:mysql://localhost:3306/inventaris_bengkel</property>
     ```

### 4. **Menjalankan Aplikasi**
   - Pastikan Anda sudah mengimpor proyek ini ke IDE seperti IntelliJ IDEA atau Eclipse.
   - Setelah itu, jalankan program Java sesuai dengan prosedur di IDE Anda.
   - Program akan terhubung ke database yang sudah Anda buat dan mulai berjalan.

Sekarang aplikasi inventaris bengkel siap digunakan untuk mengelola data stok barang di bengkel Anda!

# JobNest - Lowongan Pekerjaan 2025

JobNest adalah sebuah platform web yang menyediakan informasi lowongan pekerjaan di seluruh Indonesia. Platform ini dirancang untuk memudahkan perusahaan dalam mencari calon pekerja yang sesuai, serta membantu calon pekerja menemukan pekerjaan impian mereka.

## Fitur

- **Pencarian Lowongan Pekerjaan**: Pengguna dapat mencari lowongan pekerjaan berdasarkan nama pekerjaan dan lokasi.
- **Navigasi Perusahaan dan Calon Pekerja**: Menu navigasi yang terpisah untuk perusahaan dan calon pekerja, dengan opsi untuk sign in dan sign up.
- **Profil Calon Pekerja**: Calon pekerja dapat mengedit profil mereka, termasuk informasi pribadi, pendidikan, dan pengalaman kerja.
- **Responsive Design**: Desain yang responsif dan ramah pengguna, menggunakan Bootstrap untuk memastikan tampilan yang baik di berbagai perangkat.

## Teknologi yang Digunakan

- **PHP**: Bahasa pemrograman utama yang digunakan untuk pengembangan backend.
- **CodeIgniter 4**: Framework PHP yang digunakan untuk struktur aplikasi yang lebih baik dan pengelolaan MVC (Model-View-Controller).
- **MySQL**: Database yang digunakan untuk menyimpan data pengguna dan lowongan pekerjaan.
- **Bootstrap**: Framework CSS yang digunakan untuk desain responsif dan komponen UI.
- **JavaScript**: Digunakan untuk interaktivitas dan fungsionalitas tambahan pada halaman web.

Berikut adalah tambahan **proses instalasi** untuk README GitHub proyek **JobNest - Lowongan Pekerjaan 2025**:  

---

### **Proses Instalasi**  

Ikuti langkah-langkah berikut untuk menjalankan proyek ini di lingkungan lokal:  

#### **1. Clone Repository**  
Jalankan perintah berikut di terminal atau command prompt untuk meng-clone repository ini:  

git clone https://github.com/fandirmadhan/JobNest-Lowongan-Pekerjaan-2025.git

Lalu masuk ke folder proyek:  

cd JobNest-Lowongan-Pekerjaan-2025


#### **2. Konfigurasi Server Lokal**  
Pastikan kamu sudah menginstal **XAMPP** atau **LAMP** di sistem kamu.  
- Jika menggunakan **XAMPP**, jalankan **Apache** dan **MySQL** melalui Control Panel.  
- Jika menggunakan **LAMP**, pastikan service Apache dan MySQL berjalan.  

Salin proyek ini ke dalam direktori **htdocs** XAMPP:  

mv JobNest-Lowongan-Pekerjaan-2025 /xampp/htdocs/


#### **3. Buat Database**  
1. Buka **phpMyAdmin** di browser melalui `http://localhost/phpmyadmin`.  
2. Buat database baru dengan nama:  
   
   db_loker
   
3. Impor file database yang ada di dalam folder `database/` dengan cara:  
   - Pilih database `db_loker`.  
   - Klik **Import** → Pilih file `.sql` → Klik **Go**.  

#### **4. Konfigurasi Database di CodeIgniter**  
Buka file konfigurasi database di CodeIgniter:  

nano app/Config/Database.php

Atau gunakan text editor lainnya. Ubah bagian berikut sesuai dengan pengaturan MySQL lokal:  
public $default = [
    'DSN'      => '',
    'hostname' => 'localhost',
    'username' => 'root',  // Sesuaikan dengan user database
    'password' => '',      // Biarkan kosong jika tidak ada password
    'database' => 'jobnest_db',
    'DBDriver' => 'MySQLi',
    'DBPrefix' => '',
    'pConnect' => false,
    'DBDebug'  => (ENVIRONMENT !== 'production'),
    'cacheOn'  => false,
    'charset'  => 'utf8',
    'DBCollat' => 'utf8_general_ci',
    'swapPre'  => '',
    'encrypt'  => false,
    'compress' => false,
    'strictOn' => false,
    'failover' => [],
    'port'     => 3306,
];

Simpan perubahan dan tutup editor.

#### **5. Jalankan Aplikasi**  
Jalankan proyek dengan membuka browser dan akses:  

http://localhost/JobNest-Lowongan-Pekerjaan-2025

#### **6. Selesai!**  
Sekarang aplikasi **JobNest** sudah bisa digunakan di lokal. Jika ada kendala, pastikan **XAMPP/LAMP** berjalan dan database sudah dikonfigurasi dengan benar.  

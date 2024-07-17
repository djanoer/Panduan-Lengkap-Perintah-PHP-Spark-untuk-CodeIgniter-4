# Panduan-Lengkap-Perintah-PHP-Spark-untuk-CodeIgniter-4
Catatan ini berisi daftar lengkap perintah php spark yang tersedia dalam CodeIgniter 4, beserta penjelasan singkat mengenai fungsi dan penggunaannya.

----------------------------------------------------------------------------------------

### Perintah Dasar

Menampilkan daftar perintah yang tersedia dan cara penggunaannya.
```bash
  php spark help
```
Menjalankan server pengembangan lokal untuk menguji aplikasi Anda.
```bash
  php spark serve
```
Menampilkan daftar perintah yang tersedia, mirip dengan help.
```bash
  php spark list
```
Menampilkan versi CodeIgniter 4 dan Spark yang sedang digunakan.
```bash
  php spark version
```
Menentukan path ke binary PHP jika tidak terdeteksi otomatis.
```bash
  php spark --php-binary
```

----------------------------------------------------------------------------------------

### Perintah Pembuatan (make)

Membuat command (perintah kustom) baru.
```bash
  php spark make:command [nama]
```	
Membuat controller baru.
```bash
  php spark make:controller [nama]
```
(CI4.1+) Membuat entity untuk menghasilkan model dan migrasi sekaligus.
```bash
  php spark make:entity [nama]
```
Membuat filter untuk memfilter request HTTP.
```bash
  php spark make:filter [nama]
```
Membuat file migrasi untuk mengelola perubahan struktur database.
```bash
  php spark make:migration [nama]
```
Membuat model baru untuk berinteraksi dengan database.
```bash
  php spark make:model [nama]
```
Membuat seeder untuk mengisi data awal ke dalam database.
```bash
  php spark make:seeder [nama]
```

----------------------------------------------------------------------------------------

### Perintah Database

Menjalankan seeder tertentu untuk mengisi data ke database.
```bash
  php spark db:seed [nama]
```
Menjalankan semua migrasi database yang belum dijalankan.
```bash
php spark migrate
```
Membatalkan semua migrasi.
```bash
  php spark migrate:down
```
Menjalankan migrasi terbaru.
```bash
  php spark migrate:latest
```
Menghapus semua tabel dan menjalankan ulang semua migrasi (hati-hati!).
```bash
  php spark migrate:refresh
```
Membatalkan migrasi terakhir yang telah dijalankan.
```bash
  php spark migrate:rollback
```
Melihat status migrasi (mana yang sudah dijalankan dan mana yang belum).
```bash
  php spark migrate:status
```
Menjalankan semua migrasi yang belum dijalankan. Sama dengan php spark migrate.
```bash
  php spark migrate:up
```
Menjalankan migrasi ke versi tertentu.
```bash
  php spark migrate:version [versi]
```

----------------------------------------------------------------------------------------

### Perintah Lainnya

Membuat kunci aplikasi baru (APP_KEY) yang digunakan untuk keamanan.
```bash
  php spark key:generate
```
Menampilkan daftar rute yang tersedia dalam aplikasi Anda.
```bash
  php spark routes
```
Menjalankan command yang sudah Anda buat.
```bash
  php spark [nama_command]
```
Mempublikasikan file atau direktori tertentu ke direktori public, membuatnya dapat diakses publik.
```bash
  php spark publish [path]
```

----------------------------------------------------------------------------------------

### Contoh Penggunaan:

```Bash
# Membuat controller bernama "ProductController"
php spark make:controller ProductController

# Membuat migrasi untuk membuat tabel "products"
php spark make:migration create_products_table
```


# Kasus 01 — CRUD Manajemen Buku

**Level:** Mudah  
**Fokus:** Route, Controller, Model, Migration, Blade, validasi dasar.

## Tujuan
Mahasiswa memperbaiki fitur daftar, tambah, dan hapus buku dengan memahami alur MVC.

## Instalasi
Buat proyek Laravel baru, salin isi folder kasus ini ke proyek, lalu buat database `bug_battle_case_01`.

Atur `.env`:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=bug_battle_case_01
DB_USERNAME=root
DB_PASSWORD=
```

Jalankan:
```bash
php artisan optimize:clear
php artisan migrate
php artisan serve
```
Buka `http://127.0.0.1:8000/books`.

## Gejala yang harus diselidiki
1. Halaman daftar buku tidak dapat dibuka dengan benar.
2. Form tambah buku memiliki perilaku yang tidak sesuai.
3. Data buku tidak tampil setelah proses penyimpanan.
4. Tombol hapus tidak bekerja sebagaimana mestinya.

## Tugas
- Perbaiki routing dan kesesuaian nama method.
- Pastikan variabel yang dikirim Controller sama dengan variabel di Blade.
- Perbaiki proses penyimpanan dan penghapusan.
- Tambahkan validasi yang tepat tanpa menghilangkan fitur.
- Uji tambah, tampil, dan hapus data.

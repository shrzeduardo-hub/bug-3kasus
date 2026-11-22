# Kasus 02 — Relasi Buku dan Kategori

**Level:** Menengah  
**Fokus:** Migration, foreign key, Eloquent relationship, belongsTo, hasMany, eager loading.

## Tujuan
Mahasiswa memahami relasi one-to-many: satu kategori memiliki banyak buku, dan setiap buku dimiliki satu kategori.

## Instalasi
Buat proyek Laravel baru dan salin isi folder kasus ini ke proyek.
Buat database `bug_battle_case_02`, sesuaikan `.env`, lalu jalankan:
```bash
php artisan optimize:clear
php artisan migrate
php artisan db:seed --class=CategorySeeder
php artisan serve
```
Buka `http://127.0.0.1:8000/books`.

## Gejala yang harus diselidiki
1. Migrasi tabel buku dapat gagal atau relasinya tidak terjamin.
2. Daftar buku gagal mengambil kategori.
3. Nama kategori tidak tampil dengan benar.
4. Form buku tidak menampilkan pilihan kategori secara benar.

## Tugas
- Perbaiki foreign key `category_id`.
- Perbaiki relasi pada kedua Model.
- Perbaiki pemanggilan relasi pada Controller dan Blade.
- Pastikan satu kategori dapat memiliki banyak buku.
- Uji data buku dengan beberapa kategori.

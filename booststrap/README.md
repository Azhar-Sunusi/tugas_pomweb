# Instagram Profile Clone (Bootstrap)

Proyek ini adalah kloning sederhana dari tampilan halaman profil Instagram menggunakan **Bootstrap 5.3**. Desain ini dibuat untuk latihan front-end dan memanfaatkan sistem grid serta komponen bawaan Bootstrap untuk menampilkan struktur profil, highlight stories, dan grid postingan.

## Preview
Tampilan mirip halaman profil Instagram dengan:
- Navbar sederhana menggunakan komponen `navbar`
- Foto profil dan detail pengguna menggunakan sistem grid (`row` dan `col`)
- Highlight stories scrollable dengan utilitas `d-flex overflow-auto`
- Grid postingan 3 kolom responsif menggunakan `row row-cols-3 g-2` dan `ratio ratio-1x1`

## Teknologi yang Digunakan
- [Bootstrap 5.3](https://getbootstrap.com/)  
- [Bootstrap Icons](https://icons.getbootstrap.com/) (untuk ikon)  
- HTML5

## Struktur Folder
.
├── img/
│ ├── profile.jpeg
│ ├── highlight.jpeg
│ ├── highlight1.jpeg
│ ├── anu.jpeg
│ ├── anu2.jpeg
│ └── ... (gambar lain)
├── index.html
└── README.md

bash
Copy code

## Cara Menjalankan
1. Clone repositori ini:
   git clone https://github.com/username/instagram-profile-bootstrap.git

2. Buka folder proyek:
   cd instagram-profile-bootstrap

3. Buka file index.html di browser pilihan Anda.

## Fitur Utama
1. Navbar Minimalis – Navigasi sederhana dengan ikon Home, Add Post, dan Profile.
2. Header Profil Lengkap – Menampilkan foto profil, username, tombol Follow/Edit Profile, statistik (Posts, Followers, Following), dan bio.
3. Highlight Stories Scrollable – Lingkaran highlight yang bisa digeser horizontal di layar kecil.
4. Grid Postingan Responsif – Tata letak tiga kolom (atau menyesuaikan breakpoint) yang otomatis membuat baris baru saat postingan bertambah.
5. Desain Mobile-First – Layout dan tombol menyesuaikan ukuran layar untuk kenyamanan pengguna ponsel.
6. Ikon Modern – Menggunakan Bootstrap Icons untuk kesan mirip Instagram asli.
7. Struktur Folder Rapi – Folder img/ terpisah untuk semua gambar dan README sebagai panduan.
8.Mudah Dikustomisasi – Gambar, teks profil, dan warna dapat diubah langsung di HTML/CSS.

## Latihan Dan Pertanyaan
Mengapa memilih konfigurasi col tertentu untuk tiap breakpoint?
Sedikit kolom di layar kecil (mis. col-6 atau col-4) menjaga foto jelas dan mudah diklik, lalu tambah kolom di tablet/desktop (col-md-3, col-lg-2) agar ruang besar terpakai efisien.

Bagaimana memastikan tombol Follow/Edit Profile tetap mudah dijangkau di mobile?
Gunakan btn-sm w-100 d-md-inline-block atau flex-wrap supaya tombol lebar penuh, cukup besar disentuh, dan tetap rapi di layar sempit.

Jika postingan bertambah jadi 50, apa potensi masalah dan bagaimana solusi gridmu mengatasinya?
Grid otomatis membuat baris baru, tapi halaman bisa berat dan lambat. Atasi dengan lazy-loading gambar, pagination/infinite scroll, dan menambah kolom di layar besar (row-cols-lg-4/5) untuk menampilkan lebih banyak foto per baris.

# Instagram Profile Clone (Tailwind CSS)

Proyek ini adalah kloning sederhana dari tampilan halaman profil Instagram menggunakan **Tailwind CSS**. Desain ini dibuat untuk latihan front-end dan menampilkan struktur profil, highlight stories, dan grid postingan.

## Preview
Tampilan mirip halaman profil Instagram dengan:
- Navbar sederhana
- Foto profil dan detail pengguna
- Highlight stories scrollable
- Grid postingan 3 kolom responsif

## Teknologi yang Digunakan
- [Tailwind CSS](https://tailwindcss.com/) (CDN)
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


## Cara Menjalankan
1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/instagram-profile-tailwind.git
2. Buka folder proyek:
cd instagram-profile-tailwind

3. Buka file index.html di browser pilihan Anda.

---

## Dependensi
- [Tailwind CSS](https://tailwindcss.com/) (via CDN)  
- [Alpine.js](https://alpinejs.dev/) (via CDN, untuk navigasi tab)  
- Folder `img/` untuk resource gambar profil & posting  

---

## Cara Menjalankan
1. Clone atau download repository.  
2. Pastikan semua file gambar ada di folder `img/`.  
3. Buka `index.html` langsung di browser (atau gunakan Live Server di VS Code).  

---

## Penjelasan Desain

Proyek ini adalah kloning sederhana dari tampilan halaman profil Instagram menggunakan **Tailwind CSS**. Tujuannya untuk latihan front-end, memahami sistem utilitas Tailwind, serta meniru desain antarmuka populer.

---

## 🎨 Penjelasan Desain

1. **Navbar Minimalis**  
   - Menggunakan warna latar putih (`bg-white`) dengan border bawah abu-abu terang (`border-b`).  
   - Logo teks **Instagram** ditampilkan tebal sebagai identitas.  
   - Ikon navigasi (Home, Add Post, Profile) menggunakan **Bootstrap Icons** untuk kesan sederhana seperti Instagram asli.  
   - Tombol ikon diberi efek hover (`hover:bg-gray-200`) dan sudut membulat (`rounded-lg`) agar terasa interaktif.

2. **Bagian Profil (Header)**  
   - Foto profil ditampilkan berbentuk lingkaran (`rounded-full`) dengan border abu-abu lembut, menyerupai tampilan Instagram.  
   - Username dan tombol **Edit Profile** diletakkan horizontal menggunakan `flex` agar responsif.  
   - Informasi statistik (Posts, Followers, Following) memakai `flex space-x` sehingga terlihat rapi dan mudah dibaca.  
   - Bio pengguna ditaruh di bawahnya dengan tipografi sederhana untuk fokus pada konten.

3. **Highlight Stories**  
   - Menggunakan container `flex` dengan `overflow-x-auto` agar highlight dapat digeser horizontal di layar kecil.  
   - Setiap highlight adalah lingkaran dengan label kecil di bawahnya (`text-sm`) mirip fitur highlights Instagram.

4. **Grid Postingan**  
   - Menggunakan `grid grid-cols-3 gap-1` untuk menampilkan postingan dalam tiga kolom responsif.  
   - Gambar dipasang dengan `object-cover` agar menyesuaikan rasio tanpa distorsi.  
   - Gaya ini meniru feed Instagram yang bersih dan simetris.

5. **Responsivitas**  
   - Dengan utilitas Tailwind seperti `flex-col md:flex-row`, desain otomatis menyesuaikan layar lebih kecil (mobile) atau besar (desktop).  
   - Tailwind memastikan tampilan tetap konsisten tanpa memerlukan banyak media query manual.

---

## Pertanyaan Reflektif

**1. Jelaskan keputusan grid-cols/gap di tiap breakpoint — kenapa begitu?**  
Dipilih grid-cols-3 gap-1 agar mirip feed Instagram: 3 kolom rapi di desktop, gap-1 hemat ruang. Di mobile bisa dikurangi ke grid-cols-2 agar gambar tidak terlalu kecil, dan di layar besar bisa ditambah kolom untuk efisiensi ruang.  

**2. Bagaimana memanfaatkan utility responsive Tailwind untuk memecahkan masalah layout di mobile?**  
Gunakan prefix seperti sm:, md:, lg: untuk mengubah layout sesuai ukuran layar, misalnya flex-col md:flex-row atau hidden md:block, sehingga tampilan mobile dan desktop otomatis menyesuaikan tanpa media query manual.

**3. Jelaskan trade-off antara memakai banyak utility classes vs membuat component CSS tersendiri.**  
Utility cepat dan fleksibel tapi bisa membuat HTML penuh kelas dan kurang konsisten. Component CSS lebih rapi dan konsisten untuk proyek besar, tapi butuh waktu lebih lama menulis dan memelihara. Kombinasi keduanya sering jadi pilihan terbaik.

---

## Soal Latihan
- **Deskripsi Singkat:** Membuat halaman profil Instagram clone dengan Tailwind CSS.  
- **Ketentuan Wajib:** Header Profil, Bio, Feed minimal 12 gambar, Footer, penggunaan minimal 3 fitur responsif Tailwind (`grid-cols`, `order`, `gap`, dsb).  
- **Deliverables:**  
  1. File `index.html`  
  2. Folder `img/` berisi gambar profil & posting.  

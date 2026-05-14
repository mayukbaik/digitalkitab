# 📖 Website Kitab Kuning Digital

**SMK Roudlotul Mubtadiin Balekambang**
_"Yo Ngaji Yo Teknologi"_

## 🌟 Tentang Website

Website ini adalah perpustakaan digital kitab kuning berbasis HTML, CSS, dan JavaScript murni. Dirancang untuk memudahkan santri dalam mengakses materi pembelajaran kitab pesantren secara modern dan praktis.

### ✨ Fitur Utama

- 📚 9 Kategori Ilmu (Nahwu, Shorof, Fiqih, Ushul Fiqih, Tauhid, Tasawuf, Hadits)
- 📄 PDF flipbook untuk membaca kitab
- 🎥 Video Embed untuk pembelajaran
- 🔍 Fitur Pencarian
- 📱 Responsive Design (Mobile & Desktop)
- ⚡ Offline Capable (bisa dijalankan tanpa internet)
- 🎨 Desain Islami Modern (Hijau-Emas)

---

## 📁 Struktur Folder

```
project/
├── index.html             # Halaman Beranda
├── nahwu.html             # Halaman Kategori Ilmu Nahwu
├── shorof.html            # Halaman Kategori Ilmu Shorof
├── fiqih.html             # Halaman Kategori Fiqih
├── ushul-fiqih.html       # Halaman Kategori Ushul Fiqih
├── tauhid.html            # Halaman Kategori Tauhid
├── tasawuf.html           # Halaman Kategori Tasawuf
├── hadits.html            # Halaman Kategori Hadits
├── tafsir.html            # Halaman Kategori Tafsir
├── falak.html             # Halaman Kategori Ilmu Falak
├── detail/                # Folder Halaman Detail Kitab
│   ├── ajurumiyah.html    # Contoh: Detail Kitab Ajurumiyah
│   ├── safinah.html       # Contoh: Detail Kitab Safinah
│   └── ...                # File detail kitab lainnya
├── assets/
│   ├── css/
│   │   └── style.css      # File CSS Global
│   ├── js/
│   │   └── script.js      # File JavaScript Global
│   ├── pdf/               # Folder untuk file PDF kitab
│   │   ├── ajurumiyah.pdf
│   │   ├── safinah.pdf
│   │   └── ...
│   └── video/             # Folder untuk file Video pembelajaran
│       ├── ajurumiyah.mp4
│       ├── safinah.mp4
│       └── ...
└── README.md              # File ini
```

---

## 🚀 Cara Menjalankan Website

### Metode 1: Live Server (VS Code)

1. Install extension **Live Server** di VS Code
2. Klik kanan pada file `index.html`
3. Pilih **"Open with Live Server"**
4. Website akan otomatis terbuka di browser

### Metode 2: XAMPP

1. Copy seluruh folder project ke `C:/xampp/htdocs/`
2. Jalankan XAMPP (Apache)
3. Buka browser dan ketik: `http://localhost/project/`

### Metode 3: Langsung dari Browser

1. Buka File Explorer
2. Double-click file `index.html`
3. Website akan terbuka di browser default

---

## 📝 Daftar Kitab per Kategori

### 1. Ilmu Nahwu (4 Kitab)

- Matan Al-Ajurumiyah
- Imrithi
- Mutamimah
- Alfiyah Ibnu Malik

### 2. Ilmu Shorof (3 Kitab)

- Amtsilah At-Tashrifiyah
- Al-Izzi (Tashrif Al-Izzi)
- Nazhom Al-Maqshud

### 3. Fiqih Mazhab Syafi'i (7 Kitab)

- Safinatun Najah
- Kasyifatus Saja
- Fathul Qorib
- Sullam Taufiq
- Fathul Mu'in
- Minhajut Thalibin
- Nihayatuz Zain

### 4. Ushul Fiqih & Qawaid (3 Kitab)

- Ushul Fiqh
- Lathaiful Isyarat
- Syarah Waraqat

### 5. Tauhid / Aqidah (6 Kitab)

- Aqidatul Awam
- Nurudh Dholam
- Tijan Ad-Darari
- Sanusiyah (Ummul Barahin)
- Kifayatul Awam
- Husnul Hamidiyah

### 6. Tasawuf & Akhlak (6 Kitab)

- Ta'limul Muta'allim
- Al-Hikam
- Bidayatul Hidayah
- Nashaihul 'Ibad
- Adabul Alim wal Muta’allim
- Ayyuhal Walad

### 7. Hadits & Musthalah (5 Kitab)

- Arba'in Nawawi
- Riyadhus Shalihin
- Bulughul Maram
- Mukhtarul Ahadist
- Al-Adzkar An-Nawawiyah

**Total: 34 Kitab**

---

## ➕ Cara Menambahkan Halaman Detail Kitab

Sudah ada 2 contoh halaman detail:

- `detail/ajurumiyah.html` (Ilmu Nahwu)
- `detail/safinah.html` (Fiqih)

Untuk menambahkan halaman detail kitab lainnya:

### Langkah 1: Copy

Copy salah satu file contoh dan rename sesuai nama kitab:

```bash
# Contoh untuk kitab Imrithi
copy detail/ajurumiyah.html detail/imrithi.html
```

### Langkah 2: Edit Konten

Buka file yang baru dibuat dan ubah:

1. **Tag `<title>`**: Ganti judul kitab
2. **Tombol Kembali**: Sesuaikan link kategori
3. **Judul Kitab**: Ubah di class `detail-title`
4. **Deskripsi**: Ubah penjelasan kitab
5. **Path PDF**: Sesuaikan path file PDF
6. **Path Video**: Sesuaikan path file video
7. **Info Kitab**: Update informasi pengarang, kategori, dll

### Langkah 3: Tambahkan File PDF & Video

1. Letakkan file PDF di: `assets/pdf/nama-kitab.pdf`
2. Letakkan file video di: `assets/video/nama-kitab.mp4`

### Langkah 4: Update Link di Halaman Kategori

Pastikan link di halaman kategori mengarah ke halaman detail yang benar:

```html
<a href="detail/nama-kitab.html" class="btn-pdf">📄 Baca PDF</a>
<a href="detail/nama-kitab.html#video" class="btn-video">🎥 Tonton Video</a>
```

---

## 🎨 Kustomisasi Desain

### Mengubah Warna

Edit file `assets/css/style.css` di bagian `:root`:

```css
:root {
  --primary-green: #1a5f3f; /* Hijau Utama */
  --secondary-green: #2d7a52; /* Hijau Sekunder */
  --gold: #d4af37; /* Emas */
  --light-gold: #f4e4b7; /* Emas Muda */
  --white: #ffffff; /* Putih */
  --light-bg: #f8f9fa; /* Background Terang */
}
```

### Mengubah Font

Ganti import font di bagian atas `style.css`:

```css
@import url("https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap");
```

---

## 🔧 Troubleshooting

### PDF tidak muncul?

1. Pastikan file PDF ada di folder `assets/pdf/`
2. Cek path file di tag `<iframe src="...">` sudah benar
3. Gunakan Live Server atau XAMPP (jangan buka langsung dari file)

### Video tidak bisa diputar?

1. Pastikan format video adalah MP4 (H.264)
2. Cek path file di tag `<source src="...">` sudah benar
3. Coba convert video menggunakan HandBrake atau VLC

### Menu tidak muncul di mobile?

1. Klik icon hamburger (☰) di pojok kanan atas
2. Pastikan JavaScript berjalan dengan baik

### Search tidak berfungsi?

1. Pastikan file `assets/js/script.js` ter-load
2. Buka Console browser (F12) untuk cek error

---

## 📱 Responsive Breakpoints

Website ini responsive dengan breakpoint:

- **Desktop**: > 768px
- **Tablet**: 768px - 481px
- **Mobile**: < 480px

---

## 🤝 Kontribusi

Website ini dibuat untuk keperluan pembelajaran di SMK Roudlotul Mubtadiin Balekambang. Silakan dikembangkan sesuai kebutuhan.

### Saran Pengembangan

- [ ] Tambahkan fitur bookmark/favorit
- [ ] Tambahkan mode gelap (dark mode)
- [ ] Tambahkan fitur catatan
- [ ] Integrasi dengan database
- [ ] Sistem autentikasi user

---

## 📞 Kontak

**SMK Roudlotul Mubtadiin Balekambang**
Jawa Tengah, Indonesia

---

## 📄 Lisensi

Website ini dibuat untuk keperluan pendidikan dan pembelajaran.

---

**Barakallahu fiikum**
_Semoga bermanfaat untuk para Tholabul ilmi_

---

### 🎯 Catatan Penting

1. ✅ Semua halaman saling terhubung
2. ✅ Tidak ada link mati
3. ✅ Tombol kembali di setiap halaman
4. ✅ Bisa dijalankan offline
5. ✅ Coding terpisah (HTML, CSS, JS)
6. ✅ Struktur folder rapi

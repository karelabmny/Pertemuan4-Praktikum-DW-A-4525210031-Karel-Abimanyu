# Tugas Praktikum Pertemuan 4 - Desain Web

**Nama:** Karel Abimanyu
**NPM:** 4525210031
**Kelas:** A

## Tugas Individu

Membangun ulang halaman profil menjadi dua file (`index.html` dan `style.css`) dengan box model, minimal dua class reusable, dan satu media query di bawah 768px.

## File

| File | Keterangan |
|---|---|
| `index.html` | Struktur halaman profil (header, hero, data, tentang, keahlian, footer) |
| `style.css` | CSS |
| `img/<nama-foto>.jpg` | Foto profil |
| `arunika-studio/` | Studi kasus landing page Arunika Studio |

## Yang Dipakai

- **Box model:** `box-sizing: border-box`, `padding`, `border`, `margin` pada `.container` dan `.card`.
- **Card:** tepat 3 card (Data Pribadi, Tentang Saya, Keahlian); 3 kolom di desktop, 1 kolom di mobile.
- **Class reusable:** `.container`, `.card`, `.section-title`, `.btn`.
- **Media query:** `@media (max-width: 767px)` untuk layar di bawah 768px.

## Screenshot

| Halaman | Desktop |
|---|---|---|
| Profil |<img width="1902" height="1052" alt="output-biodata" src="https://github.com/user-attachments/assets/759b5d8c-896a-406b-8ccf-99519f00f361" /> <img width="1895" height="935" alt="output-biodata-1" src="https://github.com/user-attachments/assets/f1722855-5352-4164-945b-579a7fa905a1" />
|
| Arunika Studio | ( <img width="1920" height="996" alt="output-arunikastudio" src="https://github.com/user-attachments/assets/70a2b792-4a11-4a57-939e-15a82d0aa589" />) |

## Ringkasan Perubahan, Masalah, dan Solusi

Pada tugas ini saya sedikit merubah halaman profil dari pertemuan 3 yang sebelumnya memakai CSS inline menjadi dua file terpisah, yaitu `index.html` untuk struktur dan `style.css` untuk tampilan. Perubahan utamanya adalah memindahkan semua gaya ke satu file CSS, menambah header, hero, dan footer, serta menerapkan box model lewat `padding`, `border`, `margin`, dan `box-sizing: border-box` supaya ukuran elemen lebih mudah dihitung. Saya juga membuat class reusable seperti `.container`, `.card`, `.section-title`, dan `.btn` sehingga satu aturan bisa dipakai berulang tanpa menulis ulang kode.

Masalah yang muncul adalah gaya yang tersebar dan berulang di banyak elemen saat memakai CSS inline, serta tiga card profil yang terlalu sempit kalau tetap berjajar di layar ponsel. Solusinya, semua gaya dikumpulkan di satu tempat, lalu saya menambahkan satu media query pada lebar di bawah 768px yang mengubah hero menjadi vertikal dan tiga card menjadi satu kolom.

Studi kasus Arunika Studio juga saya rapikan dengan struktur `<main>`, tombol yang rata di dasar card, dan tiga card yang menjadi satu kolom pada layar kecil. Hasilnya sudah diuji pada ukuran desktop dan mobile tanpa scroll horizontal.

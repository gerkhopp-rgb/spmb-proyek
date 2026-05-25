# Product Requirements Document (PRD)
## Website Landing Page — SMK Budi Bakti Ciwidey

**Versi:** 1.0  
**Tanggal:** 26 Mei 2026  
**Status:** Draft  

---

## 1. Ringkasan Produk

Website landing page untuk **SMK Budi Bakti Ciwidey** yang berfungsi sebagai media promosi digital dan sarana pendaftaran siswa baru (SPMB). Website ini dirancang untuk menjawab kekhawatiran calon siswa dan orang tua mengenai prospek kerja lulusan SMK, serta memudahkan proses pendaftaran secara online.

---

## 2. Tujuan Produk

| Tujuan | Indikator Keberhasilan |
|---|---|
| Meningkatkan kesadaran (awareness) masyarakat terhadap SMK Budi Bakti Ciwidey | Jumlah pengunjung website per bulan |
| Mempermudah calon siswa menemukan informasi jurusan | Waktu rata-rata di halaman jurusan |
| Menghasilkan leads pendaftaran siswa baru | Jumlah form daftar yang tersubmit |
| Membangun kepercayaan melalui social proof | Bounce rate & durasi sesi |

---

## 3. Target Pengguna

### 3.1 Pengguna Utama
- **Calon Siswa Baru** — lulusan SMP/MTs usia 14–16 tahun yang sedang mencari sekolah lanjutan.
- **Orang Tua / Wali** — pengambil keputusan utama dalam pemilihan sekolah anak.

### 3.2 Karakteristik Pengguna
- Mengakses internet via smartphone (mobile-first).
- Familiar dengan media sosial (Instagram, YouTube, Facebook).
- Membutuhkan informasi yang jelas, singkat, dan meyakinkan.

---

## 4. Struktur Halaman & Fitur

### 4.1 Navbar (Navigasi)

**Deskripsi:** Bar navigasi yang selalu tampil di atas layar (sticky) saat pengguna scroll.

**Elemen:**
- Logo sekolah (bulat, 40×40px)
- Nama sekolah: *SMK Budi Bakti Ciwidey*
- Menu navigasi: Beranda, Jurusan *(tersembunyi di mobile)*
- Tombol CTA: **"Daftar"** — mengarah ke section form pendaftaran (`#daftar`)

**Behavior:**
- Sticky di posisi `top: 0` dengan `z-index: 50`
- Shadow ringan agar terpisah dari konten

---

### 4.2 Hero Section

**Deskripsi:** Area pertama yang dilihat pengguna, berfungsi menarik perhatian dan mendorong tindakan.

**Elemen:**
- Heading utama: *"Belajar Skill Nyata, Siap Kerja Setelah Lulus!"*
- Subheading: deskripsi singkat keunggulan SMK Budi Bakti Ciwidey
- Tombol CTA: *"Wujudkan masa depanmu hari ini!"* → mengarah ke `#daftar`
- Foto hero: gambar guru dan siswa di depan sekolah

**Spesifikasi Visual:**
- Background: gradient biru (`#1e3a8a` → `#2563eb`)
- Teks aksen: kuning (`text-yellow-300`)
- Tombol CTA: warna kuning (`#f5c518`) dengan teks gelap
- Layout: 2 kolom di desktop, 1 kolom di mobile

**Asset yang Dibutuhkan:**
- [ ] Foto hero siswa/guru: `images/tiluan.jpeg`
- [ ] Logo sekolah: `images/logo-bbc.jpeg`

---

### 4.3 Section Masalah & Solusi

**Deskripsi:** Menjelaskan pain point calon siswa dan solusi yang ditawarkan SMK Budi Bakti Ciwidey.

**Masalah yang Diangkat:**
1. Bingung masa depan — khawatir prospek kerja setelah lulus
2. Bingung memilih Program Keahlian — takut salah jurusan

**Solusi yang Ditampilkan:**
- SMK Budi Bakti Ciwidey membantu menentukan jurusan sesuai minat melalui pembelajaran praktik terarah, guru berpengalaman, dan program keahlian relevan.

**Spesifikasi Visual:**
- Background: foto sekolah dengan overlay gelap `rgba(0,0,0,0.55)`
- Card masalah: biru tua (`bg-blue-700`)
- Card solusi: kuning (`bg-yellow-400`)
- Ikon dekoratif: graduation cap SVG

---

### 4.4 Section Program Keahlian (Jurusan)

**Deskripsi:** Menampilkan 3 jurusan unggulan yang tersedia.

**Jurusan:**

| Kode | Nama Jurusan | Asset Foto |
|---|---|---|
| BRP | Bisnis Ritel dan Pemasaran | `images/bdp.jpeg` |
| RPL | Rekayasa Perangkat Lunak dan GIM | `images/rpl.jpeg` |
| DKV | Desain Komunikasi Visual | `images/dkv.jpeg` |

**Spesifikasi Visual:**
- Foto jurusan: bulat, 96×96px, border putih
- Badge kode jurusan: tombol kuning rounded-full
- Background: sama dengan section Masalah & Solusi (foto + overlay)
- Layout: 3 kolom di desktop, 1 kolom di mobile

---

### 4.5 Section Social Proof

**Deskripsi:** Menampilkan angka pencapaian sekolah untuk membangun kepercayaan.

**Data yang Ditampilkan:**

| Metrik | Nilai |
|---|---|
| Alumni Sukses | 1.000+ |
| Langsung Kerja | 999+ |
| Akreditasi | A |

**Spesifikasi Visual:**
- Background: biru tua (`bg-blue-700`)
- Card highlight: kuning (`bg-yellow-400`) untuk angka utama
- Layout: 3 kolom di desktop, stack di mobile

---

### 4.6 Section Testimoni

**Deskripsi:** Kutipan pengalaman alumni untuk memperkuat kepercayaan calon siswa.

**Konten:**

| Nama | Isi Testimoni | Rating |
|---|---|---|
| Aldiansyah | Dibekali keterampilan praktis sesuai kebutuhan dunia kerja. | ★★★★★ |
| Nina Y | Potensi diri berkembang melalui kegiatan akademik dan non-akademik. | ★★★★★ |

**Asset yang Dibutuhkan:**
- [ ] Foto profil Aldiansyah (32×32px)
- [ ] Foto profil Nina Y (32×32px)

**Spesifikasi Visual:**
- Background section: kuning (`bg-yellow-400`)
- Card testimoni: biru tua (`bg-blue-700`), teks putih

---

### 4.7 Section FAQ (Accordion)

**Deskripsi:** Menjawab pertanyaan umum calon siswa dan orang tua secara interaktif.

**Behavior:**
- Accordion: hanya satu jawaban terbuka pada satu waktu
- Ikon panah berputar 180° saat terbuka

**Daftar Pertanyaan:**

1. Kapan pendaftaran SPMB SMK Budi Bakti Ciwidey 2026/2027 dibuka?
2. Apa saja syarat dokumen yang harus disiapkan saat mendaftar?
3. Apakah tersedia program beasiswa untuk siswa baru?
4. Bagaimana alur seleksi masuk SMK Budi Bakti Ciwidey?

**Spesifikasi Visual:**
- Background: putih (`bg-white`)
- Border card: `border-gray-200`, sudut membulat
- Label atas: *"PERTANYAAN UMUM"* (biru, uppercase, tracking lebar)

---

### 4.8 Form Pendaftaran

**Deskripsi:** Form sederhana untuk mengumpulkan data awal calon pendaftar.

**Field:**

| Field | Tipe | Placeholder | Wajib |
|---|---|---|---|
| Nama | Text | Masukan Nama | Ya |
| Alamat | Text | Masukan Alamat | Ya |
| Jurusan | Dropdown | Pilih Jurusan | Ya |

**Opsi Dropdown Jurusan:**
- Bisnis Ritel dan Pemasaran (BRP)
- Rekayasa Perangkat Lunak dan GIM (RPL)
- Desain Komunikasi Visual (DKV)

**Behavior Submit:**
- Saat ini: alert konfirmasi *"Terima kasih! Pendaftaran Anda akan segera kami proses."*
- Target: integrasi ke backend / Google Sheets / WhatsApp API

**Elemen Tambahan:**
- Link sosial media: YouTube, Facebook, Instagram

**Spesifikasi Visual:**
- Background section: foto sekolah + overlay gelap
- Card form: kuning (`bg-yellow-400`), sudut membulat besar
- Tombol submit: biru tua (`bg-blue-700`), lebar penuh

---

### 4.9 Footer

**Deskripsi:** Penutup halaman dengan informasi hak cipta.

**Konten:**
- Teks: `© 2026 SMK Budi Bakti Ciwidey. All rights reserved.`
- Background: biru sangat tua (`bg-blue-900`)

---

## 5. Desain & Teknologi

### 5.1 Stack Teknologi

| Komponen | Teknologi |
|---|---|
| Markup | HTML5 |
| Styling | Tailwind CSS (CDN) |
| Font | Google Fonts — Poppins (400, 600, 700, 800) |
| JavaScript | Vanilla JS (accordion FAQ) |
| Hosting (rencana) | GitHub Pages |

### 5.2 Palet Warna

| Nama | Hex | Kegunaan |
|---|---|---|
| Biru Tua | `#1e3a8a` | Background hero, card testimoni, navbar |
| Biru Primer | `#2563eb` | Gradient hero, tombol submit |
| Kuning | `#f5c518` | Tombol CTA, card solusi, card form |
| Putih | `#ffffff` | Teks, border foto jurusan |
| Abu Terang | `#f9fafb` | Hover FAQ |

### 5.3 Tipografi

| Elemen | Style |
|---|---|
| Heading utama | Poppins 800, 2xl–4xl |
| Subheading | Poppins 700, xl–2xl |
| Body text | Poppins 400, sm–base |
| Label / Badge | Poppins 600–700, xs–sm |

### 5.4 Responsivitas

| Breakpoint | Layout |
|---|---|
| Mobile (`< 768px`) | 1 kolom, menu nav tersembunyi |
| Desktop (`≥ 768px`) | 2–3 kolom, menu nav tampil |

---

## 6. Daftar Asset yang Dibutuhkan

| File | Keterangan | Status |
|---|---|---|
| `images/logo-bbc.jpeg` | Logo bulat SMK Budi Bakti Ciwidey | ⬜ Belum |
| `images/tiluan.jpeg` | Foto hero (siswa/guru di depan sekolah) | ⬜ Belum |
| `images/bdp.jpeg` | Foto/logo jurusan BRP | ⬜ Belum |
| `images/rpl.jpeg` | Foto/logo jurusan RPL | ⬜ Belum |
| `images/dkv.jpeg` | Foto/logo jurusan DKV | ⬜ Belum |
| Foto profil Aldiansyah | Testimoni alumni 1 | ⬜ Belum |
| Foto profil Nina Y | Testimoni alumni 2 | ⬜ Belum |
| `logo-smkbbc.jpeg` | Background section blur | ⬜ Belum |

---

## 7. Fitur yang Perlu Dikembangkan (Backlog)

| Prioritas | Fitur | Keterangan |
|---|---|---|
| 🔴 Tinggi | Integrasi form ke WhatsApp / Google Sheets | Saat ini hanya alert() |
| 🔴 Tinggi | Validasi form (nama, alamat wajib diisi) | Belum ada validasi |
| 🟡 Sedang | Link sosial media aktif (YouTube, Facebook, Instagram) | Saat ini `href="#"` |
| 🟡 Sedang | Halaman detail jurusan (BRP, RPL, DKV) | Belum tersedia |
| 🟢 Rendah | Animasi scroll (fade-in saat section masuk layar) | Opsional |
| 🟢 Rendah | Halaman terima kasih setelah submit form | UX lebih baik |
| 🟢 Rendah | SEO meta tags (description, og:image, dll.) | Belum ada |

---

## 8. Catatan Tambahan

- Semua gambar menggunakan `onerror` fallback ke placeholder via `placehold.co` agar tampilan tidak rusak saat foto belum tersedia.
- File utama harus bernama `index.html` agar bisa diakses langsung via GitHub Pages.
- Folder struktur yang direkomendasikan:
  ```
  /
  ├── index.html
  ├── images/
  │   ├── logo-bbc.jpeg
  │   ├── tiluan.jpeg
  │   ├── bdp.jpeg
  │   ├── rpl.jpeg
  │   └── dkv.jpeg
  └── README.md
  ```

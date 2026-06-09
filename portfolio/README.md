# 📁 Portfolio Data Enthusiast
### Panduan Lengkap untuk Pemula — Baca dari Atas ke Bawah!

---

## 🗂️ Struktur Folder Project

```
portfolio/
│
├── index.html        ← Halaman utama (Home)
├── projects.html     ← Halaman detail project
│
├── css/
│   └── style.css     ← Semua tampilan visual ada di sini
│
├── js/
│   └── main.js       ← Interaktivitas (animasi, klik, dsb.)
│
├── images/           ← Folder untuk foto & gambar
│   └── (kosong dulu, isi nanti)
│
└── README.md         ← File panduan ini
```

---

## 🚀 Cara Menjalankan Website (Dari Nol!)

### Langkah 1 — Download & Siapkan File

1. Download semua file portfolio ini
2. Simpan di satu folder, misalnya di `Documents/portfolio/`
3. Pastikan struktur foldernya sama seperti di atas

### Langkah 2 — Buka dengan Browser

**Cara paling mudah (tanpa install apapun):**
1. Buka folder `portfolio/`
2. Double-klik file `index.html`
3. Browser akan otomatis membuka websitemu! 🎉

**Cara yang lebih baik (pakai VS Code):**
1. Download **VS Code** gratis di: https://code.visualstudio.com/
2. Install extension **"Live Server"** (cari di tab Extensions, Ctrl+Shift+X)
3. Buka folder `portfolio/` di VS Code: File → Open Folder
4. Klik kanan `index.html` → pilih **"Open with Live Server"**
5. Browser otomatis terbuka & refresh setiap kamu simpan file!

---

## ✏️ Cara Kustomisasi — Yang Wajib Diganti

### Di `index.html`:

| Cari teks ini | Ganti dengan |
|---------------|--------------|
| `Nama Kamu` | Nama lengkap kamu |
| `Data Enthusiast & Beginner Data Analyst` | Peranmu yang sesungguhnya |
| `Saya bersemangat mengubah data...` | Deskripsi tentang dirimu |
| `https://github.com/usernamekamu` | URL GitHub kamu |
| `https://linkedin.com/in/namakamu` | URL LinkedIn kamu |
| `email@kamu.com` | Email kamu |

### Di `projects.html`:

| Cari teks ini | Ganti dengan |
|---------------|--------------|
| `Dashboard Analisis Penjualan Toko Online` | Judul project aslimu |
| `Menganalisis data penjualan 12 bulan...` | Tujuan project aslimu |
| `Data transaksi penjualan dari Kaggle...` | Info dataset yang kamu pakai |
| Bagian Key Insights | Temuan nyata dari analisismu |
| Link GitHub di bagian bawah | Link repo GitHub aslimu |

---

## 🖼️ Cara Menambahkan Foto Diri

1. Siapkan foto kamu (format JPG/PNG, ukuran sekitar 400x400 pixel)
2. Rename file-nya menjadi `foto-saya.jpg`
3. Taruh di folder `images/`
4. Di `index.html`, cari bagian `about-photo` dan ganti:

```html
<!-- SEBELUM (pakai emoji): -->
<div class="about-photo">
  🧑‍💻
</div>

<!-- SESUDAH (pakai foto): -->
<div class="about-photo" style="padding:0; overflow:hidden;">
  <img src="images/foto-saya.jpg" alt="Foto Nama Kamu"
       style="width:100%; height:100%; object-fit:cover;">
</div>
```

---

## 📸 Cara Upload Screenshot Dashboard

1. Buka halaman `projects.html` di browser
2. Klik kotak bergaris putus-putus bertulisan "Klik atau drag & drop"
3. Pilih file screenshot dari komputermu
4. Gambar akan langsung tampil!

**Catatan:** Upload ini hanya sementara (di memori browser).
Untuk permanen, taruh file gambar di folder `images/` dan edit HTML-nya:

```html
<!-- Ganti screenshot-area dengan gambar statis: -->
<img src="images/screenshot-dashboard.png" alt="Screenshot Dashboard"
     style="width:100%; border-radius:14px; border:1px solid #e4e8ef;">
```

---

## 🌐 Cara Publish ke Internet (Gratis!)

### Opsi 1: GitHub Pages (Recommended untuk programmer)

1. Daftar akun di https://github.com (gratis)
2. Buat repository baru, nama bebas (misal: `portfolio`)
3. Upload semua file portfolio ke repo itu
4. Masuk ke Settings → Pages → pilih branch `main` → Save
5. Website kamu online di: `https://usernamekamu.github.io/portfolio/`

### Opsi 2: Netlify (Paling mudah, drag & drop)

1. Daftar di https://netlify.com (gratis)
2. Drag & drop folder `portfolio/` ke dashboard Netlify
3. Selesai! Websitemu langsung online dengan URL otomatis
4. Bisa custom domain gratis juga!

---

## 🎨 Cara Ganti Warna

Buka `css/style.css`, cari bagian `:root` di paling atas:

```css
:root {
  --color-accent: #3b6cf8;    /* ← Ganti ini untuk ubah warna biru utama */
  --color-bg:     #f8f9fb;    /* ← Ganti ini untuk ubah warna latar */
}
```

Contoh warna populer:
- Hijau: `#16a34a`
- Ungu: `#7c3aed`
- Orange: `#ea580c`
- Pink: `#db2777`

---

## ➕ Cara Menambah Project Baru

Di `index.html`, cari `<!-- Card Project 3 -->` dan tambahkan sesudahnya:

```html
<!-- Card Project 4 (baru) -->
<article class="project-card fade-up">
  <div class="project-thumb">
    📊  ← ganti emoji sesuai project
  </div>
  <div class="project-body">
    <div class="project-tag">Kategori</div>
    <h3 class="project-title">Nama Project Baru</h3>
    <p class="project-desc">Deskripsi singkat project baru kamu.</p>
    <div class="project-footer">
      <div class="project-tools">
        <span class="tag">Tool 1</span>
        <span class="tag">Tool 2</span>
      </div>
      <a href="projects.html" class="btn btn-ghost" style="padding:6px 14px; font-size:.8rem">
        Detail →
      </a>
    </div>
  </div>
</article>
```

---

## ❓ FAQ (Pertanyaan Umum)

**Q: Font tidak muncul / tampilan aneh**
A: Pastikan kamu terkoneksi internet saat pertama kali membuka (untuk download Google Fonts).

**Q: Animasi tidak jalan**
A: Pastikan file `js/main.js` ada dan path-nya benar. Coba buka dengan Live Server.

**Q: Mau ganti judul tab browser**
A: Cari tag `<title>` di file HTML, ganti teksnya.

**Q: Gambar tidak muncul**
A: Pastikan nama file dan path sudah benar (case-sensitive! `Foto.jpg` ≠ `foto.jpg`).

---

## 📚 Belajar Lebih Lanjut

- **HTML dasar:** https://www.w3schools.com/html/
- **CSS dasar:** https://www.w3schools.com/css/
- **JavaScript dasar:** https://javascript.info/
- **Deploy gratis:** https://netlify.com · https://pages.github.com

---

Semangat belajar! 🚀 Setiap expert dulunya adalah pemula.

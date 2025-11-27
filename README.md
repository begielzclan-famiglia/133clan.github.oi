# 133clan.github.oi# Repo template: 133clan.github.io

Ini adalah paket template lengkap untuk **Website Blog Resmi Secret Society 133Clan** yang siap Anda copy-paste ke repository GitHub Pages bernama `133clan.github.io`.

> File di bawah disusun sebagai: `path` lalu blok kode berisi isi file. Salin tiap file apa adanya ke struktur yang sama.

---

## Struktur repo

```
133clan.github.io/
│
├── _config.yml
├── index.md
├── about/index.md
├── manifesto/index.md
├── _posts/
│   └── 2025-01-01-salam-pembuka.md
├── assets/
│   ├── css/style.css
│   └── images/ (taruh logo di sini sebagai logo.png)
├── README.md
├── .gitignore
└── CNAME (opsional)
```

---

## File: _config.yml

```yml
title: "Secret Society 133Clan"
description: "Ruang senyap untuk pemikir dan eksplorator dalam lingkaran 133."
baseurl: "" # gunakan kosong untuk user/organization pages
url: "https://133clan.github.io"

theme: minima
markdown: kramdown
show_excerpts: true

author:
  name: "133 Council"
  email: "secret@133clan.org"

plugins:
  - jekyll-feed
  - jekyll-seo-tag

# Menambahkan folder assets agar disertakan
include:
  - assets

# Pengaturan navigasi sederhana
nav:
  - title: "Home"
    url: "/"
  - title: "Manifesto"
    url: "/manifesto/"
  - title: "Arsip"
    url: "/archives/"
  - title: "Tentang"
    url: "/about/"

# Opsi: aktifkan GitHub Pages built-in

display_toc: false
```

---

## File: index.md

```markdown
---
layout: home
title: "133Clan"
---

Selamat datang di lingkaran.

Situs ini memuat manifesto, arsip, dan pemikiran dari Secret Society 133Clan.

Lihat tulisan terbaru di bagian Arsip.
```

---

## File: about/index.md

```markdown
---
layout: page
title: "Tentang 133Clan"
permalink: /about/
---

**133Clan** adalah komunitas eksklusif untuk pemikir, penjelajah, dan penjaga simbol. Situs ini berfungsi sebagai arsip tulisan, pedoman, dan catatan internal yang boleh dibaca publik.

> Jika Anda ingin kontak resmi: secret@133clan.org
```

---

## File: manifesto/index.md

```markdown
---
layout: page
title: "Manifesto"
permalink: /manifesto/
---

### Manifesto 133

Kami menghargai ketenangan, kajian mendalam, dan kehati-hatian. Nama, simbol, dan ritual kami adalah alat untuk mengarahkan energi kolektif pada pengetahuan.

Dokumen ini bisa diperluas sesuai kebutuhan Council.
```

---

## File: _posts/2025-01-01-salam-pembuka.md

```markdown
---
layout: post
title: "Salam Pembuka"
date: 2025-01-01 09:00:00 +0700
categories: [pengumuman]
---

Selamat datang di ruang senyap 133Clan.

Ini adalah awal dari arsip pengetahuan dan catatan perjalanan kami.
```

---

## File: assets/css/style.css

```css
/* Gaya dasar untuk tampilan gelap & aksen emas */
:root{
  --bg: #071028;
  --muted: #0b2a4a;
  --accent: #c99a3b;
  --light: #f6f2e9;
}

body{
  background: var(--bg);
  color: var(--light);
  font-family: Inter, 'Helvetica Neue', Arial, sans-serif;
  line-height: 1.6;
}

a{ color: var(--accent); text-decoration: none }

a:hover{ text-decoration: underline }

header.site-header{ padding: 2rem 1rem; text-align:center }

.site-title{ font-family: 'Playfair Display', serif; font-size: 2rem }

.container{ max-width: 900px; margin: 0 auto; padding: 1rem }

.post-meta{ color: #bdb6a8; font-size: 0.9rem }

footer{ text-align:center; padding: 2rem 1rem; color: #bfb9a9 }

/* Pastikan gambar logo tidak terlalu besar */
.site-logo{ max-width: 140px; height: auto }
```

---

## File: assets/images/README (petunjuk)

```
Letakkan file logo PNG/WEBP/SVG dengan nama 'logo.png' di folder assets/images/
Jika Anda punya versi vektor (.svg), taruh juga untuk kepentingan cetak.
```

---

## File: README.md

```markdown
# 133clan.github.io

Template ini untuk GitHub Pages (Jekyll). Cara pakai:

1. Buat repository baru di GitHub bernama `133clan.github.io`.
2. Upload seluruh isi folder ini (atau clone dan push dari lokal).
3. Buka Settings → Pages → pilih branch `main` → root `/` → Save.
4. Tunggu beberapa menit lalu buka: https://133clan.github.io

### Cara cepat via Git (di mesin lokal)

```
# pada folder project lokal yang berisi template
git init
git add .
git commit -m "Initial commit - 133Clan site"
# ganti URL remote dengan milik Anda
git remote add origin https://github.com/USERNAME/133clan.github.io.git
git branch -M main
git push -u origin main
```

Gasss — jika Anda butuh, saya bisa buatkan file ZIP yang siap di-upload atau langsung push ke repo jika Anda beri akses token (jangan kirim token secara publik; saya akan memberi instruksi aman jika mau).
```

---

## File: .gitignore

```
.DS_Store
*.pyc
node_modules/
.sass-cache/
_site/
.idea/
.vscode/
```

---

## Opsional: CNAME

Jika Anda ingin domain kustom, tambahkan file `CNAME` berisi domain Anda, mis. `www.133clan.org`.

---

## Cara deploy & cek cepat

1. Push ke repo bernama `133clan.github.io`.
2. Buka `https://github.com/USERNAME/133clan.github.io/settings/pages` untuk memastikan Pages diaktifkan.
3. Jika masih tema minima default, Anda dapat mengganti `_layouts` dan `_includes` untuk kustom desain (saya bisa buatkan jika mau).

---

## Hyperspeed opsi (opsional oleh saya)

Jika ingin: saya bisa juga langsung:
- buatkan ZIP file proyek yang bisa di-download, atau
- buat PR ke repo Anda (butuh akses), atau
- generate versi Hugo / Next.js jika ingin lebih modern.

Sampaikan pilihan—saya langsung proses.

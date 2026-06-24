# Auto Plus Carwash — Website Deployment

## Struktur File

```
autoplus-netlify/
├── index.html       ← File utama website
├── netlify.toml     ← Konfigurasi Netlify (headers, redirects, cache)
├── _redirects       ← Fallback redirect rules
├── robots.txt       ← Panduan untuk mesin pencari (SEO)
├── sitemap.xml      ← Peta website untuk Google
└── README.md        ← Panduan ini
```

---

## Cara Deploy ke Netlify

### Opsi 1: Drag & Drop (Paling Mudah)
1. Buka https://app.netlify.com
2. Login atau daftar akun gratis
3. Di dashboard, klik **"Add new site"** → **"Deploy manually"**
4. **Drag & drop seluruh folder** `autoplus-netlify` ke kotak yang tersedia
5. Tunggu beberapa detik → website langsung live! 🎉

### Opsi 2: Via GitHub (Disarankan untuk update rutin)
1. Upload seluruh isi folder ini ke repositori GitHub
2. Di Netlify: **"Add new site"** → **"Import from Git"**
3. Pilih repositori GitHub Anda
4. Settings build otomatis terdeteksi dari `netlify.toml`
5. Klik **"Deploy site"**
6. Setiap kali Anda push ke GitHub, website otomatis update

---

## Setelah Deploy — Setting Domain

### Menggunakan domain gratis Netlify
Website langsung bisa diakses via URL seperti:
`https://autoplus-xxxxx.netlify.app`

### Menggunakan domain sendiri (misal: autoplus-pasuruan.com)
1. Di Netlify: **Site settings** → **Domain management** → **Add custom domain**
2. Masukkan domain Anda
3. Arahkan DNS domain Anda ke Netlify (ikuti instruksi yang muncul)
4. SSL/HTTPS otomatis aktif gratis via Let's Encrypt

---

## Yang Masih Perlu Dilengkapi di index.html

Cari tanda `🔧 GANTI` di dalam file `index.html`:

| # | Yang Diganti | Pencarian di file |
|---|---|---|
| 1 | Foto hero/depan lokasi | `🔧 GANTI FOTO` |
| 2 | Embed Google Maps yang tepat | `🔧 GANTI MAPS` |
| 3 | Foto before/after | `🔧 GANTI BEFORE-AFTER` |
| 4 | Foto testimoni pelanggan | `🔧 GANTI TESTIMONI` |
| 5 | Domain canonical (jika beda) | `🔧 GANTI DOMAIN` |

---

## Menambahkan Foto

Buat folder `images/` di dalam folder ini, lalu upload foto Anda.
Contoh penggunaan di HTML:
```html
<!-- Ganti URL Unsplash dengan foto lokal -->
background-image: url('/images/foto-depan.jpg')
```

---

## Dukungan

Kontak pengembang atau hubungi:
📱 WhatsApp: 0896-6117-3827
📷 Instagram: @autopluspasuruan

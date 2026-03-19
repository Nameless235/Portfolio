# 🚀 Portfolio Muhammad Adam - Deployment Guide

Portfolio interaktif dengan UI/UX modern yang sudah siap deploy ke GitHub Pages!

## 📋 Cara Deploy ke GitHub Pages

### Step 1: Buat Repository GitHub Baru

1. **Buka GitHub** → [https://github.com/new](https://github.com/new)
2. **Nama Repository**: `portfolio` (atau nama lain yang Anda suka)
3. **Visibility**: Public
4. **JANGAN centang** "Add a README file"
5. Klik **Create repository**

### Step 2: Upload File ke Repository

Ada 2 cara:

#### **Cara A: Upload via Web (Paling Mudah)**

1. Di repository baru Anda, klik tombol **Add file** → **Upload files**
2. **Drag & drop** file `index.html` yang sudah saya siapkan
3. Di bagian bawah, tulis commit message: `Initial portfolio commit`
4. Klik **Commit changes**

#### **Cara B: Via Git (Untuk yang sudah familiar)**

```bash
# Clone repository
git clone https://github.com/USERNAME/portfolio.git
cd portfolio

# Copy file index.html ke folder ini
# Lalu:
git add .
git commit -m "Initial portfolio commit"
git push origin main
```

### Step 3: Aktifkan GitHub Pages

1. Di repository, klik tab **Settings**
2. Di menu samping kiri, klik **Pages**
3. Di bagian **Source**:
   - Branch: Pilih `main`
   - Folder: Pilih `/ (root)`
4. Klik **Save**
5. **Tunggu 1-2 menit** untuk deployment

### Step 4: Akses Portfolio Anda!

Portfolio Anda akan live di:
```
https://USERNAME.github.io/portfolio/
```

Ganti `USERNAME` dengan username GitHub Anda!

---

## 🎨 Fitur Portfolio

✅ **Animasi Smooth** - Parallax scrolling & micro-interactions  
✅ **Responsive Design** - Perfect di semua device  
✅ **Custom Cursor** - Interactive cursor effect  
✅ **Particle Background** - Dynamic particle system  
✅ **Skill Cards** - Animated skill showcase  
✅ **Project Gallery** - Hover effects & modals  
✅ **Contact Form** - Ready to connect  

---

## 🔧 Customisasi Portfolio

### Ganti Informasi Pribadi

Edit file `index.html`, cari bagian-bagian ini:

```html
<!-- Nama & Title -->
<div class="hero-name">
  <div>MUHAMMAD</div>
  <div class="stroke">ADAM</div>
</div>

<!-- Email & Social Media -->
<a href="mailto:adaamputra423@gmail.com">
<a href="https://linkedin.com/in/muhammad-adam-549427314/">
```

### Ganti Foto Profile

1. Siapkan foto Anda (format: JPG/PNG, ukuran: 300x400px recommended)
2. Upload foto ke repository
3. Edit `index.html`, cari:
```html
<img src="URL_FOTO_ANDA" alt="Muhammad Adam">
```

### Ganti Warna Theme

Di bagian `:root` dalam `<style>`, edit variabel ini:

```css
:root {
  --accent: #e8c547;     /* Warna utama (kuning) */
  --accent2: #4fffb0;    /* Hijau */
  --accent3: #ff6b6b;    /* Merah */
  --accent4: #7c6bff;    /* Ungu */
}
```

---

## 📱 Custom Domain (Opsional)

Jika punya domain sendiri (misal: `muhammadadam.com`):

1. Buat file `CNAME` di repository
2. Isi dengan domain Anda: `muhammadadam.com`
3. Di DNS provider, tambah record:
   - Type: `A`
   - Name: `@`
   - Value: `185.199.108.153`
4. Tunggu propagasi DNS (bisa 24 jam)

---

## 🐛 Troubleshooting

### Portfolio tidak muncul?
- Cek apakah GitHub Pages sudah aktif di Settings → Pages
- Pastikan file bernama `index.html` (bukan `portfolio.html`)
- Clear browser cache: `Ctrl + Shift + R`

### Foto tidak muncul?
- Pastikan path foto benar
- Upload foto ke repository GitHub
- Gunakan URL lengkap: `https://raw.githubusercontent.com/USERNAME/portfolio/main/photo.jpg`

### Animasi patah di mobile?
- Refresh halaman
- Cek koneksi internet
- Coba browser lain

---

## 📞 Contact

**Muhammad Adam**  
📧 adaamputra423@gmail.com  
💼 [LinkedIn](https://www.linkedin.com/in/muhammad-adam-549427314/)  
📍 Bogor, Indonesia

---

## 📜 License

Free to use for personal portfolio. Credit appreciated! 🙏

---

**Made with ❤️ & Code**

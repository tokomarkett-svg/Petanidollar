# 🚜 PetaniDolar

> **Tanam cuan tiap hari → panen dolar.** Aplikasi (installable di HP) buat kejar target dolar dari 2Captcha, Kolotibablo, MegaTypers, Toloka, Freecash, Remotasks, dan 48+ jalur cuan lain yang terverifikasi bayar.

**Alur aplikasi:** Beranda (pilih platform) → **1️⃣ Bikin akun** (link daftar resmi) → **2️⃣ Login** (link worker panel) → **3️⃣ Pilih tugas** (setiap tugas ada link langsung ke kerjanya) → kerja di tab platform → balik → catat hasil → saldo mentok → **TARIK**. 

**Ini alat bantu disiplin, BUKAN bot captcha** — pekerjaan tetap lo kerjain sendiri sesuai aturan platform (bot = akun banned + saldo hangus).

---

## ✨ Fitur (v3 — dirombak total)

- 🚜 **Logo + ikon aplikasi** (semua ukuran) & **installable PWA** — pasang di layar utama HP kayak aplikasi beneran (manifest + service worker)
- 🏠 **Beranda = lapangan kerja** — kartu platform yang beneran kita kerjain, ketuk → buka menu dalam
- 📋 **Menu dalam tiap platform** (contoh 2Captcha):
  - **1️⃣ Daftar** → tombol langsung ke `2captcha.com/auth/register` + checklist "udah daftar"
  - **2️⃣ Login** → tombol ke worker panel + checklist "udah bisa login"
  - **3️⃣ Pilih tugas** → semua jenis tugas 2Captcha: captcha standar, image, reCAPTCHA v2 gambar, reCAPTCHA v2 token, hCaptcha — tiap tugas ada rate, tips, dan **tombol "👉 KERJAKAN INI"** yang nyambung langsung ke panel kerja
- ➕ Catat hasil 2 detik (+$0.25…+$2, mode captcha otomatis, manual)
- 📊 Target minggu/harian + progress bar + alarm **"SIAP CAIR 💸"**
- 🗺️ **Peta Cuan** — 54 platform terverifikasi per kategori + badge negara
- ⏱️ Timer sesi 25/15/5 menit
- ⬇️ Ekspor CSV, ⚙️ pengaturan lengkap, 🚨 alarm scam

Data 100% di perangkat lo (localStorage). Tanpa server, tanpa kirim data ke luar.

---

## 📂 Struktur Repo

```
Petanidollar/
├── index.html              ← aplikasi utama
├── manifest.webmanifest    ← PWA (bisa di-install)
├── sw.js                   ← service worker (cache/offline)
├── icons/                  ← logo & ikon (512/192/180/64 + sumber)
└── README.md
```

---

## 🚀 Deploy & Pasang di HP

1. **vercel.com** → Sign Up with GitHub → **Add New → Project** → pilih **Petanidollar** → **Deploy**
2. Dapet link **`https://petanidollar.vercel.app`** (auto-update tiap lo push)
3. **Android (Chrome):** buka link → menu ⋮ → **Tambahkan ke layar utama**
4. **iPhone (Safari):** tombol Bagikan ⬆️ → **Tambahkan ke Layar Utama**
5. Buka dari ikon 🚜 → fullscreen, kayak aplikasi beneran, ada tombol **📲 Install** juga di header

---

## 📅 Strategi

| Minggu | Fokus |
|---|---|
| 1 | 2Captcha (tanpa batas) + Toloka + Freecash → target $20 |
| 2–4 | + Clickworker/UHRS, Microworkers, Appen → $40–60 |
| 2–6 | Mulai profil Upwork/Fiverr (jual skill) |
| Bulan 2–3 | Freelance pertama → $100–300/bln |

**Aturan emas:** daftar gratis → kerja → saldo kebaca → tarik dana. Nol rupiah keluar. Minta deposit = scam, kabur.

---

## 🛠️ Roadmap

| Versi | Isi |
|---|---|
| **v3 (sekarang)** | Rombak total: logo, PWA installable, dashboard → detail (daftar/login/tugas) → kerja |
| v4 | Sinkron saldo otomatis via API resmi 2Captcha (getBalance) lewat serverless Vercel — API key di environment variable, TIDAK pernah di kode depan |
| v5 | Grafik tren, mode tantangan harian, leaderboard sesama petani |

---

*Kerja, catat, cair. 💪*

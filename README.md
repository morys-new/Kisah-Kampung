# 🏡 Kisah Kampung

Game web *life-sim* sederhana bergaya **Citampi Stories**: hidup di kampung, cari kerja, makan, tidur, jalan-jalan, dan naksir gadis desa. Dibuat dengan HTML, CSS, dan JavaScript murni — **tanpa library, tanpa build tool**.

## ▶️ Cara menjalankan

Pilih salah satu:

**1. Paling cepat** — klik dua kali `index.html`, langsung kebuka di browser.

**2. Lewat VSCode (disarankan)**
1. Buka folder ini di VSCode (`File > Open Folder`).
2. Install ekstensi **Live Server** (oleh Ritwick Dey).
3. Klik kanan `index.html` → **Open with Live Server**.
4. Browser kebuka otomatis dan auto-refresh tiap kamu menyimpan perubahan.

> Game ini pakai font dari Google Fonts, jadi sambungkan internet biar tampilannya pas. Tetap jalan tanpa internet, hanya fontnya jadi default.

## 📁 Struktur folder

```
kisah-kampung/
├── index.html        ← struktur halaman
├── css/
│   └── style.css     ← semua tampilan & warna
├── js/
│   ├── data.js       ← KONFIGURASI: angka, tempat, gaji (ubah di sini buat balancing)
│   └── game.js       ← logika permainan
└── README.md
```

## 🎮 Cara main

- Tiap hari punya **4 waktu**: Pagi, Siang, Sore, Malam. Aksi besar memakai 1 waktu; kalau habis, kamu tidur untuk ganti hari.
- Jaga 4 hal: **Uang, Energi, Kenyang, Senang**. Perut kosong bikin energi & mood ikut turun.
- **Kerja** di sawah, warung, atau proyek (skill naik tiap kerja → gaji ikut naik). Bisa juga **mancing** untuk rezeki tak terduga.
- **Makan** di Warung Bu Inah, main di **Taman**, dan kunjungi **Rumah Sari** untuk mendekatinya.
- **Target:** kumpulkan uang → **beli rumah** → cinta Sari 100% → **nembak**. 💍

## 🔧 Mau ngoprek?

Buka `js/data.js` — semua angka penting ada di situ:
- `S.uang` → modal awal
- `S.goalTarget` → harga rumah impian
- `GAJI_DASAR` → gaji tiap pekerjaan
- `PLACES` → tambah/ubah tempat
- `SKY` → warna langit tiap waktu

Logika tiap aksi ada di `js/game.js` (cari fungsi `kerja`, `makan`, `doAct`, `tidur`, dst).

## 💡 Ide pengembangan

- Simpan progres pakai `localStorage` (lanjut main tanpa mulai ulang).
- Tambah NPC & dialog bercabang.
- Sistem inventaris & toko (beli baju, perabot, upgrade rumah).
- Peta yang bisa dijelajahi pakai keyboard.

Selamat ngoprek! 🌾

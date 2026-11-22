# Custom Alert Stream

Kumpulan 47 template alert donasi untuk live stream. Semua template dibuat pakai HTML & CSS murni, jadi bisa langsung dipakai di **Saweria**, **SociaBuzz**, atau platform donasi lain yang mendukung fitur Custom HTML/CSS.

**Lihat semua template di sini:**  
https://farrelghibran.github.io/Custom-Alert-Stream/

---

## Cara Pilih & Ambil Kode

1. Buka halaman galeri di atas, lalu cari atau filter tema yang cocok sama gaya stream kamu.
2. Klik **Buka** di kartu template yang dipilih.
3. Di halaman preview, kamu bisa coba-coba langsung:
   - Ubah nama donatur, nominal, dan pesan buat lihat hasilnya.
   - Klik **Border: ON / OFF** kalau mau pakai atau lepas bingkai luar. Kode CSS di bawahnya bakal ikut berubah otomatis.
4. Scroll ke bagian **Source Code**, lalu klik **Salin HTML** dan **Salin CSS**.

---

## Cara Pasang ke Platform Donasi

### 1. Saweria
1. Login ke dashboard Saweria, lalu masuk ke menu **Overlay** → **Alert**.
2. Aktifkan opsi **Custom HTML & CSS**.
3. Tempel kode yang sudah disalin dari `packs.html` ke kolom **HTML**, dan kode dari `style.css` ke kolom **CSS**.
4. Pastikan variabel bawaan `{donator}`, `{amount}`, dan `{message}` tidak terhapus.
5. Klik **Simpan Tampilan**, lalu tes pakai tombol notifikasi uji coba.

### 2. SociaBuzz (atau Platform Lain)
1. Masuk ke pengaturan **Overlay / Alert** di dashboard platform yang kamu pakai (misalnya SociaBuzz Tribe).
2. Buka bagian **Custom HTML & CSS** (atau pengaturan tampilan kustom).
3. Tempel kode HTML dan CSS dari template pilihanmu.
4. **Penting:** Setiap platform kadang punya format variabel yang sedikit berbeda. Kalau nama/nominal/pesan tidak muncul, cukup ganti `{donator}`, `{amount}`, dan `{message}` di bagian HTML sesuai variabel yang dipakai platform tersebut.
5. Simpan perubahan dan lakukan tes alert.

---

## Cara Pasang ke OBS Studio

1. Salin **URL Overlay Alert** dari dashboard Saweria / SociaBuzz kamu.
2. Di OBS Studio, tambahkan source baru: **Sources (`+`) → Browser**.
3. Tempel URL overlay tadi ke kolom **URL**.
4. Atur ukuran kanvas (rekomendasi: **Width `850`**, **Height `450`** supaya animasi dan efek glow tidak kepotong).
5. Klik **OK** dan posisikan alert di layar stream sesuai selera.

---

## Struktur Folder

```text
Custom-Alert-Stream/
├── index.html              # Halaman galeri utama
└── Templates/
    └── alert1 .. alert47/
        ├── index.html      # Halaman preview + tombol salin kode
        ├── packs.html      # Kode HTML alert
        └── style.css       # Kode CSS alert
```

Kalau mau jalanin secara lokal di komputer sendiri, buka folder ini pakai **Live Server** (VS Code) atau jalankan `npx serve .` supaya fitur salin source code bisa membaca file secara otomatis.

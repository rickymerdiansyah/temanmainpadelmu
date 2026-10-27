# TMP · Teman Main Padelmu

Web app untuk mengatur turnamen padel bareng teman. Formatnya Americano, Team Americano, Mix Americano, Mexicano, Team Mexicano, Mixicano, dan King of the Court. Jadwal dibuat otomatis, skor langsung masuk klasemen, dan semua fitur gratis.

## Cara pakai di iPhone

1. Buka link GitHub Pages repo ini di **Safari**.
2. Ketuk tombol **Bagikan**, lalu pilih **Add to Home Screen**.
3. Buka TMP dari ikon di home screen.

Data turnamen tersimpan di HP itu. Kalau kamu buka TMP dari ikon home screen, data tetap ada walaupun app ditutup. Data tidak tersinkron ke HP lain.

Setelah dibuka sekali saat online, TMP tetap bisa dipakai tanpa sinyal di lapangan.

## Link live untuk peserta

Di halaman turnamen, ketuk ikon **Bagikan** lalu **Buat link live**. Kirim linknya ke grup peserta. Setiap skor yang diisi langsung ter-update di HP peserta. Peserta hanya bisa melihat, tidak bisa mengubah skor. Hanya HP yang membuat link yang bisa meng-update skornya.

Data link live disimpan di Firebase Firestore (project `temanmainpadelmu`).

## Isi repo

| File | Fungsi |
|---|---|
| `index.html` | Seluruh aplikasi dalam satu file |
| `manifest.webmanifest` | Nama, ikon, dan warna saat dipasang di home screen |
| `sw.js` | Service worker supaya bisa dipakai offline |
| `icons/` | Ikon aplikasi dan favicon |

## Menerbitkan ke GitHub Pages

1. Buka **Settings → Pages** di repo ini.
2. Di **Source**, pilih **Deploy from a branch**. Branch: `main`, folder: `/ (root)`.
3. Tunggu sekitar 1 menit. Linknya akan berbentuk `https://rickymerdiansyah.github.io/temanmainpadelmu/`.

## Update aplikasi

Ganti `index.html` dengan versi baru lalu commit. Kalau ada perubahan besar, naikkan juga `VERSION` di `sw.js`, misalnya `tmp-v2`, supaya HP pengguna mengambil versi terbaru.

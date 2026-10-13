# Maxim Driver PWA — prototipe pendamping

Prototipe ini dibuat dengan mengambil inspirasi umum dari aplikasi Taxsee Driver APK versi 3.27.4 yang diunggah pengguna, terutama konteks penggunaan driver dan gaya visual kuning-hitam. Ini **bukan konversi langsung** dari APK, bukan aplikasi resmi Maxim, dan tidak memakai atau mengubah kode internal APK.

## Yang bisa dilakukan
- Mencatat order, tarif, biaya bensin, dan perkiraan pendapatan bersih.
- Melihat ringkasan harian.
- Mengekspor catatan order ke CSV.
- Menyimpan catatan hotspot secara manual, termasuk koordinat GPS opsional.
- Mengaktifkan pengingat saat order sepi (15, 20, atau 30 menit) selama halaman tetap aktif.
- Menyimpan data di browser perangkat dengan `localStorage`.
- Cache offline dasar melalui service worker setelah aplikasi pertama kali dibuka melalui HTTPS.

## Yang tidak dilakukan
- Tidak login ke akun Maxim.
- Tidak menerima order langsung dari Maxim.
- Tidak membaca, memodifikasi, atau memanipulasi sistem dispatch, aplikasi, atau APK Taxsee Driver.
- Tidak menjamin pengingat berjalan saat Chrome ditutup atau Android membatasi aktivitas latar belakang.

## Cara memasang di Android / Realme C53
1. Ekstrak ZIP ini.
2. Unggah seluruh isi folder ke hosting statis yang mendukung HTTPS (misalnya GitHub Pages atau layanan hosting statis lain).
3. Buka alamat HTTPS tersebut di Chrome.
4. Tekan menu ⋮ lalu pilih **Instal aplikasi** atau **Tambahkan ke layar utama**.
5. Jalankan ikon **Maxim Driver** dari layar utama.

PWA memerlukan HTTPS (atau localhost untuk pengujian) agar service worker dan pemasangan aplikasi berfungsi penuh. Membuka `index.html` langsung dari file manager hanya untuk melihat demo; tidak mengaktifkan semua kemampuan PWA.

## Penyesuaian tampilan
Untuk membuat tampilannya lebih mendekati layar Taxsee Driver yang Anda gunakan, kirim 2–4 screenshot dari layar utama, pendapatan, dan menu order. Tutupi nama, nomor telepon, alamat, ID akun, dan informasi pribadi terlebih dahulu. Screenshot dipakai sebagai referensi tampilan, bukan untuk menyalin fungsi internal atau mengakses akun.

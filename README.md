# TabunganKu Kelas

Aplikasi pencatat tabungan kelas (setoran, penarikan, saldo, riwayat, total kas).
Data disimpan di perangkat. Dibungkus menjadi APK dengan Capacitor dan dibangun otomatis oleh GitHub Actions.

## Cara membuat APK
1. Buat repositori baru di GitHub (misalnya `tabunganku`).
2. Unggah seluruh isi folder ini, termasuk folder `.github` dan `www`, ke cabang `main`.
3. Buka tab **Actions**, pilih **Build APK**, lalu klik **Run workflow**. Build juga jalan otomatis setiap ada push ke `main`.
4. Tunggu sampai selesai (sekitar 3 sampai 6 menit), buka hasil run, lalu unduh **TabunganKu-debug-apk** di bagian Artifacts.
5. Ekstrak zip-nya, kirim `app-debug.apk` ke ponsel, dan pasang (izinkan pemasangan dari sumber tidak dikenal).

## Mengubah aplikasi
- Tampilan dan logika ada di `www/index.html`.
- Nama aplikasi dan ID paket ada di `capacitor.config.json`.
- APK yang dihasilkan adalah versi debug untuk uji coba. Untuk rilis resmi perlu penandatanganan (keystore).

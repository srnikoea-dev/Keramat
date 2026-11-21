KERAMAT - Proyek Android WebView Offline

Konfigurasi:
- Nama aplikasi: Keramat
- Minimum Android: 7.0 (API 24)
- Orientasi: Portrait
- Konten: UH Guru dan UH Siswa dari HTML yang diberikan
- Tidak meminta izin INTERNET dan tidak memakai layanan web
- JavaScript + DOM Storage aktif
- Mode Siswa: pemilih file JSON Android
- Mode Guru: simpan file JSON melalui pemilih lokasi penyimpanan Android

Cara membuat APK:
1. Buka folder proyek ini melalui Android Studio (Open).
2. Pastikan Android SDK Platform 35 dan Android Gradle Plugin yang diperlukan tersedia.
3. Pilih Build > Build Bundle(s) / APK(s) > Build APK(s).
4. APK debug akan dibuat di app/build/outputs/apk/debug/app-debug.apk.

Catatan:
- File ZIP ini adalah proyek sumber Android Studio, bukan APK hasil kompilasi.
- Fitur Bagikan pada halaman Guru menggunakan Web Share API dan mungkin tidak tersedia di WebView; gunakan tombol Simpan file JSON untuk menyimpan file dan membagikannya melalui aplikasi file/Bluetooth.
- Uji pada perangkat Android sasaran sebelum digunakan untuk ujian.

BUILD APK MELALUI GITHUB ACTIONS:
1. Buat repository baru di GitHub.
2. Ekstrak ZIP proyek ini di komputer.
3. Unggah seluruh isi folder keramat-app ke repository (folder .github harus ikut terunggah).
4. Buka tab Actions di repository GitHub.
5. Pilih workflow "Build APK Keramat", lalu klik Run workflow.
6. Tunggu sampai proses selesai dengan status hijau.
7. Buka hasil workflow, bagian Artifacts, lalu unduh "Keramat-debug-APK".
8. Ekstrak file ZIP artifact untuk mendapatkan app-debug.apk.

Workflow juga berjalan otomatis setiap ada push ke branch main atau master.
APK yang dihasilkan adalah APK debug untuk pengujian dan pemasangan langsung, bukan APK release bertanda tangan untuk distribusi Play Store.

# 🏫 Sistem Absensi Guru - SD Islam Al Alaq

**Aplikasi Manajemen Kehadiran & Guru Pengganti Berbasis Web**

Repository ini berisi *client-side wrapper* untuk Sistem Absensi Guru SD Islam Al Alaq. Aplikasi utama berjalan menggunakan **Google Apps Script (GAS)** yang terhubung langsung dengan Google Sheets sebagai database, dan ditampilkan di sini menggunakan metode `iframe` responsif untuk kemudahan akses via domain publik atau Vercel/GitHub Pages.

---

## 🚀 Fitur Utama

### 1. 🔐 Panel Admin & Keamanan
* **Login Terproteksi:** Akses khusus admin dengan username dan password sederhana.
* **Sesi Aman:** Logout otomatis me-refresh halaman untuk keamanan data.

### 2. 📝 Form Absensi Digital
* **Input Mudah:** Mencatat guru yang berhalangan hadir (Sakit, Izin, Cuti, Dinas, dll).
* **Tanggal Otomatis:** Form otomatis mendeteksi tanggal hari ini (Realtime).
* **Multi-Input:** Mendukung pencatatan banyak guru dalam satu waktu.

### 3. 🔄 Manajemen Guru Pengganti (Inval)
* **Penugasan Inval:** Menentukan siapa yang menggantikan guru yang absen.
* **Detail Kelas:** Mencatat Mata Pelajaran, Kelas, dan Jumlah Jam Mengajar (JJM).
* **Database Guru:** Dropdown nama guru otomatis sinkron dengan database sekolah.

### 4. 📊 Rekapitulasi & Laporan
* **Rekap Kehadiran:** Tabel bulanan status kehadiran seluruh guru (Sakit/Izin/Alpa).
* **Rekap Pengganti:** Laporan kinerja guru pengganti beserta total jam mengajar.
* **Export PDF:** Fitur cetak laporan langsung ke format PDF siap print.

### 5. 📅 Kalender Akademik
* **Setting Libur:** Admin dapat menandai hari libur nasional/sekolah.
* **Visual Kalender:** Tampilan kalender interaktif untuk manajemen tanggal merah.

---

## 🛠️ Teknologi

* **Backend:** Google Apps Script (GAS).
* **Database:** Google Sheets.
* **Frontend Wrapper:** HTML5, CSS (Full Screen Iframe).
* **UI Framework (Internal App):** Tailwind CSS, FontAwesome, SweetAlert2.
* **Hosting:** Vercel / GitHub Pages.

---

## 📦 Cara Instalasi & Deployment

Jika Anda ingin men-deploy ulang atau memindahkan ke repository lain:

1.  **Siapkan Script:** Pastikan Google Apps Script sudah di-deploy sebagai *Web App* dengan akses **"Anyone"**.
2.  **Clone Repo:** Clone repository ini ke komputer lokal atau buat repo baru di GitHub.
3.  **Update Link:** Buka file `index.html` dan ganti URL pada tag `iframe`:
    ```html
    <iframe src="https://script.google.com/macros/s/AKfycbwL5V4uP8HDRcuMDe0Nl7z1ro1nzRsStfS7kj5q-YVuHI1sN_iwo7X_VQuXArUe8KoFrw/exec"></iframe>
    ```
4.  **Push:** Commit dan push perubahan ke GitHub.
5.  **Deploy:** Aktifkan **GitHub Pages** (di menu Settings) atau hubungkan repository ke **Vercel**.

---

## 📝 Catatan Penggunaan

* **Akses:** Jika muncul pesan *"File tidak dapat dibuka"*, pastikan setting deploy di Google Script pada bagian **"Who has access"** diatur menjadi **"Anyone"**.
* **Browser:** Disarankan menggunakan Google Chrome atau browser modern lainnya untuk tampilan terbaik.

---


**© 2024 SD Islam Al Alaq - Dikembangkan untuk Penggunaan Internal.**

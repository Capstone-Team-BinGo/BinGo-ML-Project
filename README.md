# BinGo! - Edukasi Inklusif Pemilahan Sampah Berbasis Teknologi untuk Anak-anak

## Deskripsi Proyek

Pengelolaan sampah yang tepat sangat penting untuk menjaga kebersihan dan kelestarian lingkungan. Sampah terdiri dari tiga kategori utama: organik, anorganik, dan B3 (Bahan Berbahaya dan Beracun), yang masing-masing memerlukan penanganan yang berbeda. Namun, anak-anak sering kesulitan dalam memilah sampah secara manual karena kurangnya metode pembelajaran yang menarik dan mudah dipahami.

Proyek ini bertujuan mengembangkan sebuah website edukatif yang menggunakan model deep learning dengan TensorFlow untuk mengklasifikasikan sampah secara otomatis. Sistem ini dirancang untuk mempermudah anak-anak dalam belajar memilah sampah secara cepat, tepat, dan interaktif, sehingga dapat meningkatkan kesadaran lingkungan sejak usia dini.

Pengembangan website ini melibatkan kolaborasi antara tim Machine Learning (ML), Front-End Developer, dan Back-End Developer. Masing-masing tim memiliki tanggung jawab sebagai berikut:

### Machine Learning

- Mengumpulkan dan menyusun data klasifikasi sampah dari Kaggle ke dalam folder terstruktur.
- Melakukan preprocessing data, meliputi resize gambar, undersampling, augmentasi, splitting data (train/val/test), dan normalisasi.
- Membangun model klasifikasi sampah berbasis modifikasi **EfficientNetB0** menggunakan TensorFlow Keras dengan pendekatan transfer learning.
- Menambahkan layer Conv2D dan Dense untuk menyesuaikan klasifikasi tiga kategori sampah.
- Melakukan pelatihan model secara bertahap hingga fine-tuning dengan *unfreeze* sebagian layer base model.
- Menerapkan callback seperti EarlyStopping dan ModelCheckpoint untuk mencegah overfitting dan menyimpan model terbaik.
- Model yang dihasilkan memiliki akurasi sebesar 92% dan di-deploy untuk diintegrasikan dengan sistem Front-End dan Back-End.

### Front-End Developer

- Mengembangkan aplikasi web yang interaktif dan responsif menggunakan framework **Vue.js**.
- Fitur utama:
  - Pemindaian kamera untuk mengenali jenis sampah secara real-time.
  - Materi edukatif berupa konten pembelajaran interaktif dan mudah dipahami.
  - Kuis edukatif untuk menguji pemahaman pengguna secara menyenangkan.
- Fokus pada pengalaman pengguna (user experience) untuk menjangkau target usia sekolah dasar.

### Back-End Developer

- Mengembangkan server dengan **Node.js** dan **Express** untuk menangani logika aplikasi.
- Membangun RESTful API sebagai jembatan antara front-end dan model klasifikasi.
- Mengelola penyimpanan data menggunakan **PostgreSQL** untuk informasi pengguna dan artikel edukasi.
- Menerapkan **autentikasi dan otorisasi** dengan **JSON Web Token (JWT)** untuk menjaga keamanan akses pengguna.
- Menyusun struktur API yang modular untuk memudahkan pengembangan dan pemeliharaan jangka panjang.

---

## Anggota Tim

| Role  | Nama                         | Institusi                    |
|-------|------------------------------|------------------------------|
| ML    | Tiara Fitri Adani           | Universitas Sebelas Maret    |
| ML    | Kayla Argya Puruhita        | Universitas Sebelas Maret    |
| ML    | Dyana Gita Pratiwi          | Universitas Sebelas Maret    |
| FEBE  | Ayub Dwi Wicaksono          | Tiga Serangkai University    |
| FEBE  | Rizky Budiarto              | Tiga Serangkai University    |
| FEBE  | Afrian Viky Widyantono      | Tiga Serangkai University    |

---

## Repository

| Team           | Link                                                                 |
|--------------------|----------------------------------------------------------------------|
| Machine Learning | [Bingo!-ML](https://github.com/Capstone-Team-BinGo/BinGo-ML-Project)           |
| Front-End         | [Bingo!-FE](https://github.com/Capstone-Team-BinGo/BinGo-Frontend-Project) |
| Back-End          | [Bingo!-BE](https://github.com/Capstone-Team-BinGo/BinGo-Backend-Project)   |

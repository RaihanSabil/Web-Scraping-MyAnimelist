# Web Scraper MyAnimeList (Data Seiyuu & Anime) 📊

Proyek ini adalah sebuah skrip *web scraping* yang dirancang khusus untuk mengambil data dari situs [MyAnimeList.net](https://myanimelist.net/). Tujuan utamanya adalah untuk mengumpulkan informasi detail mengenai **Seiyuu (pengisi suara)** dan **Anime** yang mereka perankan.

Data yang dihasilkan bisa menjadi dasar untuk analisis, visualisasi, atau sekadar membangun database lokal terkait industri anime.


*(Tips: Ganti tag ini dengan screenshot terminal saat skrip berjalan atau cuplikan file CSV/JSON yang dihasilkan agar lebih informatif!)*

---

## ✨ Fitur Utama

* **Ekstraksi Data Seiyuu**: Mengambil informasi profil seiyuu seperti nama, tanggal lahir, biografi, dan daftar peran.
* **Ekstraksi Data Anime**: Mengumpulkan detail anime yang diperankan oleh seiyuu, termasuk judul, rating, studio, dan tahun rilis.
* **Output Terstruktur**: Menyimpan data yang telah di-scrape ke dalam format yang mudah dibaca dan diolah, seperti **CSV** atau **JSON**. `[SESUAIKAN]`
* **Efisien dan Ringan**: Dibuat menggunakan library Python yang populer dan efisien untuk tugas *web scraping*.
* **Mudah Dimodifikasi**: Kode sumber yang bersih memudahkan pengguna lain untuk memodifikasi target data yang ingin diambil.

---

## 🛠️ Teknologi yang Digunakan

* **Python 3.8+**
* **Beautiful Soup 4 (bs4)**: Library utama untuk mem-parsing konten HTML dari halaman web.
* **Requests**: Untuk mengirim permintaan HTTP dan mengambil halaman web dari MyAnimeList.
* **Pandas**: Untuk mengelola data dan menyimpannya ke dalam format CSV. `[SESUAIKAN jika Anda menggunakan library lain atau format berbeda]`
* **LXML**: Sebagai parser HTML yang cepat dan efisien.

---

## 🚀 Instalasi dan Konfigurasi

Ikuti langkah-langkah di bawah ini untuk menyiapkan dan menjalankan skrip di lingkungan lokal Anda.

1.  **Clone Repositori**
    ```bash
    git clone [https://github.com/RaihanSabil/Web-Scraping-MyAnimelist.git](https://github.com/RaihanSabil/Web-Scraping-MyAnimelist.git)
    cd Web-Scraping-MyAnimelist
    ```

2.  **(Rekomendasi) Buat Virtual Environment**
    Ini akan membantu menjaga dependensi proyek Anda tetap terisolasi.
    ```bash
    python -m venv venv
    source venv/bin/activate  # Untuk Windows, gunakan: venv\Scripts\activate
    ```

3.  **Install Dependensi**
    Semua library yang dibutuhkan tercantum dalam file `requirements.txt`.
    ```bash
    pip install -r requirements.txt
    ```
    *(Jika Anda belum punya file ini, buatlah dengan menjalankan `pip freeze > requirements.txt` setelah semua library terpasang).*

---

## 🏃‍♀️ Cara Menjalankan Skrip

Setelah instalasi selesai, Anda dapat menjalankan skrip utama dari terminal.

1.  **Jalankan Skrip**
    Buka terminal dan pastikan Anda berada di direktori proyek.
    ```bash
    python main_scraper.py
    ```
    `[SESUAIKAN]` *Ganti `main_scraper.py` dengan nama file Python utama Anda.*

2.  **Periksa Hasil**
    Setelah skrip selesai berjalan, file output bernama `[SESUAIKAN: contoh: data_seiyuu.csv]` akan dibuat di direktori utama. File ini berisi semua data yang berhasil di-scrape.

---

## 🎯 Contoh Data yang Diambil

Skrip ini akan mengambil data berikut:

| Nama Seiyuu      | Tanggal Lahir | Anime yang Diperankan | Peran            | Rating Anime |
| ---------------- | ------------- | --------------------- | ---------------- | ------------ |
| Kana Hanazawa    | Feb 25, 1989  | Bakemonogatari        | Nadeko Sengoku   | 8.32         |
| Kamiya Hiroshi   | Jan 28, 1975  | Shingeki no Kyojin    | Levi             | 8.53         |
| ...              | ...           | ...                   | ...              | ...          |

`[SESUAIKAN]` *Ubah tabel di atas agar sesuai dengan kolom dan contoh data yang benar-benar dihasilkan oleh skrip Anda.*

---

## ⚠️ **Peringatan Etika Web Scraping**

* Skrip ini dibuat untuk tujuan edukasi dan penggunaan pribadi.
* **Jangan mengirim permintaan terlalu cepat** ke server MyAnimeList untuk menghindari pemblokiran IP. Pertimbangkan untuk menambahkan jeda (`time.sleep()`) di antara permintaan.
* Patuhi file `robots.txt` dan Ketentuan Layanan dari MyAnimeList.net.

---

## 🤝 Kontribusi

Jika Anda ingin berkontribusi, silakan buat *fork* repositori ini, lakukan perubahan, dan ajukan *pull request*. Setiap saran dan perbaikan sangat diterima!

---

## 📜 Lisensi

Proyek ini dilisensikan di bawah **MIT License**. Lihat file `LICENSE` untuk detail lebih lanjut.

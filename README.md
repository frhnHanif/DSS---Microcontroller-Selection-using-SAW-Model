# 🏆 Sistem Pendukung Keputusan: Pemilihan Mikrokontroler dengan Metode SAW

Proyek ini adalah implementasi Sistem Pendukung Keputusan (SPK) menggunakan metode **Simple Additive Weighting (SAW)** dengan studi kasus pemilihan mikrokontroler terbaik untuk proyek perangkat IoT. Proyek ini dibuat sebagai pemenuhan tugas mata kuliah SPK.



---

## 📝 Deskripsi

Skrip Python ini melakukan perangkingan terhadap 12 alternatif mikrokontroler/platform pengembangan berdasarkan 30 kriteria yang relevan. Proses ini membantu *engineer* atau pengambil keputusan untuk memilih komponen secara objektif berdasarkan prioritas yang telah ditentukan melalui pembobotan.

Data alternatif dan nilai kriteria yang ada di dalam skrip ini bersifat **placeholder/contoh**. Pengguna diharapkan menggantinya dengan data hasil riset yang valid untuk mendapatkan hasil yang akurat.

---

## ⚙️ Teknologi yang Digunakan

* **Python 3.x**
* **Pandas**: Untuk manipulasi data dalam bentuk tabel (DataFrame).
* **NumPy**: Untuk operasi numerik dan verifikasi bobot.

---

## 🚀 Cara Menjalankan

1.  **Clone Repositori**
    ```bash
    git clone [https://github.com/NAMA_ANDA/NAMA_REPO_ANDA.git](https://github.com/NAMA_ANDA/NAMA_REPO_ANDA.git)
    cd NAMA_REPO_ANDA
    ```

2.  **(Opsional tapi Direkomendasikan) Buat Virtual Environment**
    ```bash
    python -m venv venv
    # Aktivasi di Windows
    .\venv\Scripts\activate
    # Aktivasi di macOS/Linux
    source venv/bin/activate
    ```

3.  **Instal Dependensi**
    Pastikan Anda memiliki file `requirements.txt` yang berisi:
    ```
    pandas
    numpy
    ```
    Kemudian jalankan perintah:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Jalankan Skrip Utama**
    ```bash
    python nama_file_anda.py
    ```

---

## 🔧 Kustomisasi

Untuk mengadaptasi skrip ini sesuai kebutuhan Anda, modifikasi variabel-variabel berikut di dalam file `.py`:

* **`alternatif`**: Ubah isi list ini untuk mengganti atau menambah daftar mikrokontroler yang akan dievaluasi.
* **`data`**: Ini adalah bagian terpenting. Ganti nilai-nilai placeholder di dalam dictionary ini dengan data hasil riset Anda. Pastikan jumlah nilai pada setiap kriteria sama dengan jumlah alternatif.
* **`bobot`**: Sesuaikan nilai bobot (kepentingan) untuk setiap kriteria. **Pastikan total dari semua bobot adalah 1.0**.
* **`tipe_kriteria`**: Pastikan setiap kriteria didefinisikan dengan benar sebagai `'benefit'` (semakin tinggi semakin baik) atau `'cost'` (semakin rendah semakin baik).

---

## 📂 Struktur File

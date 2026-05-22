# Mini-Project-Bioinformatika_BISB211606
### Protokol Filogenetika Rasbora Berbasis Marka Gen COI

Repositori ini berisi panduan langkah-demi-langkah dan dokumentasi metode untuk melakukan pengumpulan sekuens, penyelarasan (*alignment*), dan rekonstruksi pohon filogenetik pada genus *Rasbora* menggunakan marka gen *Cytochrome c Oxidase Subunit I* (COI) dengan sekuens *Danio rerio* sebagai *outgroup*.

## 🛠️ Alat dan Bahan

Untuk menjalankan protokol analisis ini, komponen-komponen berikut diperlukan:
* **Perangkat Lunak & Platform Web:**
    * Web Browser (Google Chrome, Mozilla Firefox, Safari, atau sejenisnya)
    * [NCBI GenBank](https://www.ncbi.nlm.nih.gov/genbank/) (Platform pengumpulan database sekuens nukleotida)
    * [MAFFT Web Server](https://mafft.cbrc.jp/alignment/server/) (Alat penyelarasan sekuens dan rekonstruksi pohon filogenetik)
* **Data Sekuens:**
    * Sekuens target dalam format FASTA: Genus *Rasbora*.
    * Sekuens kontrol luar (*outgroup*) dalam format FASTA: *Danio rerio* (Zebrafish).

---

## 📋 Prosedur Kerja

Ikuti langkah-langkah di bawah ini secara berurutan untuk melakukan analisis:

### 1. Pengumpulan Sekuens Nukleotida
* **Pencarian Spesies Target:** 1. Akses halaman utama [NCBI GenBank](https://www.ncbi.nlm.nih.gov/genbank/).
  2. Pada kolom pencarian database *Nucleotide*, gunakan kombinasi *query*: `Rasbora[organism] and COI[gene]`.
  3. Telusuri hasil pencarian, lalu pilih **2 hingga 3 sekuens** untuk setiap spesies *Rasbora*. 
  4. > ⚠️ **Penting:** Pastikan sekuens yang dipilih merepresentasikan **asal lokasi geografis yang berbeda** (misalnya: aliran sungai, danau, atau pulau yang berbeda) untuk kebutuhan analisis biogeografi.

* **Pencarian Outgroup:**
  1. Lakukan pencarian terpisah pada database yang sama menggunakan *query*: `Danio rerio COI`.
  2. Pilih **1 sekuens** yang paling representatif sebagai kontrol luar (*outgroup*).

* **Ekspor Data:**
  1. Centang atau pilih semua sekuens yang telah ditentukan (*Rasbora* + *outgroup*).
  2. Klik tombol **Send to** di bagian kanan atas halaman NCBI $\rightarrow$ Pilih **File** $\rightarrow$ Format: **FASTA**.
  3. Unduh data tersebut dan pastikan semua sekuens sudah tergabung ke dalam **satu file tunggal** berformat `.fasta` atau `.txt`.

---

### 2. Penyelarasan (*Alignment*) & Konstruksi Pohon Filogenetik
1. Buka browser dan akses platform **[MAFFT Web Server](https://mafft.cbrc.jp/alignment/server/)**.
2. Unggah (*upload*) file FASTA gabungan yang telah Anda unduh pada tahap pertama ke kolom input *sequence data*.
3. Pada bagian pengaturan strategi (*strategy*), pilih opsi **"Same as MAFFT (auto)"**. Pilihan ini membiarkan sistem memilih algoritma terbaik secara otomatis berdasarkan karakteristik data Anda.
4. Klik tombol **Submit** dan tunggu beberapa saat hingga proses komputasi penyelarasan selesai.
5. Setelah halaman hasil muncul:
   * **Unduh Hasil Alignment:** Simpan file sekuens yang telah sejajar untuk kebutuhan dokumentasi lanjutan.
   * **Visualisasi Pohon Filogenetik:** Untuk melihat hubungan kekerabatan, langsung klik atau gunakan fitur visualisasi pohon **Neighbor-Joining (NJ)** yang tersedia di halaman output MAFFT tersebut.

---

### 3. Analisis Data
Setelah pohon filogenetik berhasil divisualisasikan, lakukan tahapan analisis berikut:

* **Analisis Topologi Pohon:** Lakukan pengamatan mendalam terhadap struktur pohon filogenetik NJ yang terbentuk.
* **Identifikasi Clade:** Tentukan pembentukan kelompok (*clade*), grup monofiletik, atau pola percabangan yang memisahkan antar spesies.
* **Studi Biogeografi:** Lakukan analisis korelasi antara posisi *clade* spesies *Rasbora* dengan data asal lokasi geografis masing-masing sampel. Evaluasi apakah ada pola distribusi geografis atau hambatan ekologis yang memengaruhi struktur populasi dan evolusi genus tersebut.

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

Proses analisis dibagi menjadi tiga tahapan utama:

### 1. Pengumpulan Sekuens Nukleotida
1. Buka browser dan akses halaman utama **NCBI GenBank**.
2. Pada kolom pencarian database Nucleotide, masukkan *query* berikut untuk menyaring hasil spesifik:

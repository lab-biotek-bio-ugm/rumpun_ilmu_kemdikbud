# Kategori Rumpun Ilmu Dosen Kemendikbud
Repository ini dibuat untuk mempermudah dosen dalam memilih bidang keilmuan sesuai dengan [aturan baru dari Kementerian Pendidikan, Kebudayaan, Riset, dan Teknologi (Kemendikbud)](https://pusatinformasi.sister.kemdikbud.go.id/hc/en-gb/articles/31608506732057-Informasi-Umum-Rumpun-Ilmu). Informasi tabel dibaca secara otomatis dari file PDF* yang tersedia dan data divisualisasi menggunakan `sunburst chart`. Fokus dari proyek ini adalah pada bidang ilmu hayati dan kesehatan.

Hasil Visualisasi dapat dilihat di: 
- [Visualisasi Rumpun Ilmu Hayati & Kesehatan](https://htmlpreview.github.io/?https://github.com/lab-biotek-bio-ugm/rumpun_ilmu_kemdikbud/blob/main/figures/3_sunburst_chart_bio_INDONESIA.html)
- [Tabel (.tsv)](data/processed/Daftar_Rumpun_Pohon_dan_Cabang_Ilmu_(Diperbarui_05_Juni_2024).tsv)

> *\*PS: Honestly, they can just give us the d\*mn table* :confused:

# Struktur Repository

Berikut adalah penjelasan mengenai struktur proyek ini:


## Deskripsi Direktori dan File

```bash
.
├── README.md
├── data
│   └── raw
│       └── Daftar Rumpun, Pohon, dan Cabang Ilmu (2024).pdf
├── env.yaml
├── figures
│   ├── 1_sunburst_chart_all_INDONESIAN.html
│   ├── 2_sunburst_chart_all_ENGLISH.html
│   └── 3_sunburst_chart_bio_INDONESIA.html
└── notebooks
    └── 01_scraping_and_visualization.ipynb
```

### README.md
File ini berisi deskripsi proyek, panduan penggunaan, dan informasi penting lainnya terkait proyek. Membantu pengguna memahami tujuan dan cara kerja proyek ini.

### data
Direktori ini berisi data yang digunakan dalam proyek.

- **raw**: Subdirektori ini menyimpan data mentah yang belum diolah.
  - **Daftar Rumpun, Pohon, dan Cabang Ilmu (2024).pdf**: File PDF yang berisi daftar rumpun, pohon, dan cabang ilmu terbaru yang digunakan sebagai sumber data utama dalam proyek ini.

### env.yaml
File ini berisi spesifikasi lingkungan Python yang digunakan dalam proyek ini. Dapat digunakan untuk membuat lingkungan virtual yang sesuai dengan dependensi yang dibutuhkan proyek.

### figures
Direktori ini menyimpan visualisasi yang dihasilkan oleh skrip Python.

- **1_sunburst_chart_all_INDONESIAN.html**: Sunburst chart yang menampilkan seluruh rumpun ilmu dalam bahasa Indonesia.
- **2_sunburst_chart_all_ENGLISH.html**: Sunburst chart yang menampilkan seluruh rumpun ilmu dalam bahasa Inggris.
- **3_sunburst_chart_bio_INDONESIA.html**: Sunburst chart yang menampilkan rumpun ilmu hayati dan kesehatan dalam bahasa Indonesia.

### notebooks
Direktori ini berisi Jupyter Notebooks yang digunakan untuk mengolah data dan membuat visualisasi.

- **01_scraping_and_visualization.ipynb**: Notebook ini berisi skrip untuk membaca tabel dari PDF, mengolah data, dan membuat sunburst chart.

## Cara Menggunakan Proyek Ini

1. **Clone Repository**: `git clone https://github.com/username/repo-name.git`
2. **Install Dependencies**:
   - Buat environment dengan conda: `conda env create -f env.yaml`
   - Aktifkan environment: `conda activate <env_name>`
3. **Jalankan Jupyter Notebook**:
   - Jalankan perintah `jupyter notebook` di terminal
   - Buka dan jalankan `01_scraping_and_visualization.ipynb` untuk memproses data dan menghasilkan visualisasi.
4. **Lihat Visualisasi**:
   - Visualisasi akan tersimpan dalam direktori `figures` dalam format HTML yang dapat dibuka dengan browser.

Dengan mengikuti langkah-langkah di atas, Anda dapat memanfaatkan skrip yang tersedia untuk memudahkan pemilihan bidang ilmu sesuai dengan aturan baru dari Kemendikbud.

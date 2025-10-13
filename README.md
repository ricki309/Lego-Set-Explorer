# 🧩 LEGO Set Explorer — Interactive Dashboard

**📊 Build a custom, interactive tool to help users discover the perfect LEGO set**  
Proyek ini merupakan bagian dari *guided project* dari [Maven Analytics](https://app.mavenanalytics.io/guided-projects/7ea2d5de-8a63-4c92-8350-b640d6df07d4), dengan tujuan membangun **dashboard interaktif di Power BI** untuk mengeksplorasi dataset LEGO berdasarkan **tema, harga, jumlah pieces**, dan **segmentasi usia**.

---

## 🎯 Tujuan Proyek
Membangun dashboard interaktif yang memungkinkan pengguna:
- Menemukan set LEGO berdasarkan preferensi harga, tema, dan usia.
- Mengeksplorasi distribusi harga, ukuran, dan variasi tema LEGO.
- Melakukan analisis mendalam terhadap data menggunakan *visuals*, *slicers*, dan *bookmarks* di Power BI.

---

## 🧠 Langkah Pengerjaan

### 🧩 Objective 1: Load & Prepare the Data
- Menghubungkan dataset `lego_sets.csv`  
- Menghapus kolom yang tidak relevan: `minifigs`, `bricksetURL`, `thumbnailURL`
- Memastikan tipe data sesuai dan memfilter set tanpa nilai harga, usia, pieces, atau URL gambar  
- Membuat kolom tambahan:
  - **Age Range:**
    - 1–4 → “1 to 4”
    - 5–9 → “5 to 9”
    - 10–17 → “10 to 17”
    - 18+ → “Over 18”
  - **Price Range:**
    - > $500 → `$$$$$`
    - > $100 → `$$$$`
    - > $50 → `$$$`
    - > $25 → `$$`
    - ≤ $25 → `$`
- Menambahkan *measures*:
  - `Total Sets`
  - `Total Groups`
  - `Avg. Age`
  - `Avg. Price`
  - `Avg. Pieces`

---

### 🎨 Objective 2: Design the Report Layout
- Mendesain *layout* dashboard berdasarkan insight dan kebutuhan eksplorasi pengguna  
- Menambahkan elemen visual:
  - **Cards:** Total Sets, Avg. Pieces, Avg. Price  
  - **Slicers:** Theme Group, Theme, Age Range  
  - **Table:** Menampilkan `Name`, `Set ID`, `Theme`, `Age Range`, `Avg. Pieces`, `Avg. Price`, `Price Range`  
- Menyediakan halaman detail set:
  - Menampilkan gambar, nama, tahun, harga, jumlah pieces, dan usia target  
  - Placeholder untuk beberapa pilihan set  
- Mengatur interaksi visual agar tabel tidak memengaruhi kartu ringkasan

---

### ⚙️ Objective 3: Add Interactivity
- Menambahkan **parameter** `Max Price` (0–850, increment 5) untuk filter harga maksimum  
- Mengaktifkan **tooltips** untuk menampilkan gambar LEGO saat *hover*  
- Membuat **bookmark & button actions**:
  - Tombol “Reset Filter” untuk mengembalikan ke tampilan default  
- Membuat halaman kedua:
  - **Decomposition Tree** untuk analisis mendalam berdasarkan kategori, theme group, theme, dan nama  
  - **Navigasi antar halaman** dengan tombol interaktif  

---

## 🔍 Hasil Akhir: LEGO Sets Dashboard

### 📊 Ringkasan Data
| Metrik | Nilai |
|--------|--------|
| Total LEGO Sets | **4,385** |
| Rata-rata Pieces | **411** |
| Rata-rata Harga | **$44.74** |

---

### 📸 Cuplikan Dashboard
<img width="759" height="428" alt="image" src="https://github.com/user-attachments/assets/cdf5c3b0-8ecb-4035-90d3-945b5dcb56ab" />

---

### 🔎 Fitur Utama
- Filter interaktif: *Theme Group*, *Theme*, *Age Range*  
- Slicer *Max Price* untuk membatasi harga set  
- Tombol *Reset Filter* untuk mengembalikan ke tampilan default  
- Tabel interaktif berisi nama set, ID, tema, usia, pieces, dan harga  
- Halaman *Decomposition Tree* untuk analisis hierarkis  

---

## 🎯 Insight Potensial
- Dataset mencakup **4.385 LEGO sets** dengan rata-rata **411 pieces** dan **harga $44.74**
- Tema **City** menempati posisi teratas (445 set), diikuti **Star Wars** (388 set)
- Rentang usia **5–9 tahun** mendominasi, menunjukkan target utama LEGO adalah anak-anak usia sekolah dasar

---

## 🛠️ Tools & Teknologi
- **Microsoft Power BI** – data modeling, visualisasi, interaktivitas (*slicer, bookmarks, decomposition tree*)  
- **Excel / CSV Data** – pembersihan dan transformasi awal dataset LEGO  
- **Maven Analytics Guided Project** – sumber pembelajaran & referensi tugas  

---

## ✍️ Author
**ricki309**  
📘 Guided Project: [Maven LEGO Sets Explorer](https://app.mavenanalytics.io/guided-projects/7ea2d5de-8a63-4c92-8350-b640d6df07d4)  
📂 Repository ini berisi dokumentasi dan hasil akhir dashboard — *kode atau dataset asli bersifat privat.*

---



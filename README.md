# 🎓 Analisis Rantai Markov: Perpindahan Minat Kelompok Keilmuan Mahasiswa Sains Data

Repository ini berisi analisis lengkap menggunakan **Rantai Markov (Markov Chain)** untuk memodelkan perpindahan minat mahasiswa Sains Data angkatan 2022 antara dua kelompok keilmuan:

* **X₁ — Pemodelan & Simulasi Data**
* **X₂ — Computer Vision**

Analisis mencakup pembersihan data, perhitungan matriks transisi, probabilitas multi-langkah, distribusi stasioner, diagram transisi, hingga interpretasi hasil.

---

## 🚀 Fitur Utama

* 📊 Perhitungan frekuensi & probabilitas minat
* 🔁 Matriks peluang transisi (P)
* 🔮 Perhitungan probabilitas langkah ke-n (Pⁿ)
* 📈 Distribusi stasioner
* 🔍 Klasifikasi state (*recurrent* atau *transient*)
* 🎨 Diagram transisi (GraphViz / DiagrammeR)
* 🧮 Script lengkap dalam **R**

---
## 🔄 Diagram Alir Analisis

Berikut adalah diagram alir proses analisis rantai Markov yang digunakan dalam proyek ini:

![Diagram Alir Penelitian](gambar/Diagram%20Alir%20Penelitian.png)

---

## 📁 Struktur Repository

```
📦 markov-keilmuan/
│
├── data/
│   └── DATA PEMSTOK.csv
│
├── R/
│   └── CODE TUBES PEMSTOK.Rmd
│
├── gambar/
│   └── Diagram Transisi.png
|   └── Diagram Alir Penelitian.png
│
└── README.md
```

---

## 🔍 Ringkasan Hasil Utama

| Komponen             | Hasil            |
| -------------------- | ---------------- |
| State                | X₁, X₂           |
| Dominan Semester 4   | X₁ (61.90%)      |
| Dominan Semester 7   | X₁ (64.29%)      |
| Perpindahan terbesar | X₂ → X₁ (18.75%) |

---

### Matriks Transisi (P)

$$
P =
\begin{pmatrix}
0.9231 & 0.0769 \\
0.1875 & 0.8125
\end{pmatrix}
$$


### n-step Transition (P^5)

$$
P^5 =
\begin{pmatrix}
0.7717 & 0.2283 \\
0.5564 & 0.4463
\end{pmatrix}
$$


### Distribusi Stasioner (π)

$$
\pi = (0.7091\; 0.2909)
$$


---

## 🛠 Teknologi yang Digunakan

### **R**

* `dplyr`
* `expm`
* `DiagrammeR`
* `matrixcalc` *(opsional)*

---

## 🧮 Cara Menjalankan Analisis

Clone repository:

```bash
git clone https://github.com/USERNAME/REPO-NAME.git
cd REPO-NAME
```

Jalankan script di R:

```r
source("R/markov-analysis.R")
```

---

## 🎨 Diagram Transisi (Contoh)

Berikut adalah diagram transisi rantai Markov yang dihasilkan dalam proyek ini:

![Diagram Transisi](gambar/Diagram%20Transisi.png)


---

## ✨ Tentang Proyek Ini

Analisis ini disusun sebagai bagian dari tugas akademik untuk mempelajari penerapan **Rantai Markov** pada data kategorikal. Hasil analisis dapat digunakan untuk:

* Mengetahui kecenderungan minat mahasiswa
* Memprediksi arah minat jangka panjang
* Menjadi referensi bagi studi pemetaan minat akademik

---

## 👤 Pengembang

**Rayan Koemi Karuby**
Program Studi Sains Data
rayan.122450038@student.itera.ac.id

**Patricia Leondrea Diajeng Putri**
Program Studi Sains Data
patricia.122450050@student.itera.ac.id

**Azizah Kusumah Putri**
Program Studi Sains Data
azizah.122450068@student.itera.ac.id

**Renta Siahaan**
Program Studi Sains Data
renta.122450070@student.itera.ac.id

**Naufal Fakhri**
Program Studi Sains Data
naufal.122450089@student.itera.ac.id

---



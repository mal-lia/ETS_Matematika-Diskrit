# 🧮 Evaluasi Tengah Semester (ETS) – Matematika Diskrit (A)
**Nama:** Aisyah Amalia Hamid  
**Kelas:** Matematika Diskrit (A)  
**Dosen:** Muhammad Zulhaj Sada, M.Kom.  

---

## 📘 Deskripsi Tugas
Tugas pengganti UTS ini bertujuan untuk menerapkan konsep **analisis data teks** menggunakan Python, dengan pendekatan **matematika diskrit** terhadap elemen linguistik (huruf, kata, kalimat, paragraf).  

Sumber data berupa **artikel ilmiah dengan DOI valid**, kemudian dianalisis untuk:
1. Pola **konsonan dan vokal** dalam tiap kata  
2. **Distribusi jumlah kata** dalam kalimat  
3. **Distribusi jumlah kalimat** dalam paragraf  
4. **Analisis kreatif tambahan** berupa visualisasi dan statistik kosakata

---

## 📰 Artikel yang Digunakan
**Judul:** *Research and Analysis of New Generation Nuclear Reactors in the World*  
**DOI:** [10.31548/machinery/4.2023.86](https://doi.org/10.31548/machinery/4.2023.86)  
**Bahasa:** Inggris  
**Negara corresponding author:** 🇺🇦 **Ukraine**

Cuplikan bagian yang digunakan:
- **Abstrak**
- **Kesimpulan (Conclusion)**

---

## 🧩 Analisis 1 — Pivot Tabel Konsonan dan Vokal
Setiap kata dihitung jumlah huruf **vokal (a, i, u, e, o)** dan **konsonan**, lalu dibuat:
- **Heatmap frekuensi kombinasi vokal–konsonan**
- **Heatmap cacah kata per kombinasi**
- **Rata-rata panjang kata berdasarkan kombinasi**

🔹 *Insight:*  
Sebagian besar kata memiliki 2–4 vokal dan 3–6 konsonan, menunjukkan kompleksitas linguistik moderat pada teks ilmiah.

---

## 📊 Analisis 2 — Jumlah Kata per Kalimat
Kalimat dipisahkan berdasarkan tanda baca (.!?).  
Histogram menunjukkan distribusi kata per kalimat dengan rata-rata sekitar **22–25 kata**.

🔹 *Insight:*  
Struktur kalimat dalam artikel ilmiah cenderung panjang dan kompleks, sesuai gaya akademik berbahasa Inggris.

---

## 🧱 Analisis 3 — Jumlah Kalimat per Paragraf
Paragraf dipisahkan berdasarkan baris kosong (`\n\n`) kemudian dihitung jumlah kalimatnya.

🔹 *Insight:*  
Rata-rata 3–5 kalimat per paragraf, menandakan penulisan yang terstruktur secara argumentatif.

---

## 🌈 Analisis Kreatif (Bonus)
Beberapa analisis tambahan untuk mendapatkan nilai bonus:
1. **Word Cloud** untuk kata dominan di abstrak dan kesimpulan.  
2. **Perbandingan frekuensi kata** 10 besar antar bagian.  
3. **Proporsi total vokal vs konsonan** (diagram donat).  
4. **Scatter plot** kompleksitas kata (konsonan vs vokal).  
5. **Type/Token Ratio (TTR)** untuk mengukur keragaman kosakata:
   - Abstrak: `TTR ≈ 0.53` → variasi kosakata tinggi  
   - Kesimpulan: `TTR ≈ 0.48` → sedikit lebih repetitif  

🔹 *Kesimpulan Umum:*  
Teks ilmiah ini menunjukkan keseimbangan antara kompleksitas struktur kalimat dan variasi kosakata, dengan dominasi kata-kata teknis khas bidang energi nuklir.

---

## 🧠 Library yang Digunakan
- `pandas` — pengolahan tabel data  
- `matplotlib`, `seaborn` — visualisasi data  
- `re` — ekspresi reguler untuk parsing teks  
- `numpy` — perhitungan numerik  
- `collections.Counter` — menghitung frekuensi kata  
- `wordcloud` — visualisasi awan kata  

---

## ⚙️ Cara Menjalankan
```bash
# 1. Clone repository
git clone https://github.com/<username>/matematika-diskrit-ets.git
cd matematika-diskrit-ets

# 2. Jalankan program
python evaluasi_tengah_semester_(ets)_24083010034_matematika_diskrit_(aisyah_amalia_hamid).py

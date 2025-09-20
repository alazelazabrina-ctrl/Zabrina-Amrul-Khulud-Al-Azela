Zabrina-Amrul-Khulud-Al-Azela
Capstone Project: Analisis Tingkat Pengangguran Terbuka 2025 di Indonesia

Project Overview
Proyek ini adalah bagian dari Student Development Initiative HACKTIV8 yang bertujuan untuk menganalisis data publik mengenai Tingkat Pengangguran Terbuka (TPT) di setiap provinsi Indonesia pada tahun 2025. Tujuannya adalah untuk menggali wawasan bermakna dari data tersebut dengan bantuan AI.  

Proses analisis dilakukan menggunakan Google Colab, dengan memanfaatkan library Python seperti:
- Pandas untuk manipulasi data  
- Matplotlib dan Seaborn untuk membuat visualisasi data  
- AI model IBM Granite (watsonx.ai) untuk memperkaya analisis  

Raw Dataset Link
Sumber data berasal dari Badan Pusat Statistik (BPS):  

- Tingkat Pengangguran Terbuka Menurut Provinsi, 2025  
  - [Link resmi BPS](https://www.bps.go.id/id/statistics-table/2/NTQzIzI=/tingkat-pengangguran-terbuka-menurut-provinsi.html)  
  - [Salinan dataset Excel di repo ini](https://github.com/alazelazabrina-ctrl/Zabrina-Amrul-Khulud-Al-Azela/blob/a715fe9cc4b2c079ac9f259d58209583918a9fd8/Tingkat%20Pengangguran%20Terbuka%20Menurut%20Provinsi%2C%202025.xlsx) 

Insights & Findings
Berdasarkan analisis data di notebook Google Colab, diperoleh temuan berikut:

Pembersihan Data
- Dataset mentah memiliki header tambahan sehingga perlu melewatkan 3 baris awal.  
- Kolom disusun ulang menjadi `Provinsi` dan `TPT (%)`.  
- Kolom TPT diubah ke tipe numerik.  
- Baris agregat `Indonesia` dihapus agar analisis per provinsi tidak bias.  

Peringkat TPT
5 Provinsi dengan TPT Tertinggi (Februari 2025):
1. Papua - 6,92%  
2. Kepulauan Riau - 6,89%  
3. Jawa Barat - 6,74%  
4. Banten - 6,64%  
5. Papua Barat Daya - 6,61%  

5 Provinsi dengan TPT Terendah (Februari 2025):
1. Bali - 1,58%  
2. Papua Pegunungan - 1,68%  
3. Sulawesi Tengah - 3,02%  
4. Gorontalo - 3,12%  
5. Sulawesi Barat - 3,17%  

Pola Regional
- Pulau Jawa (Jawa Barat, Banten) masih berkontribusi signifikan terhadap angka pengangguran nasional.  
- Provinsi di wilayah timur (Papua dan Papua Barat Daya) mencatat TPT tinggi.  
- Bali menonjol dengan TPT terendah, yang menunjukkan pemulihan sektor pariwisata pasca pandemi.  

AI Support Explanation
Sesuai tujuan proyek, AI (Large Language Model) dari IBM Granite direncanakan untuk digunakan dalam beberapa skenario guna memperkaya analisis:

- Summarization (Peringkasan): 
  Membuat ringkasan naratif otomatis dari temuan-temuan utama.  
  Contoh: “Pengangguran di Papua dan Kepulauan Riau lebih tinggi dibanding rata-rata nasional, sementara Bali menunjukkan pemulihan signifikan.”  

- Classification (Klasifikasi):
  Mengelompokkan provinsi berdasarkan kategori TPT, misalnya:  
  - Tinggi (>6%)  
  - Sedang (3–6%)  
  - Rendah (<3%)  

- Insight Generation (Pembuatan Wawasan Lanjutan): 
  Memberikan pertanyaan analitis tambahan, misalnya:  
  - Apa kaitan antara TPT tinggi dengan struktur industri provinsi tersebut?  
  - Apakah tingkat pendidikan turut memengaruhi variasi TPT antarprovinsi?  

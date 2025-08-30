# Shopee Review Analysis — Classification & Summarization with IBM Granite

## Overview
Proyek ini menganalisis ulasan Shopee untuk menemukan pola kepuasan pelanggan.  
Analisis dilakukan dengan:
- **Klasifikasi sentimen** (positif, netral, negatif) berdasarkan review.
- **Summarization** insight dari review menggunakan IBM Granite (via Replicate).

## Dataset
- Sumber: [Shopee Text Reviews (Kaggle)](https://www.kaggle.com/datasets/shymammoth/shopee-reviews)  
- Format: CSV  
- Kolom utama:
  - `label` = rating bintang (1–5)
  - `text` = isi review

## Tools
- Google Colab + Python
- IBM Granite via Replicate API
- Matplotlib untuk visualisasi

## Insight & Findings
- Mayoritas review bersentimen **positif (~70–80%)**.
- Granite mencapai akurasi sekitar **0.75–0.80** dibanding rating bintang.
- Ringkasan insight (Granite summarization):
  - Produk sesuai deskripsi, harga terjangkau.
  - Keluhan utama: pengiriman lambat.
  - Beberapa kasus packaging rusak dan barang cacat.

## Conclusion & Recommendations
- Mayoritas pembeli puas, tapi ada masalah di aspek pengiriman & packaging.
- Rekomendasi: seller perlu memperbaiki kualitas packing dan mempercepat pengiriman.
- Insight ini bisa dipakai untuk meningkatkan kepuasan pelanggan dan reputasi toko.

## AI Support Explanation
- **IBM Granite** digunakan melalui **Replicate**.
- Peran Granite:
  - Prompt-based classification → klasifikasi sentimen review.
  - Summarization → merangkum insight ulasan menjadi poin-poin penting.
- **Kelebihan**: fleksibel, tidak perlu training model dari nol.
- **Keterbatasan**: bergantung pada kualitas dataset dan prompt.

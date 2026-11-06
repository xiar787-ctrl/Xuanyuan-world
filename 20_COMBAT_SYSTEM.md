# ⚔️ 20 — Sistem Pertempuran Taktis Berbasis Giliran (Turn-Based Combat)

> **Modul:** 20 — Tactical Turn-Based Combat System
> **Filosofi:** Kemenangan ditentukan oleh taktik, posisi, sinergi elemen, dan perhitungan risiko, bukan sekadar adu angka status semata.

---

## 1. Alur Urutan Pertempuran (Combat Flow)

Setiap putaran pertempuran diproses secara runtut oleh AI GM:

1. **Fase Inisiatif (Initiative Check):**
   Dihitung berdasarkan kecepatan reaksi ranah kultivasi + teknik gerak langkah (Akar Bayangan/Angin mendapat bonus +20 inisiatif).
2. **Fase Deklarasi Aksi Pemain:**
   Pemain memilih aksi taktis (menyerang, meluncurkan boneka pelindung, menelan pil penambah stamina, mengaktifkan jimat, atau mundur teratur).
3. **Fase Resolusi & Kalkulasi AI GM:**
   AI GM menghitung peluang mengenai sasaran (*Hit Chance*), besaran kerusakan (*Damage Output*), konsumsi Qi, dan reaksi balasan musuh.
4. **Pembaruan Status & Format Log:**
   Menampilkan kondisi sisa HP, Qi, dan status abnormal lawan maupun karakter.

---

## 2. Formula Pertempuran Standar

### 2.1 Peluang Mengenai Sasaran (Hit Chance)
$$\text{Hit Chance \%} = 70\% + (\text{Ranah Penyerang} - \text{Ranah Bertahan}) \times 10\% + \text{Modifikator Medan/Elemen} - \text{Nilai Evasion Target}$$
*(Batas minimal 15%, batas maksimal 95% kecuali jurus mutlak bersyarat)*

### 2.2 Formula Kerusakan (Damage Calculation)
$$\text{Net Damage} = (\text{Base Atk Jurus} + \text{Qi Tercurahkan}) \times \text{Keunggulan Elemen} - \text{Pertahanan Zirah/Tubuh Lawan}$$

### 2.3 Matriks Keunggulan Tiga Jalan & Elemen:
- **Elemen Daun/Kayu:** Menyerap dan meredam serangan Air/Racun (+25%), namun rentan terhadap Api Jiuyou (-30%).
- **Ortodoks vs Demonic:** Serangan Niat Pedang Lurus Ortodoks membubarkan kabut ilusi dan hawa racun iblis secara efektif.
- **Unortodoks:** Menggunakan boneka umpan untuk menyerap 100% kerusakan serangan pertama lawan, membuka celah serangan balik dari arah buta.
- **Demonic:** Serangan memiliki efek *Lifesteal* (menyerap 15% kerusakan menjadi HP jika darah lawan mengucur).

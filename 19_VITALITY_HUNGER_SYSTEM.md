# 🩸 Sistem Vitalitas, Stamina, Rasa Lapar & Toksin Tubuh Dunia Xuanyuan

> **Modul:** 19 — Vitality, Hunger, Toxin & Wound System
> **Kategori:** Hardcore Realism, Mekanik Kelangsungan Hidup, Akumulasi Toksin Pil, & Penanganan Cedera Persisten
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md`, `13_SPIRITUAL_ROOT_SYSTEM.md`, `14_CRAFTING_AND_PROFESSIONS_SYSTEM.md`, `18_ECONOMY_SYSTEM.md`, `44_ASSOCIATION_OF_HEALING_MASTERS.md`, `INDEX.md`

---

## 1. Lore & Filosofi Hardcore Realism Tubuh Manusia

Di Dunia Xuanyuan (*Xuanyuan World*), kultivator bukanlah entitas digital kebal sakit yang bisa terus bertarung tanpa batas. Sebelum melangkah mencapai tingkatan Penguasa Domain Tianjun yang melampaui jasmani, tubuh seorang pembudidaya tetap tersusun atas darah daging, pembuluh meridian rapuh, dan organ fana yang membutuhkan asupan nutrisi pangan dan air bersih.

Prinsip Realisme Tubuh: *"Qi Menopang Semangat Jiwa; Darah dan Makanan Menjaga Wadah Jasmani Tetap Kokoh"*.

Mengabaikan kebutuhan makan, memaksakan bertarung dalam kondisi lelah mental, atau menelan pil alkimia murahan secara berlebihan akan meninggalkan residu racun dan luka dalam permanen yang dapat menghancurkan prospek penerobosan ranah di masa depan.

---

## 2. Formula Dasar Atribut Tubuh (HP, Stamina & Satiety)

Kapasitas fisik karakter dihitung berdasarkan ranah kultivasi dan garis keturunan:

### 2.1 Poin Kesehatan Maksimal (Max HP)
$$\text{Max HP} = (\text{Base HP Ranah} \times \text{Pengali Sub-Stage}) + \text{Bonus Akar Spiritual} + \text{Bonus Zirah}$$

| Ranah Kultivasi | Base HP (Awal) | Mid HP (Tengah) | Peak HP (Puncak) | Karakteristik Ketahanan Jasmani |
|---|---|---|---|---|
| **Fana / Qiguan Jing** | 100 | 150 | 200 | Rentan tebasan senjata tajam fana biasa. |
| **Tongmai Jing** | 300 | 450 | 600 | Kulit mulai liat; mampu menahan memar pukulan tangan kosong. |
| **Yuanhai Jing** | 1.000 | 1.500 | 2.000 | Pembuluh darah diperkuat cairan Qi; kebal tusukan jarum biasa. |
| **Shenfu Jing** | 3.500 | 5.250 | 7.000 | Organ dalam dilindungi kesadaran roh; luka luar menutup lebih cepat. |
| **Xuanyuan Jing** | 12.000 | 18.000 | 24.000 | Terhubung denyut urat naga; tulang sekeras batu granit. |
| **PoKong Jing** | 40.000 | 60.000 | 80.000 | Daging diperkuat partikel spasial; kebal senjata fana apapun. |
| **Fashen Jing** | 150.000 | 225.000 | 300.000 | Tubuh Hukum menyatu dengan jasmani; regenerasi luka instan. |
| **Tianjun Jing** | 600.000 | 900.000 | 1.200.000 | Raga fisik diperbarui oleh hukum domain pribadi. |
| **Hunyuan Taihe** | 3.000.000 | 4.500.000 | 6.000.000 | Tubuh Primordial Keabadian Sejati. |

*Bonus Akar Spiritual:* Praktisi berakar **Darah Belantara Xueshan** mendapat bonus Max HP **+40%**, berakar **Vajra Bodhi Jinshan** mendapat **+25%**.

### 2.2 Poin Stamina Maksimal (Stamina Points)
- **Base Stamina Standar:** **100 Poin** (Bertambah +10 per peningkatan Major Realm).
- **Konsumsi Stamina Realistis:**
  - Berjalan kaki normal: **-5 Stamina / jam**.
  - Berlari cepat / Pendakian tebing curam: **-20 Stamina / jam**.
  - Mengayunkan senjata berat / Pertarungan fisik sengit: **-10 Stamina / putaran tempur**.
  - Terbang pedang mandiri: **-15 Stamina + 50 Qi / jam**.
- **Efek Kehabisan Stamina (Stamina = 0):** Status *Exhaustion Extreme* (Kecepatan gerak -50%, Hit Chance -40%, tidak dapat menggunakan teknik fisik).

---

## 3. Sistem Rasa Lapar & Dehidrasi (Satiety & Hydration 0–100%)

Karakter memiliki indikator **Tingkat Kekenyangan (Satiety)** dan **Tingkat Hidrasi (Hydration)** berskala **0% hingga 100%**:

| Persentase Satiety / Hydration | Status Fisik | Dampak Mekanik Nyata | Penanganan Wajib |
|---|---|---|---|
| **80% – 100%** | **Prima & Berenergi** | Regenerasi Stamina & HP pasif berjalan optimal (100% rate). | Tidak memerlukan tindakan khusus. |
| **50% – 79%** | **Normal / Sedikit Lapar** | Perut mulai berbunyi; tidak ada penalti stat pertempuran. | Disarankan memakan camilan ransum atau buah spirit. |
| **20% – 49%** | **Kelaparan / Dehidrasi Ringan**| Regenerasi Stamina alami terhenti; Max Stamina terpotong 25%.| Wajib makan makanan padat dan meminum air tawar. |
| **1% – 19%** | **Kelaparan Kritis / Dehidrasi Parah**| Max HP berkurang 50%; Hit Chance -30%; pusing kepala parah. | Mengonsumsi air mata air spirit atau sup herba hangat. |
| **0%** | **Sekarat Akibat Kelaparan (Starvation)**| Kehilangan 10% Max HP per jam; pingsan tak sadarkan diri. | Pertolongan pertama darurat infus getah obat. |

*Pengecualian:* Kultivator yang telah meminum **Pil Puasa (Bigu Pill / 辟谷丹)** membekukan penurunan Satiety selama durasi pil aktif (1 minggu hingga 1 bulan).

---

## 4. Sistem Akumulasi Toksin Pil (Pill Toxin System 0–100%)

Setiap pil alkimia buatan manusia—kecuali pil kemurnian kritis sempurna (*Perfect Grade*)—meninggalkan ampas residu kimia biologis di dalam saluran meridian dan dinding Dantian yang disebut **Toksin Pil (Pill Toxin / 丹毒)**:

$$\text{Total Toksin Dantian (\%)} = \sum (\text{Toksin Residu Setiap Pil yang Ditelan})$$

| Persentase Toksin Dantian | Status Meridian | Penalti Mekanik Kultivasi & Tempur |
|---|---|---|
| **0% – 15%** | **Bersih / Terkendali** | Tidak ada efek negatif; sirkulasi Qi berjalan lancar. |
| **16% – 35%** | **Keruh Ringan** | Efektivitas pil pemulihan berikutnya berkurang 20%; bau nafas beraroma logam kimia. |
| **36% – 60%** | **Kejenuhan Pil Berat** | Peluang sukses terobosan ranah terpotong -30%; konsumsi Qi bertambah +15%. |
| **61% – 85%** | **Penyumbatan Saluran Meridian**| Kerusakan berkala 2% Max HP per turn saat bertarung; batuk lendir hitam. |
| **86% – 100%** | **Ledakan Toksin Dantian (Pill Poisoning)**| **Dantian Retak / Mati Rasa Total; KULTIVASI TURUN 1 RANAH.** |

### Metode Detoksifikasi Toksin Pil:
1. **Istirahat Penuh Tanpa Meminum Pil:** Mengurangi Toksin Pil sebesar 2% per hari melalui metabolisme alami.
2. **Meminum Rebusan Herba Penawar:** Teh Daun Cyan Chaolu (-10% Toksin) atau Air Embun Bunga Teratai Emas Bodhi (-25% Toksin).
3. **Meditasi Pemurnian Api/Air:** Berendam di Danau Sari Darah Xueshan atau Danau Mendidih Wanze dipandu tabib profesional.

---

## 5. Sistem Cedera Persisten & Metode Penyembuhannya

Dunia Xuanyuan tidak mengenal sistem luka yang sembuh otomatis dalam semalam. Cedera berat bersifat **persisten** hingga diobati dengan benar:

| Jenis Cedera Berat | Pemicu Terjadinya Luka | Dampak Mekanik yang Dialami | Prosedur Penanganan Medis yang Sah |
|---|---|---|---|
| **Patah Tulang / Robek Sendi** | Hantaman senjata tumpul berat, terjatuh dari ketinggian | Tidak dapat menggunakan anggota tubuh terkait; Stamina -50% | Pemasangan gips kayu peredam, olesan Minyak Gosok Akar Vajra selama 3 hari. |
| **Luka Bakar Api Neraka Jiuyou**| Terbakar lahar atau kobaran api iblis hitam | HP tidak dapat diregenerasi; luka terasa membakar terus-menerus | Salep Embun Belerang Dingin dan kompres Air Sungai Naga. |
| **Korosi Bisa Asam Rawa Wanze**| Terpapar ludah katak beracun atau kabut asam | Armor Durability terus terkikis; kehilangan 5 HP per turn | Penawar Serum Khusus Paviliun Racun Wanze dalam 6 jam. |
| **Keretakan Meridian Dantian** | Gagal terobosan ranah, terpukul jurus pembalik Qi musuh | Kapasitas QiCap terpotong 50%; nyeri dada hebat saat menyalurkan jurus | Perawatan intensif Asosiasi Tabib dengan *Pil Penambal Surga* selama 1 bulan. |
| **Penyimpangan Qi (Qi Deviation)**| Terlalu bernafsu bertapa, terhasut ilusi iblis batin | Hilang kendali diri; menyerang kawan; risiko kematian permanen | Pembacaan Sutra Bodhi di bawah dentang Lonceng Suci Jinshan. |

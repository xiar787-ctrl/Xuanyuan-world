# 🩸 Sistem Vitalitas, Stamina, Rasa Lapar & Toksin Tubuh Dunia Xuanyuan

> **Modul:** 19 — Vitality, Hunger, Toxin & Wound System
> **Kategori:** Hardcore Realism, Mekanik Kelangsungan Hidup, Formula Penurunan Rasa Lapar, Akumulasi Toksin Pil, & Penanganan Cedera Persisten
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md`, `13_SPIRITUAL_ROOT_SYSTEM.md`, `14_CRAFTING_AND_PROFESSIONS_SYSTEM.md`, `18_ECONOMY_SYSTEM.md`, `20_COMBAT_SYSTEM.md`, `44_ASSOCIATION_OF_HEALING_MASTERS.md`, `INDEX.md`

---

## 0. Filosofi Sistem Vitalitas & Anti-Cheat Realisme Xuanyuan

Di Dunia Xuanyuan (*Xuanyuan World*), kultivator bukanlah entitas digital kebal sakit yang bisa terus bertarung tanpa batas. Sebelum melangkah mencapai tingkatan Penguasa Domain Tianjun yang melampaui jasmani fana, tubuh seorang pembudidaya tetap tersusun atas darah daging, pembuluh meridian rapuh, dan organ tubuh yang membutuhkan asupan nutrisi pangan, air bersih, serta pembuangan ampas energi.

```
===============================================================================
                     HUKUM REALISME VITALITAS XUANYUAN
===============================================================================
 1. FIXED HP FORMULA: Max HP dihitung resmi AI GM berdasar Ranah & Akar Spiritual.
 2. PERSISTENT WOUNDS: Luka dalam dan patah tulang tidak sembuh instan tanpa obat.
 3. SATIETY DECAY: Rasa lapar berkurang berdasar beban aktivitas & efisiensi Inedia.
 4. INEDIA (BIGU) THRESHOLD: Ranah PoKong Jing (Realm 6) ke atas kebal kelaparan mutlak.
 5. PILL TOXIN ACCUMULATION: Pil berkualitas rendah meninggalkan residu racun Dantian.
===============================================================================
```

---

## 1. Formula Dasar Atribut Tubuh (HP, Stamina & Regenerasi Alami)

Kapasitas fisik karakter dihitung secara ketat berdasarkan ranah kultivasi dan garis keturunan:

### 1.1 Formula Poin Kesehatan Maksimal (Max HP Formula)

$$\text{Max HP} = \text{BaseQiCap(Realm)} \times \text{StageMultiplier} \times 0.35 \times \text{SpiritualRootHPMultiplier} \times (1 + \text{BonusZirah})$$

*Parameter StageMultiplier:*
* **Awal (Early):** `1.0`
* **Menengah (Mid):** `1.5`
* **Puncak (Peak):** `2.0`

*Tabel Multiplier HP Elemen Akar Spiritual (SpiritualRootHPMultiplier):*
* **Akar Garis Darah Belantara (Xueshan):** `× 1.50` *(Vitalitas binatang purba & sumsum padat)*
* **Akar Emas Bodhi Vajra (Jinshan):** `× 1.40` *(Kekebalan tubuh lonceng emas & otot vajra)*
* **Akar Kayu & Daun Cyan (Qingye):** `× 1.30` *(Regenerasi sel alami & keuletan urat napas)*
* **Akar Anomali Spasial / Badai Pasir:** `× 1.00` *(Standar ketahanan fisik umum)*
* **Akar Api Neraka Jiuyou / Racun Wanze:** `× 0.90` *(Daya rusak energi ofensif tinggi, raga lebih rentan)*

---

### 📐 Tabel Acuan Max HP Berdasarkan 9 Ranah Xuanyuan (Stage Menengah)

| Ranah (Realm) | Base Qi Cap (Mid) | Max HP (Jiuyou/Wanze - 0.9x) | Max HP (Standar - 1.0x) | Max HP (Qingye - 1.3x) | Max HP (Jinshan - 1.4x) | Max HP (Xueshan - 1.5x) |
|---|---|---|---|---|---|---|
| **Ranah 1 — Qiguan Jing** | 150 | 47 HP | 52 HP | 68 HP | 73 HP | **78 HP** |
| **Ranah 2 — Tongmai Jing** | 750 | 236 HP | 262 HP | 341 HP | 367 HP | **393 HP** |
| **Ranah 3 — Yuanhai Jing** | 3.750 | 1.181 HP | 1.312 HP | 1.706 HP | 1.837 HP | **1.968 HP** |
| **Ranah 4 — Shenfu Jing** | 18.750 | 5.906 HP | 6.562 HP | 8.531 HP | 9.187 HP | **9.843 HP** |
| **Ranah 5 — Xuanyuan Jing** | 93.750 | 29.531 HP | 32.812 HP | 42.656 HP | 45.937 HP | **49.218 HP** |
| **Ranah 6 — PoKong Jing** | 468.750 | 147.656 HP | 164.062 HP | 213.281 HP | 229.687 HP | **246.093 HP** |
| **Ranah 7 — Fashen Jing** | 2.343.750 | 738.281 HP | 820.312 HP | 1.066.406 HP | 1.148.437 HP | **1.230.468 HP** |
| **Ranah 8 — Tianjun Jing** | 11.718.750 | 3.691.406 HP | 4.101.562 HP | 5.332.031 HP | 5.742.187 HP | **6.152.343 HP** |
| **Ranah 9 — Hunyuan Taihe**| 58.593.750 | 18.457.031 HP | 20.507.812 HP | 26.660.156 HP | 28.710.937 HP | **30.761.718 HP** |

---

### 1.2 Formula Regenerasi HP Alami per Jam

$$\text{HPRegenPerHour} = \text{Max HP} \times 0.04 \times \text{RootRegenMultiplier} \times \text{EnvironmentQiModifier}$$

*(Karakter berakar Kayu/Daun Cyan Qingye mendapat RootRegenMultiplier 1.4x; berada di Qingye Zhou atau bantaran Sungai Naga Zhongzhou memberi EnvironmentQiModifier 1.3x).*

---

## 2. Sistem Rasa Lapar & Formula Penurunan Satiety (Hunger & Inedia System)

Di Dunia Xuanyuan, kebutuhan makan dipengaruhi secara realistis oleh **Tingkat Beban Aktivitas (Activity Burden)** dan disaring oleh **Efisiensi Puasa Kultivasi (Inedia Efficiency / Bigu / 辟谷)**:

### 2.1 Formula Penurunan Rasa Lapar (Satiety Decay Formula)

$$\text{SatietyDropPerHour (\%)} = \frac{\text{ActivityRate (\%)}}{\text{InediaEfficiency(Realm)}} \times \text{MetabolismModifier}$$

*MetabolismModifier:* Karakter berakar **Darah Belantara Xueshan** memiliki metabolisme fisik tinggi (`× 1.25`), sedangkan karakter berakar **Vajra Bodhi** atau **Daun Cyan** memiliki sirkulasi hemat energi (`× 0.85`).

---

### 2.2 Tabel Koefisien Aktivitas (ActivityRate per Jam)

| Tingkat Aktivitas Karakter | Deskripsi Tindakan dalam Sesi | Laju Pengurangan Dasar (ActivityRate) |
|---|---|---|
| **Istirahat Total / Seclusion** | Tidur lelap di losmen, bermeditasi hening di ruang tertutup berformasi | **1.5% per jam** (36% per 24 jam) |
| **Aktivitas Ringan** | Percakapan sosial, tawar-menawar pasar, membaca manuskrip, menulis jimat | **3.0% per jam** (Dua kali makan per hari) |
| **Aktivitas Sedang / Perjalanan**| Berjalan kaki 12 li/jam, menunggang kuda spirit, bertani, menambang mineral | **5.0% per jam** (Cepat lapar dalam 12 jam) |
| **Aktivitas Berat / Tempur** | Pertarungan fisik sengit, berlari cepat mendaki tebing, terbang pedang mandiri | **10.0% per jam** *(atau -2.5% per putaran tempur turn-based)* |

---

### 2.3 Tabel Efisiensi Inedia (InediaEfficiency) Berdasarkan 9 Ranah Xuanyuan

Semakin tinggi ranah seseorang, simpul Dantian menyerap sari pati nafas alam secara pasif untuk menggantikan makanan fana:

| # | Ranah Kultivasi (Realm) | Nilai InediaEfficiency | Daya Tahan Tanpa Makan (Waktu sampai 0% Satiety) |
|---|---|---|---|
| 1 | **Qiguan Jing (气灌境)** | `1.0x` (Fana Normal) | ± 20–24 Jam tanpa makan (Wajib makan harian) |
| 2 | **Tongmai Jing (通脉境)** | `2.5x` (Nadi Terbuka) | ± 2–3 Hari tanpa makan |
| 3 | **Yuanhai Jing (元海境)** | `6.0x` (Cairan Yuanhai) | ± 7–10 Hari tanpa makan |
| 4 | **Shenfu Jing (神府境)** | `15.0x` (Istana Roh) | ± 20–30 Hari tanpa makan |
| 5 | **Xuanyuan Jing (轩辕境)**| `40.0x` (Nafas Naga Bumi)| ± 2–3 Bulan tanpa makan (Cukup minum embun) |
| 6 | **PoKong Jing (破空境)** | **INEDIA MUTLAK (Bigu)** | **Kebal Kelaparan (0% Satiety Drop)** |
| 7 | **Fashen Jing (法身境)** | **INEDIA MUTLAK (Bigu)** | **Kebal Kelaparan (0% Satiety Drop)** |
| 8 | **Tianjun Jing (天君境)** | **INEDIA MUTLAK (Bigu)** | **Kebal Kelaparan (0% Satiety Drop)** |
| 9 | **Hunyuan Taihe Jing** | **MELAMPAUI MATERI** | **Kebal Kelaparan (Menyerap Nafas Primordial)** |

*Catatan Bigu Pill (辟谷丹):* Meminum 1 butir *Bigu Pill Grade 2* memberikan status Inedia buatan selama **30 hari** penuh bagi kultivator Ranah 1–4.

---

### 2.4 Penalti & Debuff Penurunan Satiety

| Sisa Satiety | Status Kondisi | Dampak Mekanik Langsung |
|---|---|---|
| **75% – 100%** | **Sangat Prima** | Regenerasi HP & Stamina pasif optimal (100% rate). |
| **40% – 74%** | **Normal** | Perut mulai berbunyi pelan; tanpa penalti statistik pertempuran. |
| **20% – 39%** | **Lapar Berat** | Regenerasi Stamina terhenti; Max Stamina terpotong 25%; Hit Chance -10%. |
| **1% – 19%** | **Kelaparan Kritis**| Max HP berkurang 40%; Attack Power -30%; konsumsi Qi bertambah +25%. |
| **0%** | **Sekarat (Starvation)**| Menderita kerusakan 5% Max HP per jam; pingsan tak sadarkan diri dalam 6 jam. |

---

## 3. Sistem Akumulasi Toksin Pil (Pill Toxin System 0–100%)

Setiap pil alkimia—kecuali yang mencapai tingkatan kemurnian kritis sempurna (*Perfect Grade*)—meninggalkan endapan ampas kimia obat di saluran meridian Dantian:

$$\text{CurrentToxinPercent} = \text{Clamp}(\text{PreviousToxin} + \text{ConsumedPillToxin}, 0\%, 100\%)$$

*Residu Toksin Berdasarkan Kemurnian Pil:*
* **Kemurnian Rendah (Low):** `+15% Toksin / butir`
* **Kemurnian Normal (Mid):** `+8% Toksin / butir`
* **Kemurnian Tinggi (High):** `+3% Toksin / butir`
* **Kemurnian Puncak (Perfect):** `+0% Toksin (Murni Bebas Residu)`

### Penalti Penumpukan Toksin:
* **Toksin > 25%:** Regenerasi Qi alami lambat (-25%).
* **Toksin > 50%:** Residu menghambat terobosan ranah (-30% Breakthrough Chance, risiko Qi Deviation).
* **Toksin > 75%:** Kerusakan internal berkala 2% Max HP per turn saat menyalurkan jurus bertenaga besar.
* **Toksin 100%:** **Dantian Membeku / Retak Akut; kultivator tidak dapat menyerap Qi dari batu giok roh.**

---

## 4. Pembersihan Toksin Dantian & Perawatan Medis

1. **Detoksifikasi Alami:** Berkurang `3% Toksin per 24 jam` meditasi hening tanpa mengonsumsi pil apapun.
2. **Rebusan Herba Penawar:**
   - Teh Daun Hijau Chaolu (Qingye Zhou): Menghapus `10% Toksin`.
   - Air Seduhan Teratai Emas Bodhi (Jinshan Zhou): Menghapus `25% Toksin`.
   - Serum Pembersih Meridian Paviliun Wanze: Menghapus `40% Toksin`.
3. **Penanganan Ahli Tabib:** Rumah Sakit Asosiasi Tabib Penyembuh (`44_ASSOCIATION_OF_HEALING_MASTERS.md`) mampu melakukan pengeluaran racun Dantian total menggunakan metode tusuk jarum perak dan pembakaran moxa spirit.

---

## 5. Sistem Cedera Persisten & Prosedur Medis

| Jenis Cedera Berat | Pemicu Luka | Dampak Mekanik | Prosedur Medis Resmi |
|---|---|---|---|
| **Patah Tulang / Robek Sendi**| Benturan palu godam, tertimpa batu tebing | Tidak dapat menggunakan anggota tubuh; Stamina -50% | Pemasangan gips kayu peredam Mumian & salep akar vajra 3 hari. |
| **Luka Bakar Api Iblis Jiuyou**| Semburan magma, api neraka hitam | HP tidak dapat diregenerasi; rasa terbakar persisten | Salep Embun Belerang Dingin dan bilasan air Sungai Naga. |
| **Korosi Racun Asam Wanze**| Ludah katak sembilan warna, spora jamur | Zirah luar meleleh; kehilangan 5 HP per putaran tempur | Injeksi Serum Penawar Paviliun Racun Wanze dalam tempo 6 jam. |
| **Keretakan Meridian Dantian**| Gagal terobosan, pukulan telapak pembalik Qi | Kapasitas QiCap terpotong 50%; nyeri dada menusuk | Perawatan intensif Asosiasi Tabib dengan *Pil Penambal Surga* 1 bulan. |
| **Penyimpangan Qi (Qi Deviation)**| Terhasut amarah iblis batin saat bertapa | Kehilangan kendali; menyerang kawan; risiko permadeath | Pembacaan Sutra Bodhi di bawah dentang Lonceng Suci Jinshan. |

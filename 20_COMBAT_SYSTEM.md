# ⚔️ Sistem Pertempuran Taktis Berbasis Giliran Dunia Xuanyuan

> **Modul:** 20 — Tactical Turn-Based Combat System
> **Kategori:** Mekanik Pertarungan Turn-Based, Formula Inisiatif, Hit Chance, Konsumsi Qi, Status Efek & Aksi Profesi
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md`, `13_SPIRITUAL_ROOT_SYSTEM.md`, `14_CRAFTING_AND_PROFESSIONS_SYSTEM.md`, `19_VITALITY_HUNGER_SYSTEM.md`, `21_BESTIARY.md`, `INDEX.md`

---

## 1. Lore & Prinsip Pertempuran Dunia Xuanyuan

Di Benua Xuanyuan (*Xuanyuan World*), pertarungan kultivasi bukanlah adu tabrak angka tanpa akal, melainkan benturan antara pemahaman Niat Bela Diri (*Martial Intent*), strategi taktis medan lingkungan, pengendalian sirkulasi nafas Qi, serta keuletan raga darah.

Tiga Filosofi Tempur Tiga Faksi:
1. ⚖️ **Ortodoks (Zheng Dao):** Disiplin formasi, pertahanan kokoh tak tergoyahkan, pedang pemutus kekosongan lurus, dan teknik pemurnian penangkal hawa jahat.
2. 🎭 **Unortodoks (Zuo Dao):** Langkah senyap ilusi, penyebaran serbuk racun tersembunyi, pengerahan automaton pengalih perhatian, dan perangkap formasi portabel.
3. 🩸 **Demonic (Mo Dao):** Serbuan tenaga fisik brutal tanpa gentar, manipulasi gelombang darah tubuh (*Blood Surge*), api iblis pembakar Dantian, dan duel satu lawan satu hingga titik darah penghabisan.

AI Game Master mengeksekusi setiap putaran pertempuran secara turn-based obyektif menggunakan formula terstandarisasi demi menjamin keadilan narasi tanpa plot armor.

---

## 2. Struktur Putaran Pertarungan & Formula Inisiatif

Setiap babak pertempuran dibagi ke dalam empat fase berurutan:
1. **Fase Penentuan Inisiatif (Initiative Phase)**
2. **Fase Aksi Karakter & Penggunaan Profesi (Action Phase)**
3. **Fase Resolusi Kerusakan & Respon Bertahan (Damage & Reaction Phase)**
4. **Fase Efek Lingkungan & Status Berkelanjutan (End-of-Round Phase)**

### Formula Penentuan Urutan Giliran (Initiative Check):
$$\text{Inisiatif} = \text{D20} + \text{Modifikator Kecepatan Ranah} + \text{Bonus Langkah Angin/Bayangan} - \text{Beban Berat Zirah}$$

| Ranah Kultivasi | Modifikator Kecepatan Dasar | Batas Tindakan per Giliran |
|---|---|---|
| **Fana / Qiguan Jing** | +1 | 1 Aksi Utama + 1 Pergerakan |
| **Tongmai Jing** | +3 | 1 Aksi Utama + 1 Pergerakan |
| **Yuanhai Jing** | +5 | 1 Aksi Utama + 1 Aksi Cepat / Melayang |
| **Shenfu Jing** | +8 | 1 Aksi Utama + 1 Aksi Batin / Telepati |
| **Xuanyuan Jing** | +12 | 1 Aksi Utama + 1 Respon Taktis Urat Bumi |
| **PoKong Jing** | +18 | 2 Aksi Utama + 1 Langkah Spasial (*Void Step*) |
| **Fashen Jing** | +25 | 2 Aksi Utama + 1 Serangan Avatar Raga Hukum |
| **Tianjun Jing** | +35 | 3 Aksi Utama + Kontrol Mutlak Domain Lingkungan |
| **Hunyuan Taihe** | +50 | Memanipulasi Aliran Waktu Pertempuran |

---

## 3. Formula Peluang Mengenai Sasaran (Hit Chance) & Kalkulasi Kerusakan

### 3.1 Formula Peluang Kena Serangan (Hit Chance %)
$$\text{Hit Chance (\%)} = \text{Base 75\%} + (\text{Ranah Penyerang} - \text{Ranah Bertahan}) \times 10 + \text{Bonus Akurasi Senjata} - \text{Modifikator Elakan/Kabut} $$

- **Batas Maksimal Hit Chance:** **95%** (Selalu ada 5% peluang musuh berhasil menangkis kritis).
- **Batas Minimal Hit Chance:** **5%** (Selalu ada 5% peluang serangan mujur mengenai titik vital).
- **Serangan Kritis (Critical Hit):** Terjadi jika lemparan dadu natural menunjukkan angka 20 (Kerusakan dikalikan **×1.8** dan mengabaikan 50% pertahanan zirah).

### 3.2 Formula Kerusakan Fisik & Kerusakan Spiritual
$$\text{Kerusakan Bersih} = (\text{Base Damage Senjata} + \text{Skala Bonus Qi}) \times \text{Modifikator Elemen} - \text{Pertahanan Zirah Target} $$

- **Tipe Kerusakan:**
  - *Tebasan / Tusukan Pedang:* Efektif melawan target tanpa zirah logam; memicu efek *Bleed*.
  - *Hantaman Tumpul Gada / Tinju Raga:* Efektif meremukkan tulang dan merusak zirah pelat tebal; memicu efek *Stun*.
  - *Sihir Api Neraka Jiuyou:* Membakar HP dan membakar persediaan Qi Dantian target; memicu efek *Burn*.
  - *Toksin Rawa Wanze:* Mengabaikan pertahanan zirah luar; merusak langsung persentase Max HP.

---

## 4. Status Efek Kondisi Pertempuran (Status Conditions)

| Nama Status Efek | Pemicu Terjadinya Efek | Dampak Mekanik yang Dialami Target | Durasi Standar |
|---|---|---|---|
| **Pendarahan (Bleed)** | Tebasan senjata tajam, sayatan angin | Kehilangan 5% Max HP setiap awal giliran; Stamina -10 | 3 Putaran (Bisa dihentikan dengan bebat perban) |
| **Terbakar Api Neraka (Burn)**| Serangan elemen api Jiuyou, bara lahar| Kehilangan 8% Max HP + kehilangan 50 Qi per turn; Armor -20% | 2 Putaran (Bisa dipadamkan dengan mantra air) |
| **Keracunan Bisa (Poison)** | Bisa katak Wanze, gas spora ungu | Mengabaikan zirah; kerusakan berkala 6% HP; Hit Chance -20% | 4 Putaran (Wajib meminum penawar racun) |
| **Goncangan Sukma (Stun)** | Pukulan telapak Vajra, gelombang sonik | Kehilangan giliran berikutnya; tidak dapat menghindar/menangkis | 1 Putaran |
| **Terkunci Akar (Entangled)** | Jeratan sulur kayu Shenye, jaring sutra| Kecepatan gerak = 0; terkena serangan mendapat bonus hit +25% | 2 Putaran (Bisa ditebas dengan senjata tajam) |
| **Tersesat Ilusi (Confused)** | Kabut Youwu Zhou, cermin rawa hantu | Peluang 50% menyerang kawan sendiri atau membuang senjata | 2 Putaran |
| **Penyimpangan Qi (Deviation)**| Dantian tersumbat amarah liar, serangan batin | Kehilangan kendali jurus; menderita kerusakan balik dari Qi sendiri| Hingga disadarkan atau pingsan |

---

## 5. Aksi Spesialis Profesi dalam Pertempuran (Crafting Battle Actions)

Kultivator dengan keahlian profesi dapat mengambil tindakan taktis khusus di tengah pertempuran:
1. **Aksi Alkemis — Lemparan Botol Reaktif (Quick Bomb Throw):**
   - Menghancurkan botol kimia asam Wanze atau mesiu pasir Chiwu ke area musuh untuk menghasilkan ledakan area 3x3 zhang.
2. **Aksi Insinyur Boneka — Pengerahan Golem Pengawal (Automaton Deployment):**
   - Memanggil boneka tempur dari tas spasial untuk menyerap satu serangan mematikan yang mengarah ke tubuh penjinak.
3. **Aksi Master Jimat — Inskripsi Kertas Kilat (Insta-Cast Talisman):**
   - Mengaktifkan jimat pelindung petir instan sebagai aksi reaksi pertahanan darurat tanpa mengonsumsi waktu giliran utama.
4. **Aksi Tabib — Pembebatan Titik Akupunktur Darurat (Battlefield First-Aid):**
   - Menghentikan seketika status Bleed rekan setim dan memulihkan 20% HP dalam batas waktu satu tarikan nafas.

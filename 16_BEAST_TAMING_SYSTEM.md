# 🐾 Sistem Penjinakan & Pelatihan Spirit Beast Dunia Xuanyuan

> **Modul:** 16 — Beast Taming & Training System
> **Kategori:** Penjinakan Monster Liar, Ikatan Kontrak Jiwa/Darah, Sistem Loyalitas & Penangkaran
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md`, `12_CROSS_REGION_ORGANIZATIONS.md`, `13_SPIRITUAL_ROOT_SYSTEM.md`, `20_COMBAT_SYSTEM.md`, `21_BESTIARY.md`, `INDEX.md`

---

## 1. Lore, Prinsip Penjinakan & Hubungan Manusia-Beast

Di Benua Xuanyuan (*Xuanyuan World*), Spirit Beast (Binatang Spiritual) bukanlah hewan ternak fana tak berakal, melainkan makhluk purba yang menghirup nafas langit-bumi dan memiliki kepekaan batin tinggi. Hubungan antara penjinak (*Beast Tamer / 驭兽师*) dan monsternya dibangun di atas prinsip saling menghargai garis keturunan dan kemauan bertarung.

Dua Jalan Penjinakan yang Diakui di Benua:
1. 🕊️ **Kontrak Kesetaraan Jiwa (Soul Equality Contract / 灵魂本命契约):** Tradisi Ortodoks dan Serikat Youxia. Manusia dan Beast menyatukan sedikit percikan kesadaran jiwa mereka. Beast bertarung secara sukarela sebagai saudara hidup-mati. Jika salah satu pihak terluka, yang lain merasakan getaran batinnya; jika penjinak gugur, beast bebas kembali ke alam liar atau menjaga makam tuannya.
2. 🩸 **Kontrak Darah Penakluk Kekuatan (Blood Dominance Contract / 血煞驭兽契约):** Tradisi keras Demonic Xueshan Zhou dan klan nomaden Kuangsha. Beast ditaklukkan melalui adu kekuatan fisik langsung. Penjinak meneteskan darah intinya ke dahi beast setelah memenangkan duel. Menghasilkan kepatuhan tempur mutlak dan insting haus darah buas yang mengerikan di medan tempur.

---

## 2. Tingkat Klasifikasi Spirit Beast (Tier 1 s/d Tier 9)

Kekuatan Spirit Beast diukur berdasarkan **9 Tier Ekologis** yang setara dengan Ranah Kultivasi manusia:

| Tier Beast | Sebutan Klasifikasi | Ranah Kultivasi Manusia yang Setara | Tingkat Kecerdasan & Perilaku | Batas Jumlah Kontrak Maksimal |
|---|---|---|---|---|
| **Tier 1** | **Binatang Bernafas Qi (Spirit Awakened)** | *Qiguan Jing* (Tier 1) | Naluri hewan cerdas, memahami 10 kata perintah dasar | Maksimal 3 Ekor |
| **Tier 2** | **Binatang Pembuka Urat (Nerve Unlocked)** | *Tongmai Jing* (Tier 2) | Memahami strategi sergap sederhana, emosional | Maksimal 2 Ekor |
| **Tier 3** | **Monster Liar Samudra (Yuan Beast)** | *Yuanhai Jing* (Tier 3) | Mampu melindungi tuannya secara otonom, setia | Maksimal 2 Ekor |
| **Tier 4** | **Monster Istana Roh (Spiritual Lord)** | *Shenfu Jing* (Tier 4) | Memiliki kesadaran taktis, telepati rasa batin | Maksimal 1 Ekor Utama |
| **Tier 5** | **Raja Monster Benua (Xuanyuan King)** | *Xuanyuan Jing* (Tier 5) | Kecerdasan setara manusia dewasa, memahami bahasa fana | Maksimal 1 Ekor Utama |
| **Tier 6** | **Monster Perobek Ruang (Void Render)** | *PoKong Jing* (Tier 6) | Mampu berbicara melalui transmisi telepati suara batin | 1 Ekor (Wajib Kontrak Jiwa Penuh) |
| **Tier 7** | **Binatang Raga Hukum (Dharma Monarch)**| *Fashen Jing* (Tier 7) | Memiliki wujud humanoid parsial, memimpin ribuan bawahan | 1 Ekor (Wajib Penjinak Ranah Setara) |
| **Tier 8** | **Monster Bencana Purba (Calamity Lord)**| *Tianjun Jing* (Tier 8) | Menguasai hukum alam regional, usia ribuan tahun | Hanya melalui Perjanjian Kemitraan Sakral |
| **Tier 9** | **Binatang Dewa Primordial (Divine Beast)**| *Hunyuan Taihe* (Tier 9) | Penjelmaan pilar benua (Naga Qinglong, Qiongqi Purba)| Tak Dapat Dijinakkan; Hanya Sekutu Dao |

---

## 3. Formula Matematika Peluang Penjinakan (Taming Success Rate)

Peluang keberhasilan menjinakkan monster liar dihitung oleh AI GM dengan formula:

$$\text{Taming Rate (\%)} = \text{Base Rate} + (\text{Ranah Penjinak} - \text{Tier Beast}) \times 15 + \text{Bonus Status Melemah (\%)} + \text{Kualitas Umpan Pakan (\%)} - \text{Kebanggaan Garis Darah Beast (\%)} $$

### Variabel Penentu Penjinakan:
1. **Status Kesehatan Target (Weakened Bonus):**
   - Monster HP 100%: **+0%** (Sangat sulit dijinakkan saat bugar).
   - Monster HP < 50%: **+15%**.
   - Monster HP < 20% (Kelelahan ekstrem / Terluka): **+35%**.
2. **Kualitas Pakan Penjinak (Taming Food):**
   - Daging / Buah Biasa: **+5%**.
   - Pakan Nutrisi Formula Spirit Grade 2–4: **+15%**.
   - Ramuan *Pil Penenteram Batin Hewani*: **+25%**.
3. **Penalti Kebanggaan Beast (Pride Modifier):**
   - Predator soliter puncak (Harimau, Serigala Raja, Rajawali Badai): Penalti **-20%**.
   - Beast garis darah primordial / purba: Penalti **-35%**.

*Jika proses taming gagal, monster akan mengalami status **Berserk Rage** (+30% Serangan selama 3 giliran) atau melarikan diri ke sarangnya.*

---

## 4. Sistem Loyalitas Jiwa & Pembinaan Ikatan (Loyalty 0–100%)

Setiap Spirit Beast yang berhasil diikat kontrak memiliki skor **Loyalitas (0 s/d 100%)**:

| Rentang Skor Loyalitas | Status Ikatan Batin | Perilaku & Respons di Medan Pertempuran | Risiko Pemberontakan |
|---|---|---|---|
| **0% – 25%** | **Memberontak / Terpaksa** | Menolak perintah berisiko tinggi; hanya menyerang jika diserang | Risiko kabur 40% jika HP menipis; potensi menyerang tuannya jika dicambuk |
| **26% – 50%** | **Patuh Bersyarat** | Mematuhi perintah dasar, ragu-ragu melindungi tuannya | Menuntut makanan bergizi setiap hari; efektivitas tempur 80% |
| **51% – 75%** | **Setia & Terlatih** | Mematuhi seluruh taktik, melompat melindungi tuannya dari serangan | Efektivitas tempur 100%; bonus inisiatif giliran +2 |
| **76% – 99%** | **Kawan Sejiwa (Kindred Spirit)**| Berbagi koordinasi telepati tanpa suara, rela mengorbankan nyawa | Bonus Serangan +15%, Max HP Beast +20%, tidak akan pernah melarikan diri |
| **100% (Puncak)** | **Penyatuan Hidup-Mati (Soulbound)**| Terbukanya jurus kombinasi *Fusi Jiwa Penjinak & Beast* | **Loyalitas Permanen Mutlak**; kebal terhadap sihir penghasut musuh |

### Metode Meningkatkan Loyalitas:
- Memberikan Pakan Nutrisi Formulasi Spirit tepat waktu (+3% per hari).
- Merawat dan mengobati luka monster setelah pertempuran usai (+5%).
- Melatih teknik tanding bersama di arena penangkaran (+4% per sesi latihan).
- Menghindari memaksakan pertarungan mati konyol melawan musuh yang terlalu kuat.

---

## 5. Sistem Penangkaran & Pemuliaan Keturunan (Beast Breeding)

Penjinak berpengalaman yang memiliki lisensi Tier 2 ke atas diizinkan membuka kandang penangkaran untuk membiakkan Spirit Beast:
- **Syarat Penangkaran:** Sepasang monster jantan dan betina dari famili yang sama dalam kondisi kesehatan prima dan loyalitas di atas 70%.
- **Masa Pengeraman / Kehamilan:** 7 hari hingga 30 hari nyata tergantung pada Tier monster.
- **Peluang Mutasi Garis Darah (Bloodline Mutation Chance):**
  - Makanan induk yang diperkaya *Buah Giok Nutrisi Spirit* memberi peluang 15% bagi anak yang lahir untuk memiliki elemen sekunder (misal: Serigala Bayangan bertanduk Petir).
  - Anak monster yang lahir di kandang penangkaran memulai kontrak dengan **Loyalitas Alami 80%** sejak menetas/lahir.

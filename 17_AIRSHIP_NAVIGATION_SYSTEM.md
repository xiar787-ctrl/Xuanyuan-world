# 🚢 Sistem Navigasi Kapal Terbang & Koridor Udara Dunia Xuanyuan

> **Modul:** 17 — Airship Navigation & Sky Corridor System
> **Kategori:** Transportasi Udara, Spesifikasi Feichuan Wanxing, Konsumsi Bahan Bakar Spirit, & Risiko Badai Langit
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md`, `01_WORLD_OVERVIEW_AND_CAPITAL.md`, `12_CROSS_REGION_ORGANIZATIONS.md`, `18_ECONOMY_SYSTEM.md`, `INDEX.md`

---

## 1. Lore, Monopoli Wanxing & Koridor Udara Benua

Benua Xuanyuan (*Xuanyuan World*) yang membentang seluas ±88 juta li² dipenuhi oleh ngarai curam, rawa beracun mematikan, lautan pasir hisap, dan kaldera lahar mendidih. Menempuh perjalanan darat melintasi batas wilayah membutuhkan waktu berbulan-bulan dan membawa risiko kematian tinggi akibat sergapan monster darat.

Untuk menghubungkan sepuluh penjuru dunia, **Kamar Dagang Sembilan Bintang Wanxing (Wanxing Nine-Star Merchant Guild)** mengoperasikan ribuan armada **Kapal Terbang Roh (Feichuan / 灵舟·飞船)**. Bekerjasama dengan perajin formasi Tiangong dan insinyur mekanik Mengyin, kapal-kapal ini ditenagai oleh **Pilar Penolak Gravitasi Batu Apung** dan pendorong jet Qi angin spiritual.

Di bawah naungan dekrit netral Kekaisaran Xuanyuan, armada Wanxing memegang hak lintas damai (*Right of Innocent Passage*) di seluruh wilayah Ortodoks, Unortodoks, dan Demonic asalkan tidak membawa senjata artileri tersembunyi yang mengancam kedaulatan sekte lokal.

---

## 2. Kelas & Spesifikasi Kapal Terbang Wanxing

Armada kapal terbang di Benua Xuanyuan terbagi ke dalam lima kelas standar:

| Kelas Kapal | Nama Resmi Feichuan | Panjang Lambung | Kapasitas Penumpang & Kargo | Kecepatan Rata-Rata | Ranah Minimal Pilot |
|---|---|---|---|---|---|
| **Kelas I** | **Skiff Daun Spirit (Leaf Skiff / 叶灵飞舟)** | 5 – 8 Zhang | 1–4 Orang / Kargo 500 Kati | 1.200 li / hari (100 li / jam) | *Yuanhai Jing* (Tier 3) |
| **Kelas II** | **Perahu Awan Penjelajah (Cloud Cruiser / 云巡飞舟)** | 15 – 25 Zhang | 10–30 Orang / Kargo 10 Ton | 1.800 li / hari (150 li / jam) | *Shenfu Jing* (Tier 4) |
| **Kelas III** | **Tongkang Dagang Bintang (Star Freighter / 星商重舟)** | 40 – 60 Zhang | 100 Penumpang / Kargo 150 Ton | 1.400 li / hari (115 li / jam) | *Xuanyuan Jing* (Tier 5) |
| **Kelas IV** | **Kapal Cepat Tempur Garnisun (Strike Frigate / 破空战舟)**| 30 – 45 Zhang | 50 Prajurit / Kargo Amunisi 30 Ton | 3.500 li / hari (300 li / jam) | *PoKong Jing* (Tier 6) |
| **Kelas V** | **Benteng Melayang Dreadnought (Titan Sky-Fortress / 九龙母舰)**| 150 – 300 Zhang | 2.000 Personel / Kargo 1.000 Ton | 2.400 li / hari (200 li / jam) | *Fashen Jing* (Tier 7+) |

---

## 3. Formula Waktu Perjalanan & Konsumsi Bahan Bakar Spirit

Durasi perjalanan antar-kota dihitung secara ketat oleh AI GM untuk mencegah teleportasi instan yang merusak realisme:

$$\text{Durasi Perjalanan (Hari)} = \frac{\text{Jarak Tempuh (li)}}{\text{Kecepatan Feichuan (li/hari)} \times \text{Modifikator Cuaca Langit}}$$

### Formula Konsumsi Kristal Bahan Bakar Spirit:
$$\text{Biaya Operasional (Giok Roh)} = \text{Konsumsi Dasar Kelas} \times \text{Durasi Hari} \times \text{Koefisien Muatan Kargo}$$

| Kelas Feichuan | Konsumsi Bahan Bakar Standar | Biaya Tiket Penumpang Rata-Rata |
|---|---|---|
| **Kelas I (Leaf Skiff Pribadi)** | 5 Keping Giok Roh Menengah / Hari | Tidak dikomersialkan (Milik Pribadi) |
| **Kelas II (Perahu Awan Reguler)** | 20 Keping Giok Roh Menengah / Hari | 15 Keping Giok Roh Rendah per 100 li |
| **Kelas III (Tongkang Dagang Berat)** | 50 Keping Giok Roh Menengah / Hari | 8 Keping Giok Roh Rendah per 100 li (Kelas Ekonomi) |
| **Kelas IV (Kapal Cepat Tempur)** | 10 Keping Giok Roh Tinggi / Hari | 50 Keping Giok Roh Rendah per 100 li (Prioritas Militer) |
| **Kelas V (Benteng Dreadnought)** | 50 Keping Giok Roh Tinggi / Hari | Tiket VIP Mewah / 1 Keping Giok Roh Tinggi per rute |

---

## 4. Tabel Risiko Badai Udara & Fenomena Anomali 10 Wilayah

Setiap perjalanan udara melintasi wilayah tertentu wajib melakukan uji bahaya penerbangan (*Flight Hazard Check D20*):

| Wilayah Dilintasi | Fenomena Cuaca Udara Khas | Efek Bahaya Bila Gagal Check (< 6 D20) | Penanganan Pilot yang Efektif |
|---|---|---|---|
| **Qingye Zhou** | Pusaran Spora Hijau Berembun | Visibilitas turun 80%; mesin kemudi tertempel lumut spora | Mengaktifkan formasi hembusan angin pembersih lambung |
| **Zhongzhou** | Fluktuasi Gravitasi Kuali Sembilan Naga | Kapal mendadak oleng; penurunan ketinggian 500 zhang | Mengurangi kecepatan dan menstabilkan pilar batu apung |
| **Tianxu Zhou** | *Cloud-Sword Tempest* (Badai Niat Pedang) | Lambung kapal tergores; kerusakan zirah pelindung 15% | Menghidupkan perisai formasi besi bintang penuh |
| **Jinshan Zhou** | Gema Gelombang Sonik Lonceng Bodhi | Getaran sonik mengacaukan kompas kristal kemudi | Menggunakan pelindung telinga peredam getaran |
| **Youwu Zhou** | Kabut Halusinasi Jiwa (*Soul Delusion Mist*)| Pilot kehilangan orientasi; kapal berputar di tempat yang sama | Memasang Lentera Kabut Perak Wanxing di haluan kapal |
| **Kuangsha Zhou** | *Nine-Day Howling Dust* (Badai Debu Puyuh)| Partikel pasir menyumbat baling-baling dorong Qi | Naik ke ketinggian di atas 3.000 zhang melampaui awan debu |
| **Wanze Zhou** | Kabut Asam Organik Korosif | Korosi asam mengurangi daya tahan lambung per jam | Menyemprotkan cairan getah penawar asam ke pelat luar |
| **Jiuyou Zhou** | Gelombang Udara Magma Panas (*Heat Surge*)| Suhu kabin membakar; risiko Dantian penumpang kepanasan | Menyalakan formasi pendingin kristal es di ruang kabin |
| **Xueshan Zhou** | Turbulensi Arus Darah Liar Pegunungan | Serangan kawanan Elang Darah Pemakan Bangkai | Menyiagakan meriam busur panah formasi dek kapal |
| **Tianyuan Zhou** | **Retakan Ruang Spasial Hitam & Petir Kosmik**| **KAPAL TERHISAP RETAKAN (KEMATIAN TOTAL / HANCUR LEBUR)**| **DILARANG TERBANG TANPA KOMPAS SPASIAL & LISENSI TIER 4** |

---

## 5. Prosedur Darurat & Hak Veto Pilot Wanxing

1. **Hak Otoritas Mutlak Nahkoda:** Di atas kapal terbang Wanxing, instruksi nahkoda/pilot berlisensi bersifat mutlak. Siapapun penumpang yang memicu perkelahian fisik atau menggunakan teknik api terbuka di dekat tangki kristal spirit akan langsung diborgol rantai peredam Qi dan diturunkan di pos benteng terdekat.
2. **Prosedur Parasut Giok Darurat (Escape Talisman):** Seluruh kapal penumpang resmi Wanxing dilengkapi jimat pelambat jatuh (*Slow-Fall Talisman*) di bawah setiap kursi penumpang jika kapal mengalami kerusakan mesin kritis di udara.
3. **Penyitaan Kargo Ilegal:** Seluruh kargo yang terbukti mengandung racun busuk terlarang tanpa segel resmi atau telur monster bencana akan diserahkan ke Dewan Arbitrase Kekaisaran.

# Update Persiapan Mudik — Hasil Load Test Aki & Rekomendasi Ban

**Tanggal:** 18 Maret 2026
**Referensi:** [persiapan-mudik-final-2026.md](persiapan-mudik-final-2026.md)
**Konteks:** BMW E46 318i N42 (2003), odometer ~146.606 km, rute Serpong → Kuningan (~270 km)

---

## 1. Hasil Load Test Aki di B-Quik Puspitek

### 1.1 Data dari Struk Midtronics MDX-P300

| Parameter | Hasil | Keterangan |
|-----------|:-----:|------------|
| **Battery Test** | **GOOD, RECHARGE** | Aki masih bagus, tapi perlu di-charge |
| Voltage (mesin mati) | 12.54V | Sedikit rendah (idealnya 12.6-12.8V) |
| Measured CCA | **334 CCA** | Kemampuan cranking aktual |
| Rating CCA | **490 CCA** | Standar aki saat baru |
| **CCA Ratio** | **68.2%** | ⚠️ Di bawah threshold 70% |
| JIS Size | 80D26 | Tipe aki JIS (bukan DIN standar BMW) |
| Battery Type | Regular (basah) | Aki basah konvensional |
| **Starter Test** | **NORMAL** | 10.78V saat cranking — OK |
| **Charging Test** | **OK** | 14.02V — alternator bekerja normal |

### 1.2 Interpretasi Hasil

**Verdict: Aki masih BISA dipakai, tapi BORDERLINE.**

Penjelasan detail:

1. **"GOOD, RECHARGE"** — Tester menilai sel-sel aki masih sehat, tapi tegangan rendah karena kurang terisi penuh. Ini wajar untuk mobil yang **tidak dipakai harian** — aki pelan-pelan kehilangan muatan saat parkir.

2. **CCA 68.2%** — Berdasarkan threshold yang kita tetapkan di dokumen mudik:
   - CCA > 80% = ✅ Aman
   - CCA 70-80% = ⚠️ Borderline
   - **CCA < 70% = ❌ Ganti sebelum mudik**

   Posisi Anda saat ini **tepat di bawah 70%**, masuk zona "ganti". TAPI ada nuansa penting: CCA bisa naik setelah aki di-charge penuh. Aki yang kurang terisi (12.54V) cenderung menunjukkan CCA lebih rendah dari kondisi sebenarnya.

3. **Starter Test NORMAL** — Saat cranking, tegangan drop ke 10.78V. Ini masih di atas batas minimum 10V, artinya aki masih mampu menyalakan mesin saat ini.

4. **Charging Test OK** — Alternator menghasilkan 14.02V. Sistem charging bekerja normal — aki terisi saat mesin hidup.

5. **JIS 80D26** — Ini bukan ukuran standar BMW E46. BMW E46 seharusnya pakai aki DIN (European standard). Aki JIS 80D26 kemungkinan adalah replacement non-original. Secara fisik bisa muat, tapi dimensi dan terminal position berbeda dari spesifikasi pabrik.

### 1.3 Rekomendasi Aki

Mengingat **budget terbatas** dan hasil "GOOD, RECHARGE":

#### Opsi A: Charge dulu, test ulang (Budget-friendly)
- **Tindakan:** Pakai mobil lebih sering 1-2 minggu sebelum mudik (minimal 30-45 menit berkendara per hari), ATAU charge pakai battery charger external
- **Setelah itu:** Load test ulang di B-Quik (gratis jika minta sopan)
- **Jika CCA naik > 70%:** Aman untuk mudik, **bawa jumper cable** sebagai backup
- **Jika CCA tetap < 70%:** Ganti aki
- **Biaya:** Rp 0 (jika pakai mobil) atau Rp 50.000-100.000 (jasa charge)
- **Pro:** Hemat budget untuk ganti ban yang lebih urgent
- **Kontra:** Perlu effort dan waktu

#### Opsi B: Ganti aki sekarang (Lebih aman)
- **Tindakan:** Ganti ke aki MF (Maintenance Free) DIN LN2/LN3
- **Rekomendasi:** Delkor MF 56219 (62Ah, 580A CCA) — Rp 1.285.000-1.565.000
- **Alternatif lebih murah:** GS Astra MF DIN 60 — Rp 800.000-1.000.000
- **Pro:** Peace of mind, upgrade dari basah ke MF, ukuran DIN yang benar untuk BMW
- **Kontra:** Biaya tambahan signifikan saat ban juga harus diganti

#### Keputusan yang Disarankan

**Prioritaskan ganti BAN dulu** — ban produksi 2011 jauh lebih berbahaya daripada aki yang masih "GOOD". Untuk aki:
1. Charge aki dengan cara pakai mobil lebih sering
2. Load test ulang sebelum berangkat mudik
3. **WAJIB bawa jumper cable** saat mudik
4. Ganti aki setelah mudik jika budget sudah tersedia

---

## 2. Analisis Kondisi Ban — CRITICAL

### 2.1 Temuan

**Ban produksi tahun 2011 = USIA 15 TAHUN.**

Ini **5x lebih tua** dari batas aman standar industri (6 tahun). Menurut rekomendasi Pirelli, Bridgestone, dan semua produsen ban global:

| Umur Ban | Status |
|:--------:|--------|
| < 5 tahun | ✅ Aman |
| 5-6 tahun | ⚠️ Batas akhir |
| > 6 tahun | ❌ WAJIB GANTI |
| **15 tahun (ban Anda)** | **💀 SANGAT BERBAHAYA** |

### 2.2 Risiko Nyata Ban 15 Tahun di Tol

| Risiko | Penjelasan |
|--------|------------|
| **Blowout (pecah mendadak)** | Karet sudah keras dan rapuh. Di kecepatan 100+ km/h di tol Cipali, pecah ban bisa menyebabkan kehilangan kendali kendaraan |
| **Grip sangat rendah** | Compound karet sudah mengeras — daya cengkeram di aspal basah (hujan) hampir tidak ada |
| **Sidewall cracking** | Retakan mikro di dinding ban yang tidak terlihat mata — bisa pecah kapan saja |
| **Structural failure** | Belt separation — lapisan dalam ban terpisah saat kecepatan tinggi |

**Kesimpulan: SEMUA 4 BAN HARUS DIGANTI. Tidak ada opsi lain.** Tidak bisa ganti 2 saja — keempat ban sama-sama berbahaya.

---

## 3. Analisis Pricelist Ban dari Bengkel

### 3.1 Tabel Perbandingan Lengkap

| No | Bengkel | Ban | Harga/pcs | Total 4 pcs | Bonus | Speed Rating |
|:--:|---------|-----|----------:|------------:|-------|:------------:|
| 1 | Warna Warni Ban Pamulang | Bridgestone Turanza 6 | 1.350.000 | 5.400.000 | - | W (270 km/h) |
| 2 | Warna Warni Ban Pamulang | Bridgestone EP300 | 1.250.000 | 5.000.000 | - | V (240 km/h) |
| 3 | Warna Warni Ban Pamulang | Accelera IOTA EVT | 800.000 | 3.200.000 | - | ? |
| 4 | Ottoban Plus BSD | GT Radial Champiro GTX Pro | 820.000 | 3.280.000 | - | V (240 km/h) |
| 5 | Ottoban Plus BSD | Hankook Ventus V2 Concept2 H457 | 850.000 | 3.400.000 | - | V (240 km/h) |
| 6 | BSD Rims Center (BRC) | Accelera / Zeetex | 800.000 | 3.200.000 | Free balancing, Spooring Rp 200.000 | ? |
| 7 | **Ottoban Pamulang** | **GT Radial Champiro GTX Pro** | **820.000** | **3.280.000** | **Free balancing, nitrogen, pentil baru** | **V (240 km/h)** |

### 3.2 Klasifikasi Brand Berdasarkan Kualitas

| Tier | Brand | Asal | Reputasi |
|:----:|-------|------|----------|
| **Premium** | Bridgestone | Jepang | Top 3 global. OEM banyak pabrikan. Kualitas excellent |
| **Mid-Upper** | Hankook | Korea | Top 7 global. OEM supplier BMW, Audi, Mercedes di beberapa model. Kualitas sangat baik |
| **Mid** | GT Radial | Indonesia (Gajah Tunggal) | Produsen ban terbesar Indonesia. Ekspor ke 130+ negara. Kualitas baik, harga kompetitif |
| **Budget** | Accelera | Indonesia | Brand ekonomi. Kualitas cukup untuk pemakaian normal |
| **Budget** | Zeetex | UAE | Brand ekonomi. Kurang dikenal, quality control kurang konsisten |

### 3.3 Eliminasi — Yang TIDAK Direkomendasikan

| Ban | Alasan Tidak Direkomendasikan |
|-----|-------------------------------|
| **Bridgestone Turanza 6** (Rp 1.350.000) | Excellent tapi overkill untuk budget terbatas dan pemakaian weekend. Ban ini akan keburu tua (aging) sebelum habis tread-nya |
| **Bridgestone EP300** (Rp 1.250.000) | Sama — terlalu mahal untuk pola pemakaian Anda. Total Rp 5 juta untuk 4 ban |
| **Accelera IOTA EVT** (Rp 800.000) | Brand budget — grip dan durabilitas kurang untuk BMW E46 di kecepatan tol. Accelera adalah brand ekonomi yang lebih cocok untuk city car |
| **Accelera / Zeetex di BRC** (Rp 800.000) | Brand budget. Zeetex quality control kurang konsisten. Tidak ideal untuk highway driving |

### 3.4 Kandidat Terbaik — Head-to-Head

| Kriteria | GT Radial Champiro GTX Pro | Hankook Ventus V2 Concept2 H457 |
|----------|:--------------------------:|:-------------------------------:|
| **Harga/pcs** | Rp 820.000 | Rp 850.000 |
| **Total 4 pcs** | Rp 3.280.000 | Rp 3.400.000 |
| **Selisih total** | — | +Rp 120.000 |
| **Brand tier** | Mid (Indonesia) | Mid-Upper (Korea) |
| **Speed rating** | V (240 km/h) | V (240 km/h) |
| **Load index** | 91 (615 kg) | 94 XL (670 kg) |
| **Teknologi** | Nano Silica, directional tread | Advanced silica compound |
| **Wet grip** | Baik | Sangat baik |
| **Dry grip** | Baik | Sangat baik |
| **Kebisingan** | Normal | Rendah (quiet ride) |
| **Warranty** | Standar | 45,000 mile tread life warranty |
| **Review global** | Sedikit review internasional | Banyak review positif — "best budget performance tire" |
| **Cocok BMW E46?** | ✅ Ya | ✅ Ya — Hankook adalah OEM supplier BMW |

---

## 4. REKOMENDASI FINAL

### 🏆 Pilihan #1 (BEST VALUE): Hankook Ventus V2 Concept2 H457 di Ottoban Plus BSD

| Item | Detail |
|------|--------|
| **Ban** | Hankook Ventus V2 Concept2 H457 205/55 R16 94V XL |
| **Bengkel** | Ottoban Plus BSD |
| **Harga** | Rp 850.000 x 4 = **Rp 3.400.000** |
| **Selisih vs GT Radial** | Hanya **Rp 120.000 lebih mahal** untuk total 4 ban |

**Mengapa Hankook #1 meskipun sedikit lebih mahal:**

1. **Hankook adalah OEM supplier BMW** — brand ini memproduksi ban untuk BMW di beberapa model. Artinya mereka memahami karakter handling dan bobot mobil BMW.

2. **Load index 94 XL vs 91** — BMW E46 318i berbobot ~1.400 kg. Load index 94 (670 kg per ban) memberikan margin keamanan lebih besar, terutama saat muatan penuh mudik (penumpang + barang).

3. **Wet grip lebih superior** — Review global konsisten menyebutkan Hankook H457 punya wet grip yang excellent di kelasnya. Penting untuk musim hujan saat mudik.

4. **Quiet ride** — BMW E46 terkenal sebagai "driver's car" — ban yang tenang melengkapi karakter mobil ini.

5. **45,000 mile warranty** — Untuk pemakaian weekend, ban ini bisa bertahan bertahun-tahun sebelum habis tread-nya.

6. **Selisih hanya Rp 30.000/ban** — Ini upgrade kualitas signifikan dengan biaya tambahan minimal.

### Pilihan #2 (TERMURAH YANG AMAN): GT Radial Champiro GTX Pro di Ottoban Pamulang

| Item | Detail |
|------|--------|
| **Ban** | GT Radial Champiro GTX Pro 205/55 R16 91V |
| **Bengkel** | Ottoban Pamulang |
| **Harga** | Rp 820.000 x 4 = **Rp 3.280.000** |
| **Bonus** | Free balancing, nitrogen, pentil baru |

**Mengapa GT Radial tetap pilihan yang solid:**

1. **Gajah Tunggal adalah produsen ban terbesar Indonesia** — quality control terjamin, paham kondisi jalan Indonesia.
2. **Champiro GTX Pro adalah lini premium GT Radial** — bukan ban murahan, ini lini touring performance mereka.
3. **Nano Silica Technology** — grip basah dan kering lebih baik dari ban GT Radial biasa.
4. **Speed rating V (240 km/h)** — lebih dari cukup untuk tol Cipali.
5. **Bonus di Ottoban Pamulang** bernilai ~Rp 200.000-300.000 (balancing, nitrogen, pentil baru).

**Kekurangan:** Ottoban Pamulang **tidak menyediakan spooring**. Anda perlu spooring di tempat lain setelah ganti ban.

---

## 5. Rencana Eksekusi

### 5.1 Skenario yang Disarankan

**Langkah 1 — Ganti ban (PRIORITAS UTAMA)**

| Opsi | Lokasi | Total Biaya Ban | Spooring | Total Estimasi |
|:----:|--------|----------------:|---------:|---------------:|
| **A** | Ottoban Plus BSD (Hankook H457) | 3.400.000 | ~200.000-250.000* | **~Rp 3.600.000-3.650.000** |
| **B** | Ottoban Pamulang (GT Radial GTX Pro) | 3.280.000 | 0 (tidak tersedia)** | **Rp 3.280.000** + spooring di tempat lain |

*\*Tanyakan apakah Ottoban Plus BSD menyediakan spooring. Ottoban biasanya include balancing gratis dengan pembelian ban.*
*\*\*Jika pilih Ottoban Pamulang, spooring bisa dilakukan di B-Quik Puspitek (~Rp 150.000-250.000)*

**Langkah 2 — Spooring (WAJIB setelah ganti 4 ban)**

Spooring/wheel alignment wajib dilakukan setelah ganti keempat ban. Ini memastikan:
- Ban aus merata
- Mobil tidak narik kiri/kanan
- Handling stabil di kecepatan tinggi

Jika bengkel ban tidak menyediakan spooring:
- B-Quik Puspitek — sekalian bisa cek coolant dan charge aki

**Langkah 3 — Aki (charge dulu, evaluasi ulang)**

1. Setelah ganti ban, pakai mobil lebih sering (minimal 30-45 menit/hari) selama 1-2 minggu
2. Load test ulang di B-Quik sebelum berangkat mudik
3. Jika CCA > 70% → aman, bawa jumper cable
4. Jika CCA masih < 70% → ganti aki sebelum berangkat

### 5.2 Estimasi Budget Total

| Skenario | Item | Biaya |
|----------|------|------:|
| **Minimum (ban saja)** | 4x GT Radial GTX Pro + spooring | **~Rp 3.480.000** |
| **Rekomendasi (ban + spooring + coolant)** | 4x Hankook H457 + spooring + coolant flush | **~Rp 3.850.000-4.100.000** |
| **Lengkap (ban + aki + spooring + coolant)** | Semua item | **~Rp 4.850.000-5.650.000** |

### 5.3 Catatan Penting untuk Pemakaian Weekend

Karena mobil lebih sering parkir daripada dipakai:

1. **Cek tekanan ban setiap 2 minggu** — ban yang parkir lama cenderung kehilangan tekanan
2. **Parkir di tempat teduh** jika memungkinkan — sinar UV mempercepat aging karet ban
3. **Jangan parkir dengan handrem ditarik di tempat datar** — cukup posisi P (Parking) di transmisi matic. Handrem yang ditarik lama bisa menyebabkan kampas rem lengket
4. **Jalankan mobil minimal 1x seminggu** selama 15-20 menit — ini baik untuk ban (mencegah flat spot), aki (tetap terisi), dan mesin (pelumasan)

---

## 6. Panduan Komunikasi ke Bengkel Ban

### Jika ke Ottoban (Plus BSD atau Pamulang):

> "Pak, saya mau ganti 4 ban untuk BMW E46 318i tahun 2003. Ukuran 205/55 R16. Ban lama saya sudah produksi 2011, jadi memang harus ganti semua.
>
> Saya tertarik pakai [Hankook Ventus V2 / GT Radial GTX Pro]. Apakah stok ready?
>
> Sekalian minta tolong:
> 1. **Balancing** keempat ban setelah pasang
> 2. **Isi nitrogen** (kalau tersedia)
> 3. **Ganti pentil** baru semua
> 4. **Spooring** (apakah tersedia di sini?)
> 5. Set **tekanan ban untuk perjalanan tol jauh** — saya mau mudik 270 km lewat tol Cipali
>
> Oh ya, mobil saya jarang dipakai — biasa weekend aja. Jadi bukan daily."

### Yang Harus Ditanyakan:

1. "Apakah ban yang dipasang **produksi baru** (DOT 2025 atau 2026)? Tolong saya cek kode DOT-nya setelah dipasang."
2. "Berapa lama garansi ban ini?"
3. "Apakah ada **garansi pemasangan** — jika ada masalah balancing, bisa kembali?"

### Red Flags:

- ❌ Mekanik menawarkan ban **produksi lama** (DOT 2023 atau lebih tua) — minta yang lebih baru
- ❌ Harga naik signifikan dari pricelist yang sudah dikasih — tanya alasannya
- ❌ Tidak mau menunjukkan **kode DOT** ban baru — bisa jadi stok lama
- ❌ Bilang spooring tidak perlu setelah ganti 4 ban — **spooring WAJIB**

### Bukti yang Harus Diminta:

- [ ] Foto **kode DOT** ban baru (keempat ban)
- [ ] **Invoice** dengan detail merek, ukuran, dan harga per ban
- [ ] Print-out **hasil spooring** (jika dilakukan di sana)
- [ ] Konfirmasi **tekanan ban** yang dipasang (catat angkanya)
- [ ] Ban lama — **minta lihat** ban lama Anda untuk konfirmasi memang sudah parah kondisinya

---

## 7. Update Status Checklist Mudik

| No | Item | Status Sebelumnya | Status Sekarang | Tindakan Selanjutnya |
|:--:|------|:-----------------:|:---------------:|---------------------|
| 1 | Oli mesin + filter | ✅ OK | ✅ OK | — |
| 2 | Kampas rem | ✅ OK | ✅ OK | — |
| 3 | Fan belt | ✅ OK | ✅ OK | — |
| 4 | Oli matic | ✅ OK | ✅ OK | — |
| 5 | Speedometer RPM | ✅ OK | ✅ OK | — |
| 6 | Aditif oli | ✅ OK | ✅ OK | — |
| 7 | Air radiator | ⚠️ Pakai air AC | ⚠️ Belum diganti | Flush + ganti coolant saat spooring di B-Quik |
| 8 | **Aki** | ❌ Belum dicek | ⚠️ **GOOD, RECHARGE (CCA 68.2%)** | Charge dulu, test ulang sebelum mudik |
| 9 | **Ban** | ❌ Belum dicek | ❌ **PRODUKSI 2011 — WAJIB GANTI** | Ganti 4 ban segera |
| 10 | No crank | ✅ OK | ✅ OK | Bawa jumper cable |

### Prioritas Tindakan:

1. 🔴 **GANTI 4 BAN** — paling urgent, langsung ke Ottoban
2. 🟡 **SPOORING** — setelah ganti ban (di bengkel yang sama atau B-Quik)
3. 🟡 **COOLANT** — flush dan ganti ke coolant proper (bisa di B-Quik sekalian spooring)
4. 🟢 **AKI** — charge dulu, test ulang, bawa jumper cable sebagai backup

---

## Sumber Referensi

- [GT Radial Indonesia — Champiro GTX Pro](https://www.gtradial.co.id/en/Tire/CHAMPIRO-GTX-PRO/IndonesiaPattern000203) — Spesifikasi resmi
- [Hankook Ventus V2 Concept2 H457 — Tire Reviews](https://www.tire-reviews.com/Tire/Hankook/Ventus-V2-Concept-2-H457.htm) — Review global
- [Hankook H457 Reviews — SimpleTire](https://simpletire.com/brands/hankook-tires/ventus-v2-concept2-h457/reviews) — User reviews
- [Hankook H457 Reviews — 1010tires](https://www.1010tires.com/Tires/reviews/Hankook/ventus+v2+concept2+(h457)) — User reviews
- [Kompas — Harga Ban Mobil April 2025](https://otomotif.kompas.com/read/2025/04/11/100200615/ganti-ban-setelah-pulang-mudik-cek-harga-ban-mobil-per-april-2025?page=all) — Referensi harga pasar Indonesia
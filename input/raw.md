# PROJECT STANDARD

## BMW E46 318i N42

---

## 1. Referensi Katalog Suku Cadang (Wajib)

### Primary Source (Wajib Utama)

RealOEM
[https://www.realoem.com/bmw/enUS/partgrp?id=AY77-IDN-03-2003-E46-BMW-318i](https://www.realoem.com/bmw/enUS/partgrp?id=AY77-IDN-03-2003-E46-BMW-318i)

### Spesifikasi Kendaraan

* Model: BMW E46 318i
* Engine: N42
* Tahun: 2003
* Market: Indonesia

### Aturan Penggunaan

* Setiap part wajib mencantumkan part number OEM.
* Jika terdapat supersession (penggantian nomor part versi baru), wajib disebutkan.
* Dilarang menggunakan estimasi tanpa pengecekan di RealOEM.

---

## 2. Referensi Abbreviation & Terminologi BMW

### Sumber

BMW Sections
[https://www.bmwsections.com/info/abbreviations.php](https://www.bmwsections.com/info/abbreviations.php)

### Contoh Istilah Umum

* DME = Digital Motor Electronics
* DISA = Differential Air Intake System
* VANOS = Variable Nockenwellen Steuerung
* CCV = Crankcase Ventilation
* ICV = Idle Control Valve
* EWS = Immobilizer System

---

## 3. Device Scanner yang Digunakan

Jika AI menyarankan melakukan scan, maka wajib menggunakan device berikut dan analisa harus disesuaikan dengan kemampuan alat tersebut.

### THINKCAR THINKSAFE (Bluetooth VCI)

#### Spesifikasi Operasional

* OBD2 Full Mode (10 mode standar)
* Full System Scan (Engine, ABS, SRS, TCM, BCM, dll)
* Active Test / Bi-directional Control
* Auto VIN
* Live Data + Graph
* Freeze Frame
* Reset Function (masa aktif terbatas)

Manual:
[https://manuals.plus/ae/1005003122767964](https://manuals.plus/ae/1005003122767964)

---

## 4. Forum Referensi Teknis
karena masuk forum perlu login maka gunakan mcp chromedevtool dan login menggunakan credential dari file `.env`
(variabel: E46_FANATICS_USERNAME dan E46_FANATICS_PASSWORD)

### Forum Utama

E46 Fanatics
[https://www.e46fanatics.com](https://www.e46fanatics.com)


### Metode Pencarian

* Advanced search internal forum
  * untuk advance search gunakan: https://www.e46fanatics.com/search/?t=post
    *  This will allow you to choose to search titles only, add the member username who posted it or even select a specific forum to search from. 
* Google dengan format:
  `electric radiator fan site:e46fanatics.com`

### Prosedur Pencarian

1. Cari berdasarkan symptom.
2. Bandingkan minimal 3 thread.
3. Identifikasi pola common failure N42.
4. Cocokkan dengan hasil scan (jika dilakukan scan).

---

## 5. Riwayat Service

### File Referensi

`/Source/Riwayat Detail Service.csv`

### Aturan Interpretasi

* Ada tanggal + evidence → part sudah diganti.
* Tidak ada tanggal → part belum dibeli.
* Ada symptom tetapi belum dibeli → masuk planned purchase.

### Catatan Evaluasi

Riwayat service digunakan sebagai referensi saat merekomendasikan part:

* Jika part sudah pernah diganti, evaluasi kemungkinan kualitas part atau faktor penyebab lain.
* Pertimbangkan part lain yang belum pernah diganti.
* Perhatikan tanggal penggantian meskipun part sudah diganti (umur pakai tetap relevan).

---
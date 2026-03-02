# BMW E46 AI Assistant

AI assistant berbasis Claude Code untuk diagnosis, perawatan, dan analisis riwayat service **BMW E46 318i N42 (2003, pasar Indonesia)**.

---

## Kendaraan Target

| Parameter | Detail |
|-----------|--------|
| Model | BMW E46 318i |
| Engine | N42 (N42B20) |
| Tahun | 2003 |
| Market | Indonesia (IDN) |
| Transmisi | Automatic |
| RealOEM ID | `AY77-IDN-03-2003-E46-BMW-318i` |

---

## Fitur

Assistant ini berjalan sebagai Claude Code skill (`/bmw`) dengan 4 mode operasi:

### `/bmw diagnose [gejala atau DTC code]`
Analisis masalah berdasarkan gejala atau kode DTC. Workflow-nya:
1. Identifikasi gejala dan sistem yang terkait (spesifik N42)
2. Cek riwayat service dari CSV untuk konteks part yang sudah/belum pernah diganti
3. Riset forum E46 Fanatics untuk pola common failure N42
4. Lookup part number OEM di RealOEM + harga aktual di Tokopedia
5. Panduan scan menggunakan THINKCAR THINKSAFE

### `/bmw parts [nama sistem]`
Lookup part number OEM dan harga untuk sistem tertentu. Output berupa tabel dengan OEM part number, supersession (jika ada), dan estimasi harga dari Tokopedia.

### `/bmw history`
Analisis riwayat service dari file CSV. Menampilkan statistik pengeluaran, part yang overdue, masalah berulang, dan planned purchase yang belum dibeli.

### `/bmw mechanic [topik]`
Panduan komunikasi dengan mekanik: kalimat yang bisa langsung diucapkan, pertanyaan yang harus ditanyakan, bukti yang harus diminta, estimasi biaya wajar, dan red flag bengkel yang tidak jujur.

---

## Struktur Proyek

```
bmw-e46-ai-assistant/
├── .claude/
│   └── skills/
│       └── bmw/
│           ├── SKILL.md                  # Definisi skill /bmw
│           └── references/
│               ├── n42-failures.md       # Database common failure N42
│               └── mechanic-guide.md     # Panduan komunikasi mekanik
├── Source/
│   └── Riwayat Detail Service.csv        # Riwayat service kendaraan
├── input/
│   ├── raw.md                            # Project standard & referensi
│   ├── prompt-mudik.md                   # Contoh prompt analisis perjalanan
│   └── scan.txt                          # Output scan THINKCAR (raw)
├── output/
│   └── analisis-mudik-2026.md            # Hasil analisis kesiapan mudik
├── .env                                  # Credentials (tidak di-commit)
├── .env.example                          # Template credentials
└── .gitignore
```

---

## Prerequisites

- [Claude Code](https://claude.ai/code) CLI terinstall
- MCP server `chrome-devtools` aktif (untuk akses forum E46 Fanatics yang memerlukan login)

---

## Setup

**1. Clone repository dan masuk ke direktori:**
```bash
git clone <repo-url>
cd bmw-e46-ai-assistant
```

**2. Buat file `.env` dari template:**
```bash
cp .env.example .env
```

Isi credentials forum E46 Fanatics di file `.env`:
```
E46_FANATICS_USERNAME=your_username
E46_FANATICS_PASSWORD=your_password
```

**3. Jalankan Claude Code di direktori ini:**
```bash
claude
```

---

## Cara Penggunaan

### Diagnosa masalah berdasarkan gejala
```
/bmw diagnose mesin brebet saat akselerasi
```

### Diagnosa berdasarkan kode DTC
```
/bmw diagnose 279C
```

### Lookup part untuk sistem tertentu
```
/bmw parts cooling system
```

### Lihat ringkasan riwayat service
```
/bmw history
```

### Panduan ke mekanik
```
/bmw mechanic ganti thermostat
```

### Analisis kesiapan perjalanan jauh
Letakkan prompt analisis di folder `input/`, lalu jalankan:
```
/bmw diagnose [lihat file input/prompt-mudik.md]
```

---

## Referensi Eksternal

| Sumber | URL |
|--------|-----|
| RealOEM (Parts Catalog) | https://www.realoem.com/bmw/enUS/partgrp?id=AY77-IDN-03-2003-E46-BMW-318i |
| E46 Fanatics Forum | https://www.e46fanatics.com |
| BMW Abbreviations | https://www.bmwsections.com/info/abbreviations.php |
| THINKCAR Manual | https://manuals.plus/ae/1005003122767964 |

---

## Tools yang Digunakan AI

| Tool | Fungsi |
|------|--------|
| `Read` | Baca riwayat service CSV dan file referensi |
| `WebFetch` | Browse RealOEM untuk part number OEM |
| `WebSearch` | Cari harga di Tokopedia dan artikel teknis |
| `mcp__chrome-devtools` | Login dan search forum E46 Fanatics |

---

## Filosofi

- **Service dulu, ganti belakangan** — penggantian part hanya jika sudah tidak bisa diperbaiki
- **N42-specific** — semua analisis spesifik untuk mesin N42, bukan generic OBD2
- **Budget-conscious** — evaluasi price-quality ratio, harga aktual dari Tokopedia JABODETABEK
- **Mechanic-ready** — setiap rekomendasi dilengkapi panduan komunikasi ke mekanik
- **Selalu cantumkan sumber** — setiap informasi disertai link referensi yang bisa diverifikasi

---

## License

[MIT](LICENSE)

# Reorganisasi Struktur Folder BMW E46 AI Assistant

> **For Claude:** Gunakan subagent-driven-development untuk eksekusi plan ini.

**Goal:** Mengorganisir struktur folder proyek agar lebih terstruktur, konsisten, dan mudah dinavigasi.

**Arsitektur:** Pemisahan jelas antara data mentah, referensi, input prompt, dan output analisis dengan naming convention yang konsisten (lowercase).

**Tech Stack:** Shell commands untuk file operations, git untuk version control.

---

## Task 1: Buat struktur folder baru

**Files:**
- Create: `data/` - untuk semua data mentah kendaraan
- Create: `data/service-history/` - riwayat service
- Create: `data/references/` - dokumen referensi (PDF rute, dll)
- Create: `prompts/` - template prompt dan input analisis
- Create: `docs/analysis/` - hasil analisis (menggantikan `output/`)
- Create: `docs/procedures/` - prosedur dan panduan (ganti aki, dll)

**Step 1: Buat folder baru**

```bash
mkdir -p data/service-history data/references prompts docs/analysis docs/procedures
```

**Step 2: Verifikasi folder tercipta**

```bash
ls -la data/ docs/
```

Expected: Folder-folder baru terlihat

**Step 3: Commit**

```bash
git add data/ docs/
git commit -m "chore: create new folder structure"
```

---

## Task 2: Migrasi data service history

**Files:**
- Move: `Source/Riwayat Detail Service.csv` → `data/service-history/riwayat-service.csv`

**Step 1: Pindahkan file CSV dengan nama yang lebih deskriptif**

```bash
cp "Source/Riwayat Detail Service.csv" data/service-history/riwayat-service.csv
```

**Step 2: Verifikasi file tergandakan**

```bash
ls -la data/service-history/
```

Expected: `riwayat-service.csv` terlihat

**Step 3: Commit**

```bash
git add data/service-history/riwayat-service.csv
git commit -m "chore: migrate service history CSV with standardized name"
```

---

## Task 3: Migrasi dokumen referensi

**Files:**
- Move: `Source/Home (Pesona Remboelan J15) to Kuningan...pdf` → `data/references/rute-mudik-kuningan.pdf`
- Move: `Source/Hasil Load test Aki.jpg` → `data/references/load-test-aki.jpg`

**Step 1: Pindahkan PDF rute dengan nama yang lebih singkat**

```bash
cp "Source/Home (Pesona Remboelan J15) to Kuningan, Kuningan Regency, West Java - Google Maps.pdf" data/references/rute-mudik-kuningan.pdf
```

**Step 2: Pindahkan gambar load test aki**

```bash
cp "Source/Hasil Load test Aki.jpg" data/references/load-test-aki.jpg
```

**Step 3: Verifikasi**

```bash
ls -la data/references/
```

Expected: `rute-mudik-kuningan.pdf` dan `load-test-aki.jpg` terlihat

**Step 4: Commit**

```bash
git add data/references/
git commit -m "chore: migrate reference documents with standardized names"
```

---

## Task 4: Migrasi prompts

**Files:**
- Move: `input/prompt-mudik.md` → `prompts/analisis-mudik.md`
- Move: `input/scan.txt` → `prompts/scan-result.txt`
- Move: `input/raw.md` → `prompts/analisis-aki-ban-template.md`

**Step 1: Pindahkan prompt mudik**

```bash
cp input/prompt-mudik.md prompts/analisis-mudik.md
```

**Step 2: Pindahkan hasil scan**

```bash
cp input/scan.txt prompts/scan-result.txt
```

**Step 3: Pindahkan raw.md (sebenarnya adalah prompt template)**

```bash
cp input/raw.md prompts/analisis-aki-ban-template.md
```

**Step 4: Verifikasi**

```bash
ls -la prompts/
```

Expected: 3 file dengan nama baru terlihat

**Step 5: Commit**

```bash
git add prompts/
git commit -m "chore: migrate prompts with descriptive names"
```

---

## Task 5: Migrasi output analysis

**Files:**
- Move: `output/analisis-mudik-2026.md` → `docs/analysis/analisis-mudik-2026.md`
- Move: `output/analisis-aki-ban-mudik-2026.md` → `docs/analysis/analisis-aki-ban-mudik-2026.md`
- Move: `output/persiapan-mudik-final-2026.md` → `docs/analysis/persiapan-mudik-final-2026.md`
- Move: `output/prosedur-ganti-aki-e46.md` → `docs/procedures/prosedur-ganti-aki-e46.md`

**Step 1: Pindahkan file analisis ke docs/analysis/**

```bash
cp output/analisis-mudik-2026.md docs/analysis/
cp output/analisis-aki-ban-mudik-2026.md docs/analysis/
cp output/persiapan-mudik-final-2026.md docs/analysis/
```

**Step 2: Pindahkan prosedur ke docs/procedures/**

```bash
cp output/prosedur-ganti-aki-e46.md docs/procedures/
```

**Step 3: Verifikasi**

```bash
ls -la docs/analysis/ docs/procedures/
```

Expected: File-file analisis dan prosedur terlihat

**Step 4: Commit**

```bash
git add docs/analysis/ docs/procedures/
git commit -m "chore: migrate analysis and procedures to docs/"
```

---

## Task 6: Hapus folder lama dan cleanup

**Files:**
- Delete: `Source/` (folder kosong setelah migrasi)
- Delete: `input/` (folder kosong setelah migrasi)
- Delete: `output/` (folder kosong setelah migrasi)

**Step 1: Hapus folder Source/**

```bash
rm -rf Source/
```

**Step 2: Hapus folder input/**

```bash
rm -rf input/
```

**Step 3: Hapus folder output/**

```bash
rm -rf output/
```

**Step 4: Verifikasi cleanup**

```bash
ls -la
```

Expected: `Source/`, `input/`, `output/` sudah tidak ada

**Step 5: Commit**

```bash
git add -A
git commit -m "chore: remove old folder structure"
```

---

## Task 7: Update README.md dengan struktur baru

**Files:**
- Modify: `README.md:43-65` (section Struktur Proyek)

**Step 1: Update section Struktur Proyek di README.md**

Ganti section lama dengan:

```markdown
## Struktur Proyek

```
bmw-e46-ai-assistant/
├── data/
│   ├── service-history/
│   │   └── riwayat-service.csv          # Riwayat service kendaraan
│   └── references/
│       ├── rute-mudik-kuningan.pdf      # Peta rute mudik
│       └── load-test-aki.jpg            # Hasil load test aki
├── prompts/
│   ├── analisis-mudik.md                # Prompt analisis perjalanan
│   ├── analisis-aki-ban-template.md     # Template prompt analisis aki & ban
│   └── scan-result.txt                  # Hasil scan THINKCAR
├── docs/
│   ├── analysis/
│   │   ├── analisis-mudik-2026.md       # Analisis kesiapan mudik
│   │   ├── analisis-aki-ban-mudik-2026.md  # Analisis aki & ban
│   │   └── persiapan-mudik-final-2026.md   # Checklist final
│   └── procedures/
│       └── prosedur-ganti-aki-e46.md    # Panduan ganti aki
├── .claude/
│   └── skills/
│       └── bmw/
│           ├── SKILL.md                 # Definisi skill /bmw
│           └── references/
│               ├── n42-failures.md      # Common failure N42
│               └── mechanic-guide.md    # Panduan komunikasi mekanik
├── .env                                  # Credentials (tidak di-commit)
├── .env.example                          # Template credentials
└── README.md
```
```

**Step 2: Verifikasi README.md terupdate**

```bash
cat README.md | head -70
```

**Step 3: Commit**

```bash
git add README.md
git commit -m "docs: update README with new folder structure"
```

---

## Struktur Final

Setelah reorganisasi selesai, struktur folder akan menjadi:

```
bmw-e46-ai-assistant/
├── data/              # Data mentah kendaraan
│   ├── service-history/
│   └── references/
├── prompts/           # Input prompt untuk AI
├── docs/              # Dokumentasi & output
│   ├── analysis/
│   └── procedures/
├── .claude/           # System (tidak diubah)
├── .agents/           # System (tidak diubah)
├── .git/              # System (tidak diubah)
├── .env
├── .env.example
├── .gitignore
├── LICENSE
└── README.md
```

---

## Verification

**Step final: Tampilkan struktur lengkap**

```bash
find . -type f -not -path "*/\.*" | sort
```

Expected: Semua file terorganisir dengan rapi di folder baru
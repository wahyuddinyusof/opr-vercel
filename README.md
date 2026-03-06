# Sistem OPR — ADTEC JTM Kampus Kuantan (Vercel)

## Struktur Fail
```
opr-vercel/
├── index.html        ← Aplikasi utama
├── vercel.json       ← Konfigurasi Vercel
├── api/
│   └── claude.js     ← Backend function (simpan API key)
└── README.md
```

## Cara Deploy ke Vercel (Drag & Drop)

### Langkah 1 — Daftar Vercel
1. Pergi vercel.com
2. Sign up guna email (atau Google account)

### Langkah 2 — Deploy Folder
1. Dashboard Vercel → Klik "Add New" → "Project"
2. Pilih "Upload" (tanpa GitHub)
3. Drag & drop folder `opr-vercel` ini
4. Klik Deploy — tunggu 1-2 minit

### Langkah 3 — Set API Key (PENTING)
1. Project → "Settings" → "Environment Variables"
2. Tambah variable baru:
   - Name:  CLAUDE_API_KEY
   - Value: sk-ant-api03-... (API key Claude anda)
3. Klik Save
4. Pergi "Deployments" → Klik "..." → "Redeploy"

### Langkah 4 — Kongsi URL
URL akan jadi seperti: `https://opr-adtec.vercel.app`
Kongsi kepada semua staf — terus boleh guna!

## Tukar API Key
Settings → Environment Variables → Edit CLAUDE_API_KEY → Redeploy
Tidak perlu sentuh kod langsung.

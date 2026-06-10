# Sahabat Export — Single Page Website

Stack: **Vite + React** (static, tanpa backend). Cocok untuk Vercel free tier.

## Jalankan di lokal

```bash
npm install
npm run dev      # buka http://localhost:5173
```

## Deploy ke Vercel (free)

### Cara A — via GitHub (disarankan)
1. Push folder ini ke repo GitHub baru.
2. Buka vercel.com → Add New → Project → import repo tersebut.
3. Vercel otomatis mendeteksi Vite (build: `npm run build`, output: `dist`). Klik Deploy.
4. Setiap `git push` ke branch utama akan auto-deploy.

### Cara B — via CLI
```bash
npm i -g vercel
vercel          # ikuti prompt, lalu:
vercel --prod
```

## Custom domain (www.sahabatexport.com)
Di dashboard Vercel → Project → Settings → Domains → tambahkan domain,
lalu arahkan DNS (CNAME `www` → `cname.vercel-dns.com`) di registrar Anda.

## Edit konten
Semua teks ada di `src/App.jsx` (array `markets`, `categories`, `model` di bagian atas).
Warna & font ada di `src/index.css` bagian `:root`.

# Kelurahan LA Main

Website frontend berbasis React + Vite.

## Jalankan lokal

```bash
npm install
npm run dev
```

## Environment variables

File `.env` sudah di-ignore oleh Git, termasuk varian lain seperti `.env.*`.

Contoh variabel (buat file `.env` lokal):

```bash
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
VITE_GEMINI_API_KEY=your_gemini_api_key
```

## Auto Deploy

Repo: [Nazwadna/kelurahan-la-main](https://github.com/Nazwadna/kelurahan-la-main)

### Vercel

Project ini sudah punya `vercel.json` untuk SPA rewrite.

1. Login ke [Vercel](https://vercel.com/)
2. Klik **Add New Project**
3. Import repo `Nazwadna/kelurahan-la-main`
4. Framework preset: **Vite** (otomatis)
5. Tambahkan Environment Variables yang diperlukan
6. Klik **Deploy**

Setelah itu setiap push ke branch `main` akan auto deploy.

### Netlify

Project ini sudah punya `netlify.toml` dengan:
- build command: `npm run build`
- publish directory: `dist`
- redirect SPA ke `index.html`

Langkah setup:

1. Login ke [Netlify](https://app.netlify.com/)
2. Klik **Add new site** -> **Import an existing project**
3. Pilih GitHub dan repo `Nazwadna/kelurahan-la-main`
4. Pastikan build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
5. Tambahkan Environment Variables yang diperlukan
6. Klik **Deploy site**

Setelah itu setiap push ke branch `main` akan auto deploy.

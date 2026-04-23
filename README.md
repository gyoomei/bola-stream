# ⚽ BolaStream

BolaStream adalah web statis untuk menyimpan dan membuka kumpulan link nonton bola dengan UI modern, search cepat, favorit browser, recent history, dan dukungan PWA.

## Fitur
- Search link
- Filter kategori
- Sort A-Z / recommended / favorit
- Favorites tersimpan di `localStorage`
- Recently opened
- Installable PWA
- Offline cache dasar via service worker

## Struktur data
Link utama disimpan di:
- `links.json`

Kalau file itu tidak bisa diambil, halaman otomatis memakai data fallback dari `index.html`.

## Cara pakai
- Buka `index.html` di browser, atau
- Deploy ke Vercel / GitHub Pages

## Edit link
Tambahkan atau ubah item di `links.json` dengan format:

```json
{
  "name": "Nama Situs",
  "url": "https://contoh.com",
  "icon": "⚽",
  "color": "green",
  "category": "Live TV",
  "source": "Example",
  "priority": 1
}
```

## Catatan
Link streaming bisa berubah atau mati sewaktu-waktu. Gunakan fitur favorit dan recent untuk akses cepat.

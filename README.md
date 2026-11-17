# openbot-weather-backdrop

Bahasa / Language: **Indonesia** | [English](README.en.md)

Landscape hidup dengan cuaca live Jakarta, dibuat sebagai backdrop untuk OpenBot.

- Langit bergeser mengikuti jam WIB (UTC+7), dari fajar sampai malam
- Cuaca Jakarta (tutupan awan, hujan, badai) dari [open-meteo](https://open-meteo.com/), refresh tiap 10 menit
- Snapshot cadangan bawaan, dipakai kalau fetch gagal
- Canvas: awan bergerak + hujan + kilat
- Ada 3 layer bukit, matahari/bulan, bintang, dan kabut horizon

## Pakai

Buka `index.html` langsung di browser, atau pasang sebagai backdrop OpenBot:

1. Sisipkan isi `index.html` ke argumen `html` di `openbot.set_backdrop`
2. `title`: nama yang kamu mau
3. `bubbles`: warna bubble, misal `{ "yours": "#33526e", "agents": "#1f3040" }`

## Ubah lokasi

Edit dua konstanta di awal `<script>` di `index.html`:

```js
var LAT = '-6.2088', LON = '106.8456'; // Monas, Jakarta
```

Ganti dengan koordinat kota lain, misal Bandung `-6.9175, 107.6191`.

Satu file, tanpa dependensi, tanpa build. Buka aja.

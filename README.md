# TheVed Converter

Konverter mata uang & emas live dengan gaya cover KDP TheVed (krem, navy, merah).

**Live site:** https://vedreal.github.io/theved-converter/

## Fitur

- **Mata uang:** IDR ↔ USD ↔ HKD
- **Emas per gram:** gram ↔ IDR / USD / HKD
- **XAU:** troy ounce ↔ USD / HKD / IDR
- Harga pasar global **real-time**, auto-refresh tiap 60 detik
- 3 bahasa: Indonesia, English, 繁體中文 (Hong Kong)
- Tanpa login, tanpa database — satu file `index.html` statis

## Sumber harga (acuan TradingView)

- Emas (XAU/USD): [gold-api.com](https://api.gold-api.com/price/XAU) — harga spot global, sama seperti yang tampil di [TradingView XAU/USD](https://www.tradingview.com/symbols/XAUUSD/)
- Kurs (USD/IDR, USD/HKD): [open.er-api.com](https://open.er-api.com/v6/latest/USD) (ExchangeRate-API, data ECB) — bandingkan dengan [TradingView USD/IDR](https://www.tradingview.com/symbols/USDIDR/) dan [USD/HKD](https://www.tradingview.com/symbols/USDHKD/)
- 1 troy ounce = 31,1034768 gram

TradingView tidak menyediakan API quote gratis, jadi situs ini memakai endpoint publik di atas yang mengikuti harga spot global yang sama. Tautan TradingView disertakan di halaman untuk verifikasi.

## Menjalankan lokal

Buka `index.html` di browser, atau jalankan server statis apa pun, misal:

```sh
python3 -m http.server 8000
```

Lalu buka http://localhost:8000

## Lisensi

MIT

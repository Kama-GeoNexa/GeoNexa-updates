# GeoNexa Updates

Repository ini menyimpan manifest dan file release untuk updater GeoNexa.

## Release flow

1. Build `GeoNexa.exe` dan modul `.pyd` pada komputer developer.
2. Buat GitHub Release, misalnya `v1.1.1`.
3. Upload `GeoNexa.exe` dan `*.cp314-win_amd64.pyd` sebagai release assets.
4. Hitung SHA256 setiap asset.
5. Publish `update_manifest.json` setelah semua asset tersedia.

Jangan publish manifest yang menunjuk ke asset yang belum tersedia.

GeoNexa menggunakan AutoCAD 2021 / AcCoreConsole untuk pemrosesan DWG pada modul Extraction dan ODBC.

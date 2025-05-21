# OutageTracker

halo gengs

beberapa hal yang harus diketahui:
- `assets/` berisi semua asset seperti logo, background, dan sebagainya
- `data/mock-outage.json` kalau kita mau tes ambil data protoype
- `js/` berisi file javascript:
    - `api.js` buat semua api-nya, kalo ada yang kita pakai
    - `main.js` buat ngeload semuanya
    - `ui.js` render konten ke layar
    - `utils.js` file lainnya yang ga termasuk ke 3 file tadi

## Sample Workflow
(biar lebih paham ceunah)
pas web app-nya hidup, yang dijalanin tuh:
1. `main.js` hidupin semuanya, kaya `fetchOutages()` dari `api.js`
2. `api.js` ngasih datanya ke `main.js`, data asli (bismillah) ataupun cuman mock
3. `main.js` oper data dari `api.js` lagi ke `ui.js`
4. `ui.js` ngerender semua data tadi

## Tutorial Kolaborasi
1. Ambil part masing-masing (JANGAN LANGSUNG COMMIT DI MAIN ATAU MASTER, buat branch masing-masing)
2. Udah itu doang
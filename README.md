# JEJAK JSS

Sistem Pengurusan Keberadaan Staf Digital — Jabatan Sains Sosial, Kolej MARA Banting.

**Pautan untuk guru:** https://kmb-digital.github.io/jss/

Repo ini hanya menyimpan paparan app. Data kekal dalam Google Sheet **JEJAK JSS – Data**, dan
semua semakan PIN serta nombor gaji berlaku dalam Google Apps Script. Tiada PIN atau data guru
disimpan di sini.

## Fail

| Fail | Guna |
|---|---|
| `index.html` | App JEJAK JSS (fail yang sama dengan `Index` dalam Apps Script). |
| `thumb.jpg` | Gambar pratonton apabila pautan dikongsi di WhatsApp. |

## Bila kod dikemas kini

1. Dalam Apps Script: tampal `Code.gs` dan `Index` baharu → Ctrl+S → **Deploy → Manage deployments → pensel → New version → Deploy**.
2. Di sini: buka `index.html` → ikon pensel → padam semua → tampal `Index.html` baharu.
3. **Tampal semula link web app** pada baris ini di bahagian atas fail, kemudian **Commit changes**:

   ```js
   var JEJAK_API = "https://script.google.com/macros/s/.../exec";
   ```

Tunggu kira-kira satu minit, kemudian muat semula app.

> Langkah 3 mudah terlupa. Jika app memaparkan "Link pelayan belum ditetapkan", baris itu belum diisi.

## Jika link web app bertukar

Berlaku hanya jika dibuat **New deployment** atau app dipindahkan ke akaun lain. Kemas kini
baris `JEJAK_API` dalam `index.html`. Pautan guru (`kmb-digital.github.io/jss`) kekal sama.

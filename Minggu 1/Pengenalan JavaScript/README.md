### 🧩 1. Cara Membuat dan Memanggil Fungsi di JavaScript

* Fungsi JavaScript biasanya didefinisikan di dalam tag `<script>`.
* Pemanggilan fungsi bisa dilakukan dari elemen HTML seperti tombol, menggunakan atribut seperti `onclick`.

#### Contoh:

```html
<body>
  <button onclick="demo()">Klik Saya</button>

  <script>
    function demo() {
      alert("Ini fungsi demo!");
    }
  </script>
</body>
```

---

### 📝 2. Tanda Kutip dalam JavaScript

#### 🔸 Kutip Tunggal `'...'` dan Kutip Ganda `"..."`

* Keduanya berfungsi **sama** untuk membuat string.
* Pemilihan biasanya tergantung gaya penulisan atau kebutuhan menyisipkan kutip di dalam string.

```javascript
let satu = 'Halo';
let dua = "Dunia";
```

#### 🔸 Backtick (`` `...` ``)

* Digunakan untuk **string multiline** (beberapa baris).
* Mendukung **interpolasi variabel** dengan `${}`.

```javascript
let nama = "Rafli";
let ucapan = `Halo,
Nama saya ${nama}`;
```

---

### 🔗 3. Perbedaan `href` dan `src` dalam HTML

| Atribut | Fungsi                                                            |
| ------- | ----------------------------------------------------------------- |
| `href`  | Digunakan untuk **tautan/link** ke halaman lain atau file         |
| `src`   | Digunakan untuk **menyisipkan konten** seperti gambar, JS, iframe |

#### Contoh:

```html
<!-- href untuk link -->
<a href="https://example.com">Kunjungi Website</a>

<!-- src untuk menyisipkan konten -->
<img src="foto.jpg" alt="Foto">
<script src="app.js"></script>
```

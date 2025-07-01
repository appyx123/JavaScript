### 🧾 1. Tipe Data yang Sering Digunakan

| Tipe Data   | Deskripsi                        | Contoh            |
| ----------- | -------------------------------- | ----------------- |
| `string`    | Teks atau karakter               | `'halo'`, "rafli" |
| `number`    | Angka (bulat atau desimal)       | `10`, `3.14`      |
| `boolean`   | Nilai logika: benar atau salah   | `true`, `false`   |
| `undefined` | Variabel yang belum diberi nilai | `let a;`          |

#### Contoh Penggunaan:

```javascript
let nama = "rafli";        // string
let umur = 20;             // number
let aktif = true;          // boolean
let alamat;                // undefined
```

---

### 🔍 2. Mengecek Tipe Data dengan `typeof`

JavaScript menyediakan operator `typeof` untuk mengetahui jenis data dari sebuah variabel.

#### Contoh:

```javascript
let nama = "rafli";
console.log(typeof nama); // Output: "string"

let umur = 20;
console.log(typeof umur); // Output: "number"

let aktif = true;
console.log(typeof aktif); // Output: "boolean"

let alamat;
console.log(typeof alamat); // Output: "undefined"
```

---

### 🧠 3. Memahami Konsep Variabel dan Data

```javascript
let nama = "rafli";
```

* `nama` → adalah **variabel**
* `"rafli"` → adalah **data** (tipe: string)

Variabel berfungsi sebagai wadah untuk menyimpan data. Data itulah yang diproses selama program dijalankan.


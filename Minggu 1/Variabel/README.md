#### 🔸 `let`

* Dapat **diubah nilainya** setelah dideklarasikan.
* **Memiliki block scope**, artinya hanya berlaku di dalam `{}` tempat dia dideklarasikan.
* Tidak akan tersimpan di global object (`window` di browser) jika dibuat di luar fungsi.

```javascript
let nama = "Rafli";
nama = "Budi"; // bisa diubah
```

---

#### 🔸 `const`

* Bersifat **konstan**, **tidak bisa di-reassign** nilainya setelah dideklarasikan.
* Memiliki **block scope** seperti `let`.
* Wajib diinisialisasi saat deklarasi.

```javascript
const pi = 3.14;
pi = 3.14159; // ❌ Error: Assignment to constant variable
```

> ⚠️ Note: Jika `const` digunakan untuk objek atau array, nilai di dalamnya masih bisa diubah (mutasi), tapi tidak bisa di-reassign.

```javascript
const user = { nama: "Rafli" };
user.nama = "Budi"; // ✅ boleh
user = {}; // ❌ Error
```

---

#### 🔸 `var`

* Bisa **diubah nilainya**.
* Bersifat **function scope** (bukan block scope).
* Jika dideklarasikan di luar fungsi, akan menjadi bagian dari **global object** (`window` di browser).
* Bisa menyebabkan hoisting (naik ke atas sebelum eksekusi).

```javascript
var usia = 20;
usia = 25; // ✅ bisa diubah
```

---

#### 🔸 Scope

* **Scope** adalah wilayah akses variabel, biasanya ditandai dengan `{}` (kurung kurawal).
* `let` dan `const` hanya hidup di dalam block scope tempat mereka dibuat.
* `var` bisa diakses di seluruh function scope, bahkan di luar block `{}`.

```javascript
{
  let a = 1;
  var b = 2;
}
console.log(a); // ❌ Error: a is not defined
console.log(b); // ✅ Output: 2
```

---

#### 🔸 Tanpa Kata Kunci (`var`, `let`, `const`)

* Jika kamu mendeklarasikan variabel tanpa kata kunci, maka secara default akan dianggap sebagai `var` dan disimpan di global object (tidak direkomendasikan!).

```javascript
function tes() {
  nama = "Rafli"; // ❌ Tidak disarankan!
}
tes();
console.log(nama); // ✅ Tapi bisa diakses (global)
```

---

#### 🔸 `console.log()`

* Digunakan untuk menampilkan output ke konsol browser.
* Bisa membantu proses debugging dan melihat nilai variabel saat menjalankan kode.

```javascript
let angka = 10;
console.log(angka); // Output: 10
```

---

#### 📌 Ringkasan Perbandingan

| Fitur          | `var`          | `let`       | `const`     |
| -------------- | -------------- | ----------- | ----------- |
| Dapat diubah   | ✅              | ✅           | ❌           |
| Hoisting       | ✅              | ❌           | ❌           |
| Scope          | Function Scope | Block Scope | Block Scope |
| Global Binding | ✅              | ❌           | ❌           |

---

Semoga catatan ini membantumu memahami variabel di JavaScript dengan lebih baik! 💡

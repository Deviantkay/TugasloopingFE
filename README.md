# Tugas Looping JS Dasar Skivul #Tech4Impact Batch 4 Learning Path Front-End

Looping adalah sebuah konsep pemrograman yang digunakan untuk melakukan perulangan atau pengulangan suatu blok kode program dalam program komputer. Dalam looping, program akan mengeksekusi serangkaian perintah secara berulang-ulang sampai suatu kondisi terpenuhi atau sampai batasan waktu tertentu tercapai.

---

## Beberapa Soal yang tersedia

:heavy_check_mark: Apa perbedaan dari procedural, conditional, dan looping?\
:heavy_check_mark: Kapan harus menggunakan looping?\
:heavy_check_mark: Sebutkan 3 looping yang dapat digunakan dan fungsi masing-masing looping\

### perbedaan dari procedural, conditional, dan looping

1. Procedural\
   Procedural adalah salah satu konsep dasar dalam pemrograman, di mana program diatur dalam urutan prosedur atau fungsi yang terstruktur. Prosedur atau fungsi akan dipanggil oleh program utama ketika dibutuhkan untuk menjalankan tugas tertentu. Ini memungkinkan program untuk diorganisir secara terstruktur dan mudah dikelola. Dalam JavaScript, prosedur atau fungsi dapat didefinisikan menggunakan kata kunci `function`. Prosedur ini dapat dipanggil di dalam program utama ketika dibutuhkan untuk menjalankan tugas tertentu.

```
// Fungsi untuk menghitung luas persegi panjang
function hitungLuasPersegipanjang(panjang, lebar) {
  var luas = panjang * lebar;
  return luas;
}

// Program utama
panjang = 5
lebar = 12
var luas = hitungLuasPersegipanjang(panjang, lebar);
console.log("Luas persegi dengan panjang", panjang, "dan lebar ", lebar, "adalah", luas);
```

2. Conditional\
   Conditional adalah konsep dalam pemrograman yang memungkinkan program untuk melakukan percabangan, atau memilih tindakan yang sesuai berdasarkan kondisi yang diberikan. Ini memungkinkan program untuk mengambil keputusan yang berbeda berdasarkan kondisi tertentu. Dalam JavaScript, percabangan dapat dilakukan menggunakan kata kunci `if`, `else if`, dan `else` ataupun penggunaan `switch` yang lebih mudah dibaca dan lebih ringkas daripada penggunaan beberapa `if statements` bersarang. Ini memungkinkan program untuk memilih tindakan yang sesuai berdasarkan kondisi yang diberikan.

- If Else Example

```
// Program untuk menentukan bilangan positif, negatif, atau nol
var angka = parseFloat(prompt("Masukkan bilangan: "));

if (angka > 0) {
  console.log(angka + " adalah bilangan positif");
} else if (angka === 0) {
  console.log(angka + " adalah nol");
} else {
  console.log(angka + " adalah bilangan negatif");
}
```

- Switch Example

```
let nilai = 80;

switch (true) {
  case nilai >= 90:
    console.log("Nilai Anda A");
    break;
  case nilai >= 80:
    console.log("Nilai Anda B");
    break;
  case nilai >= 70:
    console.log("Nilai Anda C");
    break;
  case nilai >= 60:
    console.log("Nilai Anda D");
    break;
  default:
    console.log("Anda Tidak Lulus");
}
```

3. Looping\
   Looping adalah konsep dalam pemrograman yang memungkinkan program untuk melakukan perulangan tugas tertentu berulang kali sampai suatu kondisi terpenuhi atau sampai batasan waktu tertentu tercapai. Dalam JavaScript, looping dapat dilakukan menggunakan kata kunci `for`, `while`, dan `do-while`. Ini memungkinkan program untuk melakukan perulangan tugas tertentu berulang kali sampai suatu kondisi terpenuhi atau sampai batasan waktu tertentu tercapai.

```
// Program untuk mencetak bilangan genap dari 1 hingga 10
for (let i = 1; i <= 10; i++) {
  if (i % 2 == 0) {
    console.log(i, "adalah bilangan genap");
  }
}
```

### Waktu Penggunaan looping terjadi

Looping digunakan ketika kita ingin menjalankan sebuah blok kode secara berulang-ulang hingga kondisi yang telah ditentukan tercapai. Looping sangat berguna dalam melakukan pengolahan data dan pengolahan perulangan.

Beberapa contoh kasus yang memerlukan penggunaan looping antara lain:

- Ketika kita ingin mengakses atau memanipulasi setiap elemen dalam sebuah array atau objek.
- Ketika kita ingin melakukan tugas yang sama pada setiap elemen atau setiap data dalam kumpulan data.
- Ketika kita ingin melakukan iterasi sejumlah tertentu, seperti saat mencetak angka dari 1 hingga 100.
- Ketika kita ingin melakukan iterasi sampai suatu kondisi terpenuhi, seperti saat mencari nilai tertentu dalam kumpulan data.

Pada dasarnya, penggunaan looping akan memudahkan kita dalam mengeksekusi kode secara otomatis dan efisien. Namun, perlu diingat bahwa penggunaan looping yang tidak bijak atau tidak efisien dapat memperlambat kinerja program kita, terutama jika data yang diolah sangat besar. Oleh karena itu, sebaiknya kita memperhatikan dan memastikan bahwa penggunaan looping pada program kita benar dan efisien.

### 3 Jenis looping

1. `for` loop\
   `for` loop adalah jenis perulangan paling umum yang digunakan dalam bahasa pemrograman JavaScript. Fungsinya adalah untuk melakukan perulangan berdasarkan kondisi yang telah ditentukan, misalnya melakukan perulangan sebanyak n kali atau sebanyak elemen yang ada pada sebuah array. Contoh penggunaannya adalah sebagai berikut:

```
for (let i = 0; i < 10; i++) {
  console.log(i);
}
```

Kode di atas akan mengeksekusi blok kode di dalamnya sebanyak 10 kali, dimulai dari nilai i sama dengan 0, kemudian setiap kali perulangan dilakukan, nilai i akan ditambah 1 hingga mencapai nilai kurang dari 10.

2. `while` loop\
   `while` loop digunakan untuk melakukan perulangan selama kondisi yang telah ditentukan masih terpenuhi atau benar. Fungsinya adalah untuk melakukan perulangan terus-menerus sampai kondisi berhenti tercapai. Contoh penggunaannya adalah sebagai berikut:

```
let i = 0;
while (i < 10) {
  console.log(i);
  i++;
}
```

3. `do-while` loop\
   `do-while` loop hampir sama dengan `while` loop, namun bedanya `do-while` loop akan melakukan perulangan minimal satu kali meskipun kondisi yang ditentukan tidak terpenuhi. Fungsinya adalah untuk melakukan perulangan minimal satu kali, kemudian melakukan pengecekan kondisi dan mengulang jika kondisi masih terpenuhi. Contoh penggunaannya adalah sebagai berikut:

```
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 10);
```

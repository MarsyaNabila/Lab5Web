# Lab5Web - Javascript

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI.24.A4

# Langkah ke 1 Pengenalan Javascript

Membuat dokumen HTML dengan nama file lab5_javascript.html

Kode HTML di atas berfungsi untuk memperkenalkan dasar penggunaan **JavaScript** di dalam halaman web. Pada bagian `<head>`, terdapat elemen `<title>` yang menentukan judul halaman yaitu “Mengenal JavaScript”. Lalu di dalam `<body>`, terdapat judul utama `<h1>` yang bertuliskan “Pengenalan JavaScript” dan subjudul `<h3>` yang menjelaskan bahwa contoh yang ditampilkan adalah penggunaan **document.write** dan **console.log**.

Bagian penting dari kode ini adalah elemen `<script>`, yang digunakan untuk menulis perintah JavaScript. Di dalamnya terdapat dua baris kode:

* `document.write("Hello World");` digunakan untuk menampilkan teks *“Hello World”* langsung pada halaman web.
* `console.log("Hello World");` digunakan untuk menampilkan teks yang sama di **konsol browser**, biasanya terlihat melalui fitur *Inspect Element - Console*.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>
</body>
</html>
```

<img width="948" height="538" alt="Screenshot 2025-10-23 213434" src="https://github.com/user-attachments/assets/3bcdea43-789e-4ecf-a914-119bf9351991" />

# Langkah ke 2 Javascript Dasar

Berikut penjelasan dari kode pada gambar tersebut:

Kode HTML ini digunakan untuk memperkenalkan dasar-dasar **JavaScript** dengan beberapa contoh fungsinya. Pada bagian `<head>`, terdapat elemen `<meta charset="UTF-8">` untuk mendukung karakter UTF-8, dan `<title>` yang memberikan judul halaman “JavaScript Dasar”.

Bagian utama program berada di dalam elemen `<script>`, yang berisi beberapa contoh penggunaan JavaScript:

* **Pemakaian Alert**
   Baris `alert("Halo! Ini contoh penggunaan alert di JavaScript.");` menampilkan jendela pop-up (kotak peringatan) di browser yang berisi pesan teks. Fungsi ini berguna untuk memberi informasi singkat kepada pengguna.
* **Pemakaian Prompt**
   Baris `let nama = prompt("Siapa namamu?");` akan menampilkan kotak dialog yang meminta pengguna untuk memasukkan nama. Hasil input pengguna disimpan dalam variabel `nama`.
   Setelah itu, `document.write("Halo, " + nama + "!<br>");` menampilkan sapaan langsung pada halaman web sesuai dengan nama yang dimasukkan.
* **Membuat Fungsi**
   Kode `function salam(nama) { return "Selamat datang, " + nama + "!"; }` mendefinisikan sebuah fungsi bernama `salam` yang menerima satu parameter, yaitu `nama`. Fungsi ini mengembalikan (return) kalimat sapaan yang disesuaikan dengan nama pengguna.
* **Memanggil Fungsi**
   Baris `let hasil = salam(nama);` memanggil fungsi `salam()` dengan memasukkan nilai dari variabel `nama`. Hasil dari fungsi tersebut disimpan dalam variabel `hasil`.
   Lalu `document.write(hasil);` digunakan untuk menampilkan hasil sapaan “Selamat datang, [nama]!” di halaman web.





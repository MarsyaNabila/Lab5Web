# Lab5Web - Javascript

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI.24.A4

# Langkah ke 1 Pengenalan Javascript

Membuat dokumen HTML dengan nama file lab5_javascript.html

Kode HTML di atas berfungsi untuk memperkenalkan dasar penggunaan **JavaScript** di dalam halaman web. Pada bagian `<head>`, terdapat elemen `<title>` yang menentukan judul halaman yaitu “Mengenal JavaScript”. Lalu di dalam `<body>`, terdapat judul utama `<h1>` yang bertuliskan “Pengenalan JavaScript” dan subjudul `<h3>` yang menjelaskan bahwa contoh yang ditampilkan adalah penggunaan **document.write** dan **console.log**.

Bagian penting dari kode ini adalah elemen `<script>`, yang digunakan untuk menulis perintah JavaScript. Di dalamnya terdapat dua baris kode:

* `document.write("Hello World");` digunakan untuk menampilkan teks “Hello World” langsung pada halaman web.
* `console.log("Hello World");` digunakan untuk menampilkan teks yang sama di **konsol browser**, biasanya terlihat melalui fitur Inspect Element - Consol*.

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


  ```html
    <script>
        // Pemakaian Alert
        alert("Halo! Ini contoh penggunaan alert di JavaScript.");

        // Pemakaian Prompt
        let nama = prompt("Siapa namamu?");
        document.write("Halo, " + nama + "!<br>");

        // Membuat fungsi
        function salam(nama) {
            return "Selamat datang, " + nama + "!";
        }

        // Memanggil fungsi
        let hasil = salam(nama);
        document.write(hasil);
    </script>
</body>
</html>

<img width="933" height="1006" alt="Screenshot 2025-10-23 215637" src="https://github.com/user-attachments/assets/19b590ce-eef8-4664-90bc-97d50df9ce8c" />


<img width="938" height="473" alt="Screenshot 2025-10-23 215701" src="https://github.com/user-attachments/assets/a7745c0b-5b97-4292-88f9-4edc02c7ece4" />

# Langkah ke 3 Pemrograman Dasar di Javascript

Kode HTML ini berisi contoh dasar **pemrograman JavaScript**, meliputi operasi aritmatika, percabangan `if...else`, dan `switch`.
* **Operasi Aritmatika**
   Dua variabel didefinisikan: `a = 10` dan `b = 5`.
   Bagian ini menampilkan hasil dari berbagai operasi matematika seperti penjumlahan (`a + b`), pengurangan (`a - b`), perkalian (`a * b`), pembagian (`a / b`), dan sisa bagi (`a % b`) ke halaman web menggunakan `document.write()`.
* **Seleksi Kondisi if...else**
   Program meminta pengguna memasukkan nilai ujian melalui `prompt()`.
   Jika nilai lebih besar atau sama dengan 75, muncul pesan “Selamat, kamu lulus”.
   Jika kurang dari itu, tampil pesan “Maaf, kamu belum lulus”.
   Ini menunjukkan cara penggunaan percabangan sederhana dalam JavaScript.
* **Operator Switch**
   Pengguna diminta memasukkan grade (A, B, C, atau D).
   Berdasarkan input tersebut, program menampilkan pesan berbeda menggunakan `switch`.
   Misalnya, jika pengguna memasukkan “A”, maka tampil pesan “Nilai kamu sangat baik!”.
   Jika input tidak sesuai, program menampilkan “Grade tidak valid!”.

  ```html
    <script>
        // --- Operasi Aritmatika ---
        let a = 10;
        let b = 5;

        document.write("<h3>Operasi Aritmatika</h3>");
        document.write("a = " + a + ", b = " + b + "<br>");
        document.write("Penjumlahan (a + b) = " + (a + b) + "<br>");
        document.write("Pengurangan (a - b) = " + (a - b) + "<br>");
        document.write("Perkalian (a * b) = " + (a * b) + "<br>");
        document.write("Pembagian (a / b) = " + (a / b) + "<br>");
        document.write("Sisa bagi (a % b) = " + (a % b) + "<br><br>");

        // --- Seleksi Kondisi if..else ---
        document.write("<h3>Seleksi Kondisi if..else</h3>");
        let nilai = prompt("Masukkan nilai ujianmu:");
        if (nilai >= 75) {
            document.write("Selamat, kamu lulus!<br>");
        } else {
            document.write("Maaf, kamu belum lulus.<br>");
        }

        // --- Operator Switch ---
        document.write("<h3>Seleksi Kondisi switch</h3>");
        let grade = prompt("Masukkan grade (A/B/C/D):");
        switch (grade) {
            case "A":
                document.write("Nilai kamu sangat baik!<br>");
                break;
            case "B":
                document.write("Nilai kamu baik.<br>");
                break;
            case "C":
                document.write("Nilai kamu cukup.<br>");
                break;
            case "D":
                document.write("Nilai kamu kurang.<br>");
                break;
            default:
                document.write("Grade tidak valid!<br>");
        }
    </script>
</body>
</html>    




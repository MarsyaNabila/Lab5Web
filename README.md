# Lab5Web - Pratikum Javascript

Nama: Marsya Nabila Putri

NIM: 312410338

Kelas: TI.24.A4

# Langkah ke 1 Pengenalan Javascript

Membuat dokumen HTML dengan nama file `lab5_javascript.html`

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

Kode HTML di atas berfungsi untuk memperkenalkan dasar penggunaan **JavaScript** di dalam halaman web. Pada bagian `<head>`, terdapat elemen `<title>` yang menentukan judul halaman yaitu “Mengenal JavaScript”. Lalu di dalam `<body>`, terdapat judul utama `<h1>` yang bertuliskan “Pengenalan JavaScript” dan subjudul `<h3>` yang menjelaskan bahwa contoh yang ditampilkan adalah penggunaan **document.write** dan **console.log**.

Bagian penting dari kode ini adalah elemen `<script>`, yang digunakan untuk menulis perintah JavaScript. Di dalamnya terdapat dua baris kode:

* `document.write("Hello World");` digunakan untuk menampilkan teks “Hello World” langsung pada halaman web.
* `console.log("Hello World");` digunakan untuk menampilkan teks yang sama di **konsol browser**, biasanya terlihat melalui fitur Inspect Element - Consol*.

Hasil di browser: 

<img width="948" height="538" alt="Screenshot 2025-10-23 213434" src="https://github.com/user-attachments/assets/3bcdea43-789e-4ecf-a914-119bf9351991" />

# Langkah ke 2 Javascript Dasar
Membuat File baru HTML dengan nama `dasar_javascript.html`

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
```


Kode HTML ini digunakan untuk memperkenalkan dasar-dasar **JavaScript** dengan beberapa contoh fungsinya. Pada bagian `<head>`, terdapat elemen `<meta charset="UTF-8">` untuk mendukung karakter UTF-8, dan `<title>` yang memberikan judul halaman “JavaScript Dasar”. Bagian utama program berada di dalam elemen `<script>`, yang berisi beberapa contoh penggunaan JavaScript:

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


Hasil di browser: 

<img width="933" height="1006" alt="Screenshot 2025-10-23 215637" src="https://github.com/user-attachments/assets/19b590ce-eef8-4664-90bc-97d50df9ce8c" />


<img width="938" height="473" alt="Screenshot 2025-10-23 215701" src="https://github.com/user-attachments/assets/a7745c0b-5b97-4292-88f9-4edc02c7ece4" />

# Langkah ke 3 Pemrograman Dasar di Javascript
Membuat File baru HTML dengan nama `dasar_pemrograman.html`

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
```

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


Hasil di browser: 

<img width="935" height="957" alt="Screenshot 2025-10-23 220829" src="https://github.com/user-attachments/assets/350d6ffb-6752-47b8-84e9-6118b4912f16" />

<img width="942" height="927" alt="Screenshot 2025-10-23 220854" src="https://github.com/user-attachments/assets/e8705ac9-6f6f-499c-a043-6687ea36cde4" />

<img width="935" height="951" alt="Screenshot 2025-10-23 220913" src="https://github.com/user-attachments/assets/8ab23ff1-073f-4a00-8f29-68d4dfed353b" />

# Langkah ke 4 Pembuatan Formulir dan Tombol
Membuat File baru HTML dengan nama `from_button.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Pembuatan Form dan Button</title>
    <script>
        // Fungsi untuk menampilkan hasil input
        function tampilkanNama() {
            let nama = document.getElementById("nama").value;
            document.getElementById("hasil").innerHTML = "Halo, " + nama + "!";
        }
    </script>
</head>
<body>
    <h2>Form Input dan Button</h2>

    <!-- Form Input -->
    <form>
        <label for="nama">Nama:</label>
        <input type="text" id="nama" placeholder="Masukkan nama kamu">
        <button type="button" onclick="tampilkanNama()">Tampilkan</button>
    </form>

    <!-- Hasil tampil di sini -->
    <p id="hasil"></p>
</body>
</html>
```

Kode HTML ini menunjukkan cara membuat **form input dan tombol (button)** yang terhubung dengan **fungsi JavaScript** untuk menampilkan hasil dari input pengguna.
1. **Bagian JavaScript (dalam tag `<script>`)**
   Fungsi `tampilkanNama()` digunakan untuk mengambil nilai dari input teks.

   * Baris `let nama = document.getElementById("nama").value;` mengambil teks yang dimasukkan pengguna di kotak input dengan id `"nama"`.
   * Lalu, `document.getElementById("hasil").innerHTML = "Halo, " + nama + "!";` menampilkan pesan sapaan pada elemen dengan id `"hasil"`.

2. **Bagian Form HTML**
   Di dalam tag `<form>`, terdapat label dan input teks untuk mengisi nama.
   Tombol `<button>` memiliki atribut `onclick="tampilkanNama()"`, yang berarti ketika tombol diklik, fungsi JavaScript tersebut dijalankan.

3. **Menampilkan Hasil**
   Hasil output akan muncul di paragraf `<p id="hasil"></p>` setelah pengguna menekan tombol.

Hasil di browser:  

<img width="939" height="565" alt="Screenshot 2025-10-23 221640" src="https://github.com/user-attachments/assets/bf3c5e5f-a1f7-45ae-9312-5ccb3583e3cb" />

<img width="930" height="493" alt="Screenshot 2025-10-23 221703" src="https://github.com/user-attachments/assets/7497ccd6-6417-4bd6-979e-fbeb5e335d3e" />

# Langkah ke 5 HTML DOM (Kotak Ceklis Otomatis)
Membuat File baru HTML dengan nama `checbox_total.html`


```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Perhitungan Otomatis dengan Checkbox</title>
    <script>
        function hitungTotal() {
            let total = 0;

            // Ambil semua checkbox
            let item1 = document.getElementById("item1");
            let item2 = document.getElementById("item2");
            let item3 = document.getElementById("item3");

            // Cek apakah dipilih
            if (item1.checked) total += parseInt(item1.value);
            if (item2.checked) total += parseInt(item2.value);
            if (item3.checked) total += parseInt(item3.value);

            // Tampilkan hasil
            document.getElementById("total").innerHTML = "Total harga: Rp " + total.toLocaleString();
        }
    </script>
</head>
<body>
    <h2>Perhitungan Otomatis (Checkbox)</h2>

    <form>
        <input type="checkbox" id="item1" value="10000" onclick="hitungTotal()"> Ayam Bakar (Rp 15.000)<br>
        <input type="checkbox" id="item2" value="8000" onclick="hitungTotal()"> Bakso (Rp 10.000)<br>
        <input type="checkbox" id="item3" value="12000" onclick="hitungTotal()"> Ketoprak (Rp 13.000)<br><br>
    </form>

    <p id="total">Total harga: Rp 0</p>
</body>
</html>
```

Kode HTML ini berfungsi untuk menghitung **total harga secara otomatis** berdasarkan **checkbox** yang dipilih oleh pengguna menggunakan **JavaScript**.

1. **Bagian JavaScript (fungsi `hitungTotal()`)**

   * Variabel `total` diset ke 0 sebagai nilai awal.
   * Tiga elemen checkbox diambil menggunakan `document.getElementById()` dengan id `item1`, `item2`, dan `item3`.
   * Setiap checkbox memiliki nilai harga masing-masing (Rp 15.000, Rp `10.000, dan Rp 13.000).
   * Jika checkbox dipilih (`checked`), maka nilainya ditambahkan ke total menggunakan `parseInt()` untuk mengubah nilai teks menjadi angka.
   * Hasil akhirnya ditampilkan pada elemen dengan id `"total"` menggunakan `innerHTML`, dan `toLocaleString()` digunakan agar angka tampil dengan format ribuan.

2. **Bagian Form HTML**

   * Terdapat tiga checkbox yang mewakili menu makanan: Ayam Bakar, Bakso, dan Ketoprak.
   * Setiap checkbox memiliki event `onclick="hitungTotal()"`, sehingga saat pengguna mencentang atau menghapus centang, total harga otomatis diperbarui.

3. **Menampilkan Hasil Total**

   * Elemen `<p id="total">` digunakan untuk menampilkan total harga akhir di halaman, yang akan berubah sesuai pilihan pengguna.

     
Hasil di browser:  

<img width="931" height="642" alt="Screenshot 2025-10-23 222922" src="https://github.com/user-attachments/assets/bdc04c52-ab2f-42c4-91aa-11165f395bb4" />

<img width="936" height="626" alt="Screenshot 2025-10-23 222944" src="https://github.com/user-attachments/assets/821e2f75-5a6b-45b2-a62b-fbec0acd69b8" />

# Pertanyaan dan Tugas

<img width="718" height="111" alt="Screenshot 2025-10-23 223942" src="https://github.com/user-attachments/assets/0be75bd4-017c-453f-bf62-510ff7692e81" />

# 1. Buat script untuk melakukan validasi pada isian form.
  
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Validasi Form</title>
    <script>
        function validasiForm() {
            let nama = document.getElementById("nama").value;
            let email = document.getElementById("email").value;
            let password = document.getElementById("password").value;

            // Mengecek apakah kolom kosong
            if (nama == "" || email == "" || password == "") {
                alert("Semua kolom harus diisi!");
                return false;
            }

            // Validasi format email
            let polaEmail = /^[^ ]+@[^ ]+\.[a-z]{2,3}$/;
            if (!email.match(polaEmail)) {
                alert("Format email tidak valid!");
                return false;
            }

            // Validasi panjang password
            if (password.length < 6) {
                alert("Password harus minimal 6 karakter!");
                return false;
            }

            alert("Form berhasil dikirim!");
            return true;
        }
    </script>
</head>
<body>
    <h2>Form Registrasi (Validasi dengan JavaScript)</h2>

    <form onsubmit="return validasiForm()">
        <label for="nama">Nama:</label><br>
        <input type="text" id="nama" placeholder="Masukkan nama kamu"><br><br>

        <label for="email">Email:</label><br>
        <input type="text" id="email" placeholder="contoh@email.com"><br><br>

        <label for="password">Password:</label><br>
        <input type="password" id="password" placeholder="Minimal 6 karakter"><br><br>

        <input type="submit" value="Kirim">
    </form>
</body>
</html>
```

Kode ini digunakan untuk membuat **form registrasi** dengan **validasi menggunakan JavaScript**, agar data yang dikirimkan oleh pengguna sesuai dengan aturan yang ditentukan.

1. **Bagian Fungsi JavaScript (`validasiForm()`)**

   * Pertama, program mengambil nilai dari input `nama`, `email`, dan `password` menggunakan `document.getElementById().value`.
   * Lalu dilakukan tiga jenis pemeriksaan (validasi):

   * **Cek kolom kosong:** Jika ada kolom yang belum diisi, akan muncul pesan “Semua kolom harus diisi!”.
   * **Cek format email:** Menggunakan pola regex (`polaEmail`) untuk memastikan email memiliki format yang benar, misalnya “[nama@domain.com](mailto:nama@domain.com)”. Jika salah, muncul pesan “Format email tidak valid!”.
   * **Cek panjang password:** Jika password kurang dari 6 karakter, tampil pesan “Password harus minimal 6 karakter!”.
   * Jika semua validasi lolos, muncul pesan “Form berhasil dikirim!” dan form akan dikirimkan.

2. **Bagian Form HTML**

   * Form memiliki tiga input: `Nama`, `Email`, dan `Password`.
   * Atribut `onsubmit="return validasiForm()"` memastikan fungsi validasi dijalankan sebelum form dikirim. Jika ada kesalahan, form tidak akan dikirim.
   * Tombol “Kirim” digunakan untuk mengirim form setelah semua data valid.

Hasil di browser: 

<img width="934" height="804" alt="Screenshot 2025-10-23 223638" src="https://github.com/user-attachments/assets/71fc6b86-4e4d-4f2c-a1db-e60cb93743e2" />

<img width="932" height="641" alt="Screenshot 2025-10-23 223751" src="https://github.com/user-attachments/assets/17ede262-b812-49f7-92cc-10cbdd417fd1" />

<img width="931" height="826" alt="Screenshot 2025-10-23 223803" src="https://github.com/user-attachments/assets/c65ca710-2559-4ac0-8a88-32a32c0f6a66" />













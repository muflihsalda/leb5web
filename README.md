# leb5web
<p>Mata Kuliah:Pemrograman Web</p>
<p>Nama  :Muflih Salda Maulana</p>
<p>Nim    :312410527</p>
<p>Kelas  :TI.24.A5</p>

---

## 1. lab5_javascript.html

File utama pengenalan JavaScript.
Menampilkan teks **Hello World** menggunakan `document.write()` dan `console.log()`.
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
**Hasil:** Teks *Hello World* muncul di halaman dan di console browser.

<img width="660" height="364" alt="image" src="https://github.com/user-attachments/assets/84283e63-56c4-43e4-9b7b-61e4f6ce4d95" />

---

## 2. alert.html

Menampilkan pesan pop-up menggunakan fungsi `alert()`.
**Kode utama:**

```javascript
alert("Javascript pada tag head.");
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Alert Box</title>
  </head>
  <body>
    <script>
      alert("Ini merupakan pesan untuk Anda");
    </script>
  </body>
</html>
```

**Hasil:** Muncul kotak dialog dengan pesan “Javascript pada tag head.”
<img width="680" height="397" alt="image" src="https://github.com/user-attachments/assets/8a18a590-98e9-46b7-9af8-f456d5475c7d" />

---

## 3. method.html

Menampilkan teks ke halaman menggunakan `document.write()` sebagai contoh method dari objek `document`.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Pengenalan JavaScript</title>
  </head>
  <body>
    percobaan mamakai JavaScript:<br />
    <script>
      document.write("selamat mencoba javascript<br>");
      document.write("semoga sukses!");
    </script>
  </body>
</html>

```

**Hasil:** Teks tersebut tampil langsung di halaman browser.
<img width="671" height="228" alt="image" src="https://github.com/user-attachments/assets/5b9795b4-43fe-4ffc-910d-2859c2d9be8c" />


---

## 4. prompt.html

Mengambil input dari pengguna menggunakan `prompt()` dan menampilkannya kembali di halaman.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Prompt Input</title>
  </head>
  <body>
    <script>
      var nama = prompt("Siapa nama Anda?", "Masukkan nama Anda");
      document.write("Hai, " + nama);
    </script>
  </body>
</html>

```

**Hasil:** Pengguna diminta memasukkan nama, lalu muncul tulisan “Hai, [nama].”
<img width="674" height="312" alt="image" src="https://github.com/user-attachments/assets/f1a390bb-7488-46d9-ba8f-711399f25dc8" />

---

## 5. fungsi_onload.html

Menunjukkan cara membuat fungsi dan memanggilnya dengan event.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Fungsi onload</title>
    <script>
      function pesan() {
        alert("Memanggil JavaScript lewat body onload");
      }
    </script>
  </head>
  <body onload="pesan()"></body>
</html>

```

**Hasil:** Saat tombol diklik, muncul alert dengan pesan “Memanggil JavaScript lewat fungsi.”
<img width="676" height="330" alt="image" src="https://github.com/user-attachments/assets/e41c0723-cfd4-4dd7-83aa-693df1340274" />

---

## 6. aritmatika.html

Menunjukkan operasi aritmatika sederhana di JavaScript.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Operasi Aritmatika</title>
    <script>
      function hitung(val1, val2) {
        document.write("Perkalian: " + val1 * val2 + "<br>");
        document.write("Pembagian: " + val1 / val2 + "<br>");
        document.write("Penjumlahan: " + (val1 + val2) + "<br>");
        document.write("Pengurangan: " + (val1 - val2) + "<br>");
        document.write("Modulus: " + (val1 % val2));
      }
    </script>
  </head>
  <body>
    <input type="button" value="Hitung" onclick="hitung(9, 4)" />
  </body>
</html>
```

**Hasil:** Menampilkan hasil penjumlahan di halaman: “Hasil penjumlahan a + b = 9”.
<img width="674" height="256" alt="image" src="https://github.com/user-attachments/assets/d146508d-b4f3-4a65-8521-9b6ccd4c6196" />

---

## 7. if_else.html

Menampilkan contoh seleksi kondisi menggunakan `if...else`.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Seleksi Kondisi</title>
  </head>
  <body>
    <script>
      var nilai = prompt("Nilai (0-100):", 0);
      var hasil = nilai >= 60 ? "Lulus" : "Tidak Lulus";
      document.write("Hasil: " + hasil);
    </script>
  </body>
</html>

```

**Hasil:** Tampil pesan “Lulus” atau “Tidak Lulus” tergantung nilai yang dimasukkan.
1. hasil memasukan nilai di bawah 60
<img width="678" height="313" alt="image" src="https://github.com/user-attachments/assets/b47c7db6-e1cf-460a-b0ef-1a43441b0667" />

2. hasil memasukan nilai dari 60 ke atas
<img width="673" height="175" alt="image" src="https://github.com/user-attachments/assets/255afbe5-d1dd-419d-adb6-83ccd3d679e2" />

---

## 8. switch.html

Menunjukkan contoh seleksi kondisi menggunakan `switch`.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Switch Case</title>
    <script>
      function test() {
        var val1 = prompt("Input nilai (1-5):");
        switch (val1) {
          case "1":
            document.write("Bilangan satu");
            break;
          case "2":
            document.write("Bilangan dua");
            break;
          case "3":
            document.write("Bilangan tiga");
            break;
          case "4":
            document.write("Bilangan empat");
            break;
          case "5":
            document.write("Bilangan lima");
            break;
          default:
            document.write("Bilangan lainnya");
        }
      }
    </script>
  </head>
  <body>
    <input type="button" value="Switch" onclick="test()" />
  </body>
</html>

```

**Hasil:** Menampilkan keterangan sesuai nilai yang diinput.
hasil yang di input dari nilai 4
<img width="683" height="105" alt="image" src="https://github.com/user-attachments/assets/cc0e100c-e5fd-4261-b3e1-edfb8694e0df" />

---

## 9. form_buttonwarna.html

Mendemonstrasikan penggunaan tombol untuk mengubah warna elemen.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Form Button Warna</title>
    <script>
      function ubahWarnaBG(warna) {
        document.bgColor = warna;
      }

      function ubahWarnaTeks(warna) {
        document.fgColor = warna;
      }
    </script>
  </head>
  <body>
    <h1>Tes Ubah Warna</h1>
    <form>
      <input
        type="button"
        value="Latar Belakang Hijau"
        onclick="ubahWarnaBG('GREEN')"
      />
      <input
        type="button"
        value="Latar Belakang Putih"
        onclick="ubahWarnaBG('WHITE')"
      />
      <input
        type="button"
        value="Teks Kuning"
        onclick="ubahWarnaTeks('YELLOW')"
      />
      <input type="button" value="Teks Biru" onclick="ubahWarnaTeks('BLUE')" />
    </form>

    <script>
      document.write("Dimodifikasi terakhir pada: " + document.lastModified);
    </script>
  </body>
</html>

```

**Hasil:** Saat tombol diklik, warna background halaman berubah.
1. hasil dari latar tombol latar blakang hijau setelah di klik
<img width="677" height="344" alt="image" src="https://github.com/user-attachments/assets/8723f3f3-7c63-4efe-bfae-77de758223bd" />

2. hasil dari latar blakang putih setelah di klik
<img width="682" height="348" alt="image" src="https://github.com/user-attachments/assets/b8a86a4e-5366-42f0-a961-0f7790d3ab89" />

3. hasil dari tombol teks kuning setelah di klik

<img width="512" height="224" alt="image" src="https://github.com/user-attachments/assets/b0d38b34-4219-4e0d-9f91-da934350d3b7" />


4. hasil dari tombol teks biru setelah di klik
   <img width="682" height="348" alt="image" src="https://github.com/user-attachments/assets/ae03d3a9-5dd0-4016-8c65-d35513b7fd6a" />

---

## 10. form_genap_ganjil.html

Menentukan bilangan genap atau ganjil berdasarkan input pengguna.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Form Genap Ganjil</title>
    <script>
      function cekBilangan() {
        var val = document.kirim.T1.value;
        document.kirim.T2.value =
          val % 2 === 0 ? "Bilangan Genap" : "Bilangan Ganjil";
      }
    </script>
  </head>
  <body>
    <form name="kirim">
      <input type="text" name="T1" />
      <input type="text" name="T2" readonly />
      <input type="button" value="Tebak" onclick="cekBilangan()" />
    </form>
  </body>
</html>

```

**Hasil:** Menampilkan hasil “Angka Genap” atau “Angka Ganjil”.

<img width="677" height="216" alt="image" src="https://github.com/user-attachments/assets/4d383948-b077-481f-98a0-890f66647c2e" />

---

## 11. form_validasi.html

Kode ini digunakan untuk memvalidasi input nama sebelum form dikirim.
Jika kolom nama kosong, muncul pesan “Nama harus diisi!” dan form tidak dikirim.
Jika kolom sudah diisi, form akan dikirim dan halaman akan reload otomatis tanpa pesan tambahan.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Validasi Form</title>
    <script>
      function validateForm() {
        var nama = document.forms["myForm"]["nama"].value;
        if (nama === "") {
          alert("Nama harus diisi!");
          return false;
        }
      }
    </script>
  </head>
  <body>
    <form name="myForm" onsubmit="return validateForm()">
      Nama: <input type="text" name="nama" />
      <input type="submit" value="Submit" />
    </form>
  </body>
</html>

```

**Hasil:** Jika form kosong → muncul alert peringatan. Jika terisi → form berhasil dikirim.

berikut hasil jika form kosong
<img width="648" height="249" alt="image" src="https://github.com/user-attachments/assets/ce85fd17-141e-438f-b00a-3c59afc7baf9" />

---

## 12. checkbox_menu.html

Menggunakan checkbox untuk menghitung total harga secara otomatis.
**Kode utama:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Daftar Menu</title>
    <script>
      function hitung(ele) {
        var total = document.getElementById("total").value;
        total = total ? parseInt(total) : 0;
        var harga = parseInt(ele.value);
        total += ele.checked ? harga : -harga;
        document.getElementById("total").value = total;
      }
    </script>
  </head>
  <body>
    <h1>Daftar Menu Makanan</h1>
    <label
      ><input type="checkbox" value="5000" onclick="hitung(this)" /> Ayam Goreng
      Rp. 5.000</label
    ><br />
    <label
      ><input type="checkbox" value="500" onclick="hitung(this)" /> Tempe Goreng
      Rp. 500</label
    ><br />
    <label
      ><input type="checkbox" value="2500" onclick="hitung(this)" /> Telur Dadar
      Rp. 2.500</label
    ><br />
    <strong>Total Bayar: Rp. <input type="text" id="total" /></strong>
  </body>
</html>

```

**Hasil:** Saat item dicentang, total harga otomatis dijumlahkan di kolom total.
<img width="664" height="309" alt="image" src="https://github.com/user-attachments/assets/63bc5426-2063-4a58-ac1d-18267537067c" />

---



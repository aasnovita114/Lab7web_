# Lab7web_

<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Aas Novitasari</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210167</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A1</td>
  </tr>
</table>

# Instruksi Praktikum

1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama lab7_php_dasar pada docroot webserver (htdocs)
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.

# Langkah-langkah Praktikum

1. Install XAMPP Unduh XAMPP dari https://www.apachefriends.org/download.html dan pilih versi portable untuk memudahkan proses installasi. Kemudian extract file tersebut, seusikan direktorinya (misal: d:\xampp).

2. Memulai PHP Buat folder lab7_php_dasar pada root directory web server (d:\xampp\htdocs)

3. PHP Dasar Buat file baru dengan nama php_dasar.php pada directory tersebut. Kemudian buat kode seperti berikut.

   ```
   <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <title>PHP Dasar</title>
        </head>
        <body>
            <h1>Belajar PHP Dasar</h1>
            <?php
            echo "Hello World";
            ?>
        </body>
    </html>
   ```
   ![Screenshot 2023-11-24 144434](https://github.com/aasnovita114/Lab7web_/assets/116045324/afe679b8-dfd2-41ca-b1d4-cbd9d16cf578)

4. Variable PHP

```
    <?php
    $nim = "312210167";
    $nama = 'Aas Novitasari';
    echo "NIM : " . $nim . "<br>";
    echo "Nama : $nama";
    ?>
```
![Screenshot 2023-11-24 152941](https://github.com/aasnovita114/Lab7web_/assets/116045324/fb070b31-e3ed-4585-a248-45c29e3527dc)

5. Predefine Variable $_GET

```
    <?php
    echo 'Selamat Datang ' . $_GET['nama'];
    ?>
```
![Screenshot 2023-11-24 154024](https://github.com/aasnovita114/Lab7web_/assets/116045324/4e7bd6ed-c6c3-4661-9fd6-5643426fc290)

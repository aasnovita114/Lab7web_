# Lab7Web_

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

6. Membuat Form

```
    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <title>PHP Dasar</title>
        </head>
        <body>
            <h2>Form Input</h2>
            <form method="post">
                <label>Nama: </label>
                <input type="text" name="nama">
                <input type="submit" value="Kirim">
            </form>
            <?php
            echo 'Selamat Datang ' . $_POST['nama'];
            ?>
        </body>
    </html>
```
![Screenshot 2023-11-24 154800](https://github.com/aasnovita114/Lab7web_/assets/116045324/c1b770c7-11e7-4086-89e7-bee06dce658a)

7.Operator

```
    <?php
    $gaji = 1000000;
    $pajak = 0.1;
    $thp = $gaji - ($gaji*$pajak);
    echo "Gaji sebelum pajak = Rp. $gaji <br>";
    echo "Gaji yang dibawa pulang = Rp. $thp";
    ?>
```
![Screenshot 2023-11-24 155542](https://github.com/aasnovita114/Lab7web_/assets/116045324/576e2b9c-677b-4b7d-ba0f-1688bcf42fa8)

8.Kondisi IF

```
    <?php
    $nama_hari = date("l");
    if ($nama_hari == "Sunday") {
        echo "Minggu";
    } elseif ($nama_hari == "Monday") {
        echo "Senin";
    } else {
        echo "Selasa";
    }
    ?>
```
![Screenshot 2023-11-24 160135](https://github.com/aasnovita114/Lab7web_/assets/116045324/7a3350d6-7ce6-4334-aa49-8fb8bbb54fe5)

9.Kondisi Switch

```
    <?php
    $nama_hari = date("l");
    switch ($nama_hari) {
    case "Sunday":
        echo "Minggu";
        break;
    case "Monday":
        echo "Senin";
        break;
    case "Tuesday":
        echo "Selasa";
        break;
    default:
        echo "Sabtu";
    ?>
```
![Screenshot 2023-11-24 162436](https://github.com/aasnovita114/Lab7web_/assets/116045324/6df03aa5-e92a-46bc-b754-15eb54eec390)

10. Perulangan for

```
    <?php
    echo "Perulangan 1 sampai 10 <br />";
    for ($i=1; $i<=10; $i++) {
        echo "Perulangan ke: " . $i . '<br />';
    }
    echo "Perulangan Menurun dari 10 ke 1 <br />";
    for ($i=10; $i>=1; $i--) {
        echo "Perulangan ke: " . $i . '<br />';
    }
    ?>
```
![Screenshot 2023-11-24 164853](https://github.com/aasnovita114/Lab7web_/assets/116045324/e5f987d6-baa4-47ba-bd80-80ad72921ccf)

11.Perulangan while

```
    <?php
    echo "Perulangan 1 sampai 10 <br />";
    $i=1;
    while ($i<=10) {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
    }
    ?>
```
![Screenshot 2023-11-24 165555](https://github.com/aasnovita114/Lab7web_/assets/116045324/8f8703dd-79b6-4f18-b093-f9d7e1c00912)

12.Perulangan dowhile

```
    <?php
    echo "Perulangan 1 sampai 10 <br />";
    $i=1;
    do {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
    } while ($i<=10);
    ?>
```
![Screenshot 2023-11-24 170010](https://github.com/aasnovita114/Lab7web_/assets/116045324/8347267f-0ad3-4857-86fe-a8e75e26388d)


# Pertanyaan dan Tugas
Buatlah program PHP sederhana dengan menggunakan form input yang menampilkan nama, tanggal lahir dan pekerjaan. Kemudian tampilkan outputnya dengan menghitung umur berdasarkan inputan tanggal lahir. Dan pilihan pekerjaan dengan gaji yang berbeda-beda sesuai pilihan pekerjaan.

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Input PHP</title>
    <style>
    * {
    font-family: Tahoma, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    }

    span {
        font-weight: bold;
        color: darkcyan;
    }

    p {
        line-height: 25px;
        text-align: center;
    }

    h2 {
        padding: 20px;
        text-align: center;
        color: darkslateblue;
    }


    .container {
        margin: 20px auto;
        text-align: left;
        width: 60%;
    }

    form {
        background-color: rgb(100, 149, 237);
        border-radius: 10px;
        box-shadow: 2px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        text-align: center;
        padding: 20px;
    }

    form label:hover {
        cursor: pointer;
    }

    .btn {
        margin-top: 20px;
        margin-bottom: 10px;
        padding: 10px 15px;
        border-radius: 5px;
        border: 0;
        background-color: rgb(255, 255, 255);
        color: rgb(100, 149, 237);
        width: 20%;
        font-weight: bold;
    }

    .btn:hover {
        cursor: pointer;
        background-color: rgb(240, 248, 254);
        transform: scale(0.98);
    }


    form input,
    form select {
        padding: 10px;
        margin: 10px;
        width: 60%;
        border: 0;
        border-radius: 2px;
    }

    .input-group {
        display: flex;
        margin-left: 30px;
        align-items: center;
        justify-content: space-between;
    }
    </style>
</head>
<body>
    <?php
// Fungsi untuk menghitung umur berdasarkan tanggal lahir
function hitungUmur($tanggal_lahir) {
    $today = new DateTime();
    $tanggal_lahir = new DateTime($tanggal_lahir);
    $umur = $today->diff($tanggal_lahir);
    return $umur->y;
}

// Daftar pekerjaan beserta gaji
$pekerjaan_gaji = array(
    'Dokter' => 4000000,
    'Apoteker' => 8000000,
    'Hakim' => 17000000,
    'Pengacara' => 15700000,
    'CEO' => 14700000,
    'Pilot' => 10300000,
    'Direktur' => 9840000,
    'Manajer Bank' => 13000000,
    'CFO' => 14700000,
    'Dokter Gigi' => 12800000
);

// Memproses form jika sudah disubmit
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    // Mengambil data dari form
    $nama = $_POST["nama"];
    $tanggal_lahir = $_POST["tanggal_lahir"];
    $pekerjaan = $_POST["pekerjaan"];

    // Validasi data
    if (empty($nama) || empty($tanggal_lahir) || empty($pekerjaan)) {
        echo "Harap lengkapi semua field!";
    } else {
        // Menghitung umur
        $umur = hitungUmur($tanggal_lahir);

        // Menampilkan output
        echo "<h2>Hasil Output</h2>";
        echo "<p><span>Nama         :</span> $nama</p>";
        echo "<p><span>Tanggal Lahir:</span> $tanggal_lahir</p>";
        echo "<p><span>Pekerjaan    :</span> $pekerjaan</p>";
        echo "<p><span>Umur         :</span> $umur tahun</p>";
        echo "<p><span>Gaji         :</span> " . number_format($pekerjaan_gaji[$pekerjaan]) . "</p>";
    }
}
?>
<h2 class="form">Form Input</h2>
<div class="container">
    <form method="post" action="<?php echo htmlspecialchars($_SERVER["PHP_SELF"]);?>">
        <div class="input-group">
            <label for="nama">Nama </label>
            <input type="text" name="nama">
        </div>
        <div class="input-group">
            <label for="tanggal_lahir">Tanggal Lahir </label>
            <input type="date" name="tanggal_lahir">
        </div>
        <div class="input-group">
            <label for="pekerjaan">Pekerjaan </label>
            <select name="pekerjaan">
                <option value="Dokter umum">Dokter</option>
                <option value="Apoteker">Apoteker</option>
                <option value="Hakim">Hakim</option>
                <option value="Pengacara">Pengacara</option>
                <option value="CEO">CEO</option>
                <option value="Pilot">Pilot</option>
                <option value="Direktur">Direktur</option>
                <option value="Manajer Bank">Manajer Bank</option>
                <option value="CFO">CFO</option>
                <option value="Dokter Gigi">Dokter Gigi</option>
            </select>
        </div>
        
        <input type="submit" name="submit" value="Submit" class="btn">
    </form>
</div>
</body>
</html>
```

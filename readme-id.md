<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/27/PHP-logo.svg/2560px-PHP-logo.svg.png" width="720px"/>

###### Credit : Wikimedia PHP Logo

Kita semua ingin menulis program secara baik, tetapi kadang kita agak meleset dari "Standart" yang sudah diberikan. kadang kalanya mengikuti "standart" yang sudah ada itu bisa membantu kita untuk meperbaiki `source code` kita secara cepat dan gampang dibaca semua orang. 

saya akan memberikan beberapa point menarik bagaimana caranya kita menulis `source code` bahasa PHP yang bisa berguna kemudian hari.

# 💡 Langkah umum mengikuti Best Practice untuk developer PHP :

## `Table of Contents`

#### [`Point 0 : Pondasi itu harus diperkuat`](#)
asdasdasd

#### [`Point 1 : Ikuti Coding Standart yang ada`](#)
asdasdasd

#### [`Point 2 : Gunakan Version Control System untuk kerjasama`](#)
asdasdasd

#### [`Point 3 : Pahami Manajemen Dependency`](#)
asdasdasd

#### [`Point 4 : Pelajari Dasar Cyber Security dan Pahami Keamanan Aplikasi `](#)
asdasdasd

#### [`Point 5 : Optimasi Kinerja aplikasimu`](#)
asdasdasd

#### [`Point 6 : Testing.. Testing..`](#)
asdasdasd

#### [`Point 7 : Bonus Tips`](#)
asdasdasd

# Point 0️⃣
Memahami Konsep dasar adalah cara untuk memperkuat pondasi dalam bahasa. ini mencangkup sintaks, variabel, tipe data, struktur kontrol dan memahami tentang Object-Oriented Programming (OOP). Memahami PHP secara mendalam membantu untuk menulis kode secara efisien dan mudah dibaca dan dipelihara

Point penting:

### Sintaks Dasar

Sintaks dasar menjadi kunci untuk memahami dan membaca alur dari suatu program, Sintaks dasar PHP sendiri terdiri dari berbagai element yang digunakan untuk mengatur logika program. Berikut beberapa sintaks PHP yang umum :

A. Sintaks Dasar

**Variabel dan Operator**

Variabel digunakan untuk menyimpan data yang akan terpakai dalam program. Operator dalam PHP digunakan untuk melakukan operasi matematika. ini contohnya: 

```php
<?php
$nama = "Amin";
$lahir = 1996;
$umur = 2024 - $lahir;

//hasil $umur = 28
?>
```

**Fungsi Echo dan Print**

ini adalah contohnya fungsi dari Echo dan Print
```php
<?php
echo "Halo, $nama! "; print("Umur anda saat ini : "$umur);
?>
```

**Komentar**

Komentar sangat perlu ketika memahami panduan dan alur dari program. Gunakan Komentar seperti ini.
```php 
// Ini adalah komentar satu baris 

/* Ini adalah 
komentar 
beberapa baris */
```
*****

### Variabel dan Tipe Data: 

Pahami selalu dan gunakan secara tepat variabel dan tipe data yang kamu butuhkan di program. ini adalah contoh penggunaan variabel dan tipe data yang tepat :

**String**

Tipe data String adalah data berbentuk text. bisa berisi huruf, kalimat, angka atau tanda baca lainnya. Contohnya :

```php
<?php
$sapa = "Halo amin, sekarang usiamu 28 tahun!"
// Variabel tes diatas menggunakan tipe data string karena berisi text / kalimat
?>
```

**Integer**

Tipe data Integer adalah data berbentuk angka. tidak boleh ada ada karakter lain selain angka

```php
<?php
$bilangan_pertama = 4;
$bilangan_kedua = 95521;
//Kedua variabel diatas menggunakan tipe data integer untuk menyimpan nilai angka
?>
```

**Float**

Tipe data float bisa disebut juga double karena tipe data ini berisi bilangan desimal 
```php
<?php
$pi = 3.14
//variabel diatas adalah variabel bertipe data float yang berisi bilangan desimal
?>
```

**Boolean**

Tipe data boolean **Hanya** memiliki 2 buah value, yaitu `true` dan `false`

```php
<?php
    $x = true;
    $y = false;

    echo $x; // hasil: 1
    echo $y; // tidak ada data yang ditampilkan
?>
```

**Array**

Tipe data array bisa menyimpan banyak isi dalam sebuah variabel.

```php
<?php
//membuat array
$backpack = array('Wallet','Laptop','Pen','Book');

// menampilkan isi array 
echo $tas[0]."<br>"; //Wallet
echo $tas[1]."<br>"; //Laptop
echo $tas[2]."<br>"; //Pen
echo $tas[3]."<br>"; //Book
?>
```

**Object**

Tipe data ini tidak hanya sekedar menyimpan data, tetapi berisi juga informasi bagaimana cara mengolah data tersebut. contohnya seperti ini:

```php
<?php
    // membuat class dengan nama "say"
    class say
    {
        var $str;
    }

    // membuat object pesan.
    $messages = new say();

    //memberikan nilai untuk properti "str" pada object "messages"
    $messages->str="Hello World!";

    //mencetak nilai nya
    echo $messages->str;

?>
```

**Null**

Tipe data null adalah sebuah tipe data yang menujukan sebuah variabel belum memiliki nilai / data

```php
<?php
$var1 = NULL;
//atau
$var1 = null;
?>
```

Contoh penggunaan NULL
```php
<?php
// x diberi nilai 2
$x = 2;
if($x > 0) {
    echo "bisa dibandingkan karena tidak NULL";
}

// x diberi null
$x = null;
if($x > 0){
    echo "tidak bisa dibandikan, karena NULL";
}
?>
```
****








</details>

<br/>
<details><summary>© <b>Credits & read-more</b></summary>
  1. <a href='https://primakara.ac.id/blog/info-teknologi/php-adalah'>primakara.ac.id - Apa itu PHP? Kenali Bahasa Pemrograman & Fungsinya</a>
</details>

         
<br/>

# Point 1️⃣
<br/>

# Point 2️⃣
<br/>

# Point 3️⃣
<br/>

# Point 4️⃣
<br/>

# Point 5️⃣
<br/>

# Point 6️⃣
<br/>


<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/27/PHP-logo.svg/2560px-PHP-logo.svg.png" width="720px"/>

###### Credit : Wikimedia PHP Logo

Kita semua ingin menulis program secara baik, tetapi kadang kita agak meleset dari "Standart" yang sudah diberikan. kadang kalanya mengikuti "standart" yang sudah ada itu bisa membantu kita untuk meperbaiki `source code` kita secara cepat dan gampang dibaca semua orang. 

saya akan memberikan beberapa point menarik bagaimana caranya kita menulis `source code` bahasa PHP yang bisa berguna kemudian hari.

# 💡 Langkah umum mengikuti Best Practice untuk developer PHP :

## `Table of Contents`

#### [`Point 0 : Pondasi itu harus diperkuat`](#point-0️⃣)
Memahami Konsep dasar adalah cara untuk memperkuat pondasi dalam bahasa. ini mencangkup sintaks, variabel, tipe data, struktur kontrol dan memahami tentang Object-Oriented Programming (OOP). Memahami PHP secara mendalam membantu untuk menulis kode secara efisien dan mudah dibaca dan dipelihara

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

### Struktur Kontrol

Struktur kontrol dipakai untuk mengatur alur logika eksekusi program tentunya dengan kondisi dan prosedur tertentu
Dalam PHP ada beberapa struktur kontrol seperti `if-else`, `Switch-Case`, dan perulangan `for, while, do-while`

Contoh If-Else Statments :

```php
<?php
    // disini membuat kondisi, "jika $nilai lebih dari 70"
    if ($nilai > 70) {
        //ini adalah nilai yang "true"
        echo "Lulus";
    } else {
        //ini adalah nilai yang "false"
        echo "Tidak Lulus";
    }
?>
```

Contoh Looping (For and While) Statement :

```php
<?php
    //disini membuat kondisi, jika nilai $i kurang dari 5, maka akan diulang pesan yang sama 
    for ($i = 1; $i <=5; $i++){
        //ini adalah pesan nya
        echo "ini perulangan ke-$i";
    }

?>
```

### Buat dan Panggil Fungsi

Kita dapat mendefinisikan fungsi sesuai dengan kebutuhan kita, Fungsi dapat menerima input dan mengembalikan nilai tersebut sebagai output.

Seperti ini contoh dari fungsi :

```php
<?php

    //disini proses membuat fungsi
    function sapa($nama){
        echo "Halo, $nama!";
    }

    //disini proses memanggil fungsi dan menambahkan input
    sapa("Amin"); //Output : "Halo, Amin!"
?>

```


### Dasar Dasar Object-oriented programming (OOP) dengan PHP

Object-oriented programming atau biasanya kita sebut Pemrograman berorientasi objek (PBO) adalah formulasi paradigma pemrograman yang memungkinkan kita untuk mengkelompokan kode menjadi objek objek yang memiliki attribut (variabel) dan metode (fungsi). Di OOP kita akan bertemu dengan `Class, Object, Inheritence dan Polymorphism`


    Class dan Object 

Kita dapat membuat kelas sendiri menggunakan keyword `Class`. ini adalah contoh nya.

```php
<?php

    //buat kelas dengan seperti ini
    class Manusia {

        //buat public method seperti ini
        public $nama;
        public $umur;
        public funciton sapa() {
            echo "Hallo, saya adalah $this->nama. saya berumur $this->umur Tahun.";
        }
    }

    //disini kita akan menginisialisasi kelas Manusia
    $amin = new Manusia();

    //disini kita akan isi method yang ada di kelas
    $amin->nama = "Amin Syifa'";
    $amin->umur = 27;

    //disini kita akan panggil fungsi yang ada dalam kelas
    $john->sapa(); // Output: "Halo, saya adalah Amin Syifa'. saya berumur 27 tahun."
?>

```

<br/>

**Inheritence dan Polymorphism**

Inheritence mempunyai makna "pewarisan", 
secara pengertian inheritence adalah suatu kemampuan membentuk class baru yang memiliki fungsi turunan dan mirip dengan fungsi yang sudah ada sebelumnya.

ini adalah contoh dari Pewarisan :

```php
<?php

//parent class
class Manusia{

    //parent class property
    public $nama_saya;

    //method pada class manusia
    function beriNama($saya){
        $this->nama_saya=$saya;
    }
}

// buat kelas turunan / sub class dari kelas manusia
//kita hubungkan dengan class syntax "extends"

class teman extends manusia {
    public $nama_teman;

    function beriNamaTeman($teman){
        $this->nama_teman=$teman
    }
}

// inisialisasi kelas teman
$panggilTeman = new teman();

$panggilTeman->beriNama("Amin Syifa'");
$panggilTeman->beriNamaTeman("Irsyad");

//menampilkan isi property
echo "Nama Saya :".$panggilTeman->nama_saya . "<br/>";
echo "Nama Teman Saya :". $panggilTeman->nama_teman;


?>
```


polymorphism mempunyai makna "banyak bentuk", secara pengertian Polymorphism adalah konsep kemampuan dimana suatu objek berbeda-beda dapat diakses melalui satu media yaitu interface

ini adalah contoh dari polymorphism :

```php
<?php
 Interface Hewan {
    public function Makan();
    public function Bergerak();
    public function Beranak();
}

class Burung Implements Hewan{
    public function Makan() {
        echo "Burung makan biji bijian <br/>";
    }

    public function Bergerak() {
        echo "Burung bergerak dengan berjalan, dan terbang"
    }

    public function Beranak() {
        echo "Burung beranak dengan bertelur<br/>";
    }
}

class Kambing Implements Hewan {
    public function Makan() {
        echo "Kambing makan rumput<br/>";
    }

    public function Bergerak() {
        echo "kambing bergerak dengan berjalan dan berlari<br/>";
    }
    
    public function Beranak() {
        echo "kambing beranak dengan melahirkan<br/>";
    }    
}

$burung = new Burung;
$kambing = new Kambing;

echo "<b>Perilaku Burung : </b><br/>";
echo $burung->Makan();
echo $burung->Bergerak();
echo $burung->Beranak();

echo "<b>Perilaku Kambing : </b><br/>";
echo $kambing->Makan();
echo $kambing->Bergerak();
echo $kambing->Beranak();


// Output program 

// Perilaku Burung : 
// Burung makan biji-bijian
// Burung bergerak dengan berjalan, terbang dan melompat
// Burung beranak dengan bertelur

// Perilaku Kambing : 
// Kambing makan rumput
// Kambing bergerak dengan berjalan dan berlari
// Kambing beranak dengan melahirkan

?>

```
<br/>

    Kesalahan Umum dan Solusinya:

1. Kurang Pemahaman OOP
    - Programmer seringkali kurang mengerti dan tidak paham konsep dasar OOP seperti class dan inheritance, dan seringkali tidak paham ketika memperbaiki hasil kode dari orang lain.
    - Solusi : Sering seringlah Pelajari dan praktekan konsep OOP, tidak ada yang salah ketika seorang programmer untuk belajar kembali ilmu dasar. 

2. Tidak Menangani Error yang terjadi
    - Seringkali program yang sudah berjalan ada error dan sebuah kesalahan ketika pesan error itu ditampilkan ke user.
    - Solusi : Gunakan fungsi `try-catch` untuk menangani exception error ketika program sedang berjalan. dan berikan pesan error yang informatif agar user tau apa yang salah. seperti ini contohnya: 
    ```php
    <?php
        //yang salah
        $result = mysqli_query($connection, "SELECT * FROM transaksi");
        if (!$result){
            die("Query failed");
        }

        //yang benar, dengan perbaikan
        try{
            $result = mysqli_query($connection, "SELECT * FROM transaksi");
            if (!$result) {
                throw new Exception("Query failed");
            }
        } catch (Exception $e){
            echo "ERROR: Tidak bisa ambil data". $e->getMessage();
        }
    ?>
    ```


3. Kurang Pemahaman Tentang Tipe Data
    - Sering terjadi ketika seorang programmer kurang paham dengan tipe data yang digunakan, 
    seperti ini contohnya: <br/><br/>programmer membuat variabel `$bilangan1`menggunakan tipe data `String` lalu memberikan nilai `10` dan membuat variabel `$bilangan2` menggunakan tipe data `String` dan memberi nilai `20`. 
    <br/><br/>lalu ketika `$bilangan1` dan `$bilangan2` dijumlahkan. programmer itu mendapatkan ERROR. karena tipe data String tidak diperuntukan untuk nomor dan data didalam variabel tersebut tidak bisa dijumlahkan. <br/><br/>
    - Solusi : Pelajari lagi dan pahami dengan benar tentang tipe data. dan pahami alur programnya secara utuh apakah diperlukan ditengah program bekerja harus diganti variabel dengan tipe data lain. 

4. Penulisan Source Code tidak konsiten
    - sering terjadi ketika kita membuat program secara individu, kita sering tidak konsisten dengan format source code yang kita tulis. dan ketika dibaca orang lain atau berkolaborasi dengan orang lain sering membuat bingung bahkan banyak yang di refactor (diganti)
    - Solusi : Pelajari lagi tentang Standar penulisan source code, seperti PSR-1 dan PSR-2 untuk menjaga konsistensi format dari sebuah source code.


<br/>
<details><summary>© <b>Credits & read-more</b></summary>
  1. <a href='https://primakara.ac.id/blog/info-teknologi/php-adalah'>primakara.ac.id - Apa itu PHP? Kenali Bahasa Pemrograman & Fungsinya</a>
  <br/>
  2. <a href="https://www.malasngoding.com/php-oop-pewarisan-sifat-inheritance-pada-oop-php/"> Malasngoding.com - PHP OOP
  <br/>
  3. <a href="https://medium.easyread.co/php-series-tipe-data-7d389bd5d5eb">Medium.com - Jansutris Apriten Purba - PHP Series Tipe Data
</details>

         
<br/>
<!-- end Variabel & tipe data -->

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


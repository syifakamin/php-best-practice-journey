<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/27/PHP-logo.svg/2560px-PHP-logo.svg.png" width="720px"/>

###### Credit : Wikimedia PHP Logo

Kita semua ingin menulis program secara baik, tetapi kadang kita agak meleset dari "Standart" yang sudah diberikan. kadang kalanya mengikuti "standart" yang sudah ada itu bisa membantu kita untuk meperbaiki `source code` kita secara cepat dan gampang dibaca semua orang. 

saya akan memberikan beberapa point menarik bagaimana caranya kita menulis `source code` bahasa PHP yang bisa berguna kemudian hari.

# 💡 Langkah umum mengikuti Best Practice untuk developer PHP :

## `Table of Contents`

#### [`Point 0 : Pondasi itu harus diperkuat`](#point-0️⃣)
Memahami Konsep dasar adalah cara untuk memperkuat pondasi dalam bahasa. ini mencangkup sintaks, variabel, tipe data, struktur kontrol dan memahami tentang Object-Oriented Programming (OOP). Memahami PHP secara mendalam membantu untuk menulis kode secara efisien dan mudah dibaca dan dipelihara

#### [`Point 1 : Ikuti Coding Standart yang ada`](#point-1️⃣---ikuti-coding-standart-yang-ada)
Coding Standart adalah pedoman dan aturan penulisan source code yang konsisten. mengikuti standart penulisan source code membantu memperbaiki kerentanan, meningkatkan kerjasama tim, dan meningkatkan keterbacaan kode. 

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

# Point 0️⃣ - Pondasi itu harus diperkuat
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
  2. <a href="https://www.malasngoding.com/php-oop-pewarisan-sifat-inheritance-pada-oop-php/"> Malasngoding.com - PHP OOP</a>
  <br/>
  3. <a href="https://medium.easyread.co/php-series-tipe-data-7d389bd5d5eb">Medium.com - Jansutris Apriten Purba - PHP Series Tipe Data </a>
</details>

         
<br/>
<!-- end Variabel & tipe data -->

# Point 1️⃣ - Ikuti Coding Standart yang ada

Coding standards atau standar penulisan kode, adalah separangkat aturan dan pedoman yang memandu cara penulsan kode dalam suatu proyek. Hal ini sangat membantu memastikan konsistensi, kerapihan, dan kejelasan dalam kode. </br>

Standar coding menjadi penting ketika proyek melibatkan kolaborasi tim, karena memudahkan pemahaman dan perawatan code

### Apa itu PSR-4?

PSR-4 (PHP Standard Recommendation 4) adalah sebuah standar yang dikeluarkan oleh PHP Framework Interoperability Group (PHP-FIG) untuk menetapkan strukut direktori dan penamaan namespace pada proyek. PHP PSR-4 bertujuan untuk menciptakan konsistensi dalam penulsan kode yang lebih baik antara komponen-komponen yang dikembangkan oleh berbagai pihak.

Point-Point penting:

1. Namespace dan Struktur Direktori
    * PSR-4 mengikuti aturan bahwa setiap namespace dalam proyek PHP harus sesuai dengan struktur direktori yang konsisten. ini membantu memudahkan pencarian kelas dan memahami hubungan antara kelas-kelas.
2. Root Namespace
    * PSR-4 menetapkan bahwa setiap proyek PHP harus memiliki "root namespace" sebagai bagian dari namespace kelas-kelasnya. Root namespace ini biasanya mencerminkan vendor atau penulis kode.
3. Penamaan Kelas dan Berkaitan dengan Namespace :
    * Nama kelas harus mencerminkan lokasi file di dalam struktur direktori. Misalnya, 
    ```
    'NamaProjek\SubNamespace\KelasSaya' 
    ```
    harus ditempatkan di dalam direktori
    ```
    'NamaProjek/SubNamespace/KelasSaya.php'
    ```
4. Autoloading
    * PSR-4 mendukung konsep autoloading, yaitu proses di mana PHP secara otomatis memuat kelas yang dibutuhkan tanpa perlu menyertakan file secara manual. Ini memudahkan manajemen dependensi dan pengembangan.
5. Vendor Namespace
    * Namespace yang berkaitan dengan vendor (Penulis kode atau organisasi) sebaiknya dimulai dengan nama vendor.

    Contohnya, jika vendor adalah "laravel", maka namespace kelas dapat dimulai dengan `laravel\NamaspaceKhusus`        
<br/>

### Bagaimana contoh implementasi menggunakan PSR-4

Bagi yang mengimplementasikan OOP ketika menulis kode PHP, pasti tidak asing dengan implementasi pemanggilan kelas di file yang berbeda. Biasanya file yang berisi kelas tersebut dipanggil menggunakan `require` atau `include`
Contohnya :

```php
<?php
    include('Foo.php');
    include('Bar.php');

    $foo = new Foo();
    $foo->someFunction();

    $bar = new Bar();
    $bar->anotherFunction();
?>
```

tetapi dengan semakin berkembangnya aplikasi yang kita buat, kita memerlukan sebuah cara agar file file kelas yang kita punya bisa terorganisir dengan baik. 

selain itu, semkin modular fungsi-fungsi yang kita punya, maka kebutuhan untuk memanggil class di file yang berbeda akan semakin besar. Ada kalanya kita perlu memanggil lebih dari 10 class yang berbeda ketika kita ingin mengerjakan sebuah fitur. adakah cara agar kita tidak perlu menulis `include` atau `require` berulang kali?

ternyata, kita bisa memanfaatkan salah satu magic method yang ada di PHP yaitu `__autoload`

Berikut adalah contoh pemakaian `__autoload` untuk memuatkan file-file yang berisi kelas secara otomatis. 

untuk kali ini, kita akan mencoba untuk memanggil 2 kelas, yaitu `Foo` dan `Bar` via `__autoload`

Contoh Class Foo.php
```php
<?php 
    class Foo
    {
        public function someFunction()
        {
            echo "Calling ". __FUNCTION__ ."() in class ". __CLASS__ ."\n";
        }
    }
```

Contoh class Bar.php
```php
<?php
    class Bar
    {
        public function anotherFunction()
        {
            echo "Calling ". __FUNCTION__ ."() in class ". __CLASS__ ."\n";            
        }
    }
?>
```

Contoh class __autoload
```php
<?php
function __autoload($class)
{
    $file = $class . ".php";
    if (is_readable($file)){
        require $file;
    }
}

$foo = new Foo();
$foo->someFunction();

$bar = new Bar();
$bar->anotherFunction();
?>
```

dan Hasilnya adalah :

```
Calling someFunction() in class Fo
Calling anotherFunction() in class Bar
```

Dengan memakai `__autoload`, kita tidak perlu lagi memasukan file berisi class satu persatu, namun cukup dengan menginisialisasikan kelas dan PHP secara otomatis akan mengenali nama kelas dan mencari file yang memiliki nama yang sama dengan kelas tersebut. 

`is_readable()` diperlukan untuk memastikan file tersebut ada dan memiliki hak akses untuk dapat dibaca oleh kode yang memanggilnya

### Standarisasi dengan PSR-4

_Autoloading_ adalah ide yang sangat bagus. tapi dampaknya adalah setiap orang memiliki caranya sendiri untuk melakukan _autoload_. 

untuk itu perlu dibuat sebuah standar bagu _autoloader_, dengan mengikuti aturan yang disebut dengan PSR-4 (Perbaikan dari PSR-0 yang telah _deprecated_, awalnya standarissasi _autolaoader_ menggunakan PSR-0).

PSR-4 mewajibkan menggunakan _Fully Qualified Class Name_ (FQCN) dan memiliki _top-level namespace_ atau vendor namespace

Namespace adalah fitur yang diperkenalkan di PHP 5.3. namespace adalah _Virtual Directory_ yang merepresentasikan _directory_ yang sebenarnya. Sebuah FQCN terdiri dari sekumpulan namespace dan memiliki bentuk seperti ini

```
\<NamespaceName>(\<SubNamespaceNames>)*\<ClassName>
```

conthnya, kita memiliki file dengan namespace Vehicle\Car\Honda\Jazz, Vehicle\Car\Honda\HRV dan Vehicle\Car\Toyota\Yaris. maka diasumsikan project ini memiliki struktur directory:

```
-- Vehicle
   - Car
     - Honda
       - Jazz.php
       - HRV.php
     - Toyota
       - Yaris.php
```

### Mengapa Mengikuti Coding Standards

1. **Kegunaan**
    1. Memastikan konsistensi gaya kode di seluruh proyek.
    2. Meningkatkan kerjasama tim dengan memberikan panduan yang jelas
    3. Mempermudah pemeliharaan dan pembacaan kode.
2. **Kesalahan Umum**
    1. Menulis kode tanpa mengikuti aturan, menyebabkan kode sulit dipahami.
3. **Solusi**
    1. Belajar lalu terapkan standar coding yang diterima dan lakukan check source code secara berkala, kalau bisa silahkan refactor source code yang tidak menerapkan standart coding agar mempermudah programmer membaca dan memperbaiki code.

### Keuntungan PSR-4

* Konsistensi
    * Standar ini menciptakan konsistensi dalam struktur direktori dan namespace. memudahkan developer dalam memahami dan kolaborasi project

* Interoperabilitas
    * PSR-4 memungkinkan komponen-komponen dari berbagai pihak untuk bekerja bersama tanpa kesulitan dalam pengangan namespace.

* Autoloading
    * Mempermudah penggunaan _autoloading_, menghilangkan kebutuhan untuk menyertakan manual setiap file kelas.

### Contoh Coding Standards yang umum selain PSR-4
1. **Penanaman Variabel**
    - ✅ Do : Gunakan nama variabel yang jelas dan deskriptif, hindari singkatan yang tidak jelas.
    - 🚫 Don't : Menggunakan singkatan yang tidak dimengerti developer atau nama variabel yang tidak deskriptif dan sulit dipahami
    
2. **Indentasi**
    - ✅ Do : Pilih salah satu metode (biasanya spasi), terapkan secara konsisten dan terapkan di tetapnya
    - 🚫 Don't : Menggunakan campuran "Spasi" dan "tab" ditempat sembarangan untuk indentasi

3. **Panjang Baris Kode**
    - ✅ Do : Batasi panjang baris kode sesuai standar, kalau bisa silahkan dibagi ke beberapa kelas (umumnya 80 - 120 Karakter).
    - 🚫 Don't : Baris kode terlalu panjang, sulit dibaca dan sulit diperbaiki programmer 

4. **Komentar** 
    - ✅ Do : Tulis komentar yang jelas, dan perbarui jika logic dan kode berubah
    - 🚫 Don't : Tidak ada komentar di kode lalu Komentar tidak jelas dan tidak diperbaharui

Mengenali kesalahan umum seperti ini dan berusaha untuk menghindarinya melalui pemahaman yang lebih baik terhadap standar dan penggunaan alat linting adalah langkah penting menuju penulisan kode yang konsisten, mudah dipahami, dan bersih. 

Hal ini tidak hanya mendukung kolaborasi tim yang baik, tetapi juga meningkatkan kualitas dan pemeliharaan kode dalam jangka panjang.    
<br/>
<details><summary>© <b>Credits & read-more</b></summary>
  1. <a href='https://medium.com/koding-kala-weekend/autoloading-di-php-dan-implementasinya-menggunakan-psr-4-3005dd7a09e6'>medium.com - Wahyudi Wibowo - Autoloading di PHP dan Implementasinya menggunakan PSR-4</a>
  <br/>
  2. <a href="https://community.algostudio.net/implementasi-psr-4-autoloading-pada-php/"> algostudio.net -Nuzulul Huda - Implementasi PSR 4 Autoloading pada PHP </a>
  <br/>
  3. <a href="https://medium.easyread.co/memahami-konsep-psr-4-autoloading-pada-php-ba6cdefe068b">Medium.com - Mohammad Robih - Memahami Konsep PSR-4 Autoloading pada PHP </a>
</details>


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


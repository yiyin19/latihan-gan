 <!DOCTYPE html>
<html>
<head>
<style>
* 
{
    box-sizing: border-box;
}

header 
{
    background-color: #957DAD;
    padding: 25px;
    text-align: center;
    font-size: 35px;
    color: white;
    font-family: georgia;
}

nav 
{
    float: left;
    width: 40%;
    height: 400px;
    background: #E0BBE4;
    padding: 20px;
    text-align: center;
    font-size: 30px;
    font-family: comic sans ms;
    color: #000000;
}

form
{
    padding: 30px;
}

output 
{
    float: left;
    padding: 100px;
    width: 60%;
    background-color: #FFDCF4;
    height: 400px;
    font-size: 30px;
    font-family: comic sans ms;
}

section:after {
    content: "";
    display: table;
    clear: both;
}

footer {
    background-color: #957DAD;
    padding: 10px;
    text-align: center;
    color: white;
    font-size: 20px;
    font-family: georgia;
}

input[type="text"]{
    background: #fff;
    width: 300px;
    height: 40px;
    border: none;
    outline: black;
    padding: 10px;
    text-align: center;
    font-size: 20px;
}
input[type="submit"]{
    background-color: #dc659b;
    border: none;
    color: white;
    padding: 10px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    
}
}
</style>
</head>
<body>

<header>
    <h2>KALKULATOR SEDERHANA</h2>
</header>

<section>
    <nav>
        <form method= "POST" action=""><!--memberi method-->
            Bilangan 1
            <br> 
            <input type="text" name="bil1" placeholder="Masukkan Angka"><!--untuk membuat form untuk diisi bilangan 1-->
            <br>
            Bilangan 2
            <br>
            <input type="text" name="bil2"placeholder="Masukkan Angka"><!--untuk membuat form untuk diisi bilangan 2-->
            <br>
            <br>
            <input type="submit" name="submit" value="HITUNG"><!--membuat tombol button-->
            </form>
    </nav>
  
    <output>
        <?php
            $bil1 =$_POST['bil1'];//memberi variabel pada bilangan 1
            $bil2 =$_POST['bil2'];//memberi variabel pada bilangan 2
            $jumlah = $bil1 + $bil2;//operasi penjumlahan
            echo "Hasil penjumlahan adalah : $jumlah";//menampilkan operasi penjumlahan
            echo "<br>";
            $kurang = $bil1 - $bil2;//operasi pengurangan
            echo "Hasil pengurangan adalah : $kurang";//menampilkan operasi pengurangan
            echo "<br>";
            $kali = $bil1 * $bil2;//operasi perkalian
            echo "Hasil perkalian adalah : $kali";//menampilkan hasil perkalian
            echo "<br>";
            $bagi = $bil1 / $bil2;//operasi pembagian
            echo "Hasil pembagian adalah : $bagi";//menampilkan hasil pembagian
            echo "<br>";
        ?>
    </output>
</section>

<footer>
    <p>Selamat Menghitung :) </p>
</footer>
</body>
</html>

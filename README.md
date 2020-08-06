   KALKULATOR SEDERHANA
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
  
    <p>Selamat Menghitung :) </p>

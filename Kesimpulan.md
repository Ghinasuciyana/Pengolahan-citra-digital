KESIMPULAN
dari program ini terdapat beberapa point yaitu:

1. Membaca dan Menampilkan Gambar:

    Gambar yang diolah diunduh dari URL menggunakan io.imread dari skimage.
    Gambar diubah dari bgr menjadi format RGB menggunakan cv.cvtColor.
    Gambar asli dan yang diubah ditampilkan secara horizontal menggunakan cv.hconcat dan cv2_imshow.

2. Statistik Dasar Gambar:

    memuat informasi dasar dari gambar seperti Ukuran gambar, bentuk (shape), dan tipe data (uint8) dicetak.
    Histogram untuk seluruh gambar diplot menggunakan plt.hist.

3. Analisis Histogram untuk Setiap Saluran Warna (RGB):

    Histogram untuk masing-masing saluran warna (merah,biru, hijau) dihitung dan diplot dengan menggunakan cv.calcHist.
    Histogram diekspresikan dalam beberapa variasi (jumlah bins yang berbeda) untuk memberikan perspektif yang berbeda pada distribusi warna.

4. Analisis Histogram untuk Saluran Warna Tertentu :

    Histogram untuk saluran warna tertentu (misalnya, pada saluran warna biru) dipisahkan dan diplot.
    Histogram diekspresikan dalam beberapa variasi bins untuk memberikan perspektif yang berbeda pada distribusi warna dalam saluran tertentu, jumlah bins yang tinggi akan memeberikan detail yang lebih halus sedangkan bins yang rendah hanya kaan memberikan gambaran umum dari distribusi warna dan kecerahannya makanya variasi jumlah bins akan memeberikan informasi yang berbeda tergantung dari distribusi warna pada gambar sehingga memberikan pemahaman yang lebih mendalam terhadap gambar dari segi warnanya.
    untuk warna merah dan hijaupun carakerjanya sama saja di pisahkan dengan diplot lalu menampilkan histogram dengan jumlah bins yang berbeda beda.

5. Analisis Histogram untuk Gambar Grayscale:

    Gambar dikonversi menjadi citra grayscale menggunakan cv.cvtColor.
    Histogram untuk gambar grayscale diplot untuk memberikan visualisasi dari distribusi intensitas piksel dalam gambar, dalam grayscale ini histogramnya menggambarkan seberapa sering intensitas piksel yang berkisar dari 0-255 pada citra 8 bit dimana 0 mewakili warna hitam dan 255 merepresentasikan warna putih yang muncul dalam gambar.jadi semakin tinggi nila intesnsitasnya maka semakin terang dan semakin rendah maka semakin gelap.

6. Operasi pada Gambar Grayscale:

    Gambar grayscale diubah menjadi citra negatif menggunakan 255 - gray_image.
    Histogram untuk citra negatif diplot.
    Gambar diterangkan dan diserap ke dalam histogram dengan persamaan sederhana.
    Histogram untuk gambar yang diterangkan diplot.
    Gambar diperjelas (dipekakan) dan histogramnya diplot.


keseluruhan Program ini memberikan pemahaman tentang distribusi warna dalam gambar baik Gambar Asli, RGB, warna tertentu dari rgb yang di pisahkan misalnya hanya biru, hanya hijau, dan hanya merah, serta Grayscale. termasuk variasi dalam representasi histogram dengan jumlah bins yang berbeda.
operasi pada gambar grayscale juga ditunjukkan bersama dengan dampaknya pada histogram dengan distribusi intensitas piksel, Program ini merupakan alat analisis visual untuk memahami sifat-sifat gambar secara mendalam

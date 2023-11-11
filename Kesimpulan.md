KESIMPULAN
dari program ini terdapat beberapa point yaitu:

1. Membaca dan Menampilkan Gambar:

    Gambaryang diolah diunduh dari URL menggunakan io.imread dari skimage.
    Gambar diubah menjadi format RGB menggunakan cv.cvtColor.
    Gambar asli dan yang diubah ditampilkan secara horizontal menggunakan cv.hconcat dan cv2_imshow.

2. Statistik Dasar Gambar:

    memuat informasi dasar dari gambar seperti Ukuran gambar, bentuk (shape), dan tipe data (uint8) dicetak.
    Histogram untuk seluruh gambar diplot menggunakan plt.hist.

3. Analisis Histogram untuk Setiap Saluran Warna (RGB):

    Histogram untuk masing-masing saluran warna (biru, hijau, merah) dihitung dan diplot dengan menggunakan cv.calcHist.
    Histogram diekspresikan dalam beberapa variasi (jumlah bins yang berbeda) untuk memberikan perspektif yang berbeda pada distribusi warna.

4. Analisis Histogram untuk Saluran Warna Tertentu (Contoh: Saluran Biru):

    Histogram untuk saluran warna tertentu (misalnya, pada saluran warna biru) dipisahkan dan diplot.
    Histogram diekspresikan dalam beberapa variasi bins untuk memberikan perspektif yang berbeda pada distribusi warna dalam saluran tertentu,
    Jumlah bins yang berbeda memberikan informasi yang berbeda tentang variasi intensitas warna dalam gambar. Jumlah bins yang lebih tinggi dapat memberikan detail yang lebih halus, sementara jumlah bins yang lebih rendah dapat memberikan gambaran umum distribusi warna.
    untuk warna merah dan hijaupun carakerjanya sama saja

5. Analisis Histogram untuk Gambar Grayscale:

    Gambar dikonversi menjadi citra grayscale menggunakan cv.cvtColor.
    Histogram untuk gambar grayscale diplot, yang berarti bahwa histogram untuk gambar grayscale ditampilkan grafis, dengan menggunakan diagram batang atau kurva, untuk memberikan gambaran visual tentang distribusi intensitas piksel dalam gambar.

6. Operasi pada Gambar Grayscale:

    Gambar grayscale diubah menjadi citra negatif menggunakan 255 - gray_image.
    Histogram untuk citra negatif diplot.
    Gambar diterangi dan diserap ke dalam histogram dengan persamaan sederhana.
    Histogram untuk gambar yang diterangi diplot.
    Gambar diperjelas (dipekakan) dan histogramnya diplot.

keseluruhan Program ini memberikan pemahaman tentang distribusi warna dalam gambar baik Gambar Asli, RGB, warna tertentu misalnya hanya biru, hanya hijau, dan hanya merah, serta Grayscale. termasuk variasi dalam representasi histogram dengan jumlah bins yang berbeda.
operasi pada gambar grayscale juga ditunjukkan bersama dengan dampaknya pada histogram dengan distribusi intensitas piksel, Program ini merupakan alat analisis visual untuk memahami sifat-sifat gambar secara mendalam

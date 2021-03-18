

## Graph Node Search menggunakan algoritma BFS dan DFS ##
Nama    : Anisa Rosalina

NPM     : 1184016

Kelas   : D4 Teknik Informatika 3A 

MK      : Sistem Pakar (Tugas ke-2)

### Pengertian ###
- BFS (Breadth First Search)
Breadth First Search (BFS) adalah metode traversing yang digunakan dalam grafik. Ini menggunakan antrian untuk menyimpan simpul yang dikunjungi. Dalam metode ini yang ditekankan adalah pada simpul grafik, satu simpul dipilih pada awalnya kemudian dikunjungi dan ditandai. Verteks yang berdekatan dengan verteks yang dikunjungi kemudian dikunjungi dan disimpan dalam antrian berurutan. Demikian pula, simpul yang disimpan kemudian diperlakukan satu per satu, dan simpul yang berdekatan dikunjungi. Sebuah node sepenuhnya dieksplorasi sebelum mengunjungi node lain dalam grafik, dengan kata lain, node tersebut melintasi node yang belum dieksplorasi paling dangkal terlebih dahulu.

- DFS (Depth First Search)
Depth First Search (DFS) menggunakan stack untuk menyimpan simpul yang dikunjungi. DFS adalah metode berbasis tepi dan bekerja secara rekursif di mana simpul dieksplorasi di sepanjang jalur (tepi). Eksplorasi sebuah node ditangguhkan segera setelah simpul lain yang belum dijelajahi ditemukan dan simpul-simpul yang belum dijelajahi yang terdalam ditelusuri pada titik terdepan. DFS melintasi / mengunjungi setiap simpul tepat sekali dan setiap tepi diperiksa tepat dua kali.


### Perbedaan Utama Antara BFS dan DFS ###
BFS adalah algoritma berbasis vertex sedangkan DFS adalah algoritma berbasis tepi. Struktur data antrian digunakan dalam BFS. Di sisi lain, DFS menggunakan stack atau rekursi.
Ruang memori digunakan secara efisien dalam DFS sedangkan pemanfaatan ruang di BFS tidak efektif. BFS adalah algoritma optimal sedangkan DFS tidak optimal. DFS membangun pohon yang sempit dan panjang. Sebaliknya, BFS membangun pohon lebar dan pendek.


### Deskripsi ###
Aplikasi Python GUI untuk mencari node dalam grafik tertaut menggunakan pencarian pertama luas atau kedalaman dengan modul simpleguitk. Ini memungkinkan pengguna untuk memplot grafik pada kanvas dan menghubungkannya secara grafis. Ini awalnya dibuat menggunakan modul simplegui untuk codeskulptor ([http://www.codeskulptor.org/](http://www.codeskulptor.org/)), tetapi kemudian dipindahkan ke modul simpleguitk.

![Screenshot](https://raw.githubusercontent.com/Daytron/graph-bfs-dfs-gui/master/screenshots/screenshot1.png)


### Persyaratan: ###
- Python 2.7
- simpleguitk - [https://pypi.python.org/pypi/SimpleGUITk/1.1.3](https://pypi.python.org/pypi/SimpleGUITk/1.1.3 "Link")


### Pemakaian ###
    python BFS_DFS_GUI.py
Konsol digunakan untuk memantau hasil saat Anda berinteraksi di jendela bingkai. Klik di kanvas, untuk mulai merencanakan node grafik di kanvas. Jika Anda puas dengan node, tekan tombol * Lock in the node * untuk mengunci node. Anda sekarang dapat menghubungkan node bersama-sama dengan mengkliknya, satu node dalam satu waktu. Jika Anda senang dengan grafik Anda, tekan tombol * Lock in the graph * untuk menyelesaikan grafik Anda. Jika tidak, tekan tombol * Reset gambar tepi * untuk mengatur ulang semua tepi / tautan / koneksi antara node.
<br> <br>
Masukkan node awal dan tujuan, baik dengan mengirimkan angka atau huruf (kasus apa pun dapat diterima) yang sesuai dengan node dari grafik yang dibuat. Anda kemudian dapat memulai pencarian node menggunakan pencarian pertama yang luas dengan menekan tombol * temukan BFS * atau pencarian pertama kedalaman dengan menekan tombol * temukan DFS *.


### Lisensi dan Hak Cipta ###
Paket ini Hak Cipta (c) Ryan Gilera 2014 dan dilisensikan di bawah lisensi MIT. Lihat [lisensi](https://github.com/Daytron/graph-bfs-dfs-gui/blob/master/LICENSE) untuk lebih jelasnya.


### Kesimpulan ###
BFS dan DFS, kedua teknik pencarian grafik memiliki waktu berjalan yang sama tetapi konsumsi ruang yang berbeda, DFS mengambil ruang linier karena kita harus mengingat jalur tunggal dengan node yang belum dijelajahi, sementara BFS menyimpan setiap node dalam memori.

DFS menghasilkan solusi yang lebih dalam dan tidak optimal, tetapi bekerja dengan baik ketika solusinya padat sedangkan BFS optimal yang mencari tujuan optimal pada awalnya.

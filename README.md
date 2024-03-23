# Commit 1 reflection
Handle connection berfungsi untuk mengeprint semua data berupa stream dari semua koneksi yang diterima oleh TCP Listener dari port 127.0.0.1:7878

# Commit 2 reflection
![Commit 2 screenshot](/assets/images/m6-1.png)
Handle connection yang baru tersebut sekarang akan mengembalikan sebuah response baru dengan status ok (atau 200) serta menampilkan hello.html ketika terjadi koneksi melalui 127.0.0.1:7878

# Commit 3 reflection
![Commit 3 screenshot](/assets/images/md6-2.png)
Untuk memberikan response yang berbeda-beda, pertama kita perlu mendapat data mengenai jenis request serta url yang digunakan dengan membaca stream dan melakukan operasi terhadap hasil stream tersebut. Setelah itu kita tinggal menggunakan if tree untuk memberikan response yang sesuai terhadap metode dan url dari request tersebut.

Selain itu, refactoring yang terjadi diperlukan untuk membuat fungsi tersebut lebih pendek dan mudah dibaca dengan mengurangi repetisi penulisan kode dan memperjelas bagian apa yang berbeda dari tiap case.

# Commit 4 reflection
Yang terjadi adalah /sleep membuat thread yang digunakan server (komputer kita) untuk menjalankan program mengalami sleep selama 10 detik sehingga tidak akan ada operasi yang berjalan selama 10 detik karena thread tersebut sedang sleep.

# Commit 5 reflection
ThreadPool berfungsi untuk membuat program dapat berjalan menggunakan thread yang disediakan di ThreadPool serta membatasi jumlah thread yang berjalan untuk menghindari hal-hal seperti DDOS attack.
ThreadPool yang digunakan pada buku tersebut diimplementasikan secara manual menggunakan beberapa modul yang sudah disediakan pada rust untuk proses sinkronisasi serta thread yang digunakan.
ThreadPool tersebut juga menggunakan worker yang diimplementasikan secara manual untuk mngkostumisasi thread.
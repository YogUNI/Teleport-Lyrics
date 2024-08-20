# Teleport-Lyrics

Project ini adalah aplikasi Java sederhana menggunakan Swing untuk menampilkan lirik lagu dengan efek animasi teks yang muncul satu per satu di atas latar belakang gambar GIF yang bergerak. Berikut penjelasan lebih detail tentang bagaimana proyek ini bekerja serta cara menjalankannya:

1. Kelas Teleport:
Inisialisasi:
- Aplikasi ini menggunakan kelas JPanel untuk menggambar lirik dan latar belakang.
- Lirik Lagu: Disimpan dalam array lyrics, dan waktu jeda antar lirik disimpan dalam array delays.
GIF Latar Belakang:
- Gambar latar belakang berupa GIF disimpan dalam objek ImageIcon bernama backgroundGif.
- GIF ini digunakan untuk memberikan efek visual yang menarik saat lirik ditampilkan.

2. Animasi Lirik:
- Sebuah thread baru dijalankan ketika panel Teleport dibuat, yang akan menampilkan lirik satu karakter demi satu dengan jeda tertentu (Thread.sleep(130)).
- Ketika satu baris lirik selesai, program akan berhenti sejenak sesuai dengan waktu jeda yang ditentukan di array delays, kemudian melanjutkan ke baris lirik berikutnya.

3. Method paintComponent:
- paintComponent(Graphics g) digunakan untuk menggambar latar belakang dan lirik di panel.
- Lirik ditampilkan di tengah layar dan posisinya disesuaikan agar terlihat rapi.

4. Main Method:
- Di dalam method main, sebuah JFrame dibuat dan panel Teleport ditambahkan ke dalamnya.
- Jendela ini akan ditampilkan di tengah layar komputer.

How To Run This Project?
1. Persiapan:
- Pastikan kamu memiliki file GIF space.gif di direktori yang sama dengan file .java ini. Jika tidak ada, aplikasi tidak akan bisa menampilkan latar belakang.

2. Kompilasi dan Menjalankan:
- Simpan kode di atas sebagai file .java, misalnya Teleport.java.
- Buka terminal atau command prompt, arahkan ke direktori tempat file tersebut disimpan.
- Kompilasi program dengan perintah berikut: `javac Teleport.java`
- Setelah berhasil dikompilasi, jalankan program dengan perintah: `java Teleport`

3. Hasil:
- Program akan membuka sebuah jendela berukuran 800x60 piksel yang menampilkan lirik lagu dengan efek animasi di atas latar belakang GIF.

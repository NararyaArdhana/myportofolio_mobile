### Tugas 7
1.Widget tree adalah struktur hierarki yang menggambarkan bagaimana widget-widget disusun di dalam aplikasi Flutter. Setiap widget dapat memiliki widget lain sebagai anaknya sehingga membentuk sebuah pohon.
Hubungan parent-child berarti widget induk bertanggung jawab mengatur dan menampung widget anak. Sebagai contoh, widget Scaffold dapat memiliki AppBar dan Body. Di dalam Body, terdapat widget Padding, Column, Row, dan Text.
Hubungan ini memungkinkan tampilan aplikasi dibangun secara modular dan terstruktur. Ketika widget induk mengatur properti tata letak, widget anak akan ditampilkan mengikuti aturan yang diberikan oleh widget induknya.

2.Beberapa widget yang digunakan dalam project MyPortofolio Mobile adalah:
MaterialApp: Widget utama yang menyediakan konfigurasi aplikasi seperti tema dan halaman awal.
Scaffold: Menyediakan struktur dasar halaman aplikasi, termasuk AppBar dan Body.
AppBar: Menampilkan bagian atas aplikasi yang berisi judul MyPortofolio.
Text: Menampilkan teks seperti judul, identitas pemilik, dan nama tombol.
Padding: Memberikan jarak di sekitar widget.
Column: Menyusun widget secara vertikal.
Row: Menyusun widget secara horizontal.
Center: Menempatkan widget di bagian tengah.
Card: Menampilkan informasi profil dalam bentuk kartu.
Container: Mengatur ukuran, padding, dan tata letak konten.
SizedBox: Memberikan jarak atau ukuran tertentu.
GridView.count: Menampilkan daftar tombol dalam bentuk grid dengan jumlah kolom yang ditentukan.
Material: Menyediakan permukaan visual dan warna latar untuk kartu tombol.
InkWell: Memberikan interaksi ketika pengguna menekan tombol.
Icon: Menampilkan ikon untuk setiap menu.
SnackBar: Menampilkan pesan sementara setelah tombol ditekan.
IconData: Merepresentasikan data ikon yang digunakan pada menu.
ThemeData: Mengatur tema visual aplikasi.
ColorScheme: Menentukan skema warna aplikasi.

3.MaterialApp merupakan widget yang menyediakan konfigurasi dasar untuk aplikasi Flutter yang menggunakan Material Design.Widget ini biasanya digunakan sebagai root widget karena mengatur berbagai aspek utama aplikasi, seperti tema, navigasi, halaman awal, dan konfigurasi visual lainnya.Dalam project ini, MaterialApp digunakan untuk mengatur judul aplikasi, tema warna, serta menentukan MyHomePage sebagai halaman awal.Dengan menggunakan MaterialApp sebagai root widget, pengaturan tampilan dan struktur aplikasi dapat dilakukan secara terpusat.

4.StatelessWidget adalah widget yang tidak memiliki state internal yang dapat berubah selama siklus hidup widget. Tampilan widget ditentukan berdasarkan properti yang diterima dan konfigurasi yang diberikan.StatefulWidget adalah widget yang memiliki state yang dapat berubah selama aplikasi berjalan. Ketika state berubah, Flutter dapat membangun ulang tampilan widget melalui mekanisme setState().StatelessWidget sebaiknya digunakan ketika tampilan widget bersifat tetap dan tidak membutuhkan perubahan state internal, misalnya kartu informasi profil.StatefulWidget digunakan ketika widget membutuhkan pengelolaan data yang berubah, misalnya penghitung angka, formulir interaktif, atau komponen yang memperbarui tampilan berdasarkan input pengguna.Pada project ini, MyHomePage, InfoCard, dan ItemCard menggunakan StatelessWidget karena tampilan dan data yang ditampilkan tidak memerlukan state internal yang berubah.

5.BuildContext merupakan objek yang merepresentasikan lokasi sebuah widget di dalam widget tree.BuildContext penting karena memungkinkan sebuah widget mengakses informasi dari widget induk maupun lingkungan tempat widget tersebut berada.Dalam project ini, BuildContext digunakan pada metode build untuk mengakses tema aplikasi melalui Theme.of(context), misalnya ketika menentukan warna AppBar.BuildContext juga digunakan untuk mengakses ScaffoldMessenger melalui ScaffoldMessenger.of(context) agar aplikasi dapat menampilkan SnackBar ketika pengguna menekan tombol menu.Dengan demikian, BuildContext membantu widget berinteraksi dengan struktur dan konfigurasi aplikasi.

6.Hot reload adalah fitur Flutter yang memungkinkan perubahan kode diterapkan ke aplikasi yang sedang berjalan tanpa harus memulai ulang seluruh aplikasi. Fitur ini mempertahankan state aplikasi sehingga proses pengembangan menjadi lebih cepat.Hot restart memulai ulang aplikasi Flutter dari awal sehingga state aplikasi sebelumnya akan dihapus, tetapi tidak membangun ulang seluruh proses seperti full restart.Full restart dilakukan dengan menghentikan dan menjalankan kembali aplikasi. Proses ini diperlukan ketika perubahan tidak dapat diterapkan dengan hot reload atau ketika terdapat perubahan pada konfigurasi native, dependency, maupun bagian proyek yang membutuhkan proses kompilasi ulang.Hot reload cocok digunakan untuk perubahan tampilan atau kode widget yang tidak mengubah state secara mendasar. Hot restart diperlukan ketika perubahan membutuhkan inisialisasi ulang state atau struktur aplikasi. Full restart diperlukan ketika perubahan melibatkan konfigurasi native atau perubahan yang tidak dapat ditangani oleh hot reload maupun hot restart.

### AI DISCLOSURE
Dalam pengerjaan project ini, saya menggunakan ChatGPT sebagai alat bantu pembelajaran dan pengembangan aplikasi.

Bantuan AI digunakan untuk:
1.Pemahaman Materi: Membantu memahami konsep Flutter, widget tree, StatelessWidget, MaterialApp, BuildContext, serta mekanisme hot reload dan hot restart.
2.Implementasi Kode: Membantu menyusun dan memperbaiki struktur widget pada file main.dart dan menu.dart.
3.Debugging: Membantu menganalisis pesan error dari flutter analyze dan memberikan arahan perbaikan kode.

AI digunakan sebagai alat bantu, sedangkan pemahaman, pemeriksaan, penyesuaian, dan pengujian hasil implementasi dilakukan selama proses pengerjaan project.
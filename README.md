Nama: Shinta Yulistiana
NIM: 362358302076
Kelas: 2A TRPL

Praktikum 1: Dasar State dengan Model-View

Langkah 1: Buat Project Baru

![alt text](image.png)

Langkah 2: Membuat model task.dart
![alt text](image-1.png)

Langkah 3: Buat file plan.dart
![alt text](image-2.png)

Langkah 4: Buat file data_layer.dart
![alt text](image-3.png)

Langkah 5: Pindah ke file main.dart
![alt text](image-5.png)

Langkah 6: buat plan_screen.dart
![alt text](image-6.png)

Langkah 7: buat method \_buildAddTaskButton()
![alt text](image-7.png)

Langkah 8: buat widget \_buildList()
![alt text](image-8.png)

Langkah 9: buat widget \_buildTaskTile
![alt text](image-9.png)
![alt text](image-4.png)

Langkah 10: Tambah Scroll Controller
![alt text](image-10.png)

Langkah 11: Tambah Scroll Listener
![alt text](image-11.png)

Langkah 12: Tambah controller dan keyboard behavior
![alt text](image-12.png)

Langkah 13: Terakhir, tambah method dispose()
![alt text](image-13.png)

Langkah 14: Hasil
![alt text](image-14.png)

Tugas Praktikum 1: Dasar State dengan Model-View

1. Selesaikan langkah-langkah praktikum tersebut, lalu dokumentasikan berupa GIF hasil akhir praktikum beserta penjelasannya di file README.md! Jika Anda menemukan ada yang error atau tidak berjalan dengan baik, silakan diperbaiki.
   ![alt text](master_plan.gif), pada gambar tersebut telah dibuat list atau plan yang bisa ditambah sesuai kebutuhan.

2. Jelaskan maksud dari langkah 4 pada praktikum tersebut! Mengapa dilakukan demikian?
   Maksud dari langkah 4 pada praktikum 1 adalah bertujuan untuk menyederhanakan proses impor. Dengan mengekspor plan.dart dan task.dart melalui data_layer.dart, maka cukup mengimpor data_layer.dart saja untuk mendapatkan akses pada keduanya dan membuat kode lebih efisien dan rapi.

3. Mengapa perlu variabel plan di langkah 6 pada praktikum tersebut? Mengapa dibuat konstanta ?
   Perlu variabel plan di langkah 6 pada praktikum 1 karena variabel plan berfungsi sebagai wadah untuk menyimpan data rencana atau plan yang akan ditampilkan di layar.
   Dibuat konstanta karena dengan membuat plan sebagai konstanta dan memberikan nilai awal const Plan(), maka memastikan bahwa variabel tersebut memiliki nilai default
   pada saat aplikasi pertama kali dijalankan. Nilai tidak dapat diubah secara langsung setelah inisialisasi. Membuat plan sebagai konstanta membantu menjaga integritas data.

4. Lakukan capture hasil dari Langkah 9 berupa GIF, kemudian jelaskan apa yang telah Anda buat!
   ![alt text](master_plan.gif), pada gambar tersebut telah dibuat list atau plan yang bisa ditambah sesuai kebutuhan.

5. Apa kegunaan method pada Langkah 11 dan 13 dalam lifecyle state ?
   - initState() digunakan untuk inisialisasi awal.
   - dispose() digunakan untuk membersihkan sumber daya.
   - ScrollController digunakan untuk mengontrol scrolling.
   - Listener pada ScrollController digunakan digunakan untuk mendeteksi perubahan posisi scroll dan menghilangkan fokus.
     Dengan menghilangkan fokus saat scrolling, keyboard akan tertutup secara otomatis, sehingga pengguna dapat lebih fokus pada konten yang sedang dilihat.

Praktikum 2: Mengelola Data Layer dengan InheritedWidget dan InheritedNotifier
Langkah 1: Buat file plan_provider.dart
![alt text](image-15.png)

Langkah 2: Edit main.dart
![alt text](image-17.png)

Langkah 3: Tambah method pada model plan.dart
![alt text](image-16.png)

Langkah 4: Pindah ke PlanScreen
![alt text](image-18.png)

Langkah 5: Edit method \_buildAddTaskButton
![alt text](image-19.png)

Langkah 6: Edit method \_buildTaskTile
![alt text](image-20.png)

Langkah 7: Edit \_buildList
![alt text](image-21.png)

Langkah 9: Tambah widget SafeArea
![alt text](image-22.png)

Tugas Praktikum 2: InheritedWidget

2. Jelaskan mana yang dimaksud InheritedWidget pada langkah 1 tersebut! Mengapa yang digunakan InheritedNotifier?

- InheritedWidget adalah sebuah widget yang dapat memberikan data ke turunannya tanpa perlu melewati proses props secara eksplisit.
- InheritedNotifier digunakan untuk memantau perubahan data dan memudahkan akses data.
  Dengan menggunakan InheritedNotifier, PlanProvider dengan efisien membagikan Plan ke seluruh widget tree, memastikan bahwa perubahan pada data tersebut akan segera ada dalam tampilan.

3. Jelaskan maksud dari method di langkah 3 pada praktikum tersebut! Mengapa dilakukan demikian?

   - Maksud dari method di langkah 3 praktikum tersebut adalah metode getCompleteMessage berfungsi untuk membentuk sebuah pesan yang menginformasikan tentang progres penyelesaian tugas.
     Pesan tersebut akan menunjukkan berapa banyak tugas yang telah selesai dibandingkan dengan total jumlah tugas.
   - Dilakukan demikian karena memberikan informasi yang jelas kepada pengguna dengan menampilkan pesan yang spesifik tentang jumlah tugas yang selesai, meningkatkan user expirience yaitu
     pesan tersebut membuat aplikasi menjadi lebih interaktif dan informatif serta memudahkan dalam pengembangan fitur lain seperti informasi mengenai jumlah tugas yang selesai dan total
     tugas dapat digunakan untuk membuat fitur-fitur lain seperti persentase penyelesaian, notifikasi, atau laporan.

Praktikum 3: Membuat State di Multiple Screens
Langkah 1: Edit PlanProvider
![alt text](image-23.png)

Langkah 2: Edit main.dart
![alt text](image-24.png)
![alt text](image-25.png)

Langkah 3: Edit plan_screen.dart
![alt text](image-26.png)

Langkah 5: Tambah getter Plan
![alt text](image-27.png)

Langkah 6: Method initState()
![alt text](image-28.png)

Langkah 7: Widget build
![alt text](image-29.png)
![alt text](image-30.png)

Langkah 8: Edit \_buildTaskTile
![alt text](image-31.png)

Langkah 9: Buat screen baru
![alt text](image-32.png)
![alt text](image-33.png)

Langkah 10: Pindah ke class \_PlanCreatorScreenState
![alt text](image-34.png)

Langkah 11: Pindah ke method build
![alt text](image-35.png)

Langkah 12: Buat widget \_buildListCreator
![alt text](image-36.png)

Langkah 13: Buat void addPlan()
![alt text](image-37.png)

Langkah 14: Buat widget \_buildMasterPlans()
![alt text](image-38.png)
![alt text](image-39.png)

Tugas Praktikum 3: State di Multiple Screens

1. Selesaikan langkah-langkah praktikum tersebut, lalu dokumentasikan berupa GIF hasil akhir praktikum beserta penjelasannya di file README.md! Jika Anda menemukan ada yang error atau tidak berjalan dengan baik, silakan diperbaiki sesuai dengan tujuan aplikasi tersebut dibuat.
   ![alt text](master_plan2.gif), pada gambar tersebut telah dibuat list atau plan yang bisa ditambah sesuai kebutuhan.

2. Berdasarkan Praktikum 3 yang telah Anda lakukan, jelaskan maksud dari gambar diagram berikut ini!
   ![alt text](image-40.png)

   - Aplikasi memiliki struktur widget yang terdiri dari MaterialApp, PlanProvider, PlanCreatorScreen, Column, TextField, Expanded, dan ListView.
   - PlanCreatorScreen merupakan tampilan utama yang sedang aktif.
   - Terjadi sebuah tindakan navigasi yang diwakili oleh panah biru dengan label "Navigator Push".
   - Tindakan tersebut biasanya dipicu oleh suatu event, misalnya ketika pengguna menekan tombol "Tambah plan" atau yang lain.

3. Lakukan capture hasil dari Langkah 14 berupa GIF, kemudian jelaskan apa yang telah Anda buat!
   ![alt text](master_plan2.gif), pada gambar tersebut telah dibuat list atau plan yang bisa ditambah sesuai kebutuhan.

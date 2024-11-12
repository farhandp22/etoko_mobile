# etoko_mobile

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.


# Tugas 7

1. Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget, dan jelaskan perbedaan dari keduanya.
    Stateless widget adalah widget yang tidak memiliki status perubahan jika dirender. dan cocok untuk menampilkan konten 
    statis dan ringan karena tidak memerlukan pengelolaan status,stateful widget adalah widget yang memiliki status berubah selama aplikasi berjalan.cocok untuk tampilan dinamis yang membutuhkan pembaruan berdasarkan interaksi pengguna dan
    perubahan data.
2. Sebutkan widget apa saja yang kamu gunakan pada proyek ini dan jelaskan fungsinya.
   - Scaffold : sebagai kerangka dasar dan terdiri dari appBar,tombol floating buttondan body
   - Text : untuk menaplikan teks pad aplikasi android
   - Card : untuk mengelompokkan data
   - container : sebagai wadah untuk mengatur tata letak konten di dalam nya
3.  Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
     fungsi nya adalah memperbarui data di dalam suatu widget.variabel yang ada di dalam widget yang terdampak dalam fungsi
     setState
4. Jelaskan perbedaan antara const dengan final.
    perbedaan const dan final terletak pada insisiasi nilai.const mengharuskan variabel di inisiasi  pada saaat compile dan
     nilai nya berisfat konstan dan secara langsung/eksplisit sehingga pada saat kompilasi variabel const maka sudah memiliki nilai,sedangkan
     final tidak mengharuskan langsung memberi nilai pada saat kompilasi variabel
5.  Jelaskan bagaimana cara kamu mengimplementasikan checklist-checklist di atas.
    - buatlah proyek flutter
    - buat menu.dart
    - mengubah tema aplikasi
    - mengubah tema aplikasi pada main.dart yang mempunyai tipe material art.
    - mengubah sifat widget halaman menu menjadi wish stateless
    - membuat card yang berisi npm,nama,dan kelas
    - mengganti warna dan text button card 
    - mengimplementasikan info dan itemCard untuk ditampilkan pada myHomePage

# Tugas 8

1. Apa kegunaan const di Flutter? Jelaskan apa keuntungan ketika menggunakan const pada kode Flutter. Kapan sebaiknya kita menggunakan const, dan kapan sebaiknya tidak digunakan?
    kegunaan dari const adalah untuk membuat objek data yang tidak dapat diubah seperti warna dan konfigurasi.
    keuntuungan const pada flutter adalah objek data tidak berubah setelah diinisialisasi dan sebaiknya digunkan ketika objek dapat diubah dan sebaliknya tidak digunakan untuk user yang ingin merubah objek.

2. Jelaskan dan bandingkan penggunaan Column dan Row pada Flutter. Berikan contoh implementasi dari masing-masing layout widget ini!
Row merupakan widget layout yang digunakan untuk mengatur tata letak elemen-elemen dalam satu baris secara horizontal. Widget-row dapat berisi widget lainnya, seperti teks, gambar, atau widget lainnya, dan dapat diatur dalam berbagai cara, termasuk di tengah, ke kiri, ke kanan, atau rata kiri-kanan.
contoh:
Row(
children: [
Text(‘Elemen 1’),
Text(‘Elemen 2’),
Text(‘Elemen 3’),
],
)
Column adalah widget layout yang digunakan untuk mengatur tata letak elemen-elemen dalam satu kolom secara vertikal. Widget-column juga dapat berisi widget lainnya dan dapat diatur dalam berbagai cara, termasuk di tengah, ke atas, ke bawah, atau rata atas-bawah.
contoh:
Column(
children: [
Text(‘Elemen 1’),
Text(‘Elemen 2’),
Text(‘Elemen 3’),
],
)
Perbedaan antara Row dan Column dalam Flutter adalah orientasi tata letak yang mereka perlihatkan. Row mengatur widget secara horizontal dalam satu baris, sementara Column mengatur widget secara vertikal dalam satu kolom. Kedua widget ini sangat berguna untuk mengatur tata letak elemen-elemen dalam sebuah aplikasi Flutter dengan mudah dan efektif.


3. Sebutkan apa saja elemen input yang kamu gunakan pada halaman form yang kamu buat pada tugas kali ini. Apakah terdapat elemen input Flutter lain yang tidak kamu gunakan pada tugas ini? Jelaskan!
    ada seperti CheckboxListTile(checklist suatu item), SwitchListTile(mengubah fitur tombol seperti on/off), DropdownButton(untuk memilih item yang ada pada dropdown list), dan Slider(untuk mengatur intensitas suatu value dengan cara slide dari range yang ditentukan),TextFromField diimplementasikan buat memakai tiga elemen yaitu name,amount,description.

4.  Bagaimana cara kamu mengatur tema (theme) dalam aplikasi Flutter agar aplikasi yang dibuat konsisten? Apakah kamu mengimplementasikan tema pada aplikasi yang kamu buat?
    iya, pada main.dart memiliki tipe materialApp yaitu colorScheme agar aplikasi konsisten

5. Bagaimana cara kamu menangani navigasi dalam aplikasi dengan banyak halaman pada Flutter?
  caranya dengan menggunakan method push yaitu menambahkan route ke paling atas dengan menggunakan stack.kemudian,
  ada pop yaitu menghapus route yang paling atas dengan menggunakan stack
  
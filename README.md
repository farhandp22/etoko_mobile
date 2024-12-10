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
   - Text : untuk menamplikan teks pad aplikasi android
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
  
# Tugas 9

1. Jelaskan mengapa kita perlu membuat model untuk melakukan pengambilan ataupun pengiriman data JSON? Apakah akan terjadi error jika kita  tidak membuat model terlebih dahulu?
 karena dengan menggunakan model dapat mengubah json ke dalam  bentuk objek dari data json yang dapat ditampilkan di product_card dan jika tidak memakai model maka produk tidak dapat ditampilkan dan error
2.  Jelaskan fungsi dari library http yang sudah kamu implementasikan pada tugas ini?
    fungsi dari hhtp nya adalah untuk fetch data web service pada flutter
3. Jelaskan fungsi dari CookieRequest dan jelaskan mengapa instance CookieRequest perlu untuk dibagikan ke semua komponen di aplikasi Flutter.
     cookies request adalah  kelas yang dapat digunakan dalam flutter untuk mengelola permainan http dengan manipulasi cookie.instance cookierequest perlu dibagikan  ke semua komponen aplikasi  flutter karena cookies sering kali dibutuhkan untuk menjaga keadaan
     logi,sesi,atau informasi pengguna lainnya di aplikasi web.    
 4. Jelaskan mekanisme pengiriman data mulai dari input hingga dapat ditampilkan pada Flutter?
    Pertama, data JSON diambil melalui API atau dari penyimpanan lokal. Kemudian, Flutter menggunakan package seperti http untuk mengirim HTTP request dan mendapatkan JSON response dari server. Data JSON kemudian di-decode menggunakan library seperti dart:convert untuk mengubahnya menjadi objek Dart. Setelah data di-decode, nilai-nilai tersebut dapat digunakan dalam Flutter untuk mengisi widget, atau untuk meng-update state dan menampilkan informasi pada interface pengguna menggunakan widget.
 5. Jelaskan mekanisme autentikasi dari login, register, hingga logout. Mulai dari input data akun pada Flutter ke Django hingga selesainya proses autentikasi oleh Django dan tampilnya menu pada Flutter?
  - Buat instance CookieRequest menggunakan pbp_django_auth di Flutter dan simpan dalam variabel request
    final request = context.watch<CookieRequest>();
  - Pada halaman login.dart saat pengguna mengirimkan form, gunakan instance request untuk melakukan permintaan login ke server Django
  -final response = await request.login(
  "http://127.0.0.1:8000/auth/login/",
  {
    'username': username,
    'password': password
  }
);
 - Di server Django, proses permintaan login dalam views
    from django.http import JsonResponse
from django.views.decorators.csrf import csrf_exempt
from django.contrib.auth import authenticate, login as auth_login

@csrf_exempt
def login(request):
    username = request.POST['username']
    password = request.POST['password']
    user = authenticate(username=username, password=password)
    if user is not None:
        if user.is_active:
            auth_login(request, user)
            # Status login sukses.
            return JsonResponse({
                "username": user.username,
                "status": True,
                "message": "Login sukses!"
                # Tambahkan data lainnya jika ingin mengirim data ke Flutter.
            }, status=200)
        else:
            return JsonResponse({
                "status": False,
                "message": "Login gagal, akun dinonaktifkan."
            }, status=401)

    else:
        return JsonResponse({
            "status": False,
            "message": "Login gagal, periksa kembali email atau kata sandi."
        }, status=401)
 6. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step! (bukan hanya sekadar mengikuti tutorial).
  - TextField. Widget ini digunakan untuk menerima input teks dari pengguna, lebih tepatnya untuk menerima username dan password saat proses login dan registrasi.

    - SizedBox. Widget ini digunakan untuk memberikan ruang tertentu atau pemisah antara elemen-elemen dalam antarmuka pengguna, lebih tepatnya untuk memberikan jarak atau ruang antara widget TextField username dan password.

   -  ElevatedButton. Widget ini menciptakan tombol dengan efek elevasi yang terjadi saat tombol ditekan, lebih tepatnya sebagai tombol submit pada proses login dan registrasi, memicu aksi yang sesuai ketika ditekan.

    - TextButton. Widget ini menciptakan tombol berupa teks tanpa latar belakang, lebih tepatnya sebagai tombol registrasi, memberikan opsi alternatif selain login.

    - ListView.builder. Widget ini digunakan untuk membuat daftar item yang dapat discroll, lebih tepatnya untuk menampilkan daftar item yang ada, seperti daftar hasil pencarian atau item dalam kategori tertentu.

    - Text Widget. ini digunakan untuk menampilkan teks di antarmuka pengguna, lebih tepatnya untuk menampilkan teks detail saat item pada daftar item ditekan, memberikan informasi lebih lanjut tentang item tersebut.
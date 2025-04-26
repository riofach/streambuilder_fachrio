# streambuilder_fachrio

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

---

## Penjelasan Kode

### main.dart (P5: Jawaban Soal 12)

File ini adalah entry point aplikasi Flutter. Berikut penjelasan kode utamanya:

- **Import**: Mengimpor package Flutter, stream.dart, dan async.
- **main()**: Fungsi utama yang menjalankan aplikasi dengan `runApp(MyApp())`.
- **MyApp**: Widget utama yang membangun MaterialApp dengan tema ungu dan home ke `StreamHomePage`.
- **StreamHomePage**: StatefulWidget yang menyiapkan stream angka acak dari NumberStream.
- **initState()**: Menginisialisasi stream angka acak saat widget dibuat.
- **StreamBuilder**: Widget yang membangun ulang UI setiap kali ada data baru dari stream. Jika ada data, angka acak ditampilkan di tengah layar. Jika error, hanya mencetak error di konsol.

### stream.dart

File ini berisi kelas NumberStream yang menghasilkan stream angka acak:

- **NumberStream**: Kelas dengan method `getNumbers()` yang mengembalikan stream integer.
- **getNumbers()**: Menggunakan `Stream.periodic` untuk menghasilkan angka acak antara 0-9 setiap detik.
- **Random**: Digunakan untuk menghasilkan angka acak.

![1](./images/P512.gif)

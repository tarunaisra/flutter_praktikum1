# Praktikum 1 Flutter

## 1. Praktikum Text Widget
Menampilkan teks sederhana di tengah layar.

**Kode:**
```dart 
import 'package:flutter/material.dart';

class TextWidget extends StatelessWidget {
  const TextWidget({super.key});
  @override
  Widget build(BuildContext context) {
    return const Text(
      'Hello, World!',
      style: TextStyle(fontSize: 30, color: Colors.blue),
    ); //Text
  }
}
```

## OUTPUT.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/90bfdd66-d942-42ed-a430-e1a70df1c9a7" />




## 2. Praktikum Image Widget
Menampilkan gambar di tengah layar

**Kode:**
```dart 
import 'package:flutter/material.dart';

class ImageWidget extends StatelessWidget{
  const ImageWidget({super.key});

  @override
  Widget build(BuildContext context) {
    return Image.asset(
      'assets/images/muncak.jpg',
      width: 250,
      height: 250,
    );
  }
}
```
## OUTPUT.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/cbe04333-0265-497a-89a5-087cf871cd7d" />




## 3. Praktikum Kombinasi Image dan Text
Menggabungkan teks dan gambar logo Poliwangi dengan hasil template yang harus dikreasikan sendiri
```dart
import 'package:flutter/material.dart';

class Praktikum extends StatelessWidget {
  const Praktikum({super.key});

 @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.blue, 
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            const Text(
              "WELCOME",
              style: TextStyle(
                fontSize: 100,
                fontWeight: FontWeight.bold,
                color: Colors.white, 
              ),
            ),
            const SizedBox(height: 5),
            const Text(
              "Politeknik Negeri Banyuwangi",
              style: TextStyle(
                fontSize: 45,
                fontWeight: FontWeight.w600,
                color: Colors.white, 
              ),
            ),
            const SizedBox(height: 80),
            Image.asset(
              "assets/images/poliwangi_logo.jpg",
              width: 150,
            ),
          ],
        ),
      ),
    );
  }
}
```
Output :
* Background biru
* Teks "WELCOME" dan "Politeknik Negeri Banyuwangi" berwarna putih
* Logo Poliwangi di tengah
  <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0229a115-5067-4af7-8530-e684b3ae3dcd" />

## Tahapan Kombinasi Image dan Text
1. Menambahkan file logo Poliwangi ke folder images/
2. Mendaftarkan image pada pubspec.yaml
3. Membuat widget Column yang berisi Text dan Image
4. Menambahkan style pada Text agar lebih jelas
5. Memberikan Background biru pada Scaffold





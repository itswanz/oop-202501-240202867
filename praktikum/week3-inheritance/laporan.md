# Laporan Praktikum Minggu 3
Topik:Inheritance (Kategori Produk)

## Identitas
- Nama  : irwandi isnugroho
- NIM   : 240202867
- Kelas : 3IKKA

---

## Tujuan
Mahasiswa mampu menjelaskan konsep inheritance (pewarisan class) dalam OOP.
Mahasiswa mampu membuat superclass dan subclass untuk produk pertanian.
Mahasiswa mampu mendemonstrasikan hierarki class melalui contoh kode.
Mahasiswa mampu menggunakan super untuk memanggil konstruktor dan method parent class.
Mahasiswa mampu membuat laporan praktikum yang menjelaskan perbedaan penggunaan inheritance dibanding class tunggal.

---

## Dasar Teori
(Tuliskan ringkasan teori singkat (3–5 poin) yang mendasari praktikum.  
Contoh:  
1.Superclass: class induk yang mendefinisikan atribut umum.
2.Subclass: class turunan yang mewarisi atribut/method superclass, dan dapat menambahkan atribut/method baru.
3.super digunakan untuk memanggil konstruktor atau method superclass.

---

## Langkah Praktikum
1. Membuat Superclass Produk
Gunakan class Produk dari Bab 2 sebagai superclass.

2.Membuat Subclass
Benih.java → atribut tambahan: varietas.
Pupuk.java → atribut tambahan: jenis pupuk (Urea, NPK, dll).
AlatPertanian.java → atribut tambahan: material (baja, kayu, plastik).

3.Membuat Main Class
Instansiasi minimal satu objek dari tiap subclass.
Tampilkan data produk dengan memanfaatkan inheritance.

4.Menambahkan CreditBy
Panggil class CreditBy untuk menampilkan identitas mahasiswa.

5.Commit dan Push
Commit dengan pesan: week3-inheritance.

## Kode Program
Benih: Benih Padi IR64 Varietas: IR64
Pupuk: Pupuk Urea Jenis: Urea
Alat Pertanian: Cangkul Baja Material: Baja

credit by: <240202867> - <irwandi isnugroho>

Process finished with exit code 0

## Hasil Eksekusi
(Sertakan screenshot hasil eksekusi program.  
![Screenshot hasil](screenshots/hasil.png)
)
---

## Analisis
(
- Jelaskan bagaimana kode berjalan.  
- Apa perbedaan pendekatan minggu ini dibanding minggu sebelumnya.  
- Kendala yang dihadapi dan cara mengatasinya.  
)
---

## Kesimpulan
(Tuliskan kesimpulan dari praktikum minggu ini.  
Contoh: *Dengan menggunakan class dan object, program menjadi lebih terstruktur dan mudah dikembangkan.*)

---

## Quiz
1 Apa keuntungan menggunakan inheritance dibanding membuat class terpisah tanpa hubungan?
   Inheritance (pewarisan) adalah salah satu pilar utama Object-Oriented Programming (OOP), dan tujuannya adalah memanfaatkan kembali kode (code reuse) serta menjaga struktur yang terorganisir dan konsisten antar kelas.  

2.Bagaimana cara subclass memanggil konstruktor superclass?
   Dalam Python (dan bahasa OOP lain juga mirip konsepnya), subclass dapat memanggil konstruktor superclass menggunakan fungsi bawaan super().

3.Berikan contoh kasus di POS pertanian selain Benih, Pupuk, dan Alat Pertanian yang bisa dijadikan subclass.  
   hasil panen,palan ternak,pestisida,media tanam bibit buah

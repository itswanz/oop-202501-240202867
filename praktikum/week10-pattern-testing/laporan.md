# Laporan Praktikum Minggu 10 (sesuaikan minggu ke berapa?)
Topik: Design Pattern (Singleton, MVC) dan Unit Testing menggunakan JUnit

## Identitas
- Nama  : irwandi isnugroho
- NIM   : 240202867
- Kelas : 3IKKA

---

## Tujuan
Menjelaskan konsep dasar design pattern dalam rekayasa perangkat lunak.
Mengimplementasikan Singleton Pattern dengan benar.
Menjelaskan dan menerapkan Model–View–Controller (MVC) pada aplikasi sederhana.
Membuat dan menjalankan unit test menggunakan JUnit.
Menganalisis manfaat penerapan design pattern dan unit testing terhadap kualitas perangkat lunak.

---

## Dasar Teori
 Design Pattern
Design pattern adalah solusi desain yang telah teruji untuk menyelesaikan masalah umum dalam pengembangan perangkat lunak. Fokus minggu ini:

Singleton Pattern
MVC (Model–View–Controller)
2. Singleton Pattern
Tujuan: Menjamin suatu class hanya memiliki satu instance dan menyediakan titik akses global.

Karakteristik:

Constructor private
Atribut static instance
Method static getInstance()

---

## Langkah Praktikum
mplementasikan Singleton untuk DatabaseConnection.
Buat struktur MVC sederhana untuk fitur Product.
Buat minimal 1 unit test JUnit.
Jalankan unit test dan dokumentasikan hasilnya
---

## Kode Program
(Tuliskan kode utama yang dibuat, contoh:  

```java
// Contoh
Produk p1 = new Produk("BNH-001", "Benih Padi", 25000, 100);
System.out.println(p1.getNama());
```
)
---

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
(1. Mengapa constructor pada Singleton harus bersifat private?
   **Jawaban:** …  Constructor pada Singleton dibuat private agar tidak bisa dibuat objek baru dari luar class, sehingga hanya satu instance yang dapat dibuat dan digunakan di seluruh aplikasi.

2. Jelaskan manfaat pemisahan Model, View, dan Controller.
   **Jawaban:** …  Pemisahan Model, View, dan Controller (MVC) membuat kode lebih terstruktur, mudah dirawat, dan perubahan tampilan atau logika tidak saling memengaruhi.

3. Apa peran unit testing dalam menjaga kualitas perangkat lunak?
   **Jawaban:** …  )Unit testing berperan untuk memastikan tiap bagian kode berjalan benar, mendeteksi bug lebih awal, dan menjaga kualitas perangkat lunak saat terjadi perubahan kode.
4.Apa risiko jika Singleton tidak diimplementasikan dengan benar?
Jika Singleton tidak diimplementasikan dengan benar, bisa terjadi lebih dari satu instance, inkonsistensi data, dan bug sulit dilacak, terutama pada aplikasi multithreading.


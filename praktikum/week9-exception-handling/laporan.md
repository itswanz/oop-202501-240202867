# Laporan Praktikum Minggu 9
Topik: Exception Handling, Custom Exception, dan Penerapan Design Pattern

## Identitas
- Nama  : Irwandi isnugroho
- NIM   : 240202867
- Kelas : 3IKKA

---

## Tujuan
Menjelaskan perbedaan antara error dan exception.
Mengimplementasikan try–catch–finally dengan tepat.
Membuat custom exception sesuai kebutuhan program.
Mengintegrasikan exception handling ke dalam aplikasi sederhana (kasus keranjang belanja).
(Opsional) Menerapkan design pattern sederhana (Singleton/MVC) dan unit testing dasar.

---

## Dasar Teori
. Error vs Exception
Error → kondisi fatal, tidak dapat ditangani (contoh: OutOfMemoryError).
Exception → kondisi tidak normal yang dapat ditangani oleh program.
 Struktur try–catch–finally
 Membuat Custom Exception
---

## Langkah Praktikum
 Membuat Custom Exception
 Model Product dengan Stok
 Implementasi ShoppingCart dengan Exception Handling
  Main Program untuk Menguji Exception Handling
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
(1.Jelaskan perbedaan error dan exception.
   **Jawaban:** …  
   Error: Masalah serius dari sistem/JVM yang tidak bisa atau jarang ditangani program (misalnya OutOfMemoryError).

Exception: Kesalahan saat runtime yang masih bisa ditangani oleh program (misalnya NullPointerException).

2.Apa fungsi finally dalam blok try–catch–finally?
   **Jawaban:** …  finally digunakan untuk menjalankan kode yang pasti dieksekusi setelah try–catch, baik terjadi exception maupun tidak, biasanya untuk menutup resource seperti file atau koneksi.

3. Mengapa custom exception diperlukan?
   **Jawaban:** …  )Custom exception diperlukan agar kesalahan lebih spesifik dan mudah dipahami, serta memungkinkan penanganan error yang sesuai dengan logika aplikasi.
4.Berikan contoh kasus bisnis dalam POS yang membutuhkan custom exception.
pada POS, saat kasir menjual barang tetapi stok tidak mencukupi, sistem melempar custom exception seperti StokTidakCukupException agar transaksi dibatalkan dengan pesan yang jelas.

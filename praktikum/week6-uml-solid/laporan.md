# Laporan Praktikum Minggu 6
Topik: uml solid

## Identitas
- Nama  : irwandi isnugroho
- NIM   : 240202867
- Kelas : 3IKKA

---

## Tujuan
Mahasiswa mampu mengidentifikasi kebutuhan sistem ke dalam diagram UML.
Mahasiswa mampu menggambar UML Class Diagram dengan relasi antar class yang tepat.
Mahasiswa mampu menjelaskan prinsip desain OOP (SOLID).
Mahasiswa mampu menerapkan minimal dua prinsip SOLID dalam kode program.

---

## Dasar Teori
Functional Requirements
Manajemen Produk Sistem dapat menambah, mengubah, menghapus, dan menampilkan data produk pertanian (benih, pupuk, alat, obat). Produk memiliki atribut: kode, nama, kategori, harga, dan stok.

Transaksi Penjualan Kasir dapat membuat transaksi baru, menambahkan produk ke keranjang, menghitung total, dan menyelesaikan pembayaran.

Metode Pembayaran Sistem mendukung pembayaran tunai dan e-wallet. Di masa depan, metode lain seperti transfer bank harus dapat ditambahkan tanpa mengubah kode lama.

Pencetakan Struk dan Laporan Setelah pembayaran berhasil, sistem menampilkan atau mencetak struk. Admin dapat melihat laporan penjualan harian atau periodik.

Login dan Hak Akses Kasir dan admin memiliki hak akses berbeda (kasir untuk transaksi, admin untuk produk dan laporan).

. Non-Functional Requirements
Maintainability – Struktur kode mengikuti prinsip Single Responsibility dan Dependency Inversion.
Extensibility – Penambahan fitur baru tidak mengubah class inti (Open/Closed).
Reusability – Menggunakan interface dan abstraksi agar mudah diuji.
Consistency – Penamaan dan dokumentasi konsisten antar komponen.
Documentability – Semua desain didokumentasikan dalam empat diagram UML.
---

## Langkah Praktikum
membuat folder di dalam src bernama png masuk ke draw.io untuk membuat isi dari folder tersebut 
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
(1.Jelaskan perbedaan aggregation dan composition serta berikan contoh penerapannya pada desain Anda.
   **Jawaban:** …  Dalam dunia Object-Oriented Programming (OOP) dan perancangan sistem menggunakan UML, Aggregation dan Composition adalah dua bentuk khusus dari Association. Keduanya menggambarkan hubungan "has-a" (memiliki), namun perbedaan utamanya terletak pada siklus hidup (lifecycle) objeknya.

2. Bagaimana prinsip Open/Closed dapat memastikan sistem mudah dikembangkan?
   **Jawaban:** …  Prinsip Open/Closed (bagian dari SOLID) menyatakan bahwa sebuah perangkat lunak harus terbuka untuk perluasan (open for extension) tetapi tertutup untuk modifikasi (closed for modification)

3.Mengapa Dependency Inversion Principle (DIP) meningkatkan testability? Berikan contoh penerapannya.
   **Jawaban:** …  Dependency Inversion Principle (DIP) meningkatkan testability karena ia mengurangi ketergantungan langsung (tight coupling) antara kode bisnis dan implementasi konkret, sehingga mudah mengganti dependensi dengan mock/stub saat testing.)

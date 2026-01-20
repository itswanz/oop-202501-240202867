# Laporan Praktikum Minggu 1 (sesuaikan minggu ke berapa?)
Topik: [Tuliskan judul topik, misalnya "Class dan Object"]

## Identitas
- Nama  : irwandi isnugroho 
- NIM   : 240202867
- Kelas : IKKA

---

## Tujuan
Mahasiswa mampu menjelaskan konsep polymorphism dalam OOP.
Mahasiswa mampu membedakan method overloading dan overriding.
Mahasiswa mampu mengimplementasikan polymorphism (overriding, overloading, dynamic binding) dalam program.
Mahasiswa mampu menganalisis contoh kasus polymorphism pada sistem nyata (Agri-POS).

---

## Dasar Teori
Overloading → mendefinisikan method dengan nama sama tetapi parameter berbeda.
Overriding → subclass mengganti implementasi method dari superclass.
Dynamic Binding → pemanggilan method ditentukan saat runtime, bukan compile time

---

## Langkah Praktikum
Overloading

Tambahkan method tambahStok(int jumlah) dan tambahStok(double jumlah) pada class Produk.
Overriding

Tambahkan method getInfo() pada superclass Produk.
Override method getInfo() pada subclass Benih, Pupuk, dan AlatPertanian.
Dynamic Binding

Buat array Produk[] daftarProduk yang berisi objek Benih, Pupuk, dan AlatPertanian.
Loop array tersebut dan panggil getInfo(). Perhatikan bagaimana Java memanggil method sesuai jenis objek aktual.
Main Class

Buat MainPolymorphism.java untuk mendemonstrasikan overloading, overriding, dan dynamic binding.
CreditBy

Tetap panggil CreditBy.print("<NIM>", "<Nama>").
Commit dan Push

Commit dengan pesan: week4-polymorphism.

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
(1. Apa perbedaan overloading dan overriding? 
   **Jawaban:** …  
    Membuat beberapa method dengan nama yang sama dalam satu class, tapi parameter berbeda.
2. Bagaimana Java menentukan method mana yang dipanggil dalam dynamic binding?  
   **Jawaban:** …  
Dalam dynamic binding (late binding) di Java, method yang dipanggil ditentukan saat runtime berdasarkan objek sebenarnya, bukan tipe referensinya.
3. Berikan contoh kasus polymorphism dalam sistem POS selain produk pertanian.
   **Jawaban:** …  
   Menjual berbagai jenis pembayaran dengan cara proses yang berbeda, tapi dipanggil dengan interface yang sama.

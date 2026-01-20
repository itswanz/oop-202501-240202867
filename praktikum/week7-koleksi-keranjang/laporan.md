# Laporan Praktikum Minggu 7
Topik: Collections dan Implementasi Keranjang Belanja

## Identitas
- Nama  : irwandi isnugroho
- NIM   : 240202867
- Kelas : [3IKKA

---

## Tujuan
Menjelaskan konsep collection dalam Java (List, Map, Set).
Menggunakan ArrayList untuk menyimpan dan mengelola objek.
Mengimplementasikan Map atau Set sesuai kebutuhan pengelolaan data.
Melakukan operasi dasar pada collection: tambah, hapus, dan hitung total.
Menganalisis efisiensi penggunaan collection dalam konteks sistem Agri-POS.

---

## Dasar Teori

---List (implementasi: ArrayList) — Terurut, dapat menyimpan elemen duplikat.
Map (implementasi: HashMap) — Menyimpan pasangan key–value, akses cepat berdasarkan key.
Set (implementasi: HashSet) — Tidak menerima duplikat dan tidak mempertahankan urutan.

## Langkah Praktikum
 Membuat Class Product
 Implementasi Keranjang dengan ArrayList
 Main Program 
 Implementasi Alternatif Menggunakan Map (Dengan Quantity)

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
(1.Jelaskan perbedaan mendasar antara List, Map, dan Set.
   **Jawaban:** …  
List: Koleksi elemen berurutan, punya index, dan boleh duplikat.

Set: Koleksi elemen unik, tanpa index, dan tidak boleh duplikat.

Map: Struktur key–value, key unik, value boleh sama.

2.Mengapa ArrayList cocok digunakan untuk keranjang belanja sederhana?
  ArrayList cocok untuk keranjang belanja sederhana karena menyimpan data berurutan, boleh duplikat (produk sama bisa dibeli lebih dari satu), dan mudah diakses serta ditambah/dihapus. 

3.Bagaimana struktur Set mencegah duplikasi data? 
   Set mencegah duplikasi data dengan mengecek kesamaan elemen (menggunakan equals() dan hashCode()) sehingga elemen yang sama tidak ditambahkan dua kali.
4.Kapan sebaiknya menggunakan Map dibandingkan List? Jelaskan dengan contoh.
Map digunakan dibandingkan List saat data perlu diakses berdasarkan key unik, bukan urutan.
Contoh: menyimpan kode produk → nama produk, misalnya {"P001" → "Beras"}, lebih tepat memakai Map daripada List.

# Laporan Praktikum Minggu 1 (sesuaikan minggu ke berapa?)
Topik:abstraction_interface

## Identitas
- Nama  : irwandi isnugroho
- NIM   : 240202867
- Kelas : 3IKKA

---

## Tujuan
Mahasiswa mampu menjelaskan perbedaan abstract class dan interface.
Mahasiswa mampu mendesain abstract class dengan method abstrak sesuai kebutuhan kasus.
Mahasiswa mampu membuat interface dan mengimplementasikannya pada class.
Mahasiswa mampu menerapkan multiple inheritance melalui interface pada rancangan kelas.
Mahasiswa mampu mendokumentasikan kode (komentar kelas/method, README singkat pada folder minggu).

---

## Dasar Teori
Abstract class: tidak dapat diinstansiasi, dapat memiliki method abstrak (tanpa badan) dan non-abstrak. Dapat menyimpan state (field).
Interface: kumpulan kontrak (method tanpa implementasi konkret). Sejak Java 8 mendukung default method. Mendukung multiple inheritance (class dapat mengimplementasikan banyak interface).
Gunakan abstract class bila ada shared state dan perilaku dasar; gunakan interface untuk mendefinisikan kemampuan/kontrak lintas hierarki.
Dalam konteks Agri-POS, Pembayaran dapat dimodelkan se
---

## Langkah Praktikum
Abstract Class – Pembayaran

Buat Pembayaran (abstract) dengan field invoiceNo, total dan method:
double biaya() (abstrak) → biaya tambahan (fee).
boolean prosesPembayaran() (abstrak) → mengembalikan status berhasil/gagal.
double totalBayar() (konkrit) → return total + biaya();.
Subclass Konkret

Cash → biaya = 0, proses = selalu berhasil jika tunai >= totalBayar().
EWallet → biaya = 1.5% dari total; proses = membutuhkan validasi.
Interface

Validatable → boolean validasi(); (contoh: OTP).
Receiptable → String cetakStruk();
Multiple Inheritance via Interface

EWallet mengimplementasikan dua interface: Validatable, Receiptable.
Cash setidaknya mengimplementasikan Receiptable.
Main Class

Buat MainAbstraction.java untuk mendemonstrasikan pemakaian Pembayaran (polimorfik).
Tampilkan hasil proses dan struk. Di akhir, panggil CreditBy.print("[NIM]", "[Nama]").
Commit dan Push

Commit dengan pesan: week5-abstraction-interface.

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
(1.Jelaskan perbedaan konsep dan penggunaan abstract class dan interface.
   **Jawaban:** …  Abstract class adalah class yang:

Tidak bisa diinstansiasi

Digunakan sebagai kelas dasar (base class)

Bisa punya method abstrak dan non-abstrak

Cocok untuk relasi “is-a” yang kuat

Interface adalah:

Kontrak perilaku

Berisi method yang harus diimplementasikan

Fokus ke apa yang bisa dilakukan, bukan bagaimana

2.Mengapa multiple inheritance lebih aman dilakukan dengan interface pada Java? 
   **Jawaban:** …  
Multiple inheritance lebih aman menggunakan interface di Java karena menghindari konflik implementasi dan ambiguitas, sekaligus menjaga desain tetap sederhana dan terkontrol
3.Pada contoh Agri-POS, bagian mana yang paling tepat menjadi abstract class dan mana yang menjadi interface? Jelaskan alasannya.
   **Jawaban:** …  )
   Abstract class → entitas inti yang punya data & perilaku dasar

Interface → fitur / kemampuan / kontrak yang bisa dipakai banyak entitas

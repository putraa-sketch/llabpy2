# Laporan Praktikum 2

## KASUS 1 : PROGRAM PEMESANAN TIKET BIOSKOP
Repository ini berisi program Python sederhana untuk menghitung harga tiket bioskop. Program ini memperhitungkan jenis tiket (Reguler atau VIP) dan memberikan diskon 20% untuk pengguna yang memiliki kartu member.

### Deskripsi Program
Program pemesanan tiket bioskop ini bertujuan untuk menghitung total harga tiket berdasarkan pilihan pengguna:
Tiket Reguler seharga Rp50.000
Tiket VIP seharga Rp100.000
Pengguna dengan kartu member mendapatkan diskon sebesar 20%.
Program akan meminta pengguna untuk memasukkan:

Tipe tiket (Reguler atau VIP).
Status member (Ya atau Tidak).
Kemudian, program akan menampilkan total harga yang harus dibayar.

### Algoritma
Berikut langkah-langkah dari algoritma program ini:

Program meminta pengguna untuk memilih tipe tiket: Reguler atau VIP.

Program meminta pengguna untuk mengonfirmasi apakah mereka memiliki kartu member.

Berdasarkan tipe tiket, program menetapkan harga awal.

Jika pengguna memiliki kartu member, program mengurangi harga dengan diskon sebesar 20%.

Program menampilkan total harga yang harus dibayar.
```phython
# Program Pemesanan Tiket Bioskop

# Harga tiket
harga_reguler = 50000
harga_vip = 100000

# Input tipe tiket
tipe_tiket = input("Masukkan tipe tiket (reguler/vip): ").lower()

# Input status member
status_member = input("Apakah Anda memiliki kartu member? (ya/tidak): ").lower()

# Hitung harga tiket
if tipe_tiket == "reguler":
    total_harga = harga_reguler
elif tipe_tiket == "vip":
    total_harga = harga_vip
else:
    print("Tipe tiket tidak valid.")
    total_harga = 0

# Cek status member dan berikan diskon jika berlaku
diskon = 0.2 if status_member == "ya" else 0
harga_final = total_harga * (1 - diskon)

# Tampilkan hasil
if total_harga > 0:
    print(f"Total harga yang harus dibayar: Rp{harga_final:.2f}")


```
# KASUS 2 : KALKULATOR SEDERHANA
Repository ini juga mencakup program Kalkulator Sederhana yang dapat melakukan operasi aritmatika dasar. Program ini memungkinkan pengguna untuk memasukkan dua angka dan memilih jenis operasi (penjumlahan, pengurangan, perkalian, atau pembagian) yang akan diterapkan pada kedua angka tersebut.

Deskripsi Program
Kalkulator ini mendukung empat operasi aritmatika:

1.Penjumlahan (+)

2.Pengurangan (-)

3.Perkalian (*)

4.Pembagian (/)

Pengguna akan diminta untuk memasukkan dua angka dan operator aritmatika. Program kemudian akan menampilkan hasil dari operasi yang dipilih. Program ini juga menangani pembagian dengan nol dan akan memberikan pesan peringatan jika pembagian tidak bisa dilakukan.

Algoritma
Berikut langkah-langkah dari algoritma program kalkulator sederhana ini:

Program meminta pengguna untuk memasukkan angka pertama.

Program meminta pengguna untuk memasukkan operator aritmatika yang ingin digunakan (+, -, *, atau /).

Program meminta pengguna untuk memasukkan angka kedua.

Berdasarkan operator yang dimasukkan, program melakukan operasi aritmatika pada kedua angka.

Jika operasi adalah pembagian dan angka kedua adalah nol, program menampilkan pesan bahwa pembagian dengan nol tidak dapat dilakukan.

Program menampilkan hasil dari operasi yang dipilih atau pesan error jika operator tidak valid.

```phython
# Program Kalkulator Sederhana

# Input dua angka dan satu operator
angka1 = float(input("Masukkan angka pertama: "))
angka2 = float(input("Masukkan angka kedua: "))
operator = input("Masukkan operator (+, -, *, /): ")

# Hitung hasil sesuai operator
if operator == "+":
    hasil = angka1 + angka2
elif operator == "-":
    hasil = angka1 - angka2
elif operator == "*":
    hasil = angka1 * angka2
elif operator == "/":
    if angka2 != 0:
        hasil = angka1 / angka2
 else:
        hasil = "Error: Pembagian dengan nol!"
else:
    hasil = "Operator tidak valid!"

# Tampilkan hasil
print(f"Hasil: {hasil}")
```
## Flowchart
### Hasil Flowchart dari kalkulator sederhana
* (https://drive.google.com/file/d/1fjQ7IWAJ2fgd_7RDQHTiySmSI3PsXLdI/view?usp=drive_link)
### Hasil dari flowchart pemesanan tiket bioskop
* (https://drive.google.com/file/d/1OjZbS3oDoRj4h3CNE1jPvPSFm_bNJ0Ba/view?usp=drive_link)

## Screenshot Hasil Eksekusi Program
### Pembelian tiket bioskop
(![Screenshot 2024-10-28 125629](https://github.com/user-attachments/assets/09f158f9-5b9a-4aef-a5ba-d19ec8147f3e))
### Hasil
(![Screenshot 2024-10-28 152427](https://github.com/user-attachments/assets/d5f394ec-9dba-48fb-bf10-2c0cca9f6581))
## Kalkulator sederhana
(![Screenshot 2024-10-28 ](https://github.com/user-attachments/assets/7faf60b0-2c21-43fa-a83d-d4a760b2d1a5))
#### Hasil
(![Screenshot 2024-10-28 152427](https://github.com/user-attachments/assets/73b2cf4d-f176-433c-ac05-9dfb6e48be8c))
## Kesimpulan dari Tugas Pemrograman
Program Pemesanan Tiket Bioskop:

Program ini dirancang untuk menghitung total harga tiket bioskop berdasarkan tipe tiket (reguler atau VIP) dan status keanggotaan pengguna (member atau non-member).
Dengan menggunakan struktur kontrol if-else, program dapat menentukan harga tiket dan menerapkan diskon jika pengguna adalah member.
Flowchart yang dibuat memberikan gambaran visual yang jelas tentang alur logika program, memudahkan pemahaman proses yang terjadi.
Program Kalkulator Sederhana:

Program ini menerima dua angka dan operator aritmatika, kemudian melakukan perhitungan sesuai dengan operator yang dipilih oleh pengguna.
Struktur if-elif-else digunakan untuk menentukan operasi yang akan dilakukan berdasarkan input pengguna.
Flowchart berfungsi untuk menjelaskan langkah-langkah dalam proses kalkulasi, dari pengambilan input hingga pengeluaran hasil.
### Manfaat:
Visualisasi: Flowchart membantu dalam memahami logika program secara keseluruhan, menjadikan debugging dan pengembangan lebih mudah.

Penguasaan Logika Pemrograman: Tugas ini memperkuat pemahaman mengenai penggunaan struktur kontrol, input/output, serta perhitungan matematis dalam pemrograman.

Penerapan Algoritma: Mengasah keterampilan dalam merancang algoritma yang efisien dan mudah dipahami, serta menerjemahkannya ke dalam kode.
### Langkah Selanjutnya:
Melakukan pengujian lebih lanjut untuk memastikan keandalan dan ketahanan program.
Menerapkan fitur tambahan, seperti pemilihan waktu tayang dan jumlah tiket untuk program pemesanan tiket.
Menambahkan lebih banyak operator atau fungsi dalam kalkulator sederhana untuk meningkatkan fungsionalitasnya.
Dengan menyelesaikan tugas ini, pengguna tidak hanya mendapatkan keterampilan teknis dalam pemrograman Python tetapi juga belajar cara merancang dan memahami algoritma serta alur program dengan lebih baik.

## Penulisan Sintaks While
Kita bisa memulai dengan cara berikut:
```bash
 while <kondisi>:
  # blok kode yang akan diulang-ulang
```
  ## PERULANGAN TANPA BATAS
  Perulangan while **sangat berkaitan** dengan variabel boolean, atau *logical statement*. Karena penentuan **kapan suatu blok kode akan diulang-ulang** ditinjau dari True or False dari suatu pernyataan logika.
  Sehingga jika suatu kondisi itu selalu benar, maka perulangannya pun akan selalu di eksekusi.
## PROGRAM SEDERHANA UNTUK MENAMBAHKAN DATA KEDALAM SEBUAH LIST DENGAN RINCIAN BERIKUT :
1. Progam meminta memasukkan data sebanyak-banyaknya (gunakan perulangan)
2. Tampilkan pertanyaan untuk menambah data (y/t?), apabila jawaban t (Tidak), maka program akan menampilkan 3.daftar datanya.
3. Nilai Akhir diambil dari perhitungan 3 komponen nilai (tugas: 30%, uts: 35%, uas: 35%)
## Alur dan Penjelasan program tersebut
1. Pastikan kita mempunya software pycharm atau vscode, jika belum anda bisa download Pycharm atau VSCode
2. Instalasi salah satu software tersebut hingga selesai, lalu buka
3. Jika sudah semua masukan kodingan seperti dibawah ini
```bash 
print("Masukan Data Mahasiswa")
data =[]
while True :
   nama       = input    ("Nama        : ")
   nim        = input    ("NIM         : ")
   tugas      = int(input("Nilai Tugas : "))
   uts        = int(input("Nilai UTS   : "))
   uas        = int(input("Nilai UAS   : "))
   nilaiakhir = float(tugas)*30/100+(uts)*35/100+(uas)*35/100
   data.append([nama,nim,tugas,uts,uas,nilaiakhir])
   lagi= input("Tambah data (y/t)? ")
   if lagi.lower() =="t":
       break
print("=====================================================================================")
print("|  No  |     Nama     |     NIM     |   Tugas   |   UTS   |   UAS   |  Nilai Akhir  |")
print("=====================================================================================")
i=0
for x in data:
   i+=1
   print("|  {6:2}  |  {0:10}  |  {1:9}  |  {2:7}  |  {3:5}  | {4:6}  |  {5:11.2f}  |"\
         .format (x[0][:9] , x[1][:9],x[2],x[3],x[4],x[5], i))
print("=====================================================================================")
```
![image](https://user-images.githubusercontent.com/115879313/212945624-486d0c96-c63f-4ba2-9861-561e567a5849.png)
4. Lalu save dan Run program tersebut, maka akan keluar hasil

5. Input data list tersebut terserah yang kita mau, maka akan keluar hasil seperti dibawah ini

![image](https://user-images.githubusercontent.com/115879313/212945762-03e71682-dc30-49dc-820d-3620f55afa96.png)
# Penjelasan
1. Membuat list bernama data[]
2. lalu menggunakan perulangan while While True : Jika benar maka akan menjalankan kodingan selanjutnya yaitu menginput data-data
3. Untuk ```bash nama ``` dan ```bash nim ``` kita menggunakan fungsi input biasa
3. Untuk ```nama ``` dan ```nim ``` kita menggunakan fungsi input biasa
4. Untuk ```bash tugas,uts dan uas ``` kita menggunakan fungsi int untuk menjadikannya integer
4. Untuk ```tugas,uts dan uas ``` kita menggunakan fungsi int untuk menjadikannya integer
5. Dibagian nilaiakhir kita menggunakan fungsi ```bash float ``` karena dapat digunakan sebagai argumen dan dapat juga melakukan operasi hitung secara langsung di dalam fungsi dengan bilangan bertipe integer atau sesama float.
5. Dibagian nilaiakhir kita menggunakan fungsi ```float ``` karena dapat digunakan sebagai argumen dan dapat juga melakukan operasi hitung secara langsung di dalam fungsi dengan bilangan bertipe integer atau sesama float.
6. Membuat kondisi dimana ingin ```bash Tambah Data (y/t)? ``` jika ```bash y ``` maka kondisi true dan akan mengulang ke awal untuk iput data selanjutnya. Jika ```bash t ``` maka kondisi akan break, dan apabila kondisi break maka otomatis mengikuti syntax yang berada di luar perulangan seperti contoh yang ada diatas membuat list dengan rapih menggunakan kondisi string.format
6. Membuat kondisi dimana ingin ```Tambah Data (y/t)? ``` jika ```bash y ``` maka kondisi true dan akan mengulang ke awal untuk iput data selanjutnya. Jika ```t ``` maka kondisi akan break, dan apabila kondisi break maka otomatis mengikuti syntax yang berada di luar perulangan seperti contoh yang ada diatas membuat list dengan rapih menggunakan kondisi string.format
7. Penjelasan Kondisional dan Perulangan bisa anda akses [disini](https://drive.google.com/file/d/103JBAxfEujCQ9pBUfe3mM8cJo6-CEcET/view)

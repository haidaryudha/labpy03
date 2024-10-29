# Table of content

# laporan Praktikum 3
## Latihan 1: Code Program Bilangan Acak
```python
import random

n = int(input("masukkan nilai N: "))
count = 0

while count < n:
   angka = random.random()
   if angka <0.5:
      count += 1
      print(f"data ke-{count} => {angka}")

print("selesai")
```

### Step 1: Import Library
```python
import random
```
Penjelasan: Kode ini mengimpor modul random, yang menyediakan fungsi untuk menghasilkan angka acak.

### Step 2: Input Nilai N
```python
n = int(input("masukkan nilai N: "))
```
Penjelasan: Program meminta pengguna untuk memasukkan nilai integer yang akan disimpan dalam variabel n. Ini akan menentukan berapa banyak angka acak yang akan dihasilkan.

### Step 3: Inisialisasi Variabel count
```python
count = 0
```
Penjelasan: Variabel count diinisialisasi dengan nilai 0. Variabel ini digunakan untuk menghitung berapa banyak angka yang telah dihasilkan yang memenuhi syarat tertentu.

### Step 4: Loop While
```python
while count < n:
```
Penjelasan: Program memasuki loop while, yang akan terus berjalan selama nilai count kurang dari n. Ini berarti loop akan berhenti setelah n angka acak yang memenuhi syarat telah dihasilkan.

### Step 5: Menghasilkan Angka Acak
```python
angka = random.random()
```
Penjelasan: Di dalam loop, program menghasilkan angka acak antara 0 dan 1 menggunakan random.random() dan menyimpannya dalam variabel angka.

### Step 6: Memeriksa kondisi
```python
if angka < 0.5:
```
Program memeriksa apakah angka yang dihasilkan kurang dari 0.5. Jika iya, maka langkah-langkah berikutnya akan dilakukan.

### Step 7: Mengupdate Count dan Mencetak Hasil
```python
count += 1
print(f"data ke-{count} => {angka}")
```
Jika angka kurang dari 0.5, count akan ditambahkan 1. Kemudian, program mencetak nilai dari count dan angka acak yang dihasilkan.

### Step 8: Mencetak Pesan Selesai
```python
print("selesai")
```
Setelah loop selesai (ketika count mencapai n), program mencetak pesan "selesai" untuk menandakan bahwa proses telah selesai.

### Test Program

![gambar1](https://github.com/user-attachments/assets/fb844bf2-dffe-486a-983e-e28c61688331)




## Latihan 3: code Program ATM Sederhana
```python
saldo = 2_000_000

while True:
    print(f"\nsaldo saat ini: Rp {saldo}")
    print("1. Tarik Tunai")
    print("2. Keluar")

    pilihan = input("Pilih menu (1/2): ")

    if pilihan == "1":
        jumlah = int(input("Masukkan Jumlah Penarikan: "))

        if jumlah <= saldo:
            saldo -= jumlah
            print("Penarikan Berhasil!")
        else:
            print("Saldo Tidak Mencukupi!")

    elif pilihan == "2":
        print("Terimakasih Telah Menggunakan ATM ACB!")   
        break
    else:
        print("Pilihan Tidak Valid! Silahkan Pilih 1 Atau 2.")     
```

### Step 1: Inisialisasi Saldo
```python
saldo = 2_000_000
```
Variabel saldo diinisialisasi dengan nilai 2.000.000. Ini adalah jumlah uang yang tersedia untuk ditarik.

### Step 2: Infinite Loop (Loop Tak Terbatas)
```python
while True:
``` 
Loop ini akan berjalan terus-menerus sampai ada perintah break untuk menghentikannya. Ini memungkinkan pengguna untuk melakukan beberapa transaksi tanpa harus menjalankan ulang program.

### Step 3: Menampilkan Saldo dan Menu
```python
print(f"\nsaldo saat ini: Rp {saldo}")
print("1. Tarik Tunai")
print("2. Keluar")
``` 
Program mencetak saldo saat ini dan menampilkan menu dengan dua pilihan: "Tarik Tunai" dan "Keluar".

### Step 4: Menerima Pilihan Pengguna
```python
pilihan = input("Pilih menu (1/2): ")
``` 
Program meminta pengguna untuk memasukkan pilihan menu (1 atau 2).

### Step 5: Memproses Pilihan Tarik Tunai
```python
if pilihan == "1":
    jumlah = int(input("Masukkan Jumlah Penarikan: "))
``` 
Jika pengguna memilih "1", program akan meminta pengguna untuk memasukkan jumlah uang yang ingin ditarik.

### Step 6: Validasi Jumlah Penarikan
```python
if jumlah <= saldo:
    saldo -= jumlah
    print("Penarikan Berhasil!")
else:
    print("Saldo Tidak Mencukupi!")
```
Program memeriksa apakah jumlah yang diminta untuk ditarik kurang dari atau sama dengan saldo yang tersedia.

* Jika ya, saldo dikurangi dengan jumlah yang ditarik, dan program mencetak "Penarikan Berhasil!".
* Jika tidak, program mencetak "Saldo Tidak Mencukupi!".

### Step 7: Memproses Pilihan Keluar
```python
elif pilihan == "2":
    print("Terimakasih Telah Menggunakan ATM ACB!")   
    break
```
Jika pengguna memilih "2", program mencetak pesan terima kasih dan menggunakan break untuk keluar dari loop, sehingga program selesai.

### Step 8: Menangani Pilihan Tidak Valid
```python
else:
    print("Pilihan Tidak Valid! Silahkan Pilih 1 Atau 2.")
```
Jika pengguna memasukkan pilihan yang tidak valid (selain 1 atau 2), program mencetak pesan yang meminta pengguna untuk memilih menu yang benar.

### Step 9: Test Program

![Screenshot 2024-10-29 220222](https://github.com/user-attachments/assets/1e18e826-620d-4ad4-a125-f9a3ecdc57f0)



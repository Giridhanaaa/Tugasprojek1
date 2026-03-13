# Tugasprojek1
sistem sederhana pengelolaan nilai mahasiswa menggunakan array

# 1. Penjelasan Konsep Array 🎯

Array adalah struktur data yang digunakan untuk menyimpan sekumpulan data dengan tipe yang sama dalam satu variabel. Setiap elemen dalam array memiliki indeks yang digunakan untuk mengakses data tersebut. 

Dalam bahasa pemrograman Python, array sering diimplementasikan menggunakan list. List memungkinkan kita menyimpan banyak nilai dalam satu variabel dan mengaksesnya atau memanggilnya nanti menggunakan indeks.

Contoh array di Python
```python
angka = [10, 20, 30, 40, 50]
print(angka[0])

output = 10
```
- "angka" adalah array
- "10, 20, 30, 40, 50" adalah elemen array
- "angka[0]" mengakses elemen pertama pada array yaitu 10

# 2. Hasil Screenshot Program dan Hasil Eksekusi 📷
Pada program ini, array digunakan untuk menyimpan nilai 10 mahasiswa dan kemudian dilakukan proses:
- Menampilkan nilai tertinggi
- Menampilkan nilai terendah
- Menghitung rata-rata nilai
- Menghitung jumlah mahasiswa lulus, dengan kondisi (nilai >=60)
- Menampilkan grafik nilai
- Menampilkan grafik kelulusan

## Gambar 1 (Code 1 dan 2)
![alt text](https://github.com/Giridhanaaa/Tugasprojek1/blob/main/screenshot/ss1dan2.png?raw=true)

## Gambar 2 (Code 3)
![alt text](https://github.com/Giridhanaaa/Tugasprojek1/blob/main/screenshot/ss3.png?raw=true)

## Gambar 3 (Code 4)
![alt text](https://github.com/Giridhanaaa/Tugasprojek1/blob/main/screenshot/ss4.png?raw=true)

## Gambar 4 (Code 5)
![alt text](https://github.com/Giridhanaaa/Tugasprojek1/blob/main/screenshot/ss5.png?raw=true)

# 3. Analisis Kompleksitas🧲
.

---

## ⚙️ 1️. Input 10 nilai mahasiswa

Biasanya akan menggunakan perulangan seperti

```python
for i in range(10):
    nilai = int(input())
    arr.append(nilai)
```

Nantinya Program akan membaca setiap nilai satu per satu.

Maka Kompleksitasnya adalah:

```
O(n)
```

karena harus melakukan input sebanyak **n kali**


## ⚙️ 2️. Nilai terendah, tertinggi, dan rata-rata

Biasanya menggunakan

```python
max(arr)
min(arr)
sum(arr)
```

Dimana semua fungsi ini harus memeriksa seluruh elemen pada array.

Maka Kompleksitasnya adalah:

```
O(n)
```

karena setiap nilai harus diperiksa.

Walaupun ada 3 operasi (max, min, sum), akan tetap dianggap O(n) karena konstanta tidak mempengaruhi kompleksitas.



## ⚙️ 3️. Mahasiswa yang lulus dan tidak

Biasanya menggunakan

```python
for n in arr:
    if n >= 60:
        lulus += 1
```

Program akan mengecek setiap nilai yang ada dalam array.

Maka Kompleksitasnya adalah:

```
O(n)
```


## ⚙️ 4️. Grafik nilai tertinggi dan terendah

Grafik hanya menggunakan 2 data yaitu

* nilai tertinggi
* nilai terendah


```python
plt.bar(['Tertinggi','Terendah'])
```

Jumlah data akan tetap **2**.

Maka Kompleksitasnya adalah:

```
O(1)
```

karena tidak bergantung pada jumlah mahasiswa.


## ⚙️ 5️. Grafik lulus dan tidak lulus

Grafik hanya menampilkan 2 kategori atau kondisi yaitu

* lulus
* tidak lulus


```python
plt.bar([lulus, tidak_lulus])
```

Jumlah datanya akan tetap **2**

Maka Kompleksitasnya adalah:

```
O(1)
```

# Ringkasan Kompleksitas 📝

| Bagian Program                               | Kompleksitas |
| -------------------------------------------- | ------------ |
| Input nilai mahasiswa                        | **O(n)**     |
| Mencari nilai tertinggi, terendah, rata-rata | **O(n)**     |
| Menghitung mahasiswa lulus                   | **O(n)**     |
| Grafik nilai tertinggi & terendah            | **O(1)**     |
| Grafik kelulusan                             | **O(1)**     |



Jadi sebagian besar Kompleksitas program adalah

```
O(n)
```
karena operasi utama masih bergantung pada jumlah data mahasiswa dan sebagian besar operasi perlu memproses seluruh elemen array untuk melakukan perhitungan nilai mahasiswa.


# 4. Refleksi Pembelajaran 📚

Melalui proyek ini saya mempelajari bagaimana membuat struktur data array menggunakan bahasa python untuk menyimpan dan mengelola sekumpulan data. Saya juga belajar bagaimana melakukan operasi dasar pada array seperti mencari nilai tertinggi, nilai terendah, dan menghitung rata-rata, serta melakukan proses seleksi untuk menentukan mahasiswa yang lulus dan tidak lulus berdasarkan suatu kondisi.

Selain itu, proyek ini membantu memahami konsep analisis kompleksitas algoritma, khususnya bagaimana beberapa operasi pada array memiliki kompleksitas waktu O(n) karena harus memeriksa seluruh elemen data dan beberapa proses lain seperti pembuatan grafik hanya memproses data yang sudah tersedia sehingga memiliki kompleksitas O(1). lalu penggunaan library Matplotlib juga memberikan kemudahan dalam membuat visualisasi grafik data sederhana.

Secara keseluruhan, proyek ini membantu saya memahami hubungan pengolahan data menggunakan array, analisis algoritma, dan visualisasi data, sehingga bisa belajar merancang program yang dibuat tidak hanya untuk memproses data tetapi juga disajikan secara lebih baik.

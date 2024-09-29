# <h1 align="center">Laporan Praktikum Dasar-Dasar Python untuk Sains Data</h1>

<p align="center">Rizal Wahyu Pratama</p>
<p align="center">2311110029</p>
<p align="center">S1SD-04-02</p>

## Tujuan Praktikum

1. Siswa memahami dan menggunakan tipe serta struktur data dasar di Python.
2. Siswa menerapkan operator, logika, dan percabangan untuk pengambilan keputusan.
3. Siswa mampu membuat fungsi dan menggunakan pengulangan untuk efisiensi kode.

## Dasar Teori

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Gambar1.jpeg" alt="Alt Text">
</p> 
<p align="center">
 Gambar 1. Ilustrasi Programer Python
</p> 

### Sejarah Python dan Perkembangannya Hingga Python Versi 3

Python pertama kali dikembangkan oleh Guido van Rossum pada akhir tahun 1980-an di Centrum Wiskunde & Informatica (CWI) di Belanda dan resmi dirilis pada tahun 1991 . Tujuan utama Python adalah menciptakan bahasa yang sederhana, mudah dipahami, namun tetap kuat dalam hal kemampuan. Python 1.0 menekankan pada kekonsistenan sintaks yang bersih dan readable, serta menghadirkan fitur-fitur dasar seperti pengelolaan modul, kelas, dan tipe data dinamis [1].

Perkembangan Python semakin pesat dengan dirilisnya Python 2.0 pada tahun 2000. Salah satu fitur kunci dari Python 2 adalah garbage collection berbasis cycle-detecting, yang membuat pengelolaan memori lebih efisien. Selain itu, Python 2.0 juga memperkenalkan fitur list comprehensions dan augmented assignment, yang menjadikan penulisan kode lebih singkat dan efisien [2]. Namun, Python 2 memiliki keterbatasan, khususnya dalam dukungan internasionalisasi dan pengelolaan tipe data string. Ini mendorong pengembangan Python 3, yang dirilis pada tahun 2008  .

Python 3.0 membawa perubahan mendasar pada arsitektur bahasa ini, yang menyebabkan kompatibilitas ke belakang (backward compatibility) tidak sepenuhnya terjaga. Salah satu perbedaan terbesar adalah cara Python 3 menangani string; Python 3 memperlakukan string sebagai unicode secara default, yang meningkatkan kemampuannya dalam penanganan teks multibahasa . Selain itu, Python 3 memperbaiki banyak "quirks" dari versi sebelumnya, seperti penghapusan `print` sebagai keyword dan menjadikannya fungsi, serta pengenalan `type hinting` yang lebih kuat untuk meningkatkan keterbacaan dan pemeliharaan kode [3].

### Mengapa Python Banyak Digunakan oleh Programmer?

Ada beberapa alasan mengapa Python menjadi bahasa pemrograman yang sangat populer. Pertama, Python dikenal dengan sintaks yang sederhana dan mudah dibaca, sehingga programmer dari berbagai tingkat pengalaman, terutama pemula, dapat dengan cepat memahami logika program tanpa harus berkutat dengan aturan sintaks yang rumit . Selain itu, Python mendukung paradigma pemrograman multiparadigm, termasuk pemrograman berorientasi objek, pemrograman prosedural, dan pemrograman fungsional, sehingga membuatnya sangat fleksibel untuk berbagai jenis proyek .

Kedua, Python memiliki ekosistem yang kaya dengan berbagai library dan framework yang memudahkan pengembangan aplikasi secara cepat. Sebagai contoh, dalam bidang kecerdasan buatan dan machine learning, Python menyediakan pustaka terkenal seperti TensorFlow, Keras, dan scikit-learn, yang membuat pengembangan model AI menjadi lebih mudah dan cepat [4]. Dalam data science, pustaka seperti Pandas dan NumPy menjadi standar de facto untuk analisis dan manipulasi data .

Komunitas Python yang besar dan aktif juga menjadi salah satu alasan mengapa Python sangat populer. Komunitas ini tidak hanya berkontribusi dalam pengembangan Python itu sendiri, tetapi juga menyediakan ribuan tutorial, dokumentasi, dan sumber daya lainnya, sehingga membuat pembelajaran dan penyelesaian masalah menjadi lebih mudah. Selain itu, Python adalah bahasa yang cross-platform, yang artinya program yang ditulis di Python dapat berjalan di berbagai sistem operasi seperti Windows, macOS, dan Linux tanpa banyak penyesuaian .

### Contoh Penerapan Python dalam Pemrograman

Salah satu penerapan paling signifikan Python adalah di bidang data science dan big data. Pustaka seperti Pandas digunakan untuk manipulasi data, sedangkan NumPy sangat berguna dalam komputasi numerik yang efisien . Python juga menjadi bahasa pilihan dalam kecerdasan buatan dan machine learning, di mana pustaka seperti scikit-learn dan TensorFlow mempermudah pengembangan model pembelajaran mesin, mulai dari regresi sederhana hingga jaringan saraf tiruan yang kompleks.

Dalam pengembangan aplikasi web, framework Django dan Flask memungkinkan pengembangan aplikasi dengan cepat dan mudah, sambil tetap mempertahankan skalabilitas dan keamanannya. Django, misalnya, mendukung ORM (Object-Relational Mapping) yang mempermudah interaksi dengan database tanpa harus menulis query SQL secara langsung . Sementara Flask lebih ringan dan fleksibel, cocok untuk aplikasi yang lebih kecil atau proyek yang memerlukan kustomisasi lebih mendalam.

Python juga banyak digunakan dalam automasi sistem, misalnya untuk menulis skrip yang mengotomatisasi tugas-tugas rutin seperti pemrosesan file, pengelolaan server, hingga crawling data dari web. Dengan dukungan pustaka seperti Selenium dan BeautifulSoup, Python menjadi alat yang sangat efisien dalam pengembangan bot atau skrip untuk web scraping [5].

### Variabel dan Tipe Data

Dalam Python kita dapat menyimpan data dalam memori menggunakan variabel. Dalam penulisan variabel terdapat aturan-aturan yang harus diikuti seperti menggunakan huruf, angka, underscore, dan awalan variabel tidak dimulai dengan angka.

```
x = 10
y = 3.14
z = "Data Science"

user_age = 20
pi_value = 3.14159
course_name = "Python for Data Science"
```

Di atas merupakan tipe-tipe data yang ada dalam Python diantaranya:

- Integer (int): Tipe data yang berisi bilangan bulat.
- Float: Tipe data yang berisikan bilangan desimal.
- String (str): Kumpulan dari char yang membentuk sebuah kalimat.
- Boolean (bool): Tipe data yang outputnya True atau False.

```
#integer (int)
age = 25

# Floats
height = 1.67

# Strings
name = "Rizal"

# Booleans
is_student = True

print(type(age))
print(type(height))
print(type(name))
print(type(is_student))
```

### Operator dan Logika

Operator dalam Python sama dengan operator dalam matematika. Berikut operatornya:

#### Operator Aritmatika

Operator yang digunakan seperti berikut:

- +, -, *, / (penjumlahan, pengurangan, kali, bagi)
- // (pembagian bulat)
- % (modulus)
- ** (perpangkatan)

```
a = 10
b = 3

# Penjumlahan
print(a + b)

# Pembagian
print(a / b)

# Pembagian bulat
print(a // b)

# Eksponensial
print(a ** b) 
```

#### Operator Perbandingan

Operator perbandingan digunakan untuk membandingkan dua nilai yang hasilnya berupa Boolean. Adapun operator perbandingan yang digunakan dalam Python seperti berikut:

- != (tidak sama dengan)
- == (sama dengan)
- >, <, >=, <= (perbandingan nilai)

```
print(a > b) # Output: True

print(a == b) # Output: False

print(a >= b) # Output: True

print(a <= b) # Output: False
```

#### Operator Logika

Operator logika ini digunakan untuk menggabungkan ekspresi yang dihasilkan dari Boolean sesuai dengan aturan yang telah ada.

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Operator%20Logika.png" alt="Alt Text">
</p> 
<p align="center">
 Gambar 2. Penggabungan Operator Logika
</p> 

```
x = True
y = False
print(x and y)
print(x or y)
```

#### Fungsi

Dalam Python, fungsi (function) adalah blok kode yang terorganisir dan dapat digunakan kembali untuk melakukan tugas tertentu. Fungsi digunakan untuk membagi program menjadi bagian-bagian yang lebih kecil dan lebih terstruktur, sehingga memudahkan pemeliharaan dan penggunaan kembali kode. Fungsi dapat menerima input (disebut argumen), melakukan operasi tertentu, dan mengembalikan output (disebut return value).

```
# Definisi fungsi sederhana
def greet(name):
 return f"Hello, {name}!"
# Memanggil fungsi
print(greet("Rizal"))
```

#### Perulangan (Loops)

Perulangan atau loop dalam Python adalah struktur kontrol yang memungkinkan eksekusi berulang dari blok kode tertentu selama kondisi tertentu terpenuhi. Adapun dua jenis loop yang sering digunakan:

- For Loop --> digunakan dalam list, tuple, dictionary, dan range.
```
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
 print(fruit)
```
- While Loop --> loop yang dilakukan untuk memenuhi kondisi tertentu.
```
counter = 0
while counter < 3:
 print(counter)
 counter += 1
```
- List Comprehension --> menulis loop yang menghasilkan list.
```
numbers = [1, 2, 3, 4, 5]
doubled = [x * 2 for x in numbers]
print(doubled)
```

#### Percabangan

Percabangan atau kondisional dalam Python adalah struktur kontrol yang memungkinkan program untuk membuat keputusan berdasarkan kondisi tertentu. Berdasarkan hasil evaluasi kondisi tersebut (benar atau salah), program akan mengeksekusi satu blok kode atau blok lainnya. Struktur percabangan utama dalam Python adalah if, elif, dan else.

1. if: Memeriksa kondisi. Jika kondisi benar (True), maka blok kode di dalamnya akan dijalankan.
2. elif: (singkatan dari "else if") Memeriksa kondisi lain jika kondisi sebelumnya salah. Ini digunakan untuk memeriksa beberapa kondisi.
3. else: Menjalankan kode jika semua kondisi sebelumnya salah.

```
score = 85
if score >= 90:
 print("A")
elif score >= 80:
 print("B")
else:
 print("C")
```

Nested Conditionals (Percabangan bersarang atau percabangan dalam percabangan)

```
score = 85
attendance = 90
if score >= 80:
 if attendance >= 85:
 print("Lulus dengan nilai baik")
 else:
 print("Kehadiran kurang")
else:
 print("Tidak lulus")
```

Sebagai bahasa pemrograman yang telah berkembang selama lebih dari tiga dekade, Python telah berhasil menjadi salah satu bahasa yang paling populer di dunia teknologi. Kelebihannya yang mencakup sintaks yang sederhana, kemampuan lintas platform, serta ekosistem pustaka yang luas menjadikannya pilihan utama bagi pemula maupun profesional. Mulai dari data science, kecerdasan buatan, hingga pengembangan web dan otomasi sistem, Python menawarkan fleksibilitas dan kekuatan untuk berbagai jenis aplikasi. Dengan komunitas yang terus berkembang dan inovasi yang terus diperkenalkan, Python akan tetap menjadi pilar penting dalam dunia pemrograman modern di masa depan.

### 1. Guided 1

Terdapat sekitar 100 guided yang telah diberikan. Dalam guided ini, saya akan memilih beberapa guided.

Code:
```
def factorial(n):
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result

print(factorial(5))
```

Output:
```
120
```

Pada kode di atas, praktikan mendefinisikan sebuah fungsi yaitu fungsi untuk mencari faktorial dengan parameter n. Kode di atas menggunakan looping for dengan iterasi n+1. Diakhir, praktikan memasukkan parameter 5 untuk mengetahui hasil dari 5 faktorial yaitu 120.

### 2. Guided 2

Terdapat sekitar 100 guided yang telah diberikan. Dalam guided ini, saya akan memilih beberapa guided.

Code:
```
name = input("Enter your name: ")
age = int(input("Enter your age: "))
print(f"Name: {name}, Age: {age}")
```

Output:
```
Enter your name: Rizal
Enter your age: 19
Name: Rizal, Age: 19
```

Pada kode di atas, praktikan membuat 3 variabel yaitu name yang akan menerima input nama dan age yang menerima input umur. Terakhir praktikan menggunakan print untuk memunculkan output ke layar. Pada kode di atas, diinputkan nama Rizal pada variabel name, diinputkan angka 19 pada variabel age. Maka outputnya seperti Name: Rizal, Age: 19.

#### Full Code and Output Screenshot 

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Out2.png" alt="Alt Text">
</p>

### 3. Guided 3

Terdapat sekitar 100 guided yang telah diberikan. Dalam guided ini, saya akan memilih beberapa guided.

Code:
```
from functools import reduce
numbers = [1, 2, 3, 4, 5]
total = reduce(lambda x, y: x + y, numbers)
print(total)
```

Output:
```
15
```

Pada kode di atas, terdapat modul functools yang dipanggil untuk menjumlahkan semua elemen dalam list numbers. Reduce merupakan fungsi yang melakukan operasi secara berulang pada elemen dari sebuah list. Dibuatkan list numbers yang berisi 1, 2, 3, 4, 5 lalu terdapat variabel total yang akan mereduce seluruh angka pada list numbers. Ketika dicetak pada layar menggunakan fungsi print() maka akan muncul output 15.

#### Full Code and Output Screenshot 

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Out3.png" alt="Alt Text">
</p>

### 4. Guided 4

Terdapat sekitar 100 guided yang telah diberikan. Dalam guided ini, saya akan memilih beberapa guided.

Code:
```
class Person:
    def __init__(self, name):
        self.name = name

class Mahasiswa(Person):
    def __init__(self, name, umur):
        super().__init__(name)
        self.umur = umur

mahasiswa = Mahasiswa("Alice", 20)
print(mahasiswa.name, mahasiswa.umur))
```

Output:
```
Alice 20
```

Pada kode di atas, dibuatkan dua class yaitu class Person yang menerima satu parameter yaitu name sebagai atribut dari objek yang dibuat dari class Person. Lalu terdapat class Mahasiswa dengan parameter Person, dengan metode __init__ yang menerima dua parameter name dan umur. Dengan menggunakan super().__init__(name), konstruktor dari kelas Person dipanggil, yang artinya name diberikan kepada konstruktor Person untuk disimpan sebagai self.name. Berikutnya, membuat variabel Mahasiswa yang berisikan data string "Alice", integer 20. Terakhir, menggunakan fungsi print() yang digunakan untuk memunculkan output sehingga outputnya adalah Alice, 20.

#### Full Code and Output Screenshot 

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Out4.png" alt="Alt Text">
</p>


## Unguided

### 1. Unguided 1

####  Buatlah program yang dapat menghasilkan pola berbentuk angka seperti di bawah ini, dengan syarat angka yang ditampilkan adalah hasil dari penjumlahan bilangan prima sebelumnya:

1

2 3

5 7 11

13 17 19 23

**Kode Program:**

```
# Soal 1
# Fungsi untuk memeriksa apakah sebuah bilangan adalah bilangan prima
def prime(num):
    # Jika num kurang dari 2, itu bukan bilangan prima
    if num < 2:
        return False
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            return False
    return True

# Fungsi untuk membuat daftar bilangan prima dengan panjang n
# Fungsi ini menginisialisasi list dengan 1 dan mengisi bilangan prima hingga jumlah n tercapai.
def make_prime(n):
    prime_list = [1]  # Inisialisasi daftar dengan elemen pertama 1
    num = 2 
    while len(prime_list) < n:
        # Jika num adalah bilangan prima, tambahkan ke prime_list
        if prime(num):
            prime_list.append(num)
        num += 1  # Cek angka berikutnya
    return prime_list  # Kembalikan daftar bilangan prima

# Fungsi untuk mencetak pola piramida bilangan prima
# Fungsi ini menghitung jumlah bilangan yang dibutuhkan untuk membentuk pola piramida 
# berdasarkan jumlah baris yang diminta dan mencetak bilangan prima sesuai pola.
def pattern(rows):
    prime_count = sum(range(1, rows + 1))  # Jumlah bilangan yang dibutuhkan
    primes = make_prime(prime_count)  # Buat daftar bilangan prima yang sesuai

    index = 0 
    for i in range(1, rows + 1):
        for j in range(i):
            print(primes[index], end=' ') 
            index += 1
        print()

# Menentukan jumlah baris untuk pola
rows = 4
# Memanggil fungsi untuk mencetak pola bilangan prima
pattern(rows)
```

**Penjelasan:**

#### Bagian 1

```
def prime(num):
    if num < 2:
        return False  # Bilangan prima tidak ada yang lebih kecil dari 2
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            return False
    return True
```

Fungsi ini memeriksa apakah suatu angka (num) merupakan bilangan prima. if num < 2: Mengembalikan False jika num lebih kecil dari 2 karena bilangan prima dimulai dari 2. for i in range(2, int(num ** 0.5) + 1): Memeriksa faktor pembagi angka num dari 2 hingga akar kuadrat dari num. if num % i == 0: Jika num dapat dibagi habis oleh i, maka bukan bilangan prima, sehingga mengembalikan False. Jika num lolos dari semua pengecekan, fungsi ini mengembalikan True, menandakan bahwa num adalah bilangan prima.

#### Bagian 2

```
def make_prime(n):
    prime_list = [1]
    num = 2
    while len(prime_list) < n:
        if prime(num):
            prime_list.append(num)
        num += 1
    return prime_list
```

- Fungsi ini menghasilkan list bilangan prima berisi n bilangan, termasuk angka 1. prime_list = [1]: Membuat list awal yang dimulai dengan 1.
- while len(prime_list) < n: Loop berjalan hingga jumlah bilangan dalam prime_list mencapai n. if prime(num): Memeriksa apakah num adalah bilangan prima menggunakan fungsi prime(num). Jika benar, num ditambahkan ke dalam prime_list.
- num += 1: Setiap kali loop dijalankan, num bertambah satu untuk memeriksa angka berikutnya.
- Fungsi ini mengembalikan list prime_list yang berisi n bilangan prima.
  
#### Bagian 3

```
def pattern(rows):
    prime_count = sum(range(1, rows + 1))  # Menjumlahkan bilangan prima
    primes = make_prime(prime_count)
    
    index = 0
    for i in range(1, rows + 1):
        for j in range(i):
            print(primes[index], end=' ')
            index += 1
        print()
```

Fungsi ini mencetak pola piramida dengan bilangan prima.
- prime_count = sum(range(1, rows + 1)): Menghitung jumlah bilangan yang perlu dicetak berdasarkan jumlah baris (rows). Ini dilakukan dengan menjumlahkan angka-angka dari 1 hingga rows (misalnya, untuk rows = 4, jumlahnya adalah 1 + 2 + 3 + 4 = 10). Angka ini menyatakan jumlah bilangan prima yang diperlukan.
- primes = make_prime(prime_count): Memanggil fungsi make_prime(prime_count) untuk menghasilkan list bilangan prima sebanyak prime_count. index = 0: Variabel ini digunakan untuk melacak indeks bilangan prima yang akan dicetak.
- Loop pertama for i in range(1, rows + 1): Loop ini menentukan jumlah baris yang akan dicetak. Loop kedua for j in range(i): Loop ini mencetak bilangan prima sebanyak nilai dari i, sehingga pada baris pertama mencetak 1 bilangan, baris kedua mencetak 2 bilangan, dan seterusnya.
- print(primes[index], end=' '): Mencetak bilangan prima dari list primes pada baris tersebut, tanpa berpindah ke baris baru.
- index += 1: Menggeser indeks untuk mengambil bilangan prima berikutnya.
- print(): Berpindah ke baris baru setelah setiap baris pola selesai dicetak.

#### Bagian 4

```
rows = 4
pattern(rows)
```

Pada bagian ini, fungsi pattern(rows) dipanggil dengan argumen rows = 4, sehingga pola akan dicetak dalam 4 baris.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Output1.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Output1.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 1
</p> 

#### Penjelasan

Baris pertama mencetak 1 bilangan prima.
Baris kedua mencetak 2 bilangan prima.
Baris ketiga mencetak 3 bilangan prima, dan seterusnya, sesuai dengan jumlah baris yang ditentukan (rows).

### 2. Unguided 2

####  Buatlah versi program Rekursif Tidak Langsung (Indirect Recursion) dari soal nomor 1 di atas!

**Kode Program:**

```C++
#include <iostream>

// Deklarasi kedua fungsi terlebih dahulu
long long faktorialGenap(int n);
long long faktorialGanjil(int n);

// Fungsi untuk menghitung faktorial bilangan genap
long long faktorialGenap(int n) {
    if (n == 0) 
        return 1; // basis rekursi
    else
        return n * faktorialGanjil(n - 1); // memanggil fungsi faktorialGanjil
}

// Fungsi untuk menghitung faktorial bilangan ganjil
long long faktorialGanjil(int n) {
    if (n == 1) 
        return 1; // basis rekursi
    else
        return n * faktorialGenap(n - 1); // memanggil fungsi faktorialGenap
}

int main() {
    int angka;
    std::cout << "Masukkan bilangan bulat positif: ";
    std::cin >> angka;

    // Memastikan bahwa angka adalah positif
    if (angka < 0) {
        std::cout << "Faktorial tidak didefinisikan untuk bilangan negatif." << std::endl;
    } else {
        long long hasil;
        if (angka % 2 == 0) {
            hasil = faktorialGenap(angka);
        } else {
            hasil = faktorialGanjil(angka);
        }
        std::cout << "Hasil Faktorial dari " << angka << " adalah: " << hasil << std::endl;
    }

    return 0;
}
```

**Penjelasan:**

#### Bagian 1

```C++
#include <iostream>
```

Library iostream digunakan untuk menjalankan operasi input dan output pada program. Memungkinkan penggunaan fungsi std::cout dan std::cin.

#### Bagian 2

```C++
long long faktorialGenap(int n);
long long faktorialGanjil(int n);
```

Dua fungsi ini dideklarasikan terlebih dahulu sebelum definisinya. Fungsi faktorialGenap digunakan untuk menghitung faktorial bilangan genap, dan faktorialGanjil untuk bilangan ganjil.

#### Bagian 3

```C++
long long faktorialGenap(int n) {
    if (n == 0) 
        return 1; // basis rekursi
    else
        return n * faktorialGanjil(n - 1); // memanggil fungsi faktorialGanjil
}
```

Fungsi ini menghitung faktorial bilangan genap secara rekursif. Jika n adalah 0, fungsi mengembalikan 1 sebagai basis rekursi. Jika tidak, fungsi mengalikan n dengan hasil dari faktorialGanjil(n - 1), sehingga terjadi pemanggilan rekursif antara fungsi faktorialGenap dan faktorialGanjil.

#### Bagian 4

```C++
long long faktorialGanjil(int n) {
    if (n == 1) 
        return 1; // basis rekursi
    else
        return n * faktorialGenap(n - 1); // memanggil fungsi faktorialGenap
}
```

Mirip dengan faktorialGenap, fungsi ini menghitung faktorial bilangan ganjil. Jika n adalah 1, fungsi mengembalikan 1 sebagai basis rekursi. Jika tidak, fungsi mengalikan n dengan hasil dari faktorialGenap(n - 1), menciptakan rekursi antara kedua fungsi faktorial.

#### Bagian 5

```C++
int main() {
    int angka;
    std::cout << "Masukkan bilangan bulat positif: ";
    std::cin >> angka;

    if (angka < 0) {
        std::cout << "Faktorial tidak didefinisikan untuk bilangan negatif." << std::endl;
    } else {
        long long hasil;
        if (angka % 2 == 0) {
            hasil = faktorialGenap(angka);
        } else {
            hasil = faktorialGanjil(angka);
        }
        std::cout << "Hasil Faktorial dari " << angka << " adalah: " << hasil << std::endl;
    }

    return 0;
}
```

Fungsi di atas merupakan fungsi main yang berupa fungsi utama di dalam program yang disebut dengan fungsi main. Fungsi main yang pertama di eksekusi dan memengaruhi tampilan output.

- Program meminta pengguna memasukkan bilangan bulat positif.
- Jika bilangan negatif, program akan memberikan pesan bahwa faktorial tidak didefinisikan untuk bilangan negatif.
- Jika positif, program akan menentukan apakah bilangan tersebut genap atau ganjil dan memanggil fungsi faktorial yang sesuai.
- Hasilnya kemudian dicetak ke konsol.

Secara keseluruhan, program ini memperlihatkan penggunaan rekursi dan pemisahan fungsi berdasarkan kondisi (genap atau ganjil) untuk menghitung faktorial.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/CodeUn2.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/OutUn2.png" alt="Alt Text">
</p>

#### Penjelasan

Pada output di atas akan sama dengan seperti faktorial di unguided 1. Tapi yang membedakannya pada kode. Jika pengguna memasukkan nilai negatif maka output yang keluar adalah tidak dapat didefinisikan. Untuk bilangan bulat positif dibagi menjadi dua kode seperti positif genap dan ganjil. Jika memasukkan nilai faktorial 5 maka hasilnya adalah 120.

### 3. Unguided 3

####  Implementasikan hash table untuk menyimpan data mahasiswa. Setiap mahasiswa memiliki NIM dan nilai. Implementasikan fungsi untuk menambahkan data baru, menghapus data, mencari data berdasarkan NIM, dan mencari data berdasarkan nilai.

**Kode Program:**

```C++
#include <iostream>
#include <unordered_map>
#include <vector>
#include <list>
#include <algorithm>
#include <optional>

using namespace std;

struct Mahasiswa {
    string NIM;
    int nilai;
};

class HashTable {
private:
    unordered_map<int, list<Mahasiswa>> table;
    int size; // Adding size to keep track of the number of buckets

    int hashFunction(string NIM) {
        int sum = 0;
        for (char ch : NIM) {
            sum += ch;
        }
        return sum % size; // Using size instead of bucket_count
    }

public:
    HashTable(int size) : size(size) {
        table.rehash(size);
    }

    void tambahData(Mahasiswa mhs) {
        int index = hashFunction(mhs.NIM);
        table[index].push_back(mhs);
    }

    void hapusData(string NIM) {
        int index = hashFunction(NIM);
        auto& chain = table[index];
        chain.remove_if([NIM](const Mahasiswa& mhs) { return mhs.NIM == NIM; });
    }

    optional<Mahasiswa> cariDataNIM(string NIM) {
        int index = hashFunction(NIM);
        for (auto& mhs : table[index]) {
            if (mhs.NIM == NIM) {
                return mhs;
            }
        }
        return nullopt;
    }

    vector<Mahasiswa> cariDataNilai(int minNilai, int maxNilai) {
        vector<Mahasiswa> hasil;
        for (auto& chain : table) {
            for (auto& mhs : chain.second) {
                if (mhs.nilai >= minNilai && mhs.nilai <= maxNilai) {
                    hasil.push_back(mhs);
                }
            }
        }
        return hasil;
    }

    void tampilkanMenu() {
        cout << "1. Tambah Data\n";
        cout << "2. Hapus Data\n";
        cout << "3. Cari Data Berdasarkan NIM\n";
        cout << "4. Cari Data Berdasarkan Nilai\n";
        cout << "5. Keluar\n";
        cout << "Masukkan pilihan: ";
    }

    void tampilkanSubMenuNilai() {
        cout << "Pilih Rentang Nilai:\n";
        cout << "1. Nilai kurang dari 80\n";
        cout << "2. Nilai 80-90\n";
        cout << "3. Nilai 90-100\n";
        cout << "Masukkan pilihan: ";
    }
};

int main() {
    HashTable ht(10);
    int pilihan;

    do {
        ht.tampilkanMenu();
        cin >> pilihan;
        switch (pilihan) {
            case 1: {
                Mahasiswa mhsBaru;
                cout << "Masukkan NIM: ";
                cin >> mhsBaru.NIM;
                cout << "Masukkan Nilai: ";
                cin >> mhsBaru.nilai;
                ht.tambahData(mhsBaru);
                break;
            }
            case 2: {
                string NIMHapus;
                cout << "Masukkan NIM yang akan dihapus: ";
                cin >> NIMHapus;
                ht.hapusData(NIMHapus);
                break;
            }
            case 3: {
                string NIMCari;
                cout << "Masukkan NIM yang dicari: ";
                cin >> NIMCari;
                auto found = ht.cariDataNIM(NIMCari);
                if (found) {
                    cout << "NIM: " << found->NIM << ", Nilai: " << found->nilai << endl;
                } else {
                    cout << "Data tidak ditemukan." << endl;
                }
                break;
            }
            case 4: {
                int subPilihan;
                ht.tampilkanSubMenuNilai();
                cin >> subPilihan;
                vector<Mahasiswa> foundNilai;

                switch (subPilihan) {
                    case 1:
                        foundNilai = ht.cariDataNilai(0, 79);
                        break;
                    case 2:
                        foundNilai = ht.cariDataNilai(80, 90);
                        break;
                    case 3:
                        foundNilai = ht.cariDataNilai(91, 100);
                        break;
                    default:
                        cout << "Pilihan tidak valid." << endl;
                        continue; // Go back to the main menu
                }

                if (!foundNilai.empty()) {
                    for (auto& mhs : foundNilai) {
                        cout << "NIM: " << mhs.NIM << ", Nilai: " << mhs.nilai << endl;
                    }
                } else {
                    cout << "Tidak ada nilai pada rentang ini." << endl;
                }
                break;
            }
            case 5:
                cout << "Keluar dari program." << endl;
                break;
            default:
                cout << "Pilihan tidak valid." << endl;
        }
    } while (pilihan != 5);

    return 0;
}
```

**Penjelasan:**

#### Bagian 1

```C++
#include <iostream>
#include <unordered_map>
#include <vector>
#include <list>
#include <algorithm>
#include <optional>

using namespace std;
```

- #include <iostream> Digunakan untuk operasi input dan output. Dalam kode ini, iostream digunakan untuk mencetak menu ke konsol dan membaca input dari pengguna menggunakan cin dan cout.
- #include <unordered_map> Digunakan untuk menyimpan data dalam struktur tabel hash. Dalam kode ini, unordered_map digunakan untuk menyimpan dan mengelola data mahasiswa dengan kunci integer yang dihasilkan oleh fungsi hash dan nilai berupa list dari struktur Mahasiswa.
- #include <vector> Digunakan untuk menyimpan kumpulan data dalam bentuk array dinamis. Dalam kode ini, vector digunakan untuk menyimpan dan mengembalikan daftar mahasiswa yang memenuhi kriteria pencarian tertentu, seperti dalam fungsi cariDataNilai.
- #include <list> Digunakan untuk menyimpan data dalam struktur data list yang memungkinkan penyisipan dan penghapusan elemen dengan cepat. Dalam kode ini, list digunakan sebagai nilai dalam unordered_map untuk menyimpan mahasiswa yang memiliki nilai hash yang sama (collision handling).
- #include <algorithm> Digunakan untuk operasi algoritma umum seperti pencarian dan pengurutan. Dalam kode ini, algorithm digunakan untuk fungsi remove_if yang digunakan dalam metode hapusData untuk menghapus mahasiswa dari list berdasarkan NIM.
- #include <optional> Digunakan untuk mengembalikan nilai yang mungkin tidak ada. Dalam kode ini, optional digunakan untuk fungsi cariDataNIM yang mungkin tidak menemukan mahasiswa dengan NIM yang dicari, sehingga mengembalikan nullopt jika mahasiswa tidak ditemukan.
- using namespace std; digunakan agar tidak perlu mendeklarasikan std lagi disetiap fungsinya.

#### Bagian 2

```C++
struct Mahasiswa {
    string NIM;
    int nilai;
};
```

Struktur Mahasiswa menyimpan data mahasiswa yang terdiri dari NIM (Nomor Induk Mahasiswa) dan nilai.

#### Bagian 3

```C++
private:
    unordered_map<int, list<Mahasiswa>> table;
    int size;

public:
    HashTable(int size) : size(size) {
        table.rehash(size);
    }
```

- table: unordered_map yang menggunakan int sebagai kunci dan list dari Mahasiswa sebagai nilai.
- size: Jumlah bucket dalam hash table.
- Konstruktor: Menginisialisasi ukuran tabel hash dan mengatur ulang jumlah bucket.

#### Bagian 4

```C++
int hashFunction(string NIM) {
    int sum = 0;
    for (char ch : NIM) {
        sum += ch;
    }
    return sum % size;
}
```

Menghitung nilai hash dari NIM dengan menjumlahkan nilai ASCII dari setiap karakter, kemudian di modulo dengan size.

#### Bagian 5

```C++
void tambahData(Mahasiswa mhs);
void hapusData(string NIM);
optional<Mahasiswa> cariDataNIM(string NIM);
vector<Mahasiswa> cariDataNilai(int minNilai, int maxNilai);
```

- tambahData: Menambahkan data mahasiswa ke dalam tabel.
- hapusData: Menghapus data mahasiswa berdasarkan NIM.
- cariDataNIM: Mencari mahasiswa berdasarkan NIM.
- cariDataNilai: Mencari semua mahasiswa yang nilainya dalam rentang tertentu.

#### Bagian 6

```C++
int main() {
    HashTable ht(10);
    int pilihan;

    do {
        ht.tampilkanMenu();
        cin >> pilihan;
        switch (pilihan) {
            case 1: {
                Mahasiswa mhsBaru;
                cout << "Masukkan NIM: ";
                cin >> mhsBaru.NIM;
                cout << "Masukkan Nilai: ";
                cin >> mhsBaru.nilai;
                ht.tambahData(mhsBaru);
                break;
            }
            case 2: {
                string NIMHapus;
                cout << "Masukkan NIM yang akan dihapus: ";
                cin >> NIMHapus;
                ht.hapusData(NIMHapus);
                break;
            }
            case 3: {
                string NIMCari;
                cout << "Masukkan NIM yang dicari: ";
                cin >> NIMCari;
                auto found = ht.cariDataNIM(NIMCari);
                if (found) {
                    cout << "NIM: " << found->NIM << ", Nilai: " << found->nilai << endl;
                } else {
                    cout << "Data tidak ditemukan." << endl;
                }
                break;
            }
            case 4: {
                int subPilihan;
                ht.tampilkanSubMenuNilai();
                cin >> subPilihan;
                vector<Mahasiswa> foundNilai;

                switch (subPilihan) {
                    case 1:
                        foundNilai = ht.cariDataNilai(0, 79);
                        break;
                    case 2:
                        foundNilai = ht.cariDataNilai(80, 90);
                        break;
                    case 3:
                        foundNilai = ht.cariDataNilai(91, 100);
                        break;
                    default:
                        cout << "Pilihan tidak valid." << endl;
                        continue; // Go back to the main menu
                }

                if (!foundNilai.empty()) {
                    for (auto& mhs : foundNilai) {
                        cout << "NIM: " << mhs.NIM << ", Nilai: " << mhs.nilai << endl;
                    }
                } else {
                    cout << "Tidak ada nilai pada rentang ini." << endl;
                }
                break;
            }
            case 5:
                cout << "Keluar dari program." << endl;
                break;
            default:
                cout << "Pilihan tidak valid." << endl;
        }
    } while (pilihan != 5);

    return 0;
}
```

Fungsi di atas merupakan fungsi main yang berupa fungsi utama di dalam program yang disebut dengan fungsi main. Fungsi main yang pertama di eksekusi dan memengaruhi tampilan output.

- Membuat objek HashTable dengan 10 bucket.
- Menampilkan menu dan memproses input pengguna untuk melakukan operasi seperti tambah, hapus, dan cari data.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/CodeUn3.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/OutUn3.1.png" alt="Alt Text">
</p>
<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/OutUn3.2.png" alt="Alt Text">
</p>

#### Penjelasan

Output kode di atas sudah di atur juga dalam fungsi main dimana alurnya sebagai berikut: Pengguna akan melihat 5 buah pilihan --> pengguna dapat memilih --> pilihan 1 untuk menambahkan data --> pilihan 2 untuk menghapus data --> pilihan 3 untuk mencari data dari NIM --> pilihan 4 dapat mencari data berdasarkan rentang nilai --> pilihan 5 menu keluar.

## Kesimpulan

Algoritma rekursif dan hash table adalah dua konsep penting dalam ilmu komputer yang digunakan untuk memecahkan masalah dengan cara yang efisien. Algoritma rekursif, yang melibatkan fungsi atau prosedur yang memanggil dirinya sendiri, menawarkan solusi elegan dan sederhana untuk masalah yang dapat dibagi menjadi sub-masalah yang lebih kecil, meskipun memerlukan penanganan yang cermat terhadap overhead dan potensi overflow. Di sisi lain, hash table menyediakan cara yang sangat efisien untuk penyimpanan dan pengambilan data dengan waktu akses rata-rata O(1), dengan berbagai metode penanganan tabrakan seperti open hashing (chaining) dan closed hashing (open addressing). Meskipun masing-masing metode memiliki kelebihan dan kekurangan, pemilihan yang tepat bergantung pada konteks penggunaan dan karakteristik data yang akan diproses.

## Referensi

### Referensi:

1. Shaw, Z. A. (2017). *Learn Python the Hard Way: A Very Simple Introduction to the Terrifyingly Beautiful World of Computers and Code*. Addison-Wesley.
2. Lutz, M. (2019). *Python Crash Course: A Hands-On, Project-Based Introduction to Programming*. No Starch Press.
3. McKinney, W. (2017). *Python for Data Analysis: Data Wrangling with Pandas, NumPy, and IPython*. O'Reilly Media.
4. Zandbergen, P. A. (2020). *Python Scripting for ArcGIS Pro*. Esri Press.
5. Oliphant, T. E. (2015). *Guide to NumPy*. Createspace Independent Publishing Platform.

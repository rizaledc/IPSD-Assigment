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

### 1. Soal 1

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
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal1.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP1.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 1
</p> 

#### Penjelasan

Baris pertama mencetak 1 bilangan prima.
Baris kedua mencetak 2 bilangan prima.
Baris ketiga mencetak 3 bilangan prima, dan seterusnya, sesuai dengan jumlah baris yang ditentukan (rows).

### 2. Soal 2

####  Buatlah sebuah fungsi yang menerima dua input berupa list angka. Fungsi ini harus mengembalikan sebuah list baru yang berisi elemen dari dua list input yang memiliki indeks ganjil. List baru tersebut juga harus diurutkan secara menurun berdasarkan nilai elemen.

**Kode Program:**

```
# Soal 2
# Fungsi untuk menggabungkan elemen pada indeks ganjil dari dua daftar
def index_odd(list1, list2):
    # Membuat daftar baru yang berisi elemen dari list1 dan list2 yang berada pada indeks ganjil
    list1_odd = [list1[i] for i in range(1, len(list1), 2)]
    list2_odd = [list2[i] for i in range(1, len(list2), 2)]
    
    # Menggabungkan kedua daftar yang berisi elemen pada indeks ganjil
    combination = list1_odd + list2_odd
    combination.sort(reverse=True)
    
    # Mengembalikan daftar gabungan yang sudah diurutkan
    return combination

input1 = input("Input the first list (separate with commas)")
input2 = input("Input the second list (separate with commas)")

# Mengonversi input pertama menjadi daftar integer, mengabaikan input yang kosong
list1 = [int(x) for x in input1.split(',') if x.strip()]
# Mengonversi input kedua menjadi daftar integer, mengabaikan input yang kosong
list2 = [int(x) for x in input2.split(',') if x.strip()]

# Memanggil fungsi index_odd dengan kedua daftar dan menyimpan hasilnya
result = index_odd(list1, list2)
# Mencetak hasil gabungan yang sudah diurutkan
print("Result after merger: ", result)
```

**Penjelasan:**

#### Bagian 1

```
# Fungsi untuk menggabungkan elemen pada indeks ganjil dari dua daftar
def index_odd(list1, list2):
    # Membuat daftar baru yang berisi elemen dari list1 dan list2 yang berada pada indeks ganjil
    list1_odd = [list1[i] for i in range(1, len(list1), 2)]
    list2_odd = [list2[i] for i in range(1, len(list2), 2)]
```

Fungsi index_odd: Didefinisikan untuk menerima dua parameter, yaitu list1 dan list2. list1_odd dan list2_odd: Masing-masing adalah daftar yang berisi elemen-elemen dari list1 dan list2 yang berada pada indeks ganjil. Menggunakan list comprehension dan fungsi range untuk mengiterasi dari indeks 1 sampai panjang daftar, dengan langkah 2 (yaitu mengambil setiap elemen kedua).

#### Bagian 2

```
    # Menggabungkan kedua daftar yang berisi elemen pada indeks ganjil
    combination = list1_odd + list2_odd
    combination.sort(reverse=True)
    # Mengembalikan daftar gabungan yang sudah diurutkan
    return combination
```

- combination: Daftar baru yang merupakan hasil penggabungan dari list1_odd dan list2_odd.
- combination.sort(reverse=True): Mengurutkan daftar gabungan dalam urutan menurun (descending).

#### Bagian 3

```
input1 = input("Input the first list (separate with commas)")
input2 = input("Input the second list (separate with commas)")

# Mengonversi input pertama menjadi daftar integer, mengabaikan input yang kosong
list1 = [int(x) for x in input1.split(',') if x.strip()]
# Mengonversi input kedua menjadi daftar integer, mengabaikan input yang kosong
list2 = [int(x) for x in input2.split(',') if x.strip()]

# Memanggil fungsi index_odd dengan kedua daftar dan menyimpan hasilnya
result = index_odd(list1, list2)
```

- Input: Meminta pengguna untuk memasukkan dua daftar yang dipisahkan oleh koma. Input ini berupa string.
- Konversi ke Integer: Masing-masing input dipecah (split) berdasarkan koma menjadi elemen-elemen, dan kemudian setiap elemen yang tidak kosong (setelah dihapus spasi) dikonversi menjadi integer. Ini menghasilkan dua daftar list1 dan list2.
- Memanggil Fungsi: Fungsi index_odd dipanggil dengan dua daftar yang telah dibuat sebelumnya (list1 dan list2), dan hasilnya disimpan dalam variabel result.

#### Bagian 4

```
# Mencetak hasil gabungan yang sudah diurutkan
print("Result after merger: ", result)
```

Output Hasil: Mencetak hasil akhir dari gabungan elemen pada indeks ganjil yang telah diurutkan ke layar.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal2.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP2.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 2
</p> 

#### Penjelasan

List Pertama: 50, 45, 85, 76, 55

List Kedua: 7, 18, 26, 31, 45

**Proses Eksekusi**

**Menentukan Elemen pada Indeks Ganjil:**

Untuk list1 (50, 45, 85, 76, 55):

- Indeks 0: 50

- Indeks 1: 45 (ganjil)

- Indeks 2: 85

- Indeks 3: 76 (ganjil)

- Indeks 4: 55

Elemen pada indeks ganjil: [45, 76]

Untuk list2 (7, 18, 26, 31, 45):

- Indeks 0: 7

- Indeks 1: 18 (ganjil)

- Indeks 2: 26

- Indeks 3: 31 (ganjil)

- Indeks 4: 45

Elemen pada indeks ganjil: [18, 31]

Menggabungkan dan Mengurutkan:

Gabungan Elemen pada Indeks Ganjil:

Gabungan dari kedua daftar: [45, 76] + [18, 31] menjadi [45, 76, 18, 31].

Mengurutkan dalam Urutan Menurun (Descending):

Setelah diurutkan menjadi [76, 45, 31, 18].

### 3. Soal 3

####  Buat sebuah program untuk mensimulasikan transaksi ATM. Program harus: 
1. Meminta pengguna memasukkan PIN (dibatasi 3 kali percobaan).
2. Setelah PIN benar, meminta jumlah penarikan.
3. Jika saldo kurang dari jumlah yang ditarik, munculkan pesan kesalahan.
4. Jika penarikan berhasil, tampilkan saldo akhir.

**Kode Program:**

```
#Soal 3

# Simulasi ATM dengan tabungan dan menu
import os

def clear_screen():
    os.system('cls' if os.name == 'nt' else 'clear')
    
def lihat_saldo(id_user):
    print(f"Saldo Anda saat ini: Rp{users[id_user][1]}")

users = {}  # Penyimpanan data pengguna berupa dictionary {ID: [PIN, saldo]}

#Mendefinisikan sebuah fungsi untuk membuat akun
def buat_akun():
    print("== Buat Akun Tabungan ==")
    while True:
        id_user = input("Masukkan ID (kombinasi huruf dan angka): ")
        if id_user in users:
            print("ID telah digunakan, gunakan ID lainnya!")
        elif len(id_user) < 6:
            print("ID minimal terdiri dari 6 karakter!")
        else:
            break
    while True:
        pin = input("Buat PIN (4 angka): ")
        if len(pin) == 4 and pin.isdigit():
            break
        else:
            print("PIN harus terdiri dari 4 angka!")
    
    saldo_awal = int(input("Masukkan saldo awal (dalam rupiah): "))
    users[id_user] = [pin, saldo_awal]
    print(f"Akun dengan ID {id_user} berhasil dibuat!")

#Mendefinisikan sebuah fungsi untuk masuk ke dalam akun
def masuk_akun():
    print("== Masuk Akun Tabungan ==")
    attempts = 0
    while attempts < 3:
        id_user = input("Masukkan ID: ")
        pin = input("Masukkan PIN: ")
        if id_user in users and users[id_user][0] == pin:
            print("Login berhasil!")
            return id_user
        else:
            attempts += 1
            print(f"ID atau PIN salah. Percobaan {attempts} dari 3.")
    
    print("Anda telah salah memasukkan ID atau PIN 3 kali.")
    return None

#Mendefinisikan sebuah fungsi untuk melakukan setor tunai
def setor_tunai(id_user):
    print("== Setor Tunai ==")
    setor = int(input("Masukkan jumlah setor (kelipatan Rp 50.000): "))
    if setor % 50000 == 0:
        users[id_user][1] += setor
        print(f"Setoran berhasil. Saldo akhir: Rp{users[id_user][1]}")
    else:
        print("Setoran harus kelipatan Rp 50.000!")

#Mendefinisikan sebuah fungsi untuk melakukan tarik tunai
def tarik_tunai(id_user):
    print("== Tarik Tunai ==")
    print("Pilih jumlah penarikan:")
    print("1. Rp 500.000")
    print("2. Rp 1.000.000")
    print("3. Rp 2.000.000")
    print("4. Jumlah lain")
    
    pilihan = input("Masukkan pilihan (1-4): ")
    
    if pilihan == "1":
        tarik = 500000
    elif pilihan == "2":
        tarik = 1000000
    elif pilihan == "3":
        tarik = 2000000
    elif pilihan == "4":
        tarik = int(input("Masukkan jumlah penarikan: "))
    else:
        print("Pilihan tidak valid!")
        return
    
    if tarik % 50000 != 0:
        print("Penarikan harus kelipatan Rp 50.000!")
        return
    
    if users[id_user][1] >= tarik:
        users[id_user][1] -= tarik
        print(f"Penarikan berhasil. Saldo akhir: Rp{users[id_user][1]}")
    else:
        print("Maaf saldo Anda tidak mencukupi.")

#Mendefinisikan sebuah fungsi untuk memunculkan menu utama
def menu_utama():
    while True:
        clear_screen()  # Membersihkan layar
        print("\n=== Selamat Datang di ATM ===")
        print("ATM ini hanya menyediakan uang selembaran Rp.50.000,00")
        print("1. Buat Akun Tabungan")
        print("2. Masuk ke Akun Tabungan")
        print("3. Keluar")
        
        pilihan = input("Masukkan pilihan (1-3): ")
        
        if pilihan == "1":
            clear_screen()  # Membersihkan layar
            buat_akun()
        elif pilihan == "2":
            clear_screen()  # Membersihkan layar
            id_user = masuk_akun()
            if id_user:
                while True:
                    clear_screen()  # Membersihkan layar
                    print("\n== Menu Akun Tabungan ==")
                    print("1. Setor Tunai")
                    print("2. Tarik Tunai")
                    print("3. Lihat Saldo")
                    print("4. Kembali ke Menu Utama")
                    
                    sub_pilihan = input("Masukkan pilihan (1-3): ")
                    
                    if sub_pilihan == "1":
                        setor_tunai(id_user)
                    elif sub_pilihan == "2":
                        tarik_tunai(id_user)
                    elif sub_pilihan == "3":
                        lihat_saldo(id_user)
                    elif sub_pilihan == "4":
                        break
                    else:
                        print("Pilihan tidak valid!")
        elif pilihan == "3":
            print("Terima kasih telah menggunakan ATM kami!")
            break
        else:
            print("Pilihan tidak valid!")

# Menjalankan program
menu_utama()
```

**Penjelasan:**

#### Bagian 1

```
import os
def clear_screen():
    os.system('cls' if os.name == 'nt' else 'clear')
def lihat_saldo(id_user):
    print(f"Saldo Anda saat ini: Rp{users[id_user][1]}")
users = {}  # Penyimpanan data pengguna berupa dictionary {ID: [PIN, saldo]}
```

- Mengimpor modul os untuk dapat menggunakan fungsi yang berkaitan dengan sistem operasi, seperti membersihkan layar.
- Fungsi ini membersihkan layar terminal. Jika sistem operasi adalah Windows (nt), maka perintah cls digunakan, jika tidak, perintah clear digunakan untuk sistem Unix.
- Fungsi ini menampilkan saldo pengguna berdasarkan id_user yang diberikan.
- Menggunakan dictionary users untuk menyimpan informasi pengguna, di mana kunci adalah ID pengguna dan nilai adalah list yang berisi PIN dan saldo.
  
#### Bagian 2

```
def buat_akun():
    print("== Buat Akun Tabungan ==")
    while True:
        id_user = input("Masukkan ID (kombinasi huruf dan angka): ")
        if id_user in users:
            print("ID telah digunakan, gunakan ID lainnya!")
        elif len(id_user) < 6:
            print("ID minimal terdiri dari 6 karakter!")
        else:
            break
    while True:
        pin = input("Buat PIN (4 angka): ")
        if len(pin) == 4 and pin.isdigit():
            break
        else:
            print("PIN harus terdiri dari 4 angka!")
    
    saldo_awal = int(input("Masukkan saldo awal (dalam rupiah): "))
    users[id_user] = [pin, saldo_awal]
    print(f"Akun dengan ID {id_user} berhasil dibuat!")
```

Fungsi ini meminta pengguna untuk membuat akun baru. Pengguna diminta untuk memasukkan ID dan PIN, serta saldo awal. Validasi dilakukan untuk memastikan ID dan PIN memenuhi syarat yang telah ditentukan.

#### Bagian 3

```
def masuk_akun():
    print("== Masuk Akun Tabungan ==")
    attempts = 0
    while attempts < 3:
        id_user = input("Masukkan ID: ")
        pin = input("Masukkan PIN: ")
        if id_user in users and users[id_user][0] == pin:
            print("Login berhasil!")
            return id_user
        else:
            attempts += 1
            print(f"ID atau PIN salah. Percobaan {attempts} dari 3.")
    
    print("Anda telah salah memasukkan ID atau PIN 3 kali.")
    return None
```

Fungsi ini digunakan untuk login ke akun. Pengguna diberikan tiga kesempatan untuk memasukkan ID dan PIN yang benar. Jika login berhasil, id_user dikembalikan; jika tidak, fungsi akan menginformasikan bahwa percobaan login telah habis.

#### Bagian 4

```
def setor_tunai(id_user):
    print("== Setor Tunai ==")
    setor = int(input("Masukkan jumlah setor (kelipatan Rp 50.000): "))
    if setor % 50000 == 0:
        users[id_user][1] += setor
        print(f"Setoran berhasil. Saldo akhir: Rp{users[id_user][1]}")
    else:
        print("Setoran harus kelipatan Rp 50.000!")
```

Fungsi ini memungkinkan pengguna untuk melakukan setor tunai. Pengguna diminta untuk memasukkan jumlah setoran, yang harus merupakan kelipatan Rp 50.000. Jika valid, saldo diperbarui dan ditampilkan.

#### Bagian 5

```
def tarik_tunai(id_user):
    print("== Tarik Tunai ==")
    print("Pilih jumlah penarikan:")
    print("1. Rp 500.000")
    print("2. Rp 1.000.000")
    print("3. Rp 2.000.000")
    print("4. Jumlah lain")
    
    pilihan = input("Masukkan pilihan (1-4): ")
    
    if pilihan == "1":
        tarik = 500000
    elif pilihan == "2":
        tarik = 1000000
    elif pilihan == "3":
        tarik = 2000000
    elif pilihan == "4":
        tarik = int(input("Masukkan jumlah penarikan: "))
    else:
        print("Pilihan tidak valid!")
        return
    
    if tarik % 50000 != 0:
        print("Penarikan harus kelipatan Rp 50.000!")
        return
    
    if users[id_user][1] >= tarik:
        users[id_user][1] -= tarik
        print(f"Penarikan berhasil. Saldo akhir: Rp{users[id_user][1]}")
    else:
        print("Maaf saldo Anda tidak mencukupi.")
```

Fungsi ini digunakan untuk melakukan penarikan tunai. Pengguna dapat memilih dari beberapa jumlah tetap atau memasukkan jumlah lainnya. Validasi dilakukan untuk memastikan bahwa jumlah penarikan adalah kelipatan Rp 50.000 dan saldo mencukupi.

#### Bagian 6

```
def menu_utama():
    while True:
        clear_screen()  # Membersihkan layar
        print("\n=== Selamat Datang di ATM ===")
        print("ATM ini hanya menyediakan uang selembaran Rp.50.000,00")
        print("1. Buat Akun Tabungan")
        print("2. Masuk ke Akun Tabungan")
        print("3. Keluar")
        
        pilihan = input("Masukkan pilihan (1-3): ")
        
        if pilihan == "1":
            clear_screen()  # Membersihkan layar
            buat_akun()
        elif pilihan == "2":
            clear_screen()  # Membersihkan layar
            id_user = masuk_akun()
            if id_user:
                while True:
                    clear_screen()  # Membersihkan layar
                    print("\n== Menu Akun Tabungan ==")
                    print("1. Setor Tunai")
                    print("2. Tarik Tunai")
                    print("3. Lihat Saldo")
                    print("4. Kembali ke Menu Utama")
                    
                    sub_pilihan = input("Masukkan pilihan (1-3): ")
                    
                    if sub_pilihan == "1":
                        setor_tunai(id_user)
                    elif sub_pilihan == "2":
                        tarik_tunai(id_user)
                    elif sub_pilihan == "3":
                        lihat_saldo(id_user)
                    elif sub_pilihan == "4":
                        break
                    else:
                        print("Pilihan tidak valid!")
        elif pilihan == "3":
            print("Terima kasih telah menggunakan ATM kami!")
            break
        else:
            print("Pilihan tidak valid!")

menu_utama()
```

Fungsi ini menampilkan menu utama ATM. Pengguna dapat memilih untuk membuat akun baru, masuk ke akun yang sudah ada, atau keluar dari program. Jika pengguna masuk ke akun, menu tambahan akan muncul untuk melakukan setor tunai, tarik tunai, atau melihat saldo.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal3.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP3.1.png" alt="Alt Text">
</p> 
<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP3.2.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 3
</p> 

#### Penjelasan

Pada output kode di atas, user diminta untuk membuat akun tabungan terlebih dahulu dengan memasukkan ID dan membuat PIN serta memasukkan saldo awal, selanjutnya user dapat masuk ke akun tabungan untuk melakukan transaksi seperti setor tunai, tarik tunai, dan melihat saldo. Apabila dalam proses masuk ke dalam akun terjadi kesalahan melebihi 5 kali maka otomatis user tidak dapat masuk lagi ke dalam akunnya.

### 4. Soal 4

####  Buat sebuah program untuk mensimulasikan transaksi ATM. Program harus: 
Anda diberikan file CSV berisi data nilai ujian mahasiswa. Tugas Anda adalah menulis
sebuah program yang:
1. Membaca file CSV dan menyimpan datanya ke dalam dictionary.
2. Menghitung rata-rata nilai tiap mahasiswa.
3. Menampilkan mahasiswa dengan nilai tertinggi dan terendah

**Kode Program:**

```
#Soal 4

#Mengimport pandas untuk melakukan pembacaan data
import pandas as pd

#Mendefinisikan sebuah fungsi untuk membaca file csv.
def read_csv(file):
    df = pd.read_csv(file)
    return df

#Mendefinisikan sebuah fungsi untuk menghitung Average (rata-rata) nilai tertinggi dan terendah.
def count_avg(df):
    df['AVG'] = df.iloc[:, 1:].mean(axis=1)
    return df

#Mendefinisikan sebuah fungsi untuk mengetahui nilai min dan max dari data.
def min_max(df):
    max_grade = df.loc[df['AVG'].idxmax()]
    min_grade = df.loc[df['AVG'].idxmin()]
    return max_grade, min_grade

#Mendefinisikan sebuah fungsi untuk menghitung rata-rata dari seluruh nilai.
def AVG_all(df):
    overall_avg = df['AVG'].mean()
    return overall_avg

#Mendefinisikan sebuah variabel dari fungsi yang telah dibuat
file = 'siswa_nilai.csv'
df = read_csv(file)
df_AVG = count_avg(df)
max_grade, min_grade = min_max(df_AVG)
overall_AVG = AVG_all(df_AVG)

print("Rata-rata nilai mahasiswa:")
print(df_AVG[['Nama Siswa', 'Nilai']])

print("\nMahasiswa dengan nilai tertinggi:")
print(max_grade[['Nama Siswa', 'AVG']])

print("\nMahasiswa dengan nilai terendah:")
print(min_grade[['Nama Siswa', 'AVG']])

# Tampilkan rata-rata nilai seluruh mahasiswa
print(f"\nRata-rata nilai seluruh mahasiswa: {overall_AVG:.2f}")
```

**Penjelasan**

#### Bagian 1

```
import pandas as pd

def read_csv(file):
    df = pd.read_csv(file)
    return df
```

- Mengimpor pustaka pandas yang digunakan untuk manipulasi data berbasis tabel, khususnya dalam format DataFrame.
- Fungsi read_csv digunakan untuk membaca file CSV dan mengonversinya menjadi DataFrame pandas.

#### Bagian 2

```
def count_avg(df):
    df['AVG'] = df.iloc[:, 1:].mean(axis=1)
    return df
```

Fungsi count_avg menambahkan kolom baru AVG ke dalam DataFrame yang berisi rata-rata nilai dari setiap siswa.

#### Bagian 3

```
def min_max(df):
    max_grade = df.loc[df['AVG'].idxmax()]
    min_grade = df.loc[df['AVG'].idxmin()]
    return max_grade, min_grade
```

Fungsi min_max digunakan untuk mencari siswa dengan nilai rata-rata tertinggi dan terendah.
- df['AVG'].idxmax() mencari indeks (baris) dengan nilai tertinggi di kolom AVG.
- df['AVG'].idxmin() mencari indeks dengan nilai terendah di kolom AVG.
- df.loc[] digunakan untuk mengambil data baris sesuai indeks yang ditemukan.
- Fungsi ini mengembalikan dua DataFrame: satu untuk siswa dengan nilai tertinggi (max_grade) dan satu untuk siswa dengan nilai terendah (min_grade).

#### Bagian 4

```
def AVG_all(df):
    overall_avg = df['AVG'].mean()
    return overall_avg
```

Fungsi AVG_all menghitung rata-rata keseluruhan dari nilai rata-rata (AVG) semua siswa.
- df['AVG'].mean() digunakan untuk menghitung rata-rata dari kolom AVG.
- Rata-rata keseluruhan ini kemudian dikembalikan oleh fungsi.

#### Bagian 5

```
file = 'siswa_nilai.csv'
df = read_csv(file)
df_AVG = count_avg(df)
max_grade, min_grade = min_max(df_AVG)
overall_AVG = AVG_all(df_AVG)
```

- File CSV dibaca menggunakan read_csv(file) dan hasilnya disimpan dalam DataFrame df.
- Fungsi count_avg(df) dijalankan untuk menambahkan kolom AVG pada DataFrame, disimpan dalam variabel df_AVG.
- Fungsi min_max(df_AVG) dijalankan untuk menemukan siswa dengan nilai tertinggi dan terendah.
- Fungsi AVG_all(df_AVG) digunakan untuk menghitung rata-rata keseluruhan nilai semua siswa.

#### Bagian 6

```
print("Rata-rata nilai mahasiswa:")
print(df_AVG[['Nama Siswa', 'Nilai']])

print("\nMahasiswa dengan nilai tertinggi:")
print(max_grade[['Nama Siswa', 'AVG']])

print("\nMahasiswa dengan nilai terendah:")
print(min_grade[['Nama Siswa', 'AVG']])

# Tampilkan rata-rata nilai seluruh mahasiswa
print(f"\nRata-rata nilai seluruh mahasiswa: {overall_AVG:.2f}")
```

Bagian ini mencetak hasil perhitungan:
- Menampilkan nama siswa beserta nilai rata-rata mereka.
- Menampilkan informasi siswa dengan nilai tertinggi (max_grade).
- Menampilkan informasi siswa dengan nilai terendah (min_grade).
- Mencetak rata-rata keseluruhan nilai semua siswa dengan dua angka desimal.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal4.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP4.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 4
</p> 

#### Penjelasan

Dalam output kode di atas, kita mengetahui bahwa Siswa_7 memperoleh nilai tertinggi yaitu 100 dan Siswa_5 memperoleh nilai terendah. Serta rata-rata nilai seluruh mahasiswa adalah 72.00.

### 5. Soal 5

####  Buatlah permainan sederhana menggunakan Python, di mana komputer akan memilih sebuah angka secara acak antara 1 hingga 100, dan pengguna harus menebak angka tersebut. Setiap tebakan yang salah akan memberikan petunjuk apakah angka yang ditebak lebih besar atau lebihkecil dari angka sebenarnya. Batasi jumlah percobaan menjadi 5 kali. Setelah permainan selesai, tampilkan apakah pemain menang atau kalah

**Kode Program:**

```
#Soal 5

#Mengimport angka random
import random

#Mendefinisikan sebuah fungsi untuk melakukan permainan penebakan angka.
def guess_number_game():
    secret_number = random.randint(1, 100) 
    max_attempts = 5 
    attempts = 0
    lower_bound = 1
    upper_bound = 100

    #Memunculkan kata-kata di awal permainan.
    print("Selamat datang di permainan tebak angka!")
    print(f"Komputer telah memilih angka antara {lower_bound} hingga {upper_bound}.")
    print(f"Anda memiliki {max_attempts} kali percobaan untuk menebak angka tersebut.")

    #Menggunakan looping while
    while attempts < max_attempts:
        print(f"\nIndikator: {lower_bound}-{upper_bound}")
        guess = int(input(f"Percobaan {attempts + 1}: Masukkan tebakan Anda: "))

        if guess < secret_number:
            print(f"Jawaban berada di atas angka {guess}.")
            lower_bound = guess + 1  
        elif guess > secret_number:
            print(f"Jawaban berada di bawah angka {guess}.")
            upper_bound = guess - 1  
        else:
            print(f"Selamat! Anda berhasil menebak angka {secret_number} dengan benar!")
            break

        attempts += 1

    if attempts == max_attempts and guess != secret_number:
        print(f"\nMaaf, Anda kehabisan percobaan. Angka yang benar adalah {secret_number}.")

    print("Terima kasih sudah bermain!")

#Mendefinisikan fungsi main(utama)
def main():
    while True:
        guess_number_game()  # Run the game
        choice = input("\nIngin bermain ulang? (ya/tidak): ").lower()
        if choice != 'ya':
            print("Terima kasih! Sampai jumpa lagi.")
            break
            
main()
```

**Penjelasan**

#### Bagian 1

```
import random

def guess_number_game():
    secret_number = random.randint(1, 100) 
    max_attempts = 5 
    attempts = 0
    lower_bound = 1
    upper_bound = 100
```

Modul random diimpor untuk menghasilkan angka acak. Dalam hal ini, digunakan untuk menentukan angka rahasia yang akan ditebak oleh pemain.

guess_number_game adalah fungsi utama yang menjalankan permainan.
- secret_number adalah angka acak yang dipilih komputer dalam rentang 1 sampai 100. Angka ini yang harus ditebak pemain.
- max_attempts = 5 menentukan jumlah maksimum percobaan yang diberikan kepada pemain untuk menebak angka.
- attempts = 0 adalah penghitung percobaan yang dimulai dari nol.
- lower_bound dan upper_bound mengatur batas bawah dan atas rentang angka yang harus ditebak oleh pemain, dimulai dari 1 hingga 100.

#### Bagian 2

```
    print("Selamat datang di permainan tebak angka!")
    print(f"Komputer telah memilih angka antara {lower_bound} hingga {upper_bound}.")
    print(f"Anda memiliki {max_attempts} kali percobaan untuk menebak angka tersebut.")
```

Pesan ini memberikan instruksi kepada pemain mengenai aturan permainan.

#### Bagian 3

```
    while attempts < max_attempts:
        print(f"\nIndikator: {lower_bound}-{upper_bound}")
        guess = int(input(f"Percobaan {attempts + 1}: Masukkan tebakan Anda: "))
        if guess < secret_number:
            print(f"Jawaban berada di atas angka {guess}.")
            lower_bound = guess + 1  
        elif guess > secret_number:
            print(f"Jawaban berada di bawah angka {guess}.")
            upper_bound = guess - 1  
        else:
            print(f"Selamat! Anda berhasil menebak angka {secret_number} dengan benar!")
            break
    if attempts == max_attempts and guess != secret_number:
        print(f"\nMaaf, Anda kehabisan percobaan. Angka yang benar adalah {secret_number}.")
    print("Terima kasih sudah bermain!")
```

Looping while: selama jumlah percobaan (attempts) masih kurang dari jumlah maksimal percobaan (max_attempts), permainan terus berlanjut.
- print(f"\nIndikator: {lower_bound}-{upper_bound}"): Menampilkan rentang batas tebakan yang valid (rentang ini akan diperbarui setelah setiap tebakan).
- guess = int(input(...)): Pemain diminta untuk memasukkan tebakan angka, yang dikonversi ke integer.

#### Bagian 4

```
def main():
    while True:
        guess_number_game()  # Run the game
        choice = input("\nIngin bermain ulang? (ya/tidak): ").lower()
        if choice != 'ya':
            print("Terima kasih! Sampai jumpa lagi.")
            break
main()
```

Fungsi main mengatur logika utama dari permainan dan memberi pemain pilihan untuk bermain lagi atau berhenti.
- while True:: Permainan terus berjalan sampai pemain memilih untuk berhenti.
- Setelah permainan selesai, pemain ditanya apakah mereka ingin bermain ulang.
- Jika pemain memilih "ya", permainan akan dimulai lagi.
- Jika pemain memilih selain "ya", program mencetak pesan perpisahan dan keluar dari loop menggunakan break.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal5.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP5.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 5
</p> 

#### Penjelasan

Dalam program yang telah dibuat terdapat output dimana pada awal Run akan memberikan pesan kepada user. User akan diberikan 5 kali kesempatan untuk menebak angka yang dipilih oleh komputer. Dalam outputnya komputer memberikan indikator atau rentang dari nilai yang dimasukkan user apakah sudah mendekati dengan angka yang dipilih komputer. Jika dalam 5 kali tebakan salah maka akan muncul pesan kehabisan percobaan.

### 6. Soal 6

####  Buat fungsi rekursif yang menerima input bilangan bulat `n` dan menghasilkan urutan bilangan seperti berikut ini:

Input: n = 4

Output: 1, 1, 2, 6, 24

**Kode Program:**

```
#Soal 6

#Mendefinisikan sebuah fungsi untuk membuat bilangan faktorial.
def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n*factorial(n-1)

#Mendefinisikan sebuah fungsi untuk mengembalikan faktorial.
def fac_order(n):
    if n <= 0:
        return []

    result = [] #mengumpulkan hasil dalam list
    for i in range(n + 1):
        result.append(factorial(i))

    return result

n = 4 #memasukkan nilai 4 sebagai parameter
output = fac_order(n)
print(output)
```

**Penjelasan**

#### Bagian 1

```
def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n-1)
```

factorial(n) adalah fungsi rekursif yang menghitung faktorial dari sebuah bilangan. Menggunakan kasus if dan else untuk memberikan dua kondisi yang berbeda.

#### Bagian 2

```
def fac_order(n):
    if n <= 0:
        return []
    result = []  # mengumpulkan hasil dalam list
    for i in range(n + 1):
        result.append(factorial(i))
    return result
```

fac_order(n) adalah fungsi yang mengembalikan daftar semua faktorial dari 0 hingga n atau n sebagai parameter. result adalah list kosong yang akan digunakan untuk menyimpan hasil faktorial dari setiap bilangan dari 0 hingga n. Setelah loop selesai, fungsi fac_order(n) akan mengembalikan list result yang berisi semua faktorial dari 0 hingga n.

#### Bagian 3

```
n = 4  # memasukkan nilai 4 sebagai parameter
output = fac_order(n)
print(output)
```

- Variabel n = 4 berarti kita ingin menghitung faktorial dari 0 hingga 4.
- output = fac_order(n) memanggil fungsi fac_order(4), yang akan mengembalikan list faktorial dari 0 hingga 4.
- print(output) menampilkan hasil faktorial dari 0 hingga 4 dalam bentuk list.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal6.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP6.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 6
</p> 

#### Penjelasan

Dalam kode di atas, terdapat output dari nilai faktorialmnya sesuai dengan bentuk kode yang diberikan yang dimulai dengan angka 1.

### 7. Soal 7

####  Buat fungsi rekursif yang menerima input bilangan bulat `n` dan menghasilkan urutan bilangan seperti berikut ini:

Input: n = 4

Output: 1, 1, 2, 6, 24

**Kode Program:**

```
#Soal 7

#Mendefinisikan sebuah fungsi untuk menentukan minimum koin yang dibutuhkan.
def min_coins(coins, amount): #Terdapat dua parameter coins, amount
    dynamic_p = [float('inf')] * (amount + 1)
    dynamic_p[0] = 0
    coin_used = [-1] * (amount + 1)  # Array untuk menyimpan koin yang digunakan

    #Membuat looping for
    for coin in coins:
        for x in range(coin, amount + 1):
            if dynamic_p[x - coin] + 1 < dynamic_p[x]:
                dynamic_p[x] = dynamic_p[x - coin] + 1
                coin_used[x] = coin  # Simpan koin yang digunakan

    # Jika tidak ada solusi, kembalikan -1
    if dynamic_p[amount] == float('inf'):
        return -1, []

    # Mengembalikan jumlah minimum koin dan rincian koin
    count = dynamic_p[amount]
    combination = []
    while amount > 0:
        combination.append(coin_used[amount])
        amount -= coin_used[amount]

    return count, combination

#Mendefinisikan sebuah fungsi utama yaitu fungsi main sebagai eksekutor kode
def main():
    amount = int(input("Masukkan jumlah uang yang ingin dicapai: "))
    coins = list(map(int, input("Masukkan koin yang tersedia, pisahkan dengan spasi: ").split()))

    result, combination = min_coins(coins, amount)

    if result != -1:
        print(f"Jumlah minimum koin yang diperlukan: {result}")
        print("Koin yang digunakan:", combination)
    else:
        print("Tidak ada koin yang memenuhi jumlah tersebut.")

if __name__ == "__main__":
    main()
```

**Penjelasan**

#### Bagian 1

```
def min_coins(coins, amount):
    dynamic_p = [float('inf')] * (amount + 1)
    dynamic_p[0] = 0
    coin_used = [-1] * (amount + 1)  # Array untuk menyimpan koin yang digunakan
```

Pada kode di atas, dibuatkan fungsi min_coins dengan parameter coins dan amount. dynamic_p: List untuk menyimpan solusi submasalah. Indeks dari list ini merepresentasikan jumlah uang, dan nilai di setiap indeks merepresentasikan jumlah minimum koin yang dibutuhkan untuk mencapai jumlah tersebut. coin_used: List untuk melacak koin yang digunakan untuk mencapai setiap jumlah. Awalnya diisi dengan -1 sebagai tanda tidak ada koin yang digunakan.

#### Bagian 2

```
    for coin in coins:
        for x in range(coin, amount + 1):
            if dynamic_p[x - coin] + 1 < dynamic_p[x]:
                dynamic_p[x] = dynamic_p[x - coin] + 1
                coin_used[x] = coin  # Simpan koin yang digunakan
    if dynamic_p[amount] == float('inf'):
        return -1, []
    count = dynamic_p[amount]
    combination = []
    while amount > 0:
        combination.append(coin_used[amount])
        amount -= coin_used[amount]
    return count, combination
```

- Outer loop (for coin in coins): Loop ini iterasi melalui setiap koin yang tersedia.
- Inner loop (for x in range(coin, amount + 1)): Iterasi ini dimulai dari nilai koin dan berlanjut hingga amount. Setiap nilai x mewakili jumlah uang yang sedang dioptimalkan.
- Jika nilai dynamic_p[amount] tetap float('inf'), berarti tidak ada kombinasi koin yang bisa mencapai jumlah yang diinginkan. Kembalikan -1 dan list kosong.
- count: Menyimpan jumlah minimum koin yang diperlukan untuk mencapai amount.
- combination: List untuk menyimpan koin yang digunakan.

#### Bagian 3

```
def main():
    amount = int(input("Masukkan jumlah uang yang ingin dicapai: "))
    coins = list(map(int, input("Masukkan koin yang tersedia, pisahkan dengan spasi: ").split()))
    result, combination = min_coins(coins, amount)

    if result != -1:
        print(f"Jumlah minimum koin yang diperlukan: {result}")
        print("Koin yang digunakan:", combination)
    else:
        print("Tidak ada koin yang memenuhi jumlah tersebut.")

if __name__ == "__main__":
    main()
```

Fungsi ini merupakan fungsi utama yang akan mengeksekusi seluruh fungsi yang telah dibuat.
- amount: Input dari pengguna, yaitu jumlah uang yang ingin dicapai.
- coins: List dari koin yang tersedia, diambil dari input pengguna.
Fungsi if __name__ == "__main__": main() memastikan bahwa ketika file dijalankan secara langsung, program akan memanggil fungsi main() dan memulai permainan.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal7.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP7.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 7
</p> 

#### Penjelasan

Dalam output yang dihasilkan kode di atas, user diminta untuk menuliskan angka koin yang ingin dicapai. User juga memasukkan pecahan angka koin, misal 1, 5, 10, 25. Misalkan angka koin 50 dapat diperoleh dengan kombinasi koin 25 sebanyak 2 koin.

### 8. Soal 8

#### Buat sebuah program yang menerima string dari pengguna dan mengonversi string tersebut menjadi sebuah list berisi kata-kata terbalik. 

**Kode Program:**

```
#Soal 8

#Mendefinisikan sebuah fungsi untuk mereverse string yang diinputkan
def reverse_string(inp):
    x = inp.split() #melakukan split pada parameter yang diberikan
    reversed = [y[::-1] for y in x]
    return reversed

#Mendefinisikan fungsi utama untuk dieksekusi
def main():
    user_inp = input("Tuliskan kalimat atau kata: ")
    result = reverse_string(user_inp)

    print("Output: ", result)

if __name__=="__main__":
    main()
```

**Penjelasan**

#### Bagian 1

```
def reverse_string(inp):
    x = inp.split()  # Melakukan split pada parameter yang diberikan
    reversed = [y[::-1] for y in x]
    return reversed
```

Membuat fungsi reverse_string dengan parameter inp. x = inp.split(): Fungsi split() membagi string input berdasarkan spasi, memisahkannya menjadi list dari kata-kata. Misalnya, jika input adalah "Halo Dunia", hasilnya adalah ['Halo', 'Dunia']. reversed = [y[::-1] for y in x]: Ini adalah list comprehension yang melakukan iterasi pada setiap elemen (kata) dalam list x.

#### Bagian 2

```
def main():
    user_inp = input("Tuliskan kalimat atau kata: ")
    result = reverse_string(user_inp)

    print("Output: ", result)
```

- user_inp = input("Tuliskan kalimat atau kata: "): Meminta input dari pengguna berupa string.
- result = reverse_string(user_inp): Memanggil fungsi reverse_string dengan input pengguna (user_inp) sebagai argumen, lalu hasilnya disimpan dalam variabel result.
- print("Output: ", result): Menampilkan hasil pembalikan kata dalam list yang dikembalikan oleh fungsi reverse_string

#### Bagian 3

```
if __name__=="__main__":
    main()
```

Fungsi ini memastikan bahwa program hanya akan menjalankan fungsi main() jika file ini dijalankan secara langsung, bukan diimport sebagai modul.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal8.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP8.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 8
</p> 

#### Penjelasan

Pada output yang dihasilkan, user memasukkan kalimat Saya suka Python dimana ketika kalimat tersebut di reverse akan menghasilkan ayaS akus nohtyP. Hal ini sesuai dengan fungsi yang dibuat dan fungsi main di akhir kode.

### 9. Soal 9

#### Buat class bernama `Buku` yang memiliki atribut `judul`, `penulis`, dan `tahun_terbit`. Buat method dalam class untuk menampilkan informasi buku, serta method untuk menghitung usia buku berdasarkan tahun saat ini. Buatlah 3 objek dari class `Buku` dan tampilkan informasi serta usia masing-masing buku

**Kode Program:**

```
#Soal 9

#Membuat sebuah class yang akan terdiri dari beberapa fungsi yang didefinisikan
class Book:
    #Mendefinisikan sebuah fungsi yang berisikan beberapa variabel.
    def __init__(self, title, author, year_published, page_count, edition, publisher):
        self.title = title
        self.author = author
        self.year_published = year_published
        self.page_count = page_count
        self.edition = edition
        self.publisher = publisher

    #Mendefinisikan sebuah fungsi untuk display yang akan muncul di output
    def display_info(self):
        return (f"Judul: '{self.title}'\n"
                f"Penulis: {self.author}\n"
                f"Tahun Terbit: {self.year_published}\n"
                f"Tebal Halaman: {self.page_count} halaman\n"
                f"Cetakan ke: {self.edition}\n"
                f"Diterbitkan Oleh: {self.publisher}")

    def calculate_age(self, current_year): #fungsi dengan parameter self dan current_year
        return current_year - self.year_published

    def full_info(self, current_year): #fungsi dengan parameter self dan current_year
        age = self.calculate_age(current_year)
        return f"{self.display_info()}\nUsia Buku: {age} tahun\n"

#Mendifinisikan sebuah fungsi main atau fungsi utama untuk melakukan eksekusi pada kode
def main():
    # Current year
    current_year = 2024
    
    # Creating objects from the Book class
    book1 = Book("Belajar Python di Data Science", "Rizal Wahyu Pratama", 2021, 300, 2, "Gramedia")
    book2 = Book("Data Science untuk Pemula", "Khulika Malkan", 2023, 250, 1, "Elex Media")
    book3 = Book("Kecerdasan Buatan untuk Pengolahan Data", "Mikhael Setia Budi", 2019, 400, 3, "Mitra Widya")

    # Displaying information and age of each book
    book_list = [book1, book2, book3]
    
    for book in book_list:
        print(book.full_info(current_year))
        print("-" * 30)  # Separator for neater output

if __name__ == "__main__":
    main()
```

**Penjelasan**

#### Bagian 1

```
class Book:
    def __init__(self, title, author, year_published, page_count, edition, publisher):
        self.title = title
        self.author = author
        self.year_published = year_published
        self.page_count = page_count
        self.edition = edition
        self.publisher = publisher
```

- class Book:: Mendefinisikan sebuah class bernama Book yang akan digunakan untuk menyimpan data terkait buku.
- __init__(...): Merupakan konstruktor atau inisialisasi kelas. Fungsi ini dipanggil ketika objek dari kelas Book dibuat.
Parameter title, author, year_published, page_count, edition, dan publisher adalah atribut yang disimpan untuk setiap buku yang dibuat.

#### Bagian 2

```
def display_info(self):
    return (f"Judul: '{self.title}'\n"
            f"Penulis: {self.author}\n"
            f"Tahun Terbit: {self.year_published}\n"
            f"Tebal Halaman: {self.page_count} halaman\n"
            f"Cetakan ke: {self.edition}\n"
            f"Diterbitkan Oleh: {self.publisher}")
```

Fungsi ini bertujuan untuk menampilkan informasi dari objek buku dalam format string yang rapi. Fungsi f-string digunakan untuk memasukkan variabel ke dalam string.

#### Bagian 3

```
def calculate_age(self, current_year):
    return current_year - self.year_published
```

Fungsi ini menghitung usia buku berdasarkan tahun publikasi dan tahun saat ini. current_year: Parameter yang digunakan untuk menentukan tahun saat ini. Fungsi mengembalikan selisih antara tahun saat ini dan tahun terbit buku.

#### Bagian 4

```
def full_info(self, current_year):
    age = self.calculate_age(current_year)
    return f"{self.display_info()}\nUsia Buku: {age} tahun\n"
```

Fungsi ini menggabungkan informasi yang ditampilkan oleh display_info dengan informasi usia buku yang dihitung oleh calculate_age.

#### Bagian 5

```
def main():
    current_year = 2024
    
    book1 = Book("Belajar Python di Data Science", "Rizal Wahyu Pratama", 2021, 300, 2, "Gramedia")
    book2 = Book("Data Science untuk Pemula", "Khulika Malkan", 2023, 250, 1, "Elex Media")
    book3 = Book("Kecerdasan Buatan untuk Pengolahan Data", "Mikhael Setia Budi", 2019, 400, 3, "Mitra Widya")

    book_list = [book1, book2, book3]
    
    for book in book_list:
        print(book.full_info(current_year))
        print("-" * 30)

if __name__ == "__main__":
    main()
```

- current_year = 2024: Variabel untuk tahun saat ini, digunakan dalam perhitungan usia buku. Lalu membuat 3 objek buku yang diinputkan beberapa info. for book in book_list:: Melakukan iterasi untuk setiap buku dalam daftar book_list. Memanggil full_info() untuk menampilkan informasi lengkap dari setiap buku, termasuk usia buku.
- print("-" * 30): Mencetak garis pemisah agar tampilan output lebih rapi.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal9.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP9.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 9
</p> 

#### Penjelasan

Dalam output kode di atas, telah dibuat 3 jenis data buku. Misalkan data buku pertama dengan judul Belajar Python di Data Science dengan Rizal Wahyu Pratama sebagai penulisnya, tahun terbit 2021 dan lain sebagainya. Seluruh informasi dalam output sudah di atur dalam kode.

### 10. Soal 10

#### Buatlah program yang mengimplementasikan algoritma pencarian biner, namun dengan modifikasi: algoritma harus bisa mencari nilai di list yang hanya berisi angka genap, dan jika nilai yang dicari adalah angka ganjil, program harus menampilkan pesan bahwa nilai tersebut tidak bisa ditemukan.

**Kode Program:**

```
#Soal 10

#Mendefinisikan sebuah fungsi yaitu binary_search
def binary_search(even_numbers, target): #parameter even_numbers, target
    left, right = 0, len(even_numbers) - 1

    #menggunakan loop while
    while left <= right:
        mid = (left + right) // 2
        
        if even_numbers[mid] == target:
            return mid  # Mengembalikan indeks jika ditemukan
        elif even_numbers[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
            
    return -1  # Mengembalikan -1 jika tidak ditemukan

#Mendefinisikan sebuah fungsi untuk membuat even number
def generate_even_numbers(limit):
    # Menghasilkan daftar angka genap hingga limit yang ditentukan
    return [i for i in range(0, limit + 1, 2)]

#Mendefinisikan sebuah fungsi main atau fungsi utama untuk eksekusi seluruh fungsi yang dibuat
def main():
    while True:  # Loop utama program
        # Menerima batas dari pengguna
        limit = int(input("Masukkan batas atas untuk daftar angka genap: "))
        
        # Menghasilkan daftar angka genap
        even_numbers = generate_even_numbers(limit)
        
        # Menerima input dari pengguna
        target = int(input("Masukkan angka yang ingin dicari: "))
        
        # Cek apakah angka yang dicari genap atau ganjil
        if target % 2 != 0:
            print("\nNilai yang dicari adalah angka ganjil, pencarian tidak dapat dilakukan.")
        else:
            # Melakukan pencarian biner
            result = binary_search(even_numbers, target)
            
            if result != -1:
                print(f"\nAngka {target} ditemukan pada indeks {result}.")
            else:
                print(f"\nAngka {target} tidak ditemukan dalam daftar.")

        # Menanyakan kepada pengguna apakah ingin mengulang program
        ulang = input("\nApakah Anda ingin mengulang program? (ya/tidak): ").strip().lower()
        if ulang != 'ya':
            break

    print("\nTerima kasih telah menggunakan program ini!")

if __name__ == "__main__":
    main()
```

**Penjelasan**

#### Bagian 1

```
def binary_search(even_numbers, target):
    left, right = 0, len(even_numbers) - 1

    while left <= right:
        mid = (left + right) // 2
        
        if even_numbers[mid] == target:
            return mid
        elif even_numbers[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
            
    return -1
```

Membuat fungsi binary_search dengan parameter even_numbers dan target. left dan right: Variabel yang menunjukkan batas kiri dan kanan dari rentang pencarian. Awalnya, left adalah indeks pertama (0) dan right adalah indeks terakhir (len(even_numbers) - 1). Lalu menggunakan loop while yang di dalamnya terdapat pengkondisian menggunakan if dan else.

#### Bagian 2

```
def generate_even_numbers(limit):
    return [i for i in range(0, limit + 1, 2)]
```

Fungsi ini menghasilkan daftar bilangan genap hingga batas yang ditentukan oleh pengguna dengan parameter limit.

#### Bagian 3

```
def main():
    while True:
        limit = int(input("Masukkan batas atas untuk daftar angka genap: "))
        even_numbers = generate_even_numbers(limit)
        
        target = int(input("Masukkan angka yang ingin dicari: "))
        
        if target % 2 != 0:
            print("\nNilai yang dicari adalah angka ganjil, pencarian tidak dapat dilakukan.")
        else:
            result = binary_search(even_numbers, target)
            
            if result != -1:
                print(f"\nAngka {target} ditemukan pada indeks {result}.")
            else:
                print(f"\nAngka {target} tidak ditemukan dalam daftar.")

        ulang = input("\nApakah Anda ingin mengulang program? (ya/tidak): ").strip().lower()
        if ulang != 'ya':
            break

    print("\nTerima kasih telah menggunakan program ini!")
```

Fungsi main merupakan fungsi yang pertama kali dieksekusi karena merupakan fungsi utama. Dalam fungsi ini terdapat looping yang menggunakan while True dimana di dalamnya terdapat if dan else sebagai pengkondisian. ulang = input(...).strip().lower(): Menanyakan kepada pengguna apakah ingin mengulang program. Jika jawabannya bukan 'ya', program akan keluar dari loop.

#### Bagian 4

```
if __name__ == "__main__":
    main()
```

Kode ini adalah blok standar untuk memastikan bahwa fungsi main() hanya dijalankan jika file ini dijalankan langsung, bukan ketika diimport sebagai modul.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/Soal10.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%201/Assets/OP10.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 10
</p> 

#### Penjelasan

Pada output kode di atas pengguna diminta memasukkan batas atas angka genap, yang dimasukkan adalah 5000. Lalu, untuk angka yang ingin dicari adalah 2500 yang terletak pada indeks ke 1250. Lalu user diberikan pertanyaan untuk mengulang program atau tidak, dan user memilih tidak.

## Kesimpulan



## Referensi

[1] Shaw, Z. A. (2017). *Learn Python the Hard Way: A Very Simple Introduction to the Terrifyingly Beautiful World of Computers and Code*. Addison-Wesley.

[2] Lutz, M. (2019). *Python Crash Course: A Hands-On, Project-Based Introduction to Programming*. No Starch Press.

[3] McKinney, W. (2017). *Python for Data Analysis: Data Wrangling with Pandas, NumPy, and IPython*. O'Reilly Media.

[4] Zandbergen, P. A. (2020). *Python Scripting for ArcGIS Pro*. Esri Press.

[5] Oliphant, T. E. (2015). *Guide to NumPy*. Createspace Independent Publishing Platform.

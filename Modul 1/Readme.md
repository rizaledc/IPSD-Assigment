# <h1 align="center">Laporan Praktikum Dasar-Dasar Python untuk Sains Data</h1>

<p align="center">Rizal Wahyu Pratama</p>
<p align="center">2311110029</p>
<p align="center">S1SD-04-02</p>

## Tujuan Praktikum

1. Siswa memahami dan menggunakan tipe serta struktur data dasar di Python.
2. Siswa menerapkan operator, logika, dan percabangan untuk pengambilan keputusan.
3. Siswa mampu membuat fungsi dan menggunakan pengulangan untuk efisiensi kode.

## Dasar Teori

### A. Algoritma Rekursif

Algoritma rekursif merupakan metode yang baik serta efektif diekspresikan sebagai rangkaian terbatas untuk melakukan suatu perintah. Algoritma Rekursif terdiri dari dua kata yaitu algoritma dan rekursif [1]. Dimana algoritma menurut Gun Gun Maulana merupakan metode efektif yang diekspresikan sebagai rangkaian terbatas. Algoritma juga merupakan kumpulan perintah untuk menyelesaikan masalah. Menurut Wilis Kaswidjanti, S.SI., M.Kom Rekursif merupakan alat untuk memecahkan masalah dalam suatu fungsi atau procedure yang memanggil dirinya sendiri. Logika rekursif memiliki sebuah parameter yang dapat berguna untuk memaggil dirinya sendiri[2]. Logika ini digunakan untuk menggantikan proses iterasi (perulangan). Definisi menurut Niclaus Wirth : “ An object is said be recursive if it partially consist or is defines in terms of it self”

Perulangan dapat diubah menjadi kode rekursif agar lebih singkat dalam proses kompilasi dan interpretasi. Rekursi dapat diterapkan dalam masalah pengurutan, pencarian, serta penjelajahan yang sering kali diselesaikan dengan kode rekursif sederhana [3]. 

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/Gambaran%20Rekursif%20Berjalan.png" alt="Alt Text">
</p> 
<p align="center">
 Gambar 1. Ilustrasi Fungsi Rekursif Berjalan
</p> 

Pada ilustrasi di atas, terdapat 5 kali print dimulai dari perulangan pertama hingga perulangan ke 5. Perulangan ini tentunya menggunakan sebuah parameter seperti n. Selain itu, terdapat dua jenis rekursif yang harus diketahui sebagai berikut:

- Rekursif Langsung
  Fungsi memanggil dirinya sendiri secara eksplisit atau secara langsung.
- Rekursif Tidak Langsung
  Fungsi yang memiliki serangkaian pemanggilan fungsi di dalamnya, tetapi tidak ada pemanggilan langsung ke fungsi itu sendiri.

Berikut contohnya:

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/Gambaran%20Rekursif%20Langsung%20dan%20Tidak.png" alt="Alt Text">
</p> 
<p align="center">
 Gambar 2. Gambaran Code Rekursi
</p> 

Adapun kelebihan serta kekurangan dalam menggunakan kode rekursif sebagai berikut:

  A. Kelebihan
  1. Memberikan kemudahan dalam kode sehingga mudah dimengerti.
  2. Sangat efektif untuk masalah yang dapat dibagi menjadi sub-bab sub-bab yang lebih kecil.
  3. Tampilan kode yang lebih baik dan elegan.
     
  B. Kekurangan
  
  1. Rekursif menambah overhead pada call stack.
  2. Implementasi kurang efisien dalam waktu seperti overhead pemanggilan fungsi.
  3. Potensi overflow dan bug.
     
### B. Hash Table

Hash table merupakan bagian dari struktur data yang dapat digunakan untuk menyimpan nilai dengan kunci dengan efisiensi tinggi dalam pencarian, penyisipan, dan penghapusan data. Hash table biasanya terdiri dari dua komponen utama diantaranya array/vektor dan fungsi hash. Teknik hash disebut dengan hashing yang digunakan untuk mengubah rentang nilai kunci menjadi rentang indeks array.

Dalam hash table terdapat bucket yang merupakan tempat array untuk menyimpan data dalam bentuk slot-slot. Dalam hashing dapat menghasilkan nilai unik dari setiap datanya yang dapat digunakan untuk indeks dalam array. Sehingga, hash table memungkinkan pencarian data dengan waktu konstan (O(1)) dalam kasus terbaik.

Sistem hash table bekerja dengan mengambil inputan kunci lalu memetakannya ke nilai indeks menggunakan fungsi hash. Data dapat disimpan pada posisi indeks array yang dihasilkan oleh fungsi hash. Fungsi hash mengambil kunci dan mengubahnya menjadi hash code, yaitu bilangan bulat yang kemudian digunakan sebagai indeks dalam array. Jika terjadi tabrakan (collision), di mana dua kunci memiliki indeks yang sama, hash table mengatasi ini dengan berbagai metode seperti chaining (menggunakan linked list untuk setiap indeks) atau open addressing (mencari indeks kosong berikutnya dalam array). Hash table banyak digunakan dalam implementasi struktur data seperti set dan map di berbagai bahasa pemrograman karena efisiensinya yang tinggi dalam menangani sejumlah besar data.

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/Gambaran%20Hash%20Table.png" alt="Alt Text">
</p> 
<p align="center">
 Gambar 3. Gambaran Hash Table
</p> 

Pada gambar di atas dapat kita pahami bahwa fungsi hash membuat pemetaan antara kunci dan nilai. Hasil dari hashing disebut sebagai nilai hash yang akan direpresentasikan dari string karakter asli tetapi biasanya lebih kecil dibandingkan dengan aslinya.

Operasi pada hash table meliputi tiga operasi utama: penyisipan (insertion), pencarian (search), dan penghapusan (deletion). Berikut adalah penjelasan masing-masing operasi:

1. Penyisipan (Insertion)
   - Proses penyisipan dimulai dengan mengambil kunci dari pasangan kunci-nilai.
   - Kunci tersebut kemudian diproses oleh fungsi hash untuk menghasilkan indeks dalam array.
   - Jika slot pada indeks tersebut kosong, nilai disisipkan di sana.
   - Jika slot sudah terisi (terjadi tabrakan), metode penanganan tabrakan seperti chaining (menggunakan linked list) atau open addressing (mencari slot kosong berikutnya) digunakan untuk menyimpan nilai tersebut.

2. Pencarian (Search)
   - Untuk mencari nilai berdasarkan kunci, fungsi hash digunakan untuk menghitung indeks dari kunci tersebut.
   - Array diakses pada indeks yang dihasilkan. 
   - Jika kunci yang diinginkan ada di slot tersebut, nilainya dikembalikan.
   - Jika terjadi tabrakan, metode penanganan tabrakan digunakan untuk mencari kunci yang benar.
   - Proses pencarian biasanya sangat cepat, dengan kompleksitas rata-rata O(1).

3. Penghapusan (Deletion)
   - Penghapusan dimulai dengan menghitung indeks dari kunci menggunakan fungsi hash.
   - Indeks tersebut diakses dalam array.
   - Jika kunci ditemukan pada indeks tersebut, nilai dihapus.
   - Jika terjadi tabrakan, metode penanganan tabrakan digunakan untuk menemukan dan menghapus kunci yang benar.
   - Setelah penghapusan, beberapa metode mungkin memerlukan penanganan tambahan untuk menjaga integritas struktur data.

Secara umum, efisiensi hash table bergantung pada kualitas fungsi hash dan metode penanganan tabrakan yang digunakan. Idealnya, fungsi hash harus mendistribusikan kunci secara merata ke seluruh array untuk meminimalkan tabrakan dan mempertahankan performa yang optimal.

Collision Resolution

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/Resolution.png" alt="Alt Text">
</p> 
<p align="center">
 Gambar 4. Collision Resolution Technique
</p> 

Collision merupakan keterbatasan hash table ketika dua angka dimasukkan ke dalam fungsi hash yang menghasilkan nilai yang sama. Cara menyelesaikannya sebagai berikut:

1. Open Hashing (Chaining)

Metode open hashing, juga dikenal sebagai separate chaining, adalah salah satu teknik penanganan tabrakan dalam hash table di mana setiap slot dalam array menyimpan daftar terhubung (linked list) dari semua elemen yang memiliki nilai hash yang sama. Ketika terjadi tabrakan, elemen baru ditambahkan ke akhir daftar terhubung di slot yang sesuai. Proses penyisipan, pencarian, dan penghapusan elemen dalam metode ini melibatkan penanganan daftar terhubung tersebut [4]. Penyisipan dilakukan dengan menambahkan elemen baru ke dalam daftar, pencarian dilakukan dengan menelusuri daftar untuk menemukan elemen dengan kunci yang diinginkan, dan penghapusan dilakukan dengan menghapus elemen dari daftar. Metode open hashing mengelola tabrakan dengan cara yang efisien, karena daftar terhubung memungkinkan penambahan elemen baru tanpa memerlukan pencarian slot kosong berikutnya dalam array. Selain itu, metode ini juga menghindari masalah clustering yang sering terjadi pada metode open addressing, sehingga performa hash table dapat tetap stabil meskipun beban (load factor) tinggi. Namun, performa metode ini juga bergantung pada panjang rata-rata dari daftar terhubung; semakin panjang daftar, semakin tinggi kompleksitas operasinya.

2. Closed Hashing

Closed hashing, juga dikenal sebagai open addressing, adalah metode penanganan tabrakan dalam hash table yang tidak menggunakan struktur data tambahan seperti linked list. Sebaliknya, elemen-elemen yang bertabrakan ditempatkan langsung di slot lain dalam array berdasarkan aturan tertentu. Berikut adalah beberapa penjabaran mengenai closed hashing:

1. Linear Probing
   - Jika terjadi tabrakan, elemen baru ditempatkan di slot berikutnya yang kosong dalam array.
   - Pencarian dan penghapusan juga mengikuti pola yang sama: mulai dari slot yang dihitung oleh fungsi hash, kemudian memeriksa slot berikutnya satu per satu hingga elemen ditemukan atau slot kosong terdeteksi.
   - Kelebihan dari linear probing adalah kesederhanaannya, namun dapat menyebabkan clustering, yaitu ketika elemen-elemen bertumpuk dalam satu area array, sehingga mengurangi efisiensi pencarian.

2. Quadratic Probing
   - Untuk mengurangi clustering yang terjadi pada linear probing, quadratic probing menggunakan kuadrat dari indeks pergeseran untuk menentukan slot berikutnya (misalnya, \(i^2\) untuk iterasi ke-i).
   - Dengan demikian, jika terjadi tabrakan, elemen baru ditempatkan pada slot berikutnya yang dihitung sebagai \((hash + i^2) \% ukuran\_array\).
   - Quadratic probing mengurangi clustering primer, tetapi masih bisa mengalami clustering sekunder dan memerlukan lebih banyak perhitungan dibandingkan linear probing.

3. Double Hashing
   - Double hashing menggunakan dua fungsi hash berbeda untuk menentukan posisi slot berikutnya saat terjadi tabrakan.
   - Jika slot yang dihitung oleh fungsi hash pertama sudah terisi, fungsi hash kedua digunakan untuk menentukan langkah pergeseran berikutnya.
   - Sebagai contoh, jika terjadi tabrakan, elemen baru ditempatkan pada slot yang dihitung sebagai \((hash1 + i * hash2) \% ukuran\_array\).
   - Double hashing cenderung lebih kompleks namun memberikan distribusi yang lebih baik dan mengurangi masalah clustering yang ada pada linear dan quadratic probing.

### 1. Guided 1

```C++
#include<iostream>
using namespace std;

// Code ini berfungsi untuk melakukan hitung mundur
// dari angka yang diinputkan
void countdown(int n) {
    if (n == 0) {
        return; // Hanya perlu 'return;' karena fungsi ini bertipe void
    }
    cout << n << " "; // Menambahkan spasi untuk pemisah antar angka
    countdown(n - 1);
}

int main() {
    cout << "Rekursif Langsung: ";
    countdown(5); // 5 merupakan inputnya
    cout << endl;
    return 0;
}
```

**Penjelasan:**

#### Bagian 1

```C++
#include<iostream>
using namespace std;
```
- #include<iostream>: Mengimpor library standar input-output di C++ yang digunakan untuk operasi input dan output.
- using namespace std;: Memungkinkan kita menggunakan elemen-elemen dalam namespace std (standard) tanpa perlu menuliskan std:: sebelum setiap fungsi atau objek yang berasal dari library standar.

#### Bagian 2

```C++
void countdown(int n) {
    if (n == 0) {
        return; // Hanya perlu 'return;' karena fungsi ini bertipe void
    }
    cout << n << " "; // Menambahkan spasi untuk pemisah antar angka
    countdown(n - 1);
}
```
- Fungsi countdown adalah fungsi rekursif yang bertipe void (tidak mengembalikan nilai).
Parameter n adalah angka yang akan dihitung mundur.
- if (n == 0): Basis rekursi, jika n sama dengan 0, fungsi akan berhenti memanggil dirinya sendiri.
- cout << n << " ";: Menampilkan nilai n diikuti dengan spasi sebagai pemisah.
- countdown(n - 1);: Memanggil fungsi countdown lagi dengan nilai n dikurangi 1, ini adalah langkah rekursif yang mengurangi nilai n setiap kali fungsi dipanggil.

#### Bagian 3

```C++
int main() {
    cout << "Rekursif Langsung: ";
    countdown(5); // 5 merupakan inputnya
    cout << endl;
    return 0;
}
```

Fungsi main atau fungsi utama ini merupakan fungsi yang pertama kali akan dieksekusi dalam program. Pada main terdapat berbagai fungsi yang telah dibuat sebelumnya sehingga pada main hanya tinggal mengatur saja posisi fungsi yang telah di buat.

- cout << "Rekursif Langsung: ";: Menampilkan teks "Rekursif Langsung: " di layar.
- countdown(5);: Memanggil fungsi countdown dengan nilai awal 5.
- cout << endl;: Menambahkan baris baru setelah semua angka ditampilkan.
- return 0;: Mengakhiri fungsi main dengan mengembalikan nilai 0, yang menandakan bahwa program berakhir tanpa error.

#### Full Code Screenshot

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/CodeGuid1.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/OUTGUIDED1.png" alt="Alt Text">
</p>

#### Penjelasan

Output dari program diatas akan menampilkan output "Rekursif Langsung: 5 4 3 2 1" yang merupakan hasil dari hitung mundur dari 5 hingga 1 menggunakan pendekatan rekursif.

### 2. Guided 2

```C++
#include<iostream>
using namespace std;

void functionB(int n); // Deklarasi fungsi functionB

void functionA(int n) {
    if (n > 0) {
        cout << n << " ";
        functionB(n - 1); // Panggilan rekursif tidak langsung
    }
}

void functionB(int n) {
    if (n > 0) {
        cout << n << " ";
        functionA(n / 2); // Panggilan rekursif tidak langsung
    }
}

int main() { // Memperbaiki penulisan 'int main'
    int num = 5; // Memperbaiki penulisan 'int num = 5'
    cout << "Rekursif Tidak Langsung: "; // Memperbaiki penulisan string
    functionA(num);
    return 0; // Memperbaiki penulisan 'return 0'
}
```

**Penjelasan:**

#### Bagian 1

```C++
#include<iostream>
using namespace std;
```
- #include<iostream>: Mengimpor library standar input-output di C++ yang digunakan untuk operasi input dan output.
- using namespace std;: Memungkinkan kita menggunakan elemen-elemen dalam namespace std (standard) tanpa perlu menuliskan std:: sebelum setiap fungsi atau objek yang berasal dari library standar.

#### Bagian 2

```C++
   void functionB(int n); // Deklarasi fungsi functionB

   void functionA(int n) {
       if (n > 0) {
           cout << n << " ";
           functionB(n - 1); // Panggilan rekursif tidak langsung
       }
   }
   void functionB(int n) {
       if (n > 0) {
           cout << n << " ";
           functionA(n / 2); // Panggilan rekursif tidak langsung
       }
   }
```
- Fungsi functionB dideklarasikan sebelum functionA untuk memastikan bahwa ketika functionA memanggil functionB, kompiler sudah mengetahui tentang keberadaan functionB.
- Fungsi ini mencetak nilai n dan kemudian memanggil functionB dengan nilai n - 1. Ini terus terjadi secara rekursif selama n lebih besar dari 0.
- Mirip dengan functionA, fungsi ini mencetak nilai n dan memanggil functionA dengan nilai n / 2. Proses ini berlanjut secara rekursif selama n lebih besar dari 0.

#### Bagian 3

```C++
   int main() {
       int num = 5;
       cout << "Rekursif Tidak Langsung: ";
       functionA(num);
       return 0;
   }
```

Fungsi main atau fungsi utama ini merupakan fungsi yang pertama kali akan dieksekusi dalam program. Pada main terdapat berbagai fungsi yang telah dibuat sebelumnya sehingga pada main hanya tinggal mengatur saja posisi fungsi yang telah di buat.

- Variabel num diinisiasi dengan 5.
- Program mencetak string "Rekursif Tidak Langsung: " sebagai pengantar output dari fungsi rekursif.
- functionA dipanggil dengan nilai awal num (5), memulai proses rekursi.
- return 0; menandakan bahwa program berakhir dengan sukses.

#### Full Code Screenshot

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/CodeGuid2.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/OUTGUIDED2.png" alt="Alt Text">
</p>

#### Penjelasan

Output dari program diatas mengilustrasikan bagaimana dua fungsi dapat saling memanggil satu sama lain dalam pola rekursi tidak langsung, mencetak serangkaian nilai berdasarkan pemanggilan rekursif tersebut. Menampilkan output rekursif tidak langsung dengan nilai 5 4 2 1.

### 3. Guided 3

```C++
#include <iostream>
#include <string>
#include <vector>
using namespace std;

const int TABLE_SIZE = 11; // Ukuran tabel hash

// Kelas untuk menyimpan node hash
class HashNode {
public:
    string name; // Nama kunci
    string phone_number; // Nomor telepon sebagai nilai

    // Konstruktor untuk inisialisasi nama dan nomor telepon
    HashNode(string name, string phone_number) {
        this->name = name;
        this->phone_number = phone_number;
    }
};

// Kelas untuk struktur data hash map
class HashMap {
private:
    vector<HashNode*> table[TABLE_SIZE]; // Array dari vektor untuk tabel hash

public:
    // Fungsi hash untuk menghitung nilai hash dari kunci
    int hashFunc(string key) {
        int hash_val = 0;
        for (char c : key) {
            hash_val += c; // Menambahkan nilai ASCII dari setiap karakter
        }
        return hash_val % TABLE_SIZE; // Menggunakan modulo untuk mendapatkan indeks
    }

    // Fungsi untuk memasukkan pasangan kunci-nilai ke dalam hash map
    void insert(string name, string phone_number) {
        int hash_val = hashFunc(name); // Menghitung hash dari nama
        for (auto node : table[hash_val]) {
            if (node->name == name) {
                node->phone_number = phone_number; // Update nomor telepon jika nama sudah ada
                return;
            }
        }
        table[hash_val].push_back(new HashNode(name, phone_number)); // Menambahkan node baru jika nama belum ada
    }

    // Fungsi untuk menghapus node berdasarkan nama
    void remove(string name) {
        int hash_val = hashFunc(name); // Menghitung hash dari nama
        for (auto it = table[hash_val].begin(); it != table[hash_val].end(); it++) {
            if ((*it)->name == name) {
                table[hash_val].erase(it); // Menghapus node
                return;
            }
        }
    }

    // Fungsi untuk mencari nomor telepon berdasarkan nama
    string searchByName(string name) {
        int hash_val = hashFunc(name); // Menghitung hash dari nama
        for (auto node : table[hash_val]) {
            if (node->name == name) {
                return node->phone_number; // Mengembalikan nomor telepon jika ditemukan
            }
        }
        return ""; // Mengembalikan string kosong jika tidak ditemukan
    }

    // Fungsi untuk mencetak semua isi hash table
    void print() {
        for (int i = 0; i < TABLE_SIZE; i++) {
            cout << i << ": ";
            for (auto pair : table[i]) {
                if (pair != nullptr) {
                    cout << "[" << pair->name << ", " << pair->phone_number << "]"; // Mencetak nama dan nomor telepon
                }
            }
            cout << endl;
        }
    }
};

// Fungsi utama
int main() {
    HashMap employee_map;
    employee_map.insert("Mistah", "1234"); // Memasukkan data
    employee_map.insert("Pastah", "5678");
    employee_map.insert("Ghana", "91011");

    // Mencetak nomor telepon berdasarkan nama
    cout << "Nomer Hp Mistah : " << employee_map.searchByName("Mistah") << endl;
    cout << "Phone Hp Pastah : " << employee_map.searchByName("Pastah") << endl;
    cout << "Phone Hp Ghana : " << employee_map.searchByName("Ghana") << endl;

    employee_map.remove("Mistah"); // Menghapus data
    cout << "Nomer Hp Mistah setelah dihapus : " << employee_map.searchByName("Mistah") << endl << endl;

    cout << "Hash Table : " << endl;
    employee_map.print(); // Mencetak seluruh hash table

    return 0;
}
```

**Penjelasan:**

#### Bagian 1

```C++
#include <iostream>
#include <string>
#include <vector>
using namespace std;
```
- #include<iostream>: Mengimpor library standar input-output di C++ yang digunakan untuk operasi input dan output.
- #include<string>: digunakan untuk mengedit serta memanipulasi string di dalam kode.
- #include<vector>: dapat digunakan untuk memberikan arah dalam kode sebagai vektor.
- using namespace std;: Memungkinkan kita menggunakan elemen-elemen dalam namespace std (standard) tanpa perlu menuliskan std:: sebelum setiap fungsi atau objek yang berasal dari library standar.

#### Bagian 2

```C++
const int TABLE_SIZE = 11; // Ukuran tabel hash
class HashNode {
public:
    string name; // Nama kunci
    string phone_number; // Nomor telepon sebagai nilai

    HashNode(string name, string phone_number) {
        this->name = name;
        this->phone_number = phone_number;
    }
};
```
- Mendefinisikan ukuran tabel hash yang akan digunakan dalam hash map. Deklarasi konstanta TABLE_SIZE = 11.
- Kelas ini menyimpan data dalam bentuk pasangan kunci (name) dan nilai (phone_number).
- Konstruktor menginisialisasi objek dengan nama dan nomor telepon yang diberikan.

#### Bagian 3

```C++
class HashMap {
private:
    vector<HashNode*> table[TABLE_SIZE]; // Array dari vektor untuk tabel hash
  int hashFunc(string key) {
      int hash_val = 0;
      for (char c : key) {
          hash_val += c;
      }
      return hash_val % TABLE_SIZE;
  }
```

Menghitung nilai hash dari kunci yang diberikan dengan menjumlahkan nilai ASCII dari setiap karakter, kemudian di modulo dengan TABLE_SIZE

#### Bagian 4

```C++
  void insert(string name, string phone_number) {
      int hash_val = hashFunc(name);
      for (auto node : table[hash_val]) {
          if (node->name == name) {
              node->phone_number = phone_number;
              return;
          }
      }
      table[hash_val].push_back(new HashNode(name, phone_number));
  }
```

Menambahkan pasangan kunci-nilai ke dalam hash map. Jika kunci sudah ada, nilai akan diperbarui.

#### Bagian 5

```C++
  void remove(string name) {
      int hash_val = hashFunc(name);
      for (auto it = table[hash_val].begin(); it != table[hash_val].end(); it++) {
          if ((*it)->name == name) {
              table[hash_val].erase(it);
              return;
          }
      }
  }
```

Menghapus node berdasarkan namanya.

#### Bagian 6

```C++
  string searchByName(string name) {
      int hash_val = hashFunc(name);
      for (auto node : table[hash_val]) {
          if (node->name == name) {
              return node->phone_number;
          }
      }
      return "";
  }
```

Mencari nomor telepon berdasarkan nama. Mengembalikan nomor telepon jika ditemukan, atau string kosong jika tidak.

#### Bagian 7

```C++
  void print() {
      for (int i = 0; i < TABLE_SIZE; i++) {
          cout << i << ": ";
          for (auto pair : table[i]) {
              if (pair != nullptr) {
                  cout << "[" << pair->name << ", " << pair->phone_number << "]";
              }
          }
          cout << endl;
      }
  }
```

Digunakan untuk memunculkan (mengeprint) hasil dari hash table.

#### Bagian 8

```C++
int main() {
    HashMap employee_map;
    employee_map.insert("Mistah", "1234");
    employee_map.insert("Pastah", "5678");
    employee_map.insert("Ghana", "91011");

    cout << "Nomer Hp Mistah : " << employee_map.searchByName("Mistah") << endl;
    employee_map.remove("Mistah");
    cout << "Nomer Hp Mistah setelah dihapus : " << employee_map.searchByName("Mistah") << endl;

    employee_map.print();
    return 0;
}
```

Fungsi main atau fungsi utama ini merupakan fungsi yang pertama kali akan dieksekusi dalam program. Pada main terdapat berbagai fungsi yang telah dibuat sebelumnya sehingga pada main hanya tinggal mengatur saja posisi fungsi yang telah di buat. Membuat objek HashMap, memasukkan beberapa data, mencetak, menghapus, dan mencetak ulang untuk menunjukkan fungsi dari hash map.

#### Full Code Screenshot

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/CodeGuid3.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/OUTGUIDED3.png" alt="Alt Text">
</p>

#### Penjelasan

Output dari program diatas pertamanya memasukkan nomor Mistah, Pastah, dan Ghana. Berikutnya nomor di cetak --> Menghapus nomor Mistah --> Mencetak nomor Mistah setelah di hapus --> Mencetak seluruh isi Hash Table.

## Unguided

### 1. Unguided 1

####  Buatlah sebuah program Rekursif Langsung (Direct Recursion) yang menghitung nilai faktorial dari sebuah inputan bilangan bulat positif.

**Kode Program:**

```C++
#include <iostream>

// Fungsi untuk menghitung faktorial menggunakan rekursi langsung
long long faktorial(int n) {
    if 
        (n == 0 || n== 1) 
        return 1;
    else // basis rekursi
        return n * faktorial(n - 1); // rekursi
}

int main() {
    int angka;
    std::cout << "Masukkan bilangan bulat positif: ";
    std::cin >> angka;

    // Memastikan bahwa angka adalah positif
    if (angka < 0) {
        std::cout << "Faktorial tidak didefinisikan untuk bilangan negatif." << std::endl;
    } else {
        long long hasil = faktorial(angka);
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
   long long faktorial(int n) {
       if (n == 0 || n == 1) 
           return 1;
       else
           return n * faktorial(n - 1);
   }
```

- Fungsi faktorial menerima satu parameter n (bilangan bulat).
- Fungsi ini menggunakan rekursi untuk menghitung faktorial.
- Basis rekursinya adalah jika n sama dengan 0 atau 1, maka faktorialnya adalah 1.
- Jika tidak, fungsi akan memanggil dirinya sendiri dengan argumen n - 1 dan mengalikan hasilnya dengan n.
  
#### Bagian 3

```C++
   int main() {
       int angka;
       std::cout << "Masukkan bilangan bulat positif: ";
       std::cin >> angka;

       if (angka < 0) {
           std::cout << "Faktorial tidak didefinisikan untuk bilangan negatif." << std::endl;
       } else {
           long long hasil = faktorial(angka);
           std::cout << "Hasil Faktorial dari " << angka << " adalah: " << hasil << std::endl;
       }

       return 0;
   }
```

Fungsi di atas merupakan fungsi main yang berupa fungsi utama di dalam program yang disebut dengan fungsi main. Fungsi main yang pertama di eksekusi dan memengaruhi tampilan output.

- Pengguna diminta untuk memasukkan bilangan bulat positif.
- Jika bilangan yang dimasukkan negatif, program akan memberikan pesan bahwa faktorial tidak didefinisikan untuk bilangan negatif.
- Jika bilangan positif, fungsi faktorial dipanggil dengan bilangan tersebut sebagai argumen, dan hasilnya ditampilkan.
- Fungsi main mengembalikan 0, menandakan bahwa program berakhir tanpa error.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/CodeUn1.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/Praktikum-Struktur-Data-Assigment-Modul-9/blob/main/Modul%209/output/OutUn1.png" alt="Alt Text">
</p>

#### Penjelasan

Output kode di atas sudah di atur juga dalam fungsi main dimana alurnya sebagai berikut: Pengguna diminta memasukkan bilangan bulat positif --> Jika pengguna memasukkan bilangan negatif maka akan keluar pesan tidak dapat didefinisikan --> Jika bilangan yang dimasukkan benar maka akan di eksekusi kodenya --> Hasil di print sebagai output. Jika memasukkan angka 7 maka faktorialnya adalah 5040.

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

[1]	S. Setiawan, R. Manurung, and A. Azurat, “Struktur Data dan Algoritma Dasar-dasar Rekursif Devide and Conquer Mengulang : Maximum Contiguous subsequence,” 2010.

[2]	R. Munir, “Rekursi dan Relasi Rekurens Rekursi,” Rekursi dan Relasi Rekurens, pp. 1–27, 2020.

[3]	I. P. S. I Gede Wira Kusuma Jaya, Ida Bagus Nyoman Wijana Manuaba, Kadek Ryan Wijaya and I. G. A. G. Pratama Wardhana, I Made Andika Saputra, “Jurnal Ilmu Komputer Indonesia ( JIK ) Vol : 5 , No . 2, November 2020 Jurnal Ilmu Komputer Indonesia ( JIK ) Vol : 5 , No . 2 , November 2020 ISSN ( Print ): 2615-2703 , ISSN ( Online ): 2615-2711,” no. 2, pp. 1–13, 2020.

[4]	G. M. Sridevi, M. V. Ramakrishna, and D. V. Ashoka, “Comprehensive Performance Study of Hashing Functions,” Comput. Sci. J. Mold., vol. 31, no. 2, pp. 183–199, 2023, doi: 10.56415/csjm.v31.10.

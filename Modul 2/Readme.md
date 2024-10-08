# <h1 align="center">Laporan Praktikum Pengolahan Data Movie Classification</h1>

<p align="center">Rizal Wahyu Pratama</p>
<p align="center">2311110029</p>
<p align="center">S1SD-04-02</p>

## Dasar Teori

### Pengolahan Data dengan Python

Pengolahan data dengan Python merupakan salah satu keterampilan yang sangat berharga di era informasi saat ini. Dengan semakin banyaknya data yang tersedia, kemampuan untuk mengolah dan menganalisis data menjadi krusial dalam berbagai bidang, termasuk bisnis, sains, dan teknologi. Dalam konteks ini, Python muncul sebagai bahasa pemrograman yang sangat populer dan efektif untuk pengolahan data. Berikut adalah beberapa konsep dan teknik penting dalam pengolahan data dengan Python.

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Ilustrasi%20Gambar.jpeg" alt="Alt Text">
</p> 
<p align="center">
 Gambar 1. Ilustrasi Pengolahan Data dengan Python
</p> 

### Menggunakan Pandas : Struktur Data yang Baik

Pandas adalah salah satu pustaka Python yang paling banyak digunakan untuk analisis data. Pustaka ini menyediakan dua struktur data utama: Series dan DataFrame [1]. Series adalah struktur satu dimensi yang mirip dengan array atau daftar, sementara DataFrame adalah struktur dua dimensi yang mirip dengan tabel atau spreadsheet [2]. DataFrame memungkinkan pengguna untuk menyimpan data dalam format yang lebih terorganisir, memudahkan pengolahan data.

Contoh penggunaan Pandas untuk membaca data dari file CSV:

```
import pandas as pd

# Membaca file CSV
data = pd.read_csv('data.csv')
```

### Pembersihan Data

Salah satu langkah awal yang penting dalam pengolahan data adalah pembersihan data. Data yang tidak bersih dapat menyebabkan hasil analisis yang salah. Dalam Pandas, ada beberapa fungsi untuk membantu pembersihan data, seperti:

dropna(): Menghapus baris atau kolom yang memiliki nilai hilang.
fillna(): Mengganti nilai hilang dengan nilai tertentu, seperti rata-rata kolom.
duplicated(): Menemukan dan menghapus duplikat dalam dataset.

```
# Menghapus baris dengan nilai hilang
data_cleaned = data.dropna()

# Mengganti nilai hilang dengan rata-rata kolom
data['kolom'] = data['kolom'].fillna(data['kolom'].mean())
```

### Eksplorasi Data

Setelah data dibersihkan, langkah selanjutnya adalah eksplorasi data. Ini mencakup analisis deskriptif untuk mendapatkan pemahaman yang lebih baik tentang dataset. Fungsi seperti describe(), info(), dan visualisasi data menggunakan pustaka seperti Matplotlib dan Seaborn sangat membantu dalam fase ini.

```
# Melihat ringkasan statistik
print(data.describe())

# Menghitung frekuensi nilai
print(data['kolom'].value_counts())
```

### Visualisasi Data

Visualisasi merupakan alat yang kuat untuk memahami data. Dengan menggunakan pustaka seperti Matplotlib dan Seaborn, kita dapat membuat grafik dan diagram yang membantu dalam mengidentifikasi pola, tren, dan outlier dalam data.

Contoh sederhana visualisasi menggunakan Matplotlib:
```
import matplotlib.pyplot as plt

# Membuat histogram
plt.hist(data['kolom'], bins=10)
plt.title('Histogram Kolom')
plt.xlabel('Nilai')
plt.ylabel('Frekuensi')
plt.show()
```

#### Transformasi Data

Transformasi data melibatkan perubahan format atau struktur data untuk analisis lebih lanjut. Ini bisa mencakup normalisasi, pengkodean kategori, dan agregasi. Pustaka Pandas menyediakan banyak fungsi untuk transformasi data, seperti groupby(), pivot_table(), dan apply().

Contoh agregasi dengan groupby():
```
# Menghitung rata-rata berdasarkan kategori
rata_rata = data.groupby('kategori')['kolom'].mean()
print(rata_rata)
```

#### Analisis Data

Setelah melakukan eksplorasi dan transformasi, langkah berikutnya adalah analisis data. Ini bisa mencakup analisis statistik, regresi, klasifikasi, atau teknik pembelajaran mesin. Pustaka seperti Scikit-learn dan Statsmodels sangat membantu dalam melakukan analisis ini [3].

Contoh sederhana regresi linier menggunakan Scikit-learn:
```
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression

X = data[['fitur1', 'fitur2']]
y = data['target']

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)

model = LinearRegression()
model.fit(X_train, y_train)

predictions = model.predict(X_test)
```
#### Penyimpanan dan Eksplorasi Data

Setelah proses analisis selesai, Anda mungkin ingin menyimpan hasilnya. Pandas memudahkan untuk menyimpan data ke dalam berbagai format, seperti CSV, Excel, atau SQL.

```
data_cleaned.to_csv('data_cleaned.csv', index=False)
```

Pengolahan data dengan Python melibatkan berbagai langkah, mulai dari pembacaan data, pembersihan, eksplorasi, visualisasi, hingga analisis dan penyimpanan. Dengan menggunakan pustaka seperti Pandas, Matplotlib, Seaborn, dan Scikit-learn, pengguna dapat melakukan berbagai jenis analisis data secara efisien[4]. Keahlian dalam pengolahan data akan memberikan wawasan berharga yang dapat digunakan untuk pengambilan keputusan yang lebih baik di berbagai bidang[5].

## Unguided

**Data yang digunakan**
[Data Movie Classification](https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Movie_classification.csv)

### Soal 1

####   Load data (movie classification)

**Kode Program:**

```
# 1. Load data Movie_classification
import pandas as pd

df = pd.read_csv("Movie_classification.csv")
df.info()
```

**Penjelasan:**

**import pandas as pd** merupakan salah satu Library dari Python yang dapat digunakan untuk membaca data, analisis data, maupun membuat dataframe. Dalam pembacaan maupun penyimpanan data dapat digunakan dalam format CSV (Comma Separated Values), Excel, SQL, dan lain-lain. Dalam hal ini, alias pd digunakan agar kita bisa mengakses fungsionalitas Pandas dengan menuliskan pd.

**df = pd.read_csv("Movie_classification.csv")** berguna untuk membaca file CSV bernama Movie_classification.csv dan menyimpannya ke dalam variabel df (dataframe). Dataframe adalah struktur data di Pandas yang menyerupai tabel, di mana setiap kolom memiliki nama, dan isinya bisa berupa berbagai tipe data (angka, string, dll.)

**df.info()** fungsi ini memberikan informasi singkat tentang dataframe yang baru saja dimuat. Informasi yang diberikan meliputi: Jumlah baris dan kolom dalam dataframe. Nama kolom beserta jenis data di masing-masing kolom (misalnya integer, float, string/object). Jumlah nilai non-null (nilai yang tidak kosong) di setiap kolom.

#### Full code Screenshot:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Soal1.png" alt="Alt Text">
</p>

#### Screenshot Output

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out1.png" alt="Alt Text">
</p> 
<p align="center">
 Screenshot Output Unguided 1
</p> 

#### Penjelasan

Pada output memberikan penjelasan mengenai data yang diload berupa 506 data yang tersedia dengan index mencapai 505, terdapat 19 kolom pada data. Pada output di atas juga terdapat keterangan mengenai type dari data yang tersedia. Terakhir juga terdapat keterangan memori yang digunakan oleh data.

### Soal 2

####  Cek nilai duplikat dalam data

**Kode Program:**

#### Bagian 1

```
#2. Mengecek duplikat data
df.duplicated()
```

df.duplicate() merupakan sebuah kode yang dapat digunakan untuk mengecek keberadaan data yang berduplikat.

#### Screenshot Output:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out21.png" alt="Alt Text">
</p>

#### Penjelasan

Pada output kode di atas, diketahui dari 506 baris tidak ada yang terdeteksi duplikat karena hasil pengecekan seluruhnya adalah False.

#### Bagian 2

```
# Menghapus duplikat
df_cleaned = df.drop_duplicates()

# Menyimpan DataFrame yang sudah dibersihkan ke file CSV baru
df_cleaned.to_csv("Movie_classification_cleaned.csv", index=False)

df.info()
```

Apabila terdapat data duplikat, maka dapat menggunakan kode di atas, dimana jalan kodenya sebagai berikut:

**df_cleaned = df.drop_duplicates()** pada kode di atas Fungsi drop_duplicates() digunakan untuk menghapus baris-baris duplikat dari dataframe df. Dataframe df_cleaned akan berisi data dari df yang telah dihapus baris-baris duplikatnya.
Baris duplikat berarti dua baris atau lebih yang memiliki nilai yang sama di semua kolom. Fungsi ini secara default akan menghapus semua baris yang benar-benar sama di seluruh kolom, tetapi bisa disesuaikan untuk hanya mengecek kolom tertentu jika diperlukan (menggunakan parameter subset).

**df_cleaned.to_csv("Movie_classification_cleaned.csv", index=False)** Fungsi to_csv() digunakan untuk menyimpan dataframe menjadi file CSV baru. "Movie_classification_cleaned.csv" adalah nama file tempat dataframe yang telah dibersihkan disimpan. index=False berarti indeks dataframe (yang berupa angka baris) tidak akan disimpan dalam file CSV. Jika tidak dinyatakan, indeks dataframe akan ikut disimpan.

**df.info()** akan menampilkan informasi tentang dataframe df (yang masih asli, belum dihapus duplikatnya). Informasi yang ditampilkan meliputi jumlah baris dan kolom, nama kolom, tipe data di setiap kolom, serta jumlah nilai non-null di setiap kolom. Ini memungkinkan kamu untuk membandingkan data sebelum dan sesudah penghapusan duplikat.

#### Screenshot Output:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out22.png" alt="Alt Text">
</p>

#### Penjelasan

Pada output memberikan penjelasan mengenai data yang diload berupa 506 data yang tersedia dengan index mencapai 505, terdapat 19 kolom pada data. Pada output di atas juga terdapat keterangan mengenai type dari data yang tersedia. Terakhir juga terdapat keterangan memori yang digunakan oleh data.

### Soal 3

####  Menemukan null values buat presentase: 

**Kode Program:**

#### Bagian 1

```
#3 Melihat jumlah yang NA
df.isna().sum()
```

Fungsi di atas digunakan untuk melihat jumlah missing value (NA) dalam setiap kolomnya.

#### Screenshot Output:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out31.png" alt="Alt Text">
</p>

#### Bagian 2

```
# 3. Menemukan null values dan ubah ke persentase

(df.isna().sum()/len(df))*100 #Persentase NA
```

Kode di atas digunakan untuk melihat missing value (NA) dalam data dalam bentuk persentase karena pada kode ditambahkan kode untuk menghitung dalam persen yaitu _.sum()/len(df))*100_.

#### Screenshot Output:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out32.png" alt="Alt Text">
</p>

### Soal 4

####  Drop missing value berdasarkan baris, kolom, imputasi dengan mean, modus, median

**Kode Program:**

#### Bagian 1

```
# 4. Menghapus data yang NA berdasarkan Baris
Mvdrop = df.dropna(inplace=False)

#Menghapus NA pada kolom
df_dropped_columns = df.dropna(axis=1)

Mvdrop.isna().sum()
```

**Mvdrop = df.dropna(inplace=False)** dropna() digunakan untuk menghapus baris yang mengandung nilai NA atau missing values. Dalam konteks ini, inplace=False berarti dataframe asli df tidak akan dimodifikasi secara langsung. Sebaliknya, dataframe baru bernama Mvdrop akan dibuat yang tidak mengandung baris dengan nilai NA. Baris yang mengandung setidaknya satu nilai NA akan dihapus.

**df_dropped_columns = df.dropna(axis=1)** dropna(axis=1) digunakan untuk menghapus kolom yang memiliki NA. axis=1 berarti operasi penghapusan dilakukan pada kolom (bukan baris). Jadi, setiap kolom yang memiliki setidaknya satu nilai NA akan dihapus. Dataframe baru bernama df_dropped_columns akan menyimpan hasilnya.

**Mvdrop.isna().sum()** isna() digunakan untuk mengecek nilai NA dalam dataframe Mvdrop. Fungsi ini akan menghasilkan dataframe baru dengan nilai True untuk setiap elemen yang merupakan NA dan False untuk yang bukan. sum() digunakan untuk menghitung jumlah nilai NA di setiap kolom dari dataframe Mvdrop. Dengan cara ini, kamu bisa melihat jumlah nilai NA per kolom di dataframe Mvdrop setelah penghapusan baris dengan NA.

#### Screenshot Output:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out41.png" alt="Alt Text">
</p>

Berdasarkan output di atas dapat diketahui bahwa seluruh NA sudah di hapus sehingga nilai NA dari setiap kolom sudah 0.

#### Bagian 2

```
# Hanya untuk kolom numerik
df_imputed_mean = df.fillna(df.select_dtypes(include='number').mean())
print("\nDataFrame setelah imputasi dengan mean:")
df_imputed_mean
```

**df_imputed_mean = df.fillna(df.select_dtypes(include='number').mean())**

- df.select_dtypes(include='number'): Fungsi select_dtypes() digunakan untuk memilih kolom berdasarkan tipe data. Dengan parameter include='number', kamu memilih hanya kolom yang bertipe numerik (seperti int64 dan float64).

- df.select_dtypes(include='number').mean(): Setelah memilih kolom numerik, fungsi mean() menghitung nilai rata-rata untuk setiap kolom numerik di dataframe.

- df.fillna(): Fungsi ini digunakan untuk mengisi nilai yang hilang (NA). Dalam hal ini, nilai NA di kolom numerik akan diganti dengan nilai rata-rata dari kolom tersebut.

- df_imputed_mean: Hasil dari proses ini disimpan dalam variabel baru df_imputed_mean, yang berisi dataframe dengan nilai NA pada kolom numerik yang telah diisi dengan rata-rata.

**print("\nDataFrame setelah imputasi dengan mean:")** kode ini perintah untuk menampilkan pesan teks ke layar, yang menunjukkan bahwa dataframe yang akan dicetak adalah setelah proses imputasi (pengisian missing values) dengan nilai rata-rata.

**df_imputed_mean** dengan memanggil variabel ini, Python akan mencetak isi dari dataframe yang telah mengalami proses imputasi missing values menggunakan nilai rata-rata dari kolom numerik.

#### Screenshot Output:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out42.png" alt="Alt Text">
</p>

Dari output di atas, dapat dilihat hasil imputasi mean pada setiap NA yang ada dalam data.

#### Bagian 3

```
df_imputed_median = df.fillna(df.select_dtypes(include='number').median())
print("\nDataFrame setelah imputasi dengan median:")
df_imputed_median
```

**df_imputed_median = df.fillna(df.select_dtypes(include='number').median())**

- df.select_dtypes(include='number'): Ini memilih hanya kolom-kolom yang bertipe numerik di dataframe df (seperti kolom bertipe int64 dan float64).

- df.select_dtypes(include='number').median(): Setelah memilih kolom-kolom numerik, fungsi median() akan menghitung nilai median dari setiap kolom. Median adalah nilai tengah dari data yang diurutkan, yang sering digunakan sebagai ukuran sentralitas yang lebih stabil terhadap pencilan (outliers) dibandingkan rata-rata.

- df.fillna(): Fungsi ini digunakan untuk mengisi nilai yang hilang (NA) pada kolom-kolom yang memiliki missing values. Dalam hal ini, nilai NA di kolom numerik akan diisi dengan nilai median dari masing-masing kolom.

- df_imputed_median: Hasil dari proses ini disimpan ke dalam dataframe baru df_imputed_median, yang sekarang berisi data di mana semua NA di kolom numerik telah diisi dengan nilai median.

**print("\nDataFrame setelah imputasi dengan median:")** menampilkan pesan teks yang memberi tahu bahwa hasil yang akan dicetak adalah dataframe yang sudah diisi dengan nilai median.

**df_imputed_median** dengan memanggil variabel ini, Python akan menampilkan dataframe df_imputed_median yang berisi data asli di mana nilai NA pada kolom numerik telah diimputasi menggunakan median.

#### Screenshot Output:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out43.png" alt="Alt Text">
</p>

Dari output di atas, dapat dilihat hasil imputasi median pada setiap NA yang ada dalam data.

#### Bagian 4

```
# Untuk kolom non-numerik
df_imputed_mode = df.fillna(df.mode().iloc[0])
print("\nDataFrame setelah imputasi dengan modus:")
df_imputed_mode
```

**df_imputed_mode = df.fillna(df.mode().iloc[0])**

- df.mode(): Fungsi mode() digunakan untuk menghitung modus dari setiap kolom. Modus adalah nilai yang paling sering muncul dalam suatu kolom. Fungsi ini dapat digunakan baik pada kolom numerik maupun non-numerik.

- iloc[0]: Karena mode() dapat menghasilkan lebih dari satu nilai jika ada lebih dari satu modus (nilai yang sama frekuensinya), iloc[0] memastikan kita mengambil modus pertama (baris pertama hasil mode()) jika ada lebih dari satu nilai yang memenuhi kriteria modus.

- df.fillna(): Fungsi ini digunakan untuk mengisi nilai yang hilang (NA) dalam dataframe. Pada baris ini, nilai NA dalam dataframe df akan diisi dengan nilai modus dari masing-masing kolom, baik itu kolom numerik maupun non-numerik.

- df_imputed_mode: Hasil dari proses ini disimpan dalam dataframe df_imputed_mode, yang berisi data di mana nilai NA pada kolom sudah diganti dengan nilai modus.

**print("\nDataFrame setelah imputasi dengan modus:")** perintah untuk menampilkan pesan teks yang memberi tahu bahwa hasil yang akan dicetak adalah dataframe setelah dilakukan imputasi dengan modus.

**df_imputed_mode** dengan memanggil variabel ini, Python akan mencetak dataframe df_imputed_mode, yang berisi data setelah proses imputasi dilakukan. Nilai NA pada kolom numerik dan non-numerik diisi dengan nilai modus dari kolom yang sesuai.

#### Screenshot Output:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out44.png" alt="Alt Text">
</p>

Dari output di atas, dapat dilihat hasil imputasi modus pada setiap NA yang ada dalam data.

### Soal 5

####  Export data ke csv dan excel

**Kode Program:**

#### Bagian 1

```
# 5. Simpan data sebagai excel
Mv = df.to_excel('Movie_classification.xlsx',index = False)
```

- df.to_excel(): Fungsi ini digunakan untuk menyimpan data dari dataframe df ke dalam file Excel dengan ekstensi .xlsx. Dalam hal ini, nama file yang diberikan adalah Movie_classification.xlsx.

- Movie_classification.xlsx merupakan nama file yang akan dibuat dan tempat data dari dataframe disimpan. File ini akan berformat Excel (berekstensi .xlsx).

- index=False: Parameter index=False digunakan untuk mencegah penulisan indeks (nomor baris) ke dalam file Excel. Jika tidak disertakan, indeks dataframe akan ikut tersimpan sebagai kolom tambahan.

#### Bagian 2

```
Mv = pd.read_excel('Movie_classification.xlsx')
Mv.head()
```
**Mv = pd.read_excel('Movie_classification.xlsx')**

- pd.read_excel(): Fungsi ini digunakan untuk membaca file Excel (.xlsx) dan mengubahnya kembali menjadi dataframe Pandas. Dalam hal ini, file Excel yang dibaca adalah Movie_classification.xlsx.

- Movie_classification.xlsx: Ini adalah nama file Excel yang berisi data yang sebelumnya disimpan dan sekarang akan dibaca kembali ke dalam dataframe Mv.

**Mv.head()**

- head(): Fungsi ini digunakan untuk menampilkan lima baris pertama dari dataframe Mv. Ini berguna untuk memeriksa isi dataframe dan melihat sebagian kecil dari data yang ada tanpa mencetak seluruh dataframe, terutama jika dataframe sangat besar.

- Kamu bisa juga menyesuaikan jumlah baris yang ditampilkan dengan menambahkan argumen, seperti Mv.head(10) untuk menampilkan 10 baris pertama.

#### Screenshot Output:

<p align="center">
  <img src="https://github.com/rizaledc/IPSD-Assigment/blob/main/Modul%202/Assets/Out5.png" alt="Alt Text">
</p>

#### Bagian 3

```
# Simpan sebagai file CSV
df.to_csv('Movie_classification.csv', index=False)  # index=False untuk menghindari penulisan index ke file CSV
```

**df.to_csv('Movie_classification.csv', index=False)**

- df.to_csv(): Fungsi ini digunakan untuk menyimpan dataframe df ke dalam file CSV (Comma Separated Values), yang merupakan format data berbasis teks di mana setiap nilai dipisahkan oleh koma.

- Movie_classification.csv: Ini adalah nama file tempat dataframe akan disimpan. File tersebut akan memiliki ekstensi .csv dan berisi data dari dataframe.

- index=False: Parameter ini digunakan untuk mengabaikan penyimpanan indeks dataframe (nomor baris) ke dalam file CSV. Jika parameter ini tidak digunakan, indeks akan ikut tersimpan sebagai kolom tambahan dalam file CSV.

## Kesimpulan

Pengolahan data dengan Python merupakan keterampilan penting di era informasi, karena data saat ini menjadi aset berharga di berbagai sektor. Pandas, sebagai salah satu pustaka utama dalam ekosistem Python, memainkan peran vital dalam analisis data. Dengan dua struktur utama, Series dan DataFrame, Pandas memungkinkan pengguna mengelola data dalam format yang terstruktur, sehingga memudahkan berbagai proses pengolahan data. Langkah-langkah utama dalam pengolahan data meliputi pembersihan data, eksplorasi, transformasi, dan analisis data.

Pembersihan data merupakan langkah awal yang sangat penting. Data yang tidak bersih dapat menghasilkan analisis yang salah. Fungsi seperti dropna() dan fillna() dalam Pandas memungkinkan pengguna untuk menangani data yang hilang secara efisien, sementara duplicated() dapat mendeteksi dan menghapus data duplikat. Setelah data dibersihkan, eksplorasi dilakukan untuk mendapatkan wawasan awal. Fungsi seperti describe() dan info() digunakan untuk menganalisis data deskriptif, sementara visualisasi dengan pustaka Matplotlib dan Seaborn membantu mengidentifikasi pola dalam data.

Transformasi data juga merupakan proses penting untuk mempersiapkan data agar siap dianalisis lebih lanjut. Proses seperti normalisasi, pengkodean kategori, dan agregasi dapat dilakukan dengan menggunakan Pandas, sehingga data dapat diolah dalam format yang lebih tepat untuk analisis statistik atau pembelajaran mesin. Pada akhirnya, pustaka seperti Scikit-learn menyediakan berbagai alat untuk melakukan regresi, klasifikasi, dan analisis lanjutan. Semua langkah ini memungkinkan pengguna untuk tidak hanya menganalisis data tetapi juga menyimpan hasilnya ke dalam berbagai format untuk digunakan lebih lanjut.

Dengan kombinasi pustaka Python yang kuat seperti Pandas, Matplotlib, Seaborn, dan Scikit-learn, pengolahan data dapat dilakukan secara efisien dan efektif, memberikan wawasan yang sangat berharga untuk pengambilan keputusan dalam bisnis, teknologi, dan sains.

## Referensi

[1] M. Lutz, Python Crash Course, 2nd Edition: A Hands-On, Project-Based Introduction to Programming, 2nd ed. No Starch Press, 2019.

[2] J. VanderPlas, Python Data Science Handbook: Essential Tools for Working with Data, O'Reilly Media, 2019. 

[3] S. Raschka, and V. Mirjalili, Python Machine Learning, 3rd ed., Packt Publishing, 2019.

[4] T. Alguliyev, R. Aliguliyev, and L. Imamverdiyev, "Big Data: Big Promises for Information Security," IEEE Transactions on Knowledge and Data Engineering, vol. 32, no. 8, pp. 1361-1378, Aug. 2020.

[5] A. Bertsimas, M. Lundberg, and D. Nohadani, "Data-Driven Analytics in the Era of Big Data," Operations Research, vol. 68, no. 2, pp. 465-488, Mar. 2020.

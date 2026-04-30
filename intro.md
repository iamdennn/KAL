# SISTEM PERSAMAAN LINIER

Tentu, ini adalah teks lengkap dari gambar-gambar yang Anda berikan, sudah saya format ke dalam **Markdown** agar rapi dan mudah Anda *copy-paste* ke VS Code (misalnya untuk file `.md` atau konten Jupyter Book Anda).

---

# 1.1 Sistem Persamaan Linear

## 1.1.1. Definisi Sistem Persamaan Linear

Suatu sistem persamaan linear (*system of linear equations* atau *linear system*) adalah suatu himpunan persamaan-persamaan linear. Sistem linear homogen adalah himpunan persamaan linear yang semuanya berbentuk homogen (ruas kanannya nol).

Jika kita menuliskan suatu sistem yang terdiri atas $m$ persamaan dalam $n$ peubah $x_1, x_2, \dots, x_n$, biasanya setiap persamaan ditulis dalam bentuk standar dan suku-suku yang bersesuaian disejajarkan dalam kolom sebagai berikut:

$$
\begin{aligned}
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n &= b_1 \\
a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n &= b_2 \\
\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n &= b_m
\end{aligned}
$$

Sistem linear homogen biasanya dituliskan sebagai:

$$
\begin{aligned}
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n &= 0 \\
a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n &= 0 \\
\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n &= 0
\end{aligned}
$$

## 1.1.2 Tujuan Dari Operasi Persamaan Linear

Operasi persamaan linear bertujuan untuk menemukan solusi dengan cara menyederhanakan persamaan tanpa mengubah nilai kebenarannya, seperti contoh di bawah ini:
Diberikan persamaan:
$2x + 4 = 10$
Tujuan kita adalah mencari $x$, langkah operasi yang bisa kita lakukan dengan menggunakan cara:

1. Kita kurangi kedua sisi dengan 4:
   $2x + 4 - 4 = 10 - 4$
   $2x = 6$
2. Kita bagi kedua sisi dengan 2:
   $x = 3$

---

## 1.1.2. Persamaan Linear dan Nonlinear

### 1. Persamaan Linear
Persamaan linear adalah persamaan yang variabelnya memiliki pangkat tertinggi **satu (derajat satu)** dan grafiknya berbentuk **garis lurus**.

**Contoh Bentuk Umum (dua bentuk)**

1. **Satu variabel**
   $[ ax + b = 0 ]$
   Keterangan:
   * 0 = konstanta
   * a, b = koefisien
   * x = variabel
   Contoh: $[ 2x + 5 = 0 ]$

2. **Dua variabel**
   $[ ax + by + c = 0 ]$
   Keterangan:
   * (a, b, c) = konstanta
   * (x, y) = variabel
   Contoh: $[ 2x + y - 4 = 0 ]$

**Ciri-ciri Persamaan Linear:**
* Pangkat variabel = 1
* Tidak ada perkalian antar variabel
* Tidak ada akar atau pangkat lebih dari satu

---

### 2. Persamaan Nonlinear
Persamaan nonlinear adalah persamaan yang memiliki variabel dengan pangkat **lebih dari satu**, berada dalam akar, atau saling dikalikan sehingga grafiknya **bukan garis lurus**.

**Bentuk Umum (dua bentuk)**

1. **Persamaan kuadrat**
   $[ ax^2 + bx + c = 0 ]$
   Keterangan:
   * Pangkat tertinggi variabel adalah 2.
   Contoh: $[ x^2 + 3x - 4 = 0 ]$

2. **Persamaan dengan perkalian variabel**
   $[ xy + x + y = 0 ]$
   Contoh: $[ xy + 2x - y = 3 ]$

**Ciri-ciri Persamaan Nonlinear:**
* Pangkat variabel lebih dari 1 atau berbentuk akar
* Bisa terdapat perkalian antar variabel ($xy$)
* Grafik berupa kurva (parabola, lingkaran, dll.)

---

## 1.1.3. Definisi Solusi Sistem Persamaan Linear

**Pengertian Solusi dalam persamaan linear** adalah nilai variabel yang membuat persamaan menjadi **benar** ketika nilai tersebut disubstitusikan ke dalam persamaan.
Dengan kata lain, solusi adalah nilai yang menyebabkan **ruas kiri = ruas kanan**.

**Penjelasan**: Pada persamaan linear, tujuan utama adalah mencari nilai variabel (misalnya $x, y, z$) yang memenuhi persamaan.
Jika suatu nilai dimasukkan ke dalam persamaan dan menghasilkan kesamaan yang benar, maka nilai tersebut disebut **solusi**.

**Jenis solusi pada persamaan linear diantaranya:**
1. **Solusi tunggal**: Hanya ada satu set nilai variabel yang memenuhi semua persamaan.
2. **Tidak ada solusi**: Tidak ada nilai variabel yang memenuhi semua persamaan (sistem inkonsisten).
3. **Solusi tak terhingga**: Ada tak terhingga banyaknya solusi (sistem dependen).

**Contoh grafis (2D) dalam solusi persamaan linear:**
* Garis berpotongan $\to$ Solusi tunggal
* Garis sejajar $\to$ Tidak ada solusi
* Garis berimpit $\to$ Solusi tak terhingga

```{code-cell} python
from IPython.display import IFrame

IFrame(
    "[https://www.geogebra.org/classic/ekkrznta?embed](https://www.geogebra.org/classic/ekkrznta?embed)",
    width=800,
    height=600
)
```
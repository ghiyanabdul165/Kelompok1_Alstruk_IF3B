Variabel a = 10

Di sini kita membuat sebuah variabel bernama a, dan kita kasih nilai 10.

Variabel itu ibarat kotak penyimpanan, dan angka 10 adalah isi di dalam kotaknya.

1. Type data Integer

data_integer = 30

Ini adalah angka bulat, alias angka yang nggak punya koma.

Contohnya: 10, 30, 100, -5

Di program, Python mengenali tipe ini sebagai int.

Ketika kita print, hasilnya menunjukkan:

Nilai: 30

Tipe datanya: <class 'int'>

2. Type data Float

data_float = 2.5

Ini adalah angka yang punya koma, misalnya 2.5, 10.75, dan sebagainya.

Python mengenal tipe ini sebagai float.

Output-nya:

Nilai: 2.5

Tipe datanya: <class 'float'>

3. Type data String

data_string = "ridho"

String adalah kumpulan karakter, bisa berupa huruf, angka, atau simbol.

Contohnya: "ridho", "123", "Hello World"

Ditandai dengan tanda kutip.

Output:

Nilai: ridho

Tipe: <class 'str'>

4. Type data Boolean

data_bool = True

Boolean cuma punya dua kemungkinan nilai: True atau False.

Tipe data ini sering dipakai untuk logika, seperti pengecekan suatu kondisi.

Output:

Nilai: True

Tipe: <class 'bool'>

5. Type data Kompleks

data_complex = complex(5,7)

Ini adalah angka kompleks yang terdiri dari bagian real dan imajiner.

complex(5,7) artinya:

real = 5

imajiner = 7

Bentuknya jadi: 5 + 7j

Tipe: <class 'complex'>

6. Type data dari bahasa C (Ctypes)

from ctypes import c_double

data_c_double = c_double(20.05)

ctypes memungkinkan kita menggunakan tipe data seperti yang ada di bahasa pemrograman C.

c_double adalah tipe data angka desimal dengan presisi tinggi.

Biasanya dipakai kalau kita perlu interaksi dengan program lain yang dibuat pakai bahasa C.

Output:

Nilai: 20.05

Tipe: <class 'ctypes.c_double'>
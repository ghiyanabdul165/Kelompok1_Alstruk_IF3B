
Kode ini membuat aplikasi kalkulator sederhana berbasis teks yang dapat melakukan operasi:
Penjumlahan
Pengurangan
Perkalian
Pembagian 
1. Fungsi Operasi Matematika
a. Fungsi tambah(a, b)
def tambah(a, b): return a + b 
Menjumlahkan dua angka dan mengembalikan hasilnya.
b. Fungsi kurang(a, b)
def kurang(a, b): return a - b 
Mengurangi angka a dengan b.
c. Fungsi kali(a, b)
def kali(a, b): return a * b 
Mengalikan dua angka.
d. Fungsi bagi(a, b)
def bagi(a, b): if b == 0: return "Error: Tidak bisa membagi dengan nol!" return a / b 
Melakukan pembagian, tetapi:
Jika b == 0, maka fungsi mengembalikan pesan error (untuk mencegah error pembagian nol). 
2. Fungsi main() – Bagian Utama Program
a. Menampilkan menu
print("=== Aplikasi Kalkulator Sederhana ===") print("1. Tambah") print("2. Kurang") print("3. Kali") print("4. Bagi") 
Program menampilkan pilihan operasi yang tersedia.
b. Input pilihan operasi
pilihan = input("Pilih operasi (1-4): ") 
User memilih operasi dengan memasukkan angka 1–4.
c. Validasi input
if pilihan not in ["1", "2", "3", "4"]: print("Pilihan tidak valid!") return 
 Jika input bukan 1–4, program berhenti dan menampilkan pesan error.
d. Input angka
angka1 = float(input("Masukkan angka pertama: ")) angka2 = float(input("Masukkan angka kedua: ")) 
 User memasukkan dua angka.
float() digunakan agar angka desimal dapat diterima.
e. Menjalankan operasi sesuai pilihan
if pilihan == "1": hasil = tambah(angka1, angka2) operasi = "+" elif pilihan == "2": hasil = kurang(angka1, angka2) operasi = "-" elif pilihan == "3": hasil = kali(angka1, angka2) operasi = "×" elif pilihan == "4": hasil = bagi(angka1, angka2) operasi = "÷" 
Program memanggil fungsi sesuai nomor yang dipilih.
operasi digunakan untuk menampilkan simbol pada output.
f. Menampilkan hasil
print(f"Hasil: {angka1} {operasi} {angka2} = {hasil}") 
Mencetak hasil lengkap operasi, contoh:
Hasil: 5 × 3 = 15
 3. Eksekusi Program
main() 
Memanggil fungsi utama untuk menjalankan aplikasi.

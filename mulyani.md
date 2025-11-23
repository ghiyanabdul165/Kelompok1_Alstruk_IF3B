Kode ini adalah program Python sederhana yang meminta dua angka dari pengguna, lalu menjumlahkannya menggunakan fungsi khusus.


1. Fungsi tambah

def tambah(angka1, angka2):
  """
  Fungsi ini menerima dua angka sebagai input dan mengembalikan jumlahnya.
  """
  hasil = angka1 + angka2
  return hasil

Penjelasan:

Fungsi ini menerima dua parameter: angka1 dan angka2.

Di dalam fungsi, kedua angka tersebut dijumlahkan dan disimpan di variabel hasil.

return hasil mengembalikan nilai hasil penjumlahan kembali ke pemanggil fungsi.

Fungsi ini membuat kode lebih rapi karena proses penjumlahan dipisahkan dari logika utama program.


2. Fungsi main

def main():
  """
  Fungsi ini adalah titik masuk utama dari program.
  """

  # Meminta input dari pengguna

  try:
    angka_pertama = float(input("Masukkan angka pertama: "))
    angka_kedua = float(input("Masukkan angka kedua: "))
  except ValueError:
    print("Input tidak valid. Masukkan angka yang benar.")
    return

Penjelasan:

Program meminta pengguna memasukkan dua input angka.

float() digunakan agar input bisa berupa bilangan desimal.

try-except digunakan untuk menangani kesalahan jika input bukan angka.

Jika pengguna salah memasukkan (misalnya huruf), program menampilkan pesan error dan berhenti.



3. Memanggil Fungsi tambah

jumlah = tambah(angka_pertama, angka_kedua)

Nilai dari angka_pertama dan angka_kedua dikirim ke fungsi tambah.

Hasil penjumlahan dikembalikan dan disimpan ke variabel jumlah.



4. Menampilkan Hasil

print("Jumlah dari", angka_pertama, "dan", angka_kedua, "adalah:", jumlah)

Program mencetak hasil penjumlahan ke layar.



5. Bagian Pemanggilan Program

if __name__ == "__main__":
  main()

Fungsinya:

Baris ini memastikan bahwa fungsi main() hanya dijalankan jika file ini dieksekusi langsung.

Tidak akan berjalan jika file di-import oleh file Python lain.
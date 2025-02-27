LatihanArray
int [] bilanganGenap = new int[10];
int jumlah = 0;
mendeklarasikan array 'bilanganGenap' dengan 10 elemen bertipe 'int' dan variabel 'jumlah' dengan nilai awal 0.
for (int i = 0; i < bilanganGenap.length; i++) {}
bilanganGenap[i] = (i + 1) * 2;
mengisi array 'bilanganGenap' dengan bilangan genap, mulai dari 2 sampai seterusnya, sesuai indeks array.
System.out.println("isi array : ");
for (int bilangan : bilanganGenap) {}
System.out.print(bilangan + " ");
jumlah += bilangan;
mencetak isi array 'bilanganGenap', terus tiap angkanya dijumlahin ke variabel 'jumlah'.
System.out.println("\nJumlah semua elemen : " + jumlah);
mencetak total dari semua elemen yang udah dijumlahin di variabel 'jumlah'.

//PencarianArray
int [] nilai = {75, 80, 85, 70, 95, 88};
int cari = 90;
boolean ketemu = false;
Kode itu menyimpen daftar nilai dalam array 'nilai', terus menyiapkan variabel 'cari' buat nyari angka 90 di array. Variabel 'ketemu' dipakai buat angka yang dicari ada atau tidak.
for (int i = 0; i < nilai.length; i++) {}
if (nilai[i] == cari) {}
ketemu = true;
indeks = i;
break;
Looping ini nyari angka 'cari', kalau ketemu langsung tandain, simpan indeksnya, terus berhenti.
if (ketemu) {}
System.out.println("Nilai " + cari + " ditemukan pada indeks " + indeks);
else {}
System.out.println("Nilai " + cari + " tidak ditemukan ");
mengecek hasil pencarian, kalau ketemu ditampilin indeksnya.

//StatistikArray
int [] nilai = {75, 80, 65, 90, 85, 70, 95, 88};
untuk menyimpan sekumpulan angka.
int tertinggi = nilai[0];
int terendah = nilai[0];
int total = nilai[0];
menginisialisasi 'tertinggi', 'terendah', dan 'total' dengan nilai pertama di array.
for (int i = 0; i < nilai.length; i++) {}
if (nilai[i] > tertinggi) {}
tertinggi = nilai[i];
if (nilai[i] < terendah) {}
terendah = nilai[i];
total += nilai[i];
mengecek tiap nilai untuk mencari yang paling tinggi, paling rendah, dan menjumlahkan semua angka ke 'total'.
double rataRata = (double) total / nilai.length;
menghitung rata-rata dengan bagi total nilai sama jumlah elemen di array, hasilnya dikonversi ke 'double' biar presisi.
System.out.println("Nilai tertinggi : " + tertinggi);
System.out.println("Nilai terendah : " + terendah);
System.out.println("Rata-Rata : " + rataRata);
menampilkan nilai tertinggi, terendah, dan rata-rata yang udah dihitung sebelumnya.

//OperasiMatriks
int [][] matriksA = {}
{1, 2, 3},
{4, 5, 6}
membuat array dua dimensi 'matriksA' dengan 2 baris dan 3 kolom, berisi angka 1 sampai 6. 
int [][] matriksB = {}
{7, 8, 9},
{10, 11, 12}
membuat array dua dimensi 'matriksB' dengan 2 baris dan 3 kolom, berisi angka 7 sampai 12.
int [][] hasil = new int[2][3];
membuat array 'hasil' dengan ukuran 2x3 buat menyimpan hasil operasi matriks.
for (int i = 0; i < matriksA.length; i++) {}
for (int j = 0; j < matriksA[0].length; j++) {}
hasil [i][j] = matriksA[i][j] + matriksB[i][j];
menjalankan operasi penjumlahan elemen di 'matriksA' dan 'matriksB', lalu menyimpan hasil.
System.out.println("Hasil penjumlahan matriks : ");
for (int[] baris : hasil) {}
for (int nilai : baris) {}
System.out.print( nilai + " ");
System.out.println();
menampilkan hasil penjumlahan matriks dengan nge-loop tiap baris dan cetak nilainya satu per satu.

//SistemNilai
String [] namaSiswa = {"Ani", "Budi", "Cici", "Dodi", "Edi"};
int [][] nilai = {};
{80, 85, 90}, // nilai Ani
{75, 70, 85}, // nilai Budi
{85, 80, 88}, // nilai Cici
{90, 85, 95}, // nilai Dodi
{70, 75, 80}  // nilai Edi
menyimpan daftar nama siswa di array 'namaSiswa' dan nilai mereka di array dua dimensi 'nilai', di mana tiap baris sesuai urutan nama siswa.
String [] mapel = {"Matematika", "Bahasa Inggris", "IPA"};
menyimpan daftar mata pelajaran dalam array 'mapel', sesuai urutan kolom di array 'nilai'.
System.out.println("Rata-rata nilai per siswa : ");
for (int i = 0; i < nilai.length; i++) {}
double total = 0;
for (int n : nilai[i]) {}
total += n;
membuat loop tiap siswa, menjumlahkan semua nilainya, buat nanti dihitung rata-ratanya.
double rataSiswa = total / nilai[i].length;
System.out.printf("%s:%.2f\n", namaSiswa[i], rataSiswa); 
menghitung rata-rata nilai tiap siswa lalu menampilkan namanya&hasilnya dengan dua angka di belakang koma.    
System.out.println("\nRata-rata nilai per mata pelajaran : ");
for (int j = 0; j < nilai[0].length; j++) {}
double total = 0;
for (int i = 0; i < nilai.length; i++) {}
total += nilai[i][j];      
double rataMapel = total / nilai.length;
System.out.printf("%s:%.2f\n", mapel[j], rataMapel);
menghitung rata-rata tiap mata pelajaran dengan bagi total nilai sama jumlah siswa, lalu menampilkan hasilnya dengan format dua angka di belakang koma.

//TicTacToe

public class TicTacToe {} : digunakan untuk mendeklarasi kelas
public static void main(String[] args) {} : metode utama main yang akan dijalankan
char [][] papan = new char[3][3]; : array 2d yang berukuran 3*3
for (int i = 0; i < 3; i++) {}
for (int j = 0; j < 3; j++) {}
papan [i][j] = '-';
for dalam for untuk mengisi seluruh elemen papan jika '_' yang berarti masih kosong

papan [0][0] = 'X';
papan [1][1] = 'Y';
papan [2][2] = 'Z';
mengisi dengan simbol 'X', 'Y', 'Z'

System.out.println("Status papan : ");
tampilkanPapan(papan);
mencetak baris ke bawah dan menampilkan "Status papan : ", memanggil metode tampilkanPapan(papan) untuk mencetak isi

public static void tampilkanPapan(char [][] papan) {} : mendeklarasi metode statis dengan Array 2d

for (int i = 0; i < 3; i++) {}
for (int j = 0; j < 3; j++) {}
System.out.print(papan[i][j] + " ");
System.out.println();
dua loop for untuk menelusuri elemen baris per baris, mencetak setiap elemen ditambahkan spasi, mencetak baris berikutnya

   


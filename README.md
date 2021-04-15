# Magang-Iris
Variabel adalah symbol dari suatu besaran yang merepresentasikan sebuah lokasi dalam memori komputer.

Nilai variabel adalah informasi dari suatu besaran yang tersimpan dalam lokasi tersebut.

Pointer adalah variabel spesial yang menampung alamat memori, bukan nilai seperti variabel biasa.

Deklarasi pointer adalah sebuah pernyataan yang memberikan informasi tentang variabel kepada compiler C++ dengan Operator: *

Contoh:

Int * ptr;

Int* ptr;

inisialisasi adalah tugas pemberian nilai awal yang dilakukan saat deklarasi variabel.

int var = 55;

int *ptr = &var; // Inisialisasi menggunakan alamat dari var

Assignment merupakan operator yang digunakan untuk memberi nilai kepada tujuan.


contoh:

int var, *ptr;

var = 55;

ptr = &var; // Assignment pada variabel pointer menggunakan alamat dari var

Operator dereference digunakan untuk mengakses nilai yang ditunjuk (pointed) dari sebuah variabel pointer.

Contoh:

int var = 55;

int *ptr = &var;


printf("%d\n", *ptr);

*ptr = 20;


printf("%d\n", *ptr);

printf("%d\n", var);

double pointer Variabel pointer juga dapat menunjuk variabel pointer lainnya. Kegunaan paling umum dari variabel double pointer adalah untuk membuat array dua dimensi secara dinamis.

contoh:

int **dbPtr;

contoh:

#include <iostream>

using namespace std;

int main(){

int data [1];

int *nilai;

nilai = data;

cout << "input data : ";

for(int i=0; i<1; i++) {

cin >> data [i];

}

for(int i=0; i<1; i++) {

cout<<"data : "<<data[i]<<"menempati alamat memori : ";

cout<<&nilai[i];

cout<<endl;

}

}


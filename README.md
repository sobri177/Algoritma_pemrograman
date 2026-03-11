Algoritma dan Pemrograman - Java



Repository ini berisi kumpulan program sederhana yang dibuat untuk memenuhi tugas Mata Kuliah Algoritma dan Pemrograman.
Program dibuat menggunakan bahasa pemrograman Java untuk memahami konsep dasar seperti array dan perhitungan bangun ruang.

 #Daftar Program
No	Program	Deskripsi
1	Bangun Ruang	Program menghitung volume bangun ruang
2	Array 1 Dimensi	Program menyimpan dan menampilkan data menggunakan array
3	Array 2 Dimensi	Program mengolah data dalam bentuk matriks

 #Program Array 1 Dimensi
Program ini menggunakan array satu dimensi untuk menyimpan beberapa data seperti nama, NIM, dan nilai mahasiswa.

Contoh Source Code
public class DataMahasiswa {

    public static void main(String[] args) {

        String[] nama = {"Sobri", "Diky", "Bara"};
        String[] nim = {"312510236", "312510207", "312510253"};
        int[] nilai = {90, 85, 88};

        for(int i = 0; i < nama.length; i++){
            System.out.println("Nama  : " + nama[i]);
            System.out.println("NIM   : " + nim[i]);
            System.out.println("Nilai : " + nilai[i]);
            System.out.println();
        }

    }
}
 #Program Array 2 Dimensi

Program ini menggunakan array dua dimensi untuk menyimpan data dalam bentuk baris dan kolom (matriks).

Contoh Source Code
public class ArrayDuaDimensi {

    public static void main(String[] args) {

        int[][] matriks = {
            {1,2,3},
            {4,5,6},
            {7,8,9}
        };

        for(int i = 0; i < matriks.length; i++){
            for(int j = 0; j < matriks[i].length; j++){
                System.out.print(matriks[i][j] + " ");
            }
            System.out.println();
        }

    }
}
#Program Bangun Ruang

Program ini digunakan untuk menghitung volume bangun ruang kubus.

Contoh Source Code
import java.util.Scanner;

public class BangunRuang {

    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        System.out.print("Masukkan sisi kubus: ");
        int sisi = input.nextInt();

        int volume = sisi * sisi * sisi;

        System.out.println("Volume Kubus = " + volume);

    }
}

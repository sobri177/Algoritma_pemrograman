# PROGRAM ARRAY 2 DIMENSI – DATA MAHASISWA (JAVA)

Program ini dibuat menggunakan **bahasa pemrograman Java** untuk mempelajari konsep **Array 2 Dimensi** dalam mata kuliah **Algoritma dan Pemrograman**.

Array dua dimensi digunakan untuk menyimpan data dalam bentuk **baris dan kolom**, sehingga data dapat disusun seperti **tabel**.

Pada program ini array digunakan untuk menyimpan **data mahasiswa**, yaitu:

- Nama
- NIM
- Nilai

---

## TUJUAN PROGRAM

Tujuan dari pembuatan program ini adalah:

- Memahami konsep dasar **Array 2 Dimensi**
- Menyimpan data dalam bentuk **tabel**
- Melatih penggunaan **perulangan (looping)**
- Menampilkan data menggunakan **bahasa pemrograman Java**

---

## PERBEDAAN ARRAY 1 DIMENSI DAN ARRAY 2 DIMENSI

### Array 1 Dimensi

Array 1 dimensi adalah array yang hanya memiliki **satu indeks**.  
Biasanya digunakan untuk menyimpan data dalam bentuk **daftar (list)**.

Contoh:

```java
String[] nama = {"Sobri", "Diky", "Bara"};
```

Ciri-ciri array 1 dimensi:

- Memiliki **1 indeks**
- Data disimpan dalam **satu baris**
- Menggunakan **satu perulangan**

---

### Array 2 Dimensi

Array 2 dimensi adalah array yang memiliki **dua indeks**, yaitu **baris dan kolom**.

Contoh:

```java
String[][] mahasiswa = {
 {"Sobri","312510236","90"},
 {"Diky","312510207","85"},
 {"Bara","312510253","88"}
};
```

Ciri-ciri array 2 dimensi:

- Memiliki **2 indeks (baris dan kolom)**
- Data disimpan dalam bentuk **tabel**
- Biasanya menggunakan **perulangan bersarang (nested loop)**

---

## SOURCE CODE PROGRAM

```java
public class Array2Dimensi {

    public static void main(String[] args) {

        String[][] mahasiswa = {
            {"Sobri", "312510236", "90"},
            {"Diky", "312510207", "85"},
            {"Bara", "312510253", "88"}
        };

        System.out.println("DATA MAHASISWA (ARRAY 2 DIMENSI)");
        System.out.println("----------------------------------");

        for(int i = 0; i < mahasiswa.length; i++){
            for(int j = 0; j < mahasiswa[i].length; j++){
                System.out.print(mahasiswa[i][j] + " ");
            }
            System.out.println();
        }

    }
}
```

---

# 📊 CONTOH OUTPUT PROGRAM

<img width="562" height="322" alt="image" src="https://github.com/user-attachments/assets/9165b91b-7369-4923-9bf0-d529c1fee86b" />



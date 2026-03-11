# PROGRAM BANGUN RUANG (JAVA)
## Author = Diky Muhammad Azdzikro
Program ini dibuat menggunakan **bahasa pemrograman Java** untuk menghitung **volume berbagai bangun ruang** dalam mata kuliah **Algoritma dan Pemrograman**.

Bangun ruang yang dihitung dalam program ini yaitu:

- Kubus
- Balok
- Limas
- Bola
- Prisma
- Tabung
- Kerucut

Program akan meminta pengguna memasukkan ukuran bangun ruang kemudian program akan menghitung volumenya.

---

## TUJUAN PROGRAM

Tujuan dari program ini adalah:

- Memahami konsep **bangun ruang**
- Mempelajari **perhitungan volume**
- Menggunakan **input dari pengguna**
- Mengimplementasikan **rumus matematika ke dalam Java**

---

## RUMUS BANGUN RUANG

| Bangun Ruang | Rumus |
|---|---|
| Kubus | s × s × s |
| Balok | p × l × t |
| Limas | ⅓ × luas alas × tinggi |
| Bola | 4/3 × π × r³ |
| Prisma | luas alas × tinggi |
| Tabung | π × r² × t |
| Kerucut | ⅓ × π × r² × t |

---

## SOURCE CODE

import java.util.Scanner;

public class BangunRuangLengkap {

    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        int pilihan;

        System.out.println("=== PROGRAM MENGHITUNG BANGUN RUANG ===");
        System.out.println("1. Kubus");
        System.out.println("2. Balok");
        System.out.println("3. Tabung");
        System.out.println("4. Kerucut");
        System.out.println("5. Bola");
        System.out.println("6. Prisma");
        System.out.println("7. Limas");
        System.out.print("Pilih bangun ruang (1-7): ");
        pilihan = input.nextInt();

        switch (pilihan) {

            case 1:
                System.out.print("Masukkan sisi kubus: ");
                double sisi = input.nextDouble();

                double volumeKubus = sisi * sisi * sisi;
                double luasKubus = 6 * sisi * sisi;

                System.out.println("Volume Kubus = " + volumeKubus);
                System.out.println("Luas Permukaan Kubus = " + luasKubus);
                break;

            case 2:
                System.out.print("Masukkan panjang: ");
                double p = input.nextDouble();
                System.out.print("Masukkan lebar: ");
                double l = input.nextDouble();
                System.out.print("Masukkan tinggi: ");
                double t = input.nextDouble();

                double volumeBalok = p * l * t;
                double luasBalok = 2 * (p*l + p*t + l*t);

                System.out.println("Volume Balok = " + volumeBalok);
                System.out.println("Luas Permukaan Balok = " + luasBalok);
                break;

            case 3:
                System.out.print("Masukkan jari-jari tabung: ");
                double rTabung = input.nextDouble();
                System.out.print("Masukkan tinggi tabung: ");
                double tTabung = input.nextDouble();

                double volumeTabung = Math.PI * rTabung * rTabung * tTabung;
                double luasTabung = 2 * Math.PI * rTabung * (rTabung + tTabung);

                System.out.println("Volume Tabung = " + volumeTabung);
                System.out.println("Luas Permukaan Tabung = " + luasTabung);
                break;

            case 4:
                System.out.print("Masukkan jari-jari kerucut: ");
                double rKerucut = input.nextDouble();
                System.out.print("Masukkan tinggi kerucut: ");
                double tKerucut = input.nextDouble();

                double s = Math.sqrt((rKerucut*rKerucut) + (tKerucut*tKerucut));

                double volumeKerucut = (1.0/3) * Math.PI * rKerucut * rKerucut * tKerucut;
                double luasKerucut = Math.PI * rKerucut * (rKerucut + s);

                System.out.println("Volume Kerucut = " + volumeKerucut);
                System.out.println("Luas Permukaan Kerucut = " + luasKerucut);
                break;

            case 5:
                System.out.print("Masukkan jari-jari bola: ");
                double rBola = input.nextDouble();

                double volumeBola = (4.0/3) * Math.PI * rBola * rBola * rBola;
                double luasBola = 4 * Math.PI * rBola * rBola;

                System.out.println("Volume Bola = " + volumeBola);
                System.out.println("Luas Permukaan Bola = " + luasBola);
                break;

            case 6:
                System.out.print("Masukkan luas alas prisma: ");
                double luasAlasPrisma = input.nextDouble();
                System.out.print("Masukkan tinggi prisma: ");
                double tinggiPrisma = input.nextDouble();

                double volumePrisma = luasAlasPrisma * tinggiPrisma;

                System.out.println("Volume Prisma = " + volumePrisma);
                break;

            case 7:
                System.out.print("Masukkan luas alas limas: ");
                double luasAlasLimas = input.nextDouble();
                System.out.print("Masukkan tinggi limas: ");
                double tinggiLimas = input.nextDouble();

                double volumeLimas = (1.0/3) * luasAlasLimas * tinggiLimas;

                System.out.println("Volume Limas = " + volumeLimas);
                break;

            default:
                System.out.println("Pilihan tidak tersedia");
        }

    }
}
## HASIL RUN
<img width="698" height="480" alt="image" src="https://github.com/user-attachments/assets/acc991dc-cec1-4c85-9b41-bc2562f1598c" />


# Praktikum6
- Pertemuan 10
# praktikum 1
```
print("PROGRAM DAFTAR NILAI")
print("====================")
print()
data={}
while True:
    print()
    a=input("[(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar] :")
    print()

    if a=="t" or a=="T":
        print("TAMBAH DATA")
        print("-----------")
        nim=int(input("NIM\t: "))
        nama=input("Nama\t: ")
        tugas=int(input("Tugas\t: ")) 
        uts=int(input("UTS\t: "))
        uas=int(input("UAS\t: "))
        akhir=(int(tugas)*30/100)+(int(uts)*35/100)+(int(uas)*35/100)
        data[nim]=nama, tugas, uts, uas, akhir
        print()

    elif a=="l" or a=="L":
        if data.items():
            print("DAFTAR NILAI")
            print("------------")
            print(72*"=")
            print("| {0:^10} | {1:^10} | {2:^6} | {3:^6} | {4:^6} |   {5:^12}  |".format("NIM", "NAMA", "TUGAS", "UTS", "UAS", "NILAI AKHIR"))
            print(72*"=")
            for item in data.items(): 
                print("| {0:>10} | {1:>10} | {2:>6} | {3:>6} | {4:>6} |   {5:>12}  |".format(nim, nama, tugas, uts, uas, akhir))
                print(72*"=")
            print()
        else:
            print("DAFTAR NILAI")
            print("------------")
            print(72*"=")
            print("| {0:^10} | {1:^10} | {2:^6} | {3:^6} | {4:^6} |   {5:^12}  |".format("NIM", "NAMA", "TUGAS", "UTS", "UAS", "NILAI AKHIR"))
            print(72*"=")
            print("|                             TIDAK ADA DATA                           |")
            print(72*"=")
            print()

    elif a=="u" or a=="U":
        print("UBAH DATA")
        print("---------")
        b=input("Masukkan NIM anda: ")
        print()
        if data.keys():
            tugas=int(input("Tugas\t: ")) 
            uts=int(input("UTS\t: "))
            uas=int(input("UAS\t: "))
            akhir=(int(tugas)*30/100)+(int(uts)*35/100)+(int(uas)*35/100)

    elif a=="h" or a=="H":
        print("HAPUS DATA")
        print("----------")
        b=input("Masukkan NIM anda: ")
        print()
        if data.keys():
            del data[nim]
                   
    elif a=="c" or a=="C":
        print("CARI DATA")
        print("---------")
        b=input("Masukkan NIM anda: ")
        print()
        if data.keys():
            print(72*"=")
            print("| {0:^10} | {1:^10} | {2:^6} | {3:^6} | {4:^6} |   {5:^12}  |".format("NIM", "NAMA", "TUGAS", "UTS", "UAS", "NILAI AKHIR"))
            print(72*"=")
            print("| {0:>10} | {1:>10} | {2:>6} | {3:>6} | {4:>6} |   {5:>12}  |".format(nim, nama, tugas, uts, uas, akhir))
            print(72*"=")
            print()
            
    elif a=="k" or a=="K":
         break
```
![image](https://user-images.githubusercontent.com/115526901/204200529-43b9b697-7bbd-4887-98e0-6f0dca202873.png)




print("========== LATIHAN 1 - DICTIONARY ==========")
print()
r = {'Ari' : '081267888', 'Dina' : '087677776'}
print("# Daftar Kontak :\n", r)
print()

#Menampilkan Kontak
print("# Menampilkan kontak Ari : 081267888")
print("~~~~~~~~~~~~~~~~~~~~~~~~~")

#Menambahkan kontak baru
print("# Menambahkan kontak baru\n", r)
print("Daftar kontak sebelumnya :\n", r)
r['Riko']= '087654544';
print("Daftar kontak setelah ditambahkan :\n", r)
print("~~~~~~~~~~~~~~~~~~~~~~~~~")

#Mengubah kontak Dina
print("# Mengubah Kontak Dina\n")
print("Daftar Kontak Dina Sebelumnya :\n", r)
r['Dina'] = '088999776'
print("Daftar Kontak Dina Setelah Diubah :\n", r)
print("~~~~~~~~~~~~~~~~~~~~~~~~~")

#Menampilkan semua nama
print("# Menampilkan Semua Nama Kontak :\n")
print(r.keys())
print("~~~~~~~~~~~~~~~~~~~~~~~~~")

#Menampilkan semua nomor
print("# Menampilkan Semua Nomor :\n")
print(r.values())
print("~~~~~~~~~~~~~~~~~~~~~~~~~")

#Menampilkan Keseluruhan
print("# Daftar Kontak Keseluruhan :\n")
print(r.items())
print("~~~~~~~~~~~~~~~~~~~~~~~~~")

#Menghapus Kontak Dina
print("# Menghapus Kontak Dina\n")
print("Daftar Kontak Sebelumnya :\n", r)
del r['Dina'];
print("Daftar Kontak Setelah Dihapus :\n", r)


![image](https://user-images.githubusercontent.com/115526901/204201586-8367fa2b-a02f-4ad8-aeae-41e7a7ff6ba7.png)




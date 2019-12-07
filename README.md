# praktikum5

Pada praktek kali ini, saya mencoba membuat program menentukan nilai mahasiswa dengan menggunakan list.

-Source Code dan Penjelasan
	print("PROGRAM INPUT NILAI")
	print("===================")

	while True:
	    print("")
	    c = input("L)ihat, T)ambah, U)bah, H)apus, C)ari, K)eluar: ")
	    if c.lower() == 'l':
	        break
	print("Daftar Nilai")
	print("========================================================================")
	print("| No |    NIM    |       NAMA      |  TUGAS  |  UTS  |  UAS  |  AKHIR  |")
	print("========================================================================")
	print("|                            TIDAK ADA DATA                            |")
	print("========================================================================")
	while True:
	    print("")
	    c = input("L)ihat, T)ambah, U)bah, H)apus, C)ari, K)eluar: ")
	    if c.lower() == 't':
	        break
	print("Tambah Data")
	nilai = []
	nim = input("NIM: ")
	nama = input("Nama: ")
	nilaiUts = int(input("Nilai UTS: "))
	nilaiUas = int(input("Nilai UAS: "))
	nilaiTugas = int(input("Nilai Tugas: "))
	nilaiAkhir = (nilaiUts * 35/100) + (nilaiUas * 35/100) + (nilaiTugas * 30/100)
	
	nilai.append([nama, nim, nilaiTugas, nilaiUts, nilaiUas, int(nilaiAkhir)])

	while True:
	    print("")
	    c = input("L)ihat, T)ambah, U)bah, H)apus, C)ari, K)eluar: ")
	    if c.lower() == 'l':
	        break
	print("\n   Daftar Nilai   ")
	print("========================================================================")
	print("| No |    NIM    |       NAMA      |  TUGAS  |  UTS  |  UAS  |  AKHIR  |")
	print("========================================================================")
	i = 0
	for item in nilai:
	    i += 1
	    print("| {no:2d} |{nim:12s}|   {nama:9s}    |  {nilaiTugas:5d}  | {nilaiUts:5d} | {nilaiUas:5d} |  {nilaiAkhir:6.2f} |"
            .format(no=i, nim=item[0], nama=item[1], nilaiTugas=item[2], nilaiUts=item[3], nilaiUas=item[4], nilaiAkhir=item[5]))
	print("========================================================================")
-input

![input1](https://user-images.githubusercontent.com/56243857/70374511-a8851600-1925-11ea-9bd9-9b7eb124d4be.PNG)

![input2](https://user-images.githubusercontent.com/56243857/70374513-ad49ca00-1925-11ea-8819-8014a3ca79b5.PNG)

-output

![output1 1](https://user-images.githubusercontent.com/56243857/70374514-b175e780-1925-11ea-9c7b-5b7143e0fac8.PNG)

-flowchart

![flow](https://user-images.githubusercontent.com/56243857/70374554-4678e080-1926-11ea-891a-1b78d4c32ea2.PNG)

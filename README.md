# TugasPraktikum6

Praktikumtugas6
Kali ini kita akan mencoba membuat program tentang nilai data mahasiswa, dengan menggunkan Dectionary. Berikut ini code atau cara:

print("PROGRAM INPUT NILAI") 
print("===================")

while True: 
	print("") 
	c = input("L)ihat, T)ambah, U)bah, H)apus, C)ari, K)eluar: ") 
	if c.lower() == 'l': 
	break 
print("			  	     Daftar Nilai			       ") 
print("========================================================================") 
print("| No |    NIM    |   NAMA   |   TUGAS   |   UTS   |   UAS   |   AKHIR  |") 
print("========================================================================") 
print("| 			   TIDAK ADA DATA 			      |") 
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
print("\n                     Daftar Nilai (TI 19 A 1 )                        ") 
print("========================================================================") 
print("| No |    NIM    |    NAMA    |  TUGAS  |  UTS  |  UAS  |   AKHIR   |   ") 
print("========================================================================") 
i = 0 
for item in nilai: 
i += 1 
print("| {no:2d} |{nim:12s}| {nama:9s} | {nilaiTugas:5d} | {nilaiUts:5d} | {nilaiUas:5d} | {nilaiAkhir:6.2f} |" 
	.format(no=i, nim=item[0], nama=item[1], nilaiTugas=item[2], nilaiUts=item[3], nilaiUas=item[4], nilaiAkhir=item[5])) 
print("========================================================================")

![input1](https://github.com/hasanmaulana/TugasPraktikum6/blob/master/gambar/Tugas6%20INPUT%201.png)
![input2](https://github.com/hasanmaulana/TugasPraktikum6/blob/master/gambar/Tugas6%20INPUT%202.png)
![output1](https://github.com/hasanmaulana/TugasPraktikum6/blob/master/gambar/Tugas6%20OUTPUT1.png)
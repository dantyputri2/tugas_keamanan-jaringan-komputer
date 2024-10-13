* NAMA		: PUTRI DANTY APRIANI
* NIM		: 09011182126005
* KELAS		: SK7A INDRALAYA
* MATA KULIAH 	: KEAMANAN JARINGAN KOMPUTER
***

# Dumping and Cracking SAM Hashes to Extract Plaintext Passwords

Tools :
* Windows 11
* Pwdump7
* Ophrack

> Pwdump7 dan Ophcrack adalah alat yang digunakan untuk keamanan dan pemulihan kata sandi pada sistem Windows.
1.	Pwdump7:  adalah alat yang digunakan untuk mengekstrak kata sandi hash dari file SAM (Security Account Manager) di Windows. Pwdump7 dapat membantu dalam mengumpulkan informasi untuk audit keamanan atau dalam pengujian penetrasi.
2.	Ophcrack: adalah alat pemulihan kata sandi yang menggunakan teknik rainbow table untuk memecahkan kata sandi Windows. Ophcrack dapat digunakan untuk mengembalikan akses ke akun pengguna jika kata sandi terlupakan.

Langkah-langkah :
1.	Jalankan command prompt dengan mode run as administrator.
![image](https://github.com/user-attachments/assets/0e99b291-cf96-47f3-bff7-ba8ac8dee00f)

2.	Masukkan command prompt berikut untuk mengetahui nama pengguna dan UserIDs.
![image](https://github.com/user-attachments/assets/9882cb84-3f7e-4e6d-835c-da747b925041)

3.	Jalankan PwDump7.exe untuk mengumpulkan hashes dan UserIDs.
![image](https://github.com/user-attachments/assets/31a27d16-34a9-4440-8462-2dbcd732f6d6)

4.	Menampilkan isi dari file  hashes.txt
![image](https://github.com/user-attachments/assets/ebfdfe43-52ec-40ee-8d74-6f91df626c68)
![image](https://github.com/user-attachments/assets/ee795798-d35b-44f0-bd14-31f87033909e)

5.	Ganti nama pengguna sebelum UserIDs masing-masing yang telah didapatkan pada Langkah 2.
![image](https://github.com/user-attachments/assets/2a95bdad-c053-43c7-a822-ce0b66968569)

6.	Jalankan aplikasi ophcrack.axe dan masukkan file hashes.txt melalui PWDUMP file
![image](https://github.com/user-attachments/assets/6e066681-b5dc-4370-8209-fdebe2396767)
![image](https://github.com/user-attachments/assets/356f3386-8e93-42de-a0b8-232dce458b81)

7.	Selanjutnya klik menu Tables, install file Vista free dan menginstallnya
![image](https://github.com/user-attachments/assets/77da2c1b-8dea-476e-bf9e-e71508f594f4)
![image](https://github.com/user-attachments/assets/b18d05e4-f8ce-4f52-bde4-c2da42c87fe2)
![image](https://github.com/user-attachments/assets/3f619764-bb8b-4a51-9275-ff3c0393aaf6) 

8.	Langkah terakhir malakukan Crack.
![image](https://github.com/user-attachments/assets/055785d0-ed39-4338-b6ab-ae794aa83c2a)

9.	Dapat dilihat bahwa tidak ada password yang dipakai, seperti yang ditampilkan hasil percobaan berikut ini. 
![image](https://github.com/user-attachments/assets/509d6c04-9363-4064-ba7a-04a1a42ba770)

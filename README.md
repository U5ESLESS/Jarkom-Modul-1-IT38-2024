# Praktikum Jarkom-Modul-1-IT38-2024

## Anggota Kelompok
### Rafael Gunawan (5027231019)
### Randist Prawanda Putra (5027231059)
<hr>

## 1. Advance Sanity Check
![image](https://github.com/user-attachments/assets/72404291-f721-414d-8c5e-5013cabd9b42)
### Penjelasan:
- frame contains “username”.
![image](https://github.com/user-attachments/assets/b0d42e22-ffd5-4100-b234-24395e8f3c61) <br><br><br>
- frame containts “.txt”.
![image](https://github.com/user-attachments/assets/885fc7d4-d22d-4cde-8397-28fe515880ec) <br><br><br>
- Di Clue3.txt ada kalimat untuk membuka PPT dan saat melihat bagian Peraturan Soal Shift pada PPT terdapat sesuatu yang harus kita decode menggunakan base64. 
![image](https://github.com/user-attachments/assets/90c7e607-2d96-4855-88a1-3a5b0e9295a7) <br><br><br>
- Lalu input hasil Decodenya dan Flag pun muncul.
![image](https://github.com/user-attachments/assets/633c4c1e-c704-4b10-9a9a-efe5e601a335) <br><br><br><br>


## 2. Illegal Breakthrough
![image](https://github.com/user-attachments/assets/73a31576-16f5-4f2b-877e-8b1d35ec69a8)
### Penjelasan:
- Ketika Wireshark terbuka, saya langsung memilih IP Destination teratas, lalu saya melihat dari IP destinationnya.
![image](https://github.com/user-attachments/assets/a61e0bc2-01fc-4bb6-af8c-a270dd76ceeb) <br><br><br>
- Setelah membaca pertanyaan terkait port yang digunakan, saya menggunakan filter dengan kata "username". Disini saya dapat jawaban untuk pertanyaan port, endpoint, tools yang digunakan attacker, dan juga username + password.
![image](https://github.com/user-attachments/assets/e738b1c1-1be7-4f97-a489-0b74e7bac466) <br><br><br><br>

## 3. Packets Barrage
![image](https://github.com/user-attachments/assets/891286bb-4521-4b9d-b465-51b653fbb2e8)
### Penjelasan: 
- Ketika Wireshark terbuka, saya langsung memilih IP Source teratas, lalu saya melihat dari IP sourcenya.
![image](https://github.com/user-attachments/assets/a61e0bc2-01fc-4bb6-af8c-a270dd76ceeb) <br><br><br>
- Saya menggunakan filter http && ip.src eq 172.21.88.207, terlihat di bagian kanan bawah yang terdisplay ada angka 1918, yang kemudian dapat dikurangi 1 menjadi 1917.
![image](https://github.com/user-attachments/assets/42a5997b-24f7-449c-abc3-31131fb61125) <br><br><br>
- Follow file terakhir dari hasil yang telah didapatkan tadi untuk mendapatkan nama file yang didownload dan isi pesan yang disisipkan oleh attacker. 
![image](https://github.com/user-attachments/assets/6bc9862b-34e7-4597-9a84-71f427cdca6b) <br><br><br><br>

## 4. FTP Login
![image](https://github.com/user-attachments/assets/a679376f-6612-4bc5-9ea2-a7ee493a0f20)
### Penjelasan:
- Filter FTP sesuai nama soalnya lalu scroll untuk menemukan login yang sukses. Disitu kita akan menemuka username dan juga passwordnya.
![image](https://github.com/user-attachments/assets/61983403-cbe0-4157-938e-af816a861111)
![image](https://github.com/user-attachments/assets/07d21460-f52c-48d7-ad81-9ff4060b62a8) <br><br><br><br>

## 5. Surprise
![image](https://github.com/user-attachments/assets/3cc33f1d-3940-4f3f-867c-60ea947602db)
### Penjelasan:
- Dari isi file sebelumnya, kita bisa menemukan nama service yang digunakan dan file yang dikirim oleh attacker.
![image](https://github.com/user-attachments/assets/07d21460-f52c-48d7-ad81-9ff4060b62a8) <br><br><br>
- Lalu semisal kita scroll kebawah, kita akan menemukan isi dari file .cp tersebut. kita kemudian jalankan kode tersebut dan akan keluar sebuah pesan.
![image](https://github.com/user-attachments/assets/4ca9a2f1-0f61-469f-bdbe-d24445cc306e) <br><br><br><br>

## 6. Corporate Breach
![image-3](https://github.com/user-attachments/assets/c68238c3-0f6e-42b6-8f48-9c8f97945729)
### Penjelasan:
- buka pcap file ke wireshark dan buka juga nc (netcat) pada linux untuk hint
- untuk soal pertama kita dapat menemukan nya dengan cara follow line paling atas
![image-1](https://github.com/user-attachments/assets/b7ff3bac-dbc5-4c16-a3c0-ec02baf1933c)
- kemudian untuk soal ke 2 & 3 saya menemukan nya sekaligus pada salah satu protocol http
![image-2](https://github.com/user-attachments/assets/9ec3141d-a89b-4618-a114-623223c60129)

## 7. Pegawai Negeri Sebelah
![image-4](https://github.com/user-attachments/assets/305116b0-03da-4693-9bed-89a91a7a1b4d)
### Penjelasan:
- buka pcap file ke wireshark dan buka juga nc (netcat) pada linux untuk hint
- untuk soal pertama kita dapat menggunakan fitur filter dengan mengetik `frame contains "nNnM%coQuF"`
![image-5](https://github.com/user-attachments/assets/e56f9d94-44ee-4e78-9c2d-80104eafc478)
- untuk soal-soal berikutnya gunakan fitur find pada follow
- Soal 2
![image-6](https://github.com/user-attachments/assets/ab58dae4-a44a-4e26-8d1a-733defda5e72)
- Soal 3
![image-7](https://github.com/user-attachments/assets/0754278f-6561-48e1-967c-84eca15edf66)
- Soal 4
![image-8](https://github.com/user-attachments/assets/e3ea9b01-bf0d-43da-ad0d-ae80ce0214da)

## 8. EZ
![image-9](https://github.com/user-attachments/assets/2f4c4843-89d1-431e-8a52-5c5ed4a24c06)
### Penjelasan:
- buka pcap file ke wireshark dan buka juga nc (netcat) pada linux untuk hint
- untuk soal pertama kita bisa menemukan nya saat menggunakan fitur follow di line pertama
![image-10](https://github.com/user-attachments/assets/db429447-cacf-4c86-910f-6b8c566384d9)
- untuk jawaban dari soal kedua, kita hanya butuh mengeclick pada pesan yang ingin kita liat port nya
![image-11](https://github.com/user-attachments/assets/1bfc00ab-e3f9-4777-91db-38c6a3dff4cc)

## 9. Rizzset
![image-12](https://github.com/user-attachments/assets/191cd11e-8c4a-49bf-8559-f67a607d6a20)
### Penjelasan:
- buka pcap file ke wireshark dan buka juga nc (netcat) pada linux untuk hint
- untuk soal 1 dan 2 kita bisa melihat nya langsung pada info dari line no. 8
![image-13](https://github.com/user-attachments/assets/112956ec-f6ce-4a77-b8bf-fbcaefdc20d6)
- untuk soal ke 3 kita harus menggunakan tools jarm pada domain dari `www.its.ac.id` pada terminal linux
![WhatsApp Image 2024-09-21 at 00 34 41_4e0e572c](https://github.com/user-attachments/assets/316357a3-000b-415c-b490-54124e110009)

## 10. 22 Nightmare
![image-14](https://github.com/user-attachments/assets/3548b0cc-e05c-401a-b498-a4514804a5b0)
### Penjelasan:
- untuk soal 1 (nama file jpg) & 2 (isi gambar dari file jpg)  karena saya menemukan kejanggalan pada salah satu line FTP yang mempunyai file gambar, kita dapat menggunakan fitur Export object dan pilih opsi FTP-DATA kemudian download seluruh data yang ada (Sh1k4.jpg & noko.py)
![image-15](https://github.com/user-attachments/assets/9df430b1-67c2-4830-86da-625805b516ba)
- untuk mencari soal 3 saya tidak sengaja menemukan info `stor noko.py` pada stream 141
![image-16](https://github.com/user-attachments/assets/70f551ab-d69e-4c48-83d9-6dbffb8c983b)
- untuk soal terakhir kita dapat membuka file python (noko.py) kemudian mengubah code agar bisa menjalankan operasi XOR dan memasukan nilai key dengan cara perhatikan clue dalam code python `img msg` yaitu NUN
![image-17](https://github.com/user-attachments/assets/05baaf14-7bec-4685-b0a8-00105f6aca2c)

# Soal Tambahan
## 11. Malicious Code
![image](https://github.com/user-attachments/assets/20eaaac0-20c1-40e3-a83e-3d80c999ad78)
### Penjelasan:
- Gunakan filter http.request.method=="GET" && frame contains ".php" untuk menemukan jumlah attempt dirlist dari attacker.
![image](https://github.com/user-attachments/assets/a473a2c4-a5e1-4105-83aa-6383697a8d0d)
- Lalu, scroll dan follow hasil filter sampai paling bawah untuk mendapatkan endpoint yg berhasil didapatkan attacker.
![image](https://github.com/user-attachments/assets/d6d425e8-3962-4a10-9ae2-6354413a8749)
- Kemudian, filter http.request.method=="POST" untuk mememukan pada percobaan ke berapa attacker berhasil menemukan email dan password yang benar. Ketika difilter terdapat 169 traffic yang terdisplay, nah disini saya mengesampingkan 5 file terbawah karena hanya berisi pesan. Saya menemukan kejanggalan dari length file di urutan 153 karena ukurannya lebih besar dibanding file lainnya dan kemudian saya buka dan benar hasilnya.
![image](https://github.com/user-attachments/assets/b78fa8fb-6959-4fc0-b68e-02a2f463452d)
- Terakhir, di 5 file yang saya sampingkan tadi, ada pesan berbahasa ASCII yang menurut saya adalah cluenya. Benar saja, ketika saya pisahkan satu-satu dan kemudian saya convert ternyata ada cluenya.
![image](https://github.com/user-attachments/assets/aef66ba0-2c70-4627-9648-ed415a35c4af)

## 12. Gajah Terbang (Server Recon)
![image](https://github.com/user-attachments/assets/50dd7757-7377-4f04-99dc-8667298bfee1)
### Penjelasan:
- Saat membuka wireshark langsung keluar jenis protocol PGSQL yang merupakan DBMS, tapi untuk format yang kita masukan merupakan kepanjangannya yaitu PostgreSQL.
![image](https://github.com/user-attachments/assets/ca300d25-35c7-4aaa-91a2-2829c3ad93e8)
- Lalu kita disuruh untuk memasukkan port nya PGSQL itu, awalnya saya coba memasukan port 5432 yang merupakan port defaultnya tetapi tidak bisa. Selanjutnya, saya pun sadar kalo ada banyak interaksi dari port   6969 jadi saya coba dan berhasil.
![image](https://github.com/user-attachments/assets/3b0670a9-027a-4642-a2d6-3c2863de8094)
- Selanjutnya, saya mencoba follow satu-satu dari semua interaksi port 6969 dan ketemu lah file berikut. Dari sini pun kita bisa tau OS dari server, username DBMS, nama database, jumlah user yang ada, dan email + password yang harus didecode dari admin.
![image](https://github.com/user-attachments/assets/0b48a48f-f086-4a3f-80ba-44a3c2c358bb)

## 13. Gajah Terbang (Attacker Recon)
![image](https://github.com/user-attachments/assets/6032c4cb-c805-4307-8d1a-b839b0658357)
### Penjelasan:
- Masih memakai gambar sebelumnya, untuk menemukan siapa attackernya saya coba satu-satu dari user yang ada dan yang benar adalah kunto aji. Kemudian untuk passwordnya dari kunto aji juga saya hashing yang hingga mendapat hasilnya. Selanjutnya untuk melihat kapan akun attacker di ban kita bisa melihat pada bagian SELECT * FROM banned_users. Lalu untuk melihat tabel apa saja yang di edit oleh attacker disini kita bisa lihat dari command UPDATE users dan DELETE FROM banned_users. Terakhir untuk produk yang dibeli saya coba input satu-satu dan akhirnya yang benar adalah rokok dan eskrim, untuk total harganya juga bisa dilihat dari SELECT * FROM products.
![image](https://github.com/user-attachments/assets/0b48a48f-f086-4a3f-80ba-44a3c2c358bb)

## 14. Stegography
![image](https://github.com/user-attachments/assets/5e7b7d8c-a29b-4156-8cfa-1605ba32e3c2)
### Penjelasan:
- Filter dengan frame contains "png" untuk melihat ada berapa banyak gambar yang dikirim, kemudian ekspor object file FTP-DATA ke dalam direktori kita.
![image](https://github.com/user-attachments/assets/f0635853-ae7d-4975-a6f7-be33ac60bc55)
- Kemudian kita modifikasi sedikit kode dalam file reversed.py dan kita run. Kalau dilihat dari gambar diatas hanya 3 gambar yang memiliki message, nah tetapi message disini masih terbalik maka dari itu harus di balik dan urutkan menjadi "pahlawan keamanan siber".
![image](https://github.com/user-attachments/assets/4c15723d-b80e-4a32-b5fe-6cd9a1096712) ![image](https://github.com/user-attachments/assets/37b97b62-750c-4f71-9163-e85f416d3335)

## 15. inneRCE
![image](https://github.com/user-attachments/assets/053b98c2-e2d2-4eb5-9ee8-e281bc623cf2)
### Penjelasan:
- Untuk menemukan hacker berhasil mengupload webshell, kita bisa filter http terlebih dahulu. Di hasil filter kita bisa lihat bahwa ada endpoint /upload.php, kemudian disitu saya buka detail packagenya dan melihat arrival timenya.
![image](https://github.com/user-attachments/assets/826049a0-5dbe-4780-b9ca-0edae9b47736)
- Langkah selanjutnya, karena diminta mencari hostname saya coba untuk memfilter menggunakan frame contains "hostname" dan benar saja keluar satu package yang saat saya follow seperti ini hasilnya. Dari sini kita bisa tahu endpoint url, hostname, dan webshell yang diupload hacker.
![image](https://github.com/user-attachments/assets/b115f097-6570-430c-8d7e-889ea1c689d9)
- Kemudian, untuk menemukan command pertama yg di eksekusi hacker, saya menggunakan filter frame contains "idzoyyshell.php" dan saya menemuka command pertamanya seperti berikut.
![image](https://github.com/user-attachments/assets/2c120ab1-2bbc-4f8a-9f7e-2494a7383a89)
- Terakhir, untuk menemukan pesan yang hacker tuliskan, saya gunakan dari filter tadi juga. Kalau diliat di gambar sebelumnya, ada package yang mengandung base64, disini saya langsung follow dan ada pesan yang dienkripsi. Untuk mendapat pesannya kita harus mendekripsi kata-katanya sehingga hasil akhirnya menjadi pls rate soal ini.
![image](https://github.com/user-attachments/assets/16156fde-a4ca-4e31-9335-cb965e6f04bd) ![image](https://github.com/user-attachments/assets/5b418131-9ddb-47e4-aba2-3dc999b8940e)

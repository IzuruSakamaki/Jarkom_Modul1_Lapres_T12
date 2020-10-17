# Jarkom Modul1 Lapres T12

## Soal
Terdapat tiga buah file *.pcapng yang mendukung soal-soal display filter, yaitu:
- File pertama untuk menjawab soal nomor 1-5 dan nomor 10.
- File kedua untuk menjawab soal nomor 6, 7, dan 9.
- File ketiga untuk menjawab soal nomor 8.
#### A. Display Filter
1. Sebutkan webserver yang digunakan pada "testing.mekanis.me"!
2. Simpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"!
3. Cari username dan password ketika login di "ppid.dpr.go.id"!
4. Temukan paket dari web-web yang menggunakan basic authentication method!
5. Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!
6. Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).
7. Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut. Your Super Mega Ultra Rare Hint = nama pdf-nya "Yes.pdf"
8. Cari objek apa saja yang didownload (RETR) dari koneksi FTP dengan Microsoft FTP Service!
9. Cari username dan password ketika login FTP pada localhost!
10. Cari file .pdf di wireshark lalu download dan buka file tersebut! clue: "25 50 44 46"
#### B. Capture Filter
11. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
12. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!
13. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
14. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
15. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id!
## Jawaban
#### A. Display Filter
1. *http.host == “testing.mekanis.me”*
![Gambar 1.1](img/11.png)
![Gambar 1.2](img/12.png)

2. ...
![Gambar 2.1](img/21.png)
![Gambar 2.2](img/22.png)

3. *http.host == “ppid.dpr.go.id”*
![Gambar 3.1](img/31.png)

4. ...

5. *http.host == “aku.pengen.pw”*
![Gambar 5.1](img/51.png)
![Gambar 5.2](img/52.png)

6. ...

7. ...

8. *ftp.request.command == RETR*
![Gambar 8.1](img/81.jpg)

9. *ftp.request.command =="USER"
![Gambar 9.1](img/no9.PNG)
   ftp.request.command =="PASS"
![Gambar 9.2](img/no9pass.PNG)
10. *Control+F
![Gambar 10.1](img/no10(1).PNG)
    Klik kanan kemudian follow tcp stream, lalu ubah show and save data as menjadi RAW.
![Gambar 10.2](img/no10(2).PNG)
    Klik tombol Save as dan simpan file pdf
![Gambar 10.3](img/no10(3).PNG)
    Buka file yang telah didownload
![Gambar 10.4](img/no10(4).PNG)
#### B. Capture Filter
11. ...
12. ...
13. ...
14. ...
15. ...

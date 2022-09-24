# Lapres Praktikum Jarkom 2022 Modul 1 Kelompok F09

## Anggota Kelompok

<table>
    <tr>
        <th>NRP</th>
        <th>Nama</th>
    </tr>
    <tr>
        <td>Muhammad Lintang Panjerino</td>
        <td>5025201045</td>
    </tr>
    <tr>
        <td>Sayid Ziyad Ibrahim Alaydrus</td>
        <td>5025201147</td>
    </tr>
    <tr>
        <td>Wahyu Tri Saputro</td>
        <td>5025201217</td>
    </tr>
<table>

<br>

## NO 1.

### Sebutkan web server yang digunakan pada "monta.if.its.ac.id"!

### **Jawab:**

Untuk mengerjakan soal 1, Open file resource terlebih dahulu pada aplikasi _Wireshark_. File resource yang dimaksud adalah file pada **soal/soal1-2.pcapng**. Kemudian dilakukan _display filter_ dengan meng-apply **http.host**. Setelah itu, pilih salah satu hasil filter (di sini kami memilih hasil filter paling atas, No. 321), kemudian klik kanan --> Follow --> TCP Stream. Setelah itu, keluar sebuah window dan dapat dilihat isinya bahwa web server yang digunakan pada "monta.if.its.ac.id" adalah **nginx/1.10.3**

Wireshark filter expression: **http.host** <br>
**Server: nginx/1.10.3**

Screenshot bukti: [screenshot](https;//github.com/mlintang20/Jarkom-Modul-1-F09-2022/img/screenshot 1.png)

## NO 2.

### Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?

### **Jawab:**

Untuk mengerjakan soal 2, Open file resource terlebih dahulu pada aplikasi _Wireshark_. File resource yang dimaksud adalah file pada **soal/soal1-2.pcapng**. Kemudian dilakukan _display filter_ dengan meng-apply **http.request.uri contains "detail"**. Setelah itu, muncul satu hasil filter, kemudian klik kiri --> lihat pada bagian tengah tampilan Wireshark --> klik _Hypertext Transfer Protocol_ --> klik _GET /index.php/topik/detailTopik/194 HTTP/1.1\r\n_ --> lihat pada bagian _Request URI_. Terlihat bahwa isinya adalah **/index.php/topik/detailTopik/194**. Setelah itu, buka web browser dan ketikkan **http://monta.if.its.ac.id/index.php/topik/detailTopik/194**, dan pada web tersebut dapat terlihat judul TA yang dimaksud

Wireshark filter expression: **http.request.uri contains "detail"** <br>
**Judul TA: Evaluasi unjuk kerja User Space Filesystem (FUSE) oleh WAHYU SUADI, Rabu 17 Maret 2021 pukul 05:13:50 WIB**

## NO 3.

## NO 4.

## NO 5.

## NO 6.

## NO 7.

### Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

### **Jawab:**

Pada soal ini kami menggunakan IP dari salah satu anggota kami, di mana IP nya adalah 192.168.43.89, yang dapat dilihat melalui Taskbar --> Wi-Fi network --> Properties --> IPv4 address. Pada aplikasi _Wireshark_ dipilih Capture Filter Wi-Fi, kemudian setelah masuk, apply perintah pada Display Filter, yaitu **ip.src == 192.168.43.89**. Setelah itu, keluar filter yang menampilkan paket yang berasal dari IP tersebut. Captured packet disave menjadi sebuah file .pcapng dan dapat dilihat pada **soal/soal7.pcapng**

Wireshark filter expression: **ip.src == 192.168.43.89**

## NO 8.

## NO 9.

## NO 10.

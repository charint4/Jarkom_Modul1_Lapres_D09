# Praktikum Modul 1
Kelompok D09
- 05111840000058 Rafif Ridho
- 05111840000128 Muhammad Rivadhli Purnomo

<br>

#### Soal 1
>Sebutkan webserver yang digunakan pada "testing.mekanis.me"!

Cari paket testing.mekanime.me dengan filter http.host == testing.mekanisme.me

![gambar1.1](/img/1.1.jpg)

Lalu follow tcp stream pada packet http/1.1

![gambar1.2](/img/1.3.jpg)

dapat dilihat webserver yang digunakan pada "testing.mekanisme.me"

![gambar1.3](/img/1.2.jpg)


#### Soal 2
>Simpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"!

cari packet yang berisi "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg" dengan menggunakan find packet dan ubah tipe data menjadi string 

![gambar2.1](/img/2.1.jpg)

setelah dapat packetnya di export httpnya

![gambar2.2](/img/2.2.jpg)

berikut gambar yang dimaksud soal

![gambar2.3](/img/2.3.jpg)


#### Soal 3
> Cari username dan password ketika login di "ppid.dpr.go.id"!

Melalui filter cari http.host == ppid.dpr.go.id

![gambar3.1](/img/3.1.jpg)

cari paket yang FTP nya Post atau terdapat kata login, username dan password dapat dilihat di kolom paling bawah dan baris paling bawah wireshark

![gambar3.2](/img/3.2.jpg)

#### soal 4
> Temukan paket dari web-web yang menggunakan basic authentication method!

Melalui filter ketik http.authbasic

![gambar4.1](/img/4.1.jpg)

#### Soal 5
> Ikuti perintah di "aku.pengen.pw"! Username dan password bisa didapatkan dari file .pcapng!

cari packet "aku.pengen.pw"

![gambar5.1](/img/5.1jpg)

username dan password dapat dilihat di dropdown hypertext lalu authorization

![gambar5.1](img?5.2.jpg)


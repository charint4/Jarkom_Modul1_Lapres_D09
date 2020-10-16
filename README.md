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

#### Soal 4
> Temukan paket dari web-web yang menggunakan basic authentication method!

Melalui filter ketik http.authbasic

![gambar4.1](/img/4.1.jpg)

#### Soal 5
> Ikuti perintah di "aku.pengen.pw"! Username dan password bisa didapatkan dari file .pcapng!

cari packet "aku.pengen.pw"

![gambar5.1](/img/5.1.jpg)

username dan password dapat dilihat di dropdown hypertext lalu authorization

![gambar5.2](/img/5.2.jpg)

pada "aku.pengen.pw" ditanyakan Urutan konfigurasi pengkabelan T568B

![gambar5.3](/img/5.3.jpg)

konfigurasi pengkabelan T568B adalah

Putih orange, orange, putih hijau, biru, putih biru, hijau, putih coklat, coklat

#### Soal 6
>Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).

Mencari password zip melalui find packet, dan search "zipkey.txt" yang FTP DATA

![gambar6.1](/img/6.1.jpg)

Follow tcp stream packet yang terfilter, password akan langsung ada dalam bentuk ascii

![gambar6.2](/img/6.2.jpg)

Setelah mengcopy pastekan password, cari file "answer.zip" yang FTP DATA melauli find packet

![gambar6.3](/img/6.3.jpg)

Follow tcp stream juga, akan tetapi ubah dari ascii ke raw lalu save as "Answer.zip"

![gambar6.4](/img/6.4.jpg)

setelah dapat file dan passwordnya extract file, berikut tampilan file yang ada dalam "Answer.zip" :

![gambar6.5](/img/6.5.jpg)

#### Soal 7
>Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut.
Your Super Mega Ultra Rare Hint = nama pdf-nya "Yes.pdf"

Mencari file pdf dengan filter frame contains "Yes.pdf", pilih yang FTP DATA 

![gambar7.1](/img/7.1.jpg)

Lalu follow tcp stream dan ubah ke raw

![gambar7.2](/img/7.2.jpg)

Berikut Tampilan File yang dicari :

![gambar7.3](/img/7.3.jpg)






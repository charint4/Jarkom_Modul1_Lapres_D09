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

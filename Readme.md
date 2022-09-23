# Laporan Hasil Praktikum 1

## 1. Sebutkan web server yang digunakan pada "monta.if.its.ac.id"!

- display filter: `http.request and http.host eq "monta.if.its.ac.id"`

![img 1](./assets/1_1.png)

- klik kanan, lalu tekan `follow tcp stream`

![img 2](./assets/1_2.png)

- terlihat bahwa server pada web menggunakan `Nginx`

![img 3](./assets/1_3.png)

## 2. Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?

- display filter: `ip.host == 103.94.189.5 && http contains "detailTopik"`

![img 1](./assets/1_3.png)

- setelah itu terlihat bahwa client mengunjungi link index.php/topik/detailTopik/194. Lalu diketikkan ke mesin pencari.

![img 2](./assets/1_3.png)

hasil yang didapat adalah sebagai berikut

- Link: http://monta.if.its.ac.id/index.php/topik/detailTopik/194

- Judul: `Evaluasi unjuk kerja User Space Filesystem (FUSE)`

## 6. Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id !

- display filter: `http contains "lipi.go.id"`

![img 1](./assets/6_1.png)

## 7. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

- display filter: ` ip.src_host == 192.168.255.24`

![img 1](./assets/7_1.png)

## Kesulitan

- susah mencari keyword dari beberapa case di search engine

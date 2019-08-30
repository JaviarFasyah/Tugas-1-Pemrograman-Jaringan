# Tugas-1-Pemrograman-Jaringan
### Javiar Fasyah - 1301164477

**Jawaban Soal No. 1:**
  Diagram yang dimaksud adalah diagram TCP three-way handshake, yang terjadi saat client dan server berkomunikasi dalam suatu jaringan. 
  Dari sisi client, hal pertama yang dilakukannya setelah aktif adalah mengirim pesan SYN (synchronize) kepada server. Jika pesan diterima dan server menjawab dengan pesan SYN, ACK (synchronize, acknowledge), maka kedua entitas tersebut sudah membangun koneksi dan siap berkomunikasi. Disaat client menyudahi sesi dengan server (mengirim pesan FIN (finish) dan server menjawab dengan mengirim pesan ACK lalu FIN (atau kebalikannya), maka kedua entitas tersebut resmi terputus koneksinya.
  Dari sisi server, disaat server sudah siap dan menerima pesan SYN dari client, maka server akan mengrimkan pesan SYN, ACK untuk memulai koneksi dengan client. Setelah mendapat jawaban ACK dari client, koneksi diantara keduanya terbangun dan siap berkomunikasi. Disaat client ingin menyudahi sesi dan mengirim pesan FIN, server akan mengirim pesan ACK lalu mengirim pesan FIN setelah sesi diterminasi. Setelah client menjawab ACK, maka koneksi keduanya resmi terputus.

**Jawaban Soal. No. 2:**
  Program pertama adalah tentang berbagai macam sintaks iterasi dalam bahasa Go, output yang dihasilkan adalah “1, 2, 3; 7, 8, 9; loop; 1, 3, 5”. Pada iterasi pertama, variabel di-assign nilai diluar sintaks iterasi, iterasi dilakukan hingga batas yang ditentukan dengan mencetak nilai variabel saat iterasi lalu menambah nilai variabelnya hingga memenuhi batas iterasi. Pada iterasi kedua, nilai iterasi di-assign dalam sintaks beserta penambahan nilai variabelnya, iterasi dilakukan hingga batas yang ditentukan sembari mencetak nilai variabel.
  Pada iterasi ketiga, terdapat sintaks break yang akan menyudahi iterasi sesuai keinginan (dalam kasus ini setelah mencetak string “loop”). Pada iterasi terakhir, iterasi dilakukan mirip dengan pada iterasi kedua, namun dalam pencetakan nilai variabel terdapat sebuah kondisi dimana jika nilai variabel di-mod 2 sama dengan 0 (bilangan genap), maka pencetakan nilai variabel dilewati (dengan sintaks continue).
![2a_0.png](/screenshot/2a_0.png)
![2a_1.png](/screenshot/2a_1.png)

  Program kedua adalah tentang penulisan sintaks kondisi pada bahasa Go, output yang dihasilkan adalah “7 is odd; 8 is divisible by 4; 9 has 1 digit”. Pada kondisi pertama, terdapat pengecekan nilai 7 dengan di-mod 2, jika hasilnya 0 maka dicetaklah “7 is even”, jika tidak maka dicetak “7 is odd”. Pada kondisi kedua, terdapat kondisi mirip dengan kondisi pertama (jika 8 di-mod 4 adalah 0, maka dicetak “8 is divisible by 4”), namun jika seandainya 8 di-mod 4 bukan 0, maka program tidak akan mencetak apapun. Pada kondisi terakhir, nilai variabel di-assign didalam sintaks kondisi untuk kemudian dibandingkan, jika variabel kurang dari 0 maka dicetak “is negative”, jika variabel kurang dari 10 maka dicetak “has 1 digit”, dan jika bukan kedua-duanya maka dicetak “has multiple digits”.
![2b.png](/screenshot/2b.png)

**Jawaban Soal No. 3:**
  Program pertama adalah tentang array dalam bahasa Go, output yang dihasilkan adalah “emp” [0 0 0 0 0], set: [0 0 0 0 100], get: 100, len: 5; dcl: [1 2 3 4 5]; 2d: [0 1 2] [1 2 3]”. Array pertama di-assign sebagai array integer dan dicetak saat array masing kosong, lalu array tersebut di-assign nilai 100 pada index ke-4 sehingga saat array dicetak kembali terdapat nilai 100 pada index terkahir, nilai pada index terakhir juga dicetak tersendiri dan panjang dari array dicetak dengan sintaks len. Array kedua juga merupakan array integer yang di-assign langsung dengan nilai pada masing-masing index, sehingga saat dicetak array menampilkan nilai-nilai dari masing-masing index. Array terakhir merupakan array dua dimensi (2 array dengan masing-masing 3 index), array dua dimensi ini di-assign nilainya dengan iterasi bersarang (iterasi didalam iterasi).
![3a.png](/screenshot/3a.png)

  Program kedua adalah tentang fungsi dalam bahasa Go, outputnya adalah “1+2= 3; 1+2+3= 6”. Fungsi pertama adalah fungsi khusus tipe data integer yang akan mengembalikan hasil penambahan dari dua variabel masukan parameter, parameter pada fungsi ini dideklarasikan tipe datanya satu persatu. Fungsi kedua mirip dengan fungsi pertama yang khusus untuk tipe data integer dan mengembalikan hasil penambahan dari tiga variabel parameter, namun parameter pada fungsi dideklarasikan semuanya pada suatu tipe data.
![3b.png](/screenshot/3b.png)

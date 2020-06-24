[English](README.md) ∷ [Bahasa Melayu Rumi](README_ms.md) ∷ [بهاس ملايو جاوي](README_ms-Arab.md)

# Jawi Font (Fon Jawi)

Fail-fail fon tulisan Arab yang disunting untuk menambah sokongan huruf-huruf Jawi.


## Apakah kegunaan repositori ini?

Repositori ini mempunyak fail-fail terbitan asal bagi beberapa fon tulisan Arab bersumber terbuka yang terpilih, fail-fail FontForge untuk fon Arab yang telah disunting, dan juga pakej fon Arab tersunting yang diterbitkan yang mengandungi sokongan [tulisan Jawi](https://ms.wikipedia.org/wiki/Tulisan_Jawi).


## Kenapa sunting fail-fail fon?

Jumlah fon Arab bersumber terbuka adalah sedikit, dan daripada situ pun, hanya sebilangan kecil sahaja yang sebenarnya menyokong tulisan Jawi.

Fon-fon yang diterbitkan daripada repositori ini akan mempunyai sokongan penuh untuk tulisan Jawi dan ia juga akan mampu digunakan pada aplikasi-aplikasi lama di mana kegunaan set penggayaan fon (*stylistic sets*, seperti ss01 dll) tidak dapat digunakan.


## Bilakah repositori ini dicipta?

Repositori ini dicipta pada 30 Mei 2020 (tarikh bahasa Melayusia).


## Di manakah suntingan fon dilakukan?

Kesemua fon disunting menggunakan FontForge yang dijalankan pada tika Ubuntu melalui aplikasi UserLAnd dekat telefon saya. Saya tidak mempunyai capaian kepada mana-mana komputer dan tidak akan dapat sebarang komputer selagi mana saya belum mendapat kerja untuk dapatkan wang yang cukup untuk membina komputer.


Maklumat teknikal:

- Versi FontForge: 11:12 UTC 24-Sep-2017 (versi terbaru yang ada di APT setakat 30 Mei 2020)
- Versi Ubuntu: Ubuntu 18.04.4 LTS aarch64 (pemasangan asal Ubuntu di UserLAnd)
- Versi UserLAnd: UserLAnd 2.7.2 (versi terbaru yang ada di Play store saya setakat 30 Mei 2020)
- Versi Android: 8.0.0 (versi terbaru yang ada untuk telefon ini setakat 30 Mei 2020)
- Model telefon: Samsung Galaxy S7 Edge (SM-G935F), diberikan oleh maksu saya pada bulan Disember 2019 (sebelum itu, saya gunakan Sony Xperia C5 Ultra Dual sejak tahun 2014, ia telah tamat riwayat pada Mac 2020, tidak mampu but sudah.)


## Siapa yang menyenggara kesemua fon-fon yang telah disunting ini?

Pemilik repositori, [Yaya MNH48](https://meta.mnh48.moe), selaku pemilik tunggal organisasi jawi-mnh48.


## Kenapa tidak gunakan alatan asal untuk fon-fon yang mempunyai sumber tersedia?

Saya tidak mempunyai sebarang peranti yang mampu menjalankan alat tersebut. Sekiranya mana-mana fon dalam repositori yang mempunyai sumber tersedia yang boleh disunting terus secara natif di FontForge maka saya akan sudah tentu gunakannya. Kebanyakan fon yang saya jumpa disunting menggunakan perisian berbayar yang dikenali sebagai Glyph, bukan sahaja ianya sangat mahal, malah ia juga tidak tersedia untuk Linux arm64.


## Bagaimanakah cara fon-fon ini disunting?

Dengan mengikut langkah-langkah dalam tutorial berbahasa Inggeris yang bertajuk "[Adding Glyphs to an Arabic Font](http://designwithfontforge.com/en-US/Adding_Glyphs_to_an_Arabic_Font.html)" (Menambah Glif ke Fon Arab) di laman web [Design With FontForge](http://designwithfontforge.com/) (Merekacipta Menggunakan FontForge).

Glif-glif yang saya sunting untuk membuatnya sokong tulisan Jawi termasuklah:

- Mengubah koma Arab (،) di U+060C menjadi koma Jawi.
  - Kebanyakan pengguna tulisan Jawi digital menggunakan U+060C untuk koma kerana itulah yang ada pada kebanyakan papan kekunci walaupun ia bukanlah aksara sebenar untuk koma Jawi, kerana ia belum wujud dalam Unicode.
  - Dalam sesetengah aturcara dan fon, koma Jawi dipaparkan di tempat koma Arab apabila aturcara tersebut memberitahu fon bahawa bahasa yang digunakan pada tulisan yang dinyatakan merupakan bahasa Melayu, namun tidak semua aturcara atau fon menyokong fungsi ini.
    - Fon yang diketahui menyokong fungsi ini ialah Calibri dan Amiri.
    - Aturcara yang diketahui menyokong fungsi ini ialah Microsoft Office dan LibreOffice 6.1+, dengan sokongan terhad di GIMP.
  - Dalam tulisan tangan dunia nyata, semua pengguna Jawi menulis koma dengan cara yang betul, dan ianya lain daripada koma Arab.
  - Fon yang disunting mengubah fungsi ini agar glif yang dipaparkan secara lalainya ialah koma Jawi, dan koma Arab hanya dipaparkan jika bahasa ditetapkan kepada bahasa Arab. Ini membuatkannya paparkan koma Jawi secara lalai apabila tiada bahasa dinyatakan, berguna untuk aturcara lama untuk paparkan Jawi.
  - Koma Jawi kelihatan seperti ini: <br /> ![jawicomma](img/github/jawicomma.png).
- Halakan glif Koma Cermin (⹁) di U+2E41 kepada Koma Arab di U+060C selepas perubahan glif di situ daripada koma Arab kepada koma Jawi.
  - Sebilangan kecil pengguna menggunakan U+2E41 untuk koma kerana ia kelihatan lebih serupa dengan koma Jawi berbanding U+060C, tetapi aksara tersebut berada di luar bongkah tulisan Arab membuatkan sesetengah aturcara rosak.
- Mengubah koma bertitik Arab (؛) di U+061B kepada koma bertitik Jawi.
  - Kebanyakan pengguna tulisan Jawi digital menggunakan U+061B untuk koma bertitik kerana itulah yang ada pada kebanyakan papan kekunci walaupun ia bukanlah aksara sebenar untuk koma bertitik Jawi, kerana ia belum wujud dalam Unicode.
  - Dalam sesetengah aturcara dan fon, koma bertitik Jawi dipaparkan di tempat koma bertitik Arab apabila aturcara tersebut memberitahu fon bahawa bahasa yang digunakan pada tulisan yang dinyatakan merupakan bahasa Melayu, namun tidak semua aturcara atau fon menyokong fungsi ini.
    - Fon yang diketahui menyokong fungsi ini ialah Calibri dan Amiri.
    - Aturcara yang diketahui menyokong fungsi ini ialah Microsoft Office dan LibreOffice 6.1+, dengan sokongan terhad di GIMP.
  - Dalam tulisan tangan dunia nyata, semua pengguna Jawi menulis koma bertitik dengan cara yang betul, dan ianya lain daripada koma bertitik Arab.
  - Fon yang disunting mengubah fungsi ini agar glif yang dipaparkan secara lalainya ialah koma bertitik Jawi, dan koma bertitik Arab hanya dipaparkan jika bahasa ditetapkan kepada bahasa Arab. Ini membuatkannya paparkan koma bertitik Jawi secara lalai apabila tiada bahasa dinyatakan, berguna untuk aturcara lama untuk paparkan Jawi.
  - Koma bertitik Jawi kelihatan seperti ini:<br /> ![jawisemicolon](img/github/jawisemicolon.png).
- Halakan glif Koma Bertitik Cermin (⁏) di U+2E41 kepada Koma Bertitik Arab di U+060C selepas perubahan glif di situ daripada koma bertitik Arab kepada koma bertitik Jawi.
  - Sebilangan kecil pengguna menggunakan U+204F untuk koma bertitik kerana ia kelihatan lebih serupa dengan koma bertitik Jawi berbanding U+061B, tetapi aksara tersebut berada di luar bongkah tulisan Arab membuatkan sesetengah aturcara rosak.
- Tambah glif untuk huruf Jawi NGA (ڠ) di U+06A0, dikenali dalam Unicode sebagai Arabic Letter Ain with Three Dots Above, digunakan dalam bahasa Melayu untuk bunyi /ŋ/.
- Tambah glif untuk huruf Jawi GA (ݢ) di U+0762, dikenali dalam Unicode sebagai Arabic Letter Keheh with Dot Above, digunakan dalam bahasa Melayu untuk bunyi /g/.
- Tambah glif untuk huruf Jawi VA (ۏ) di U+06CF, dikenali dalam Unicode sebagai Arabic Letter Waw with Dot Above, digunakan dalam bahasa Melayu untuk bunyi /v/.
- Tambah glif untuk huruf Jawi NYA (ڽ) di U+06BD, dikenali dalam Unicode sebagai Arabic Letter Noon with Three Dots Above, digunakan dalam bahasa Melayu untuk bunyi /ɲ/.
- Mengubah glif untuk Hamzah Arab (ء) di U+0621 menjadi huruf Jawi Hamzah Tiga Suku.
  - Kebanyakan pengguna digital tulisan Jawi menggunakan U+0621 untuk hamzah tiga suku kerana itulah yang ada pada kebanyakan papan kekunci walaupun ia bukanlah aksara sebenar untuk huruf Jawi hamzah tiga suku, yang tidak wujud dalam Unicode.
  - Kedudukan tiga suku tersebut kadang-kadang dibuat-buat dengan meletakkan U+0621 dalam keadaan superskrip, tetapi ia hanya boleh dilakukan pada aturcara yang mampu menyuperskripkan huruf bukan-superskrip. Kedudukannya juga kadang-kadang lebih tinggi daripada jangkaan dan kelihatan kecil saiznya daripada biasa apabila disuperskripkan, yang mana ianya lain daripada apa yang kita gunakan dalam bahasa Melayu.
  - Hamzah tiga suku Jawi tidak disokong dalam mana-mana fon yang diketahui.
  - Dalam tulisan tangan dunia nyata, semua pengguna Jawi menulis hamzah tiga suku dengan cara yang betul, dan ianya lain daripada koma bertitik Arab.
  - Fon yang disunting mengubah fungsi ini agar glif yang dipaparkan secara lalainya ialah huruf Jawi hamzah tiga suku, dan hamzah Arab hanya dipaparkan jika bahasa ditetapkan kepada bahasa Arab. Ini membuatkannya paparkan huruf Jawi hamzah tiga suku secara lalai apabila tiada bahasa dinyatakan, berguna untuk aturcara lama untuk paparkan Jawi.
  - Hamzah tiga suku Jawi kelihatan seperti ini:<br /> ![jawi¾hamzah](img/github/jawi¾hamzah.png).
- Halakan glif hamzah Arabic tinggi (ٴ) di U+0674 kepada Hamzah Arab di U+0621 selepas perubahan glif di situ daripada hamzah Arab kepada hamzah tiga suku Jawi.
  - Sebilangan kecil pengguna menggunakan U+0674 untuk hamzah tiga suku kerana ia kelihatan lebih serupa dengan hamzah Jawi berbanding U+0621, tetapi aksara tersebut sepatutnya menjadi sebahagian daripada diftong dan diletakkan bersama-sama huruf lain dalam bahasa yang lain, tidak seperti Jawi di mana hamzah tiga suku merupakan hurufnya sendiri.
- Tambah glif untuk huruf Jawi lama GA (ڬ) di U+06AC, dikenali dalam Unicode sebagai Arabic Letter Kaf with Dot Above, dahulunya digunakan dalam bahasa Melayu untuk bunyi /g/ apabila Arabic Letter Keheh with Dot Above (ݢ) di U+0762 tidak boleh dimasukkan dengan papan kekunci.
  - Glif disertakan untuk kegunaan keserasian
  - Dalam tulisan tangan dunia nyata, ڬ tidak pernah digunakan dalam tulisan lama, dan ia tidak digunakan melainkan untuk tujuan penggayaan dalan penulisan baharu atau tersalahguna oleh orang ramai yang mempelajari Jawi menggunakan alatan digital yang dicipta pada zaman di mana aksara ݢ tidak dapat dimasukkan menggunakan papan kekunci, ia mestilah sentiasa ditulis sebagai ݢ dalam penulisan sebenar.
  - ڬ tidak dikenali secara formalnya sebagai sebuah huruf dalam bahasa Melayu.
- Tambah glif untuk Tilde Jawi (~) di U+007E, dikenali dalam Unicode sebagai Tilde, digunakan dalam bahasa Melayu untuk melambangkan bunyi panjang atau bertindak sebagai penanda penggantian.
  - Untuk pastikan ia masih berfungsi sebagai tilde yang biasa di luar Jawi, hanya variasi atau penggabung yang akan ditambah dan bukannya menggantikan keseluruhan glif tersebut.
  - Sekiranya ada huruf Jawi sebelum atau selepas tanda tilde, tilde Jawi akan dipaparkan. Jika tidak, tilde biasa akan dipaparkan.

Sesetengah fon-fon Arab mempunyai liputan glif yang kurang dan lebih banyak kerja perlu dibuat termasuklah:

- Tambah glif untuk huruf Jawi CA (چ) di U+0686, dikenali dalam Unicode sebagai Arabic Letter Tcheh, digunakan dalam bahasa Melayu untuk bunyi /t͡ʃ/.
- Tambah glif untuk huruf Jawi PA (ڤ) di U+06A4, dikenali dalam Unicode sebagai Arabic Letter Veh, digunakan dalam bahasa Melayu untuk bunyi /p/.
- Tambah glif untuk huruf Jawi KAF (ک) di U+06A9, dikenali dalam Unicode sebagai Arabic Letter Keheh, digunakan dalam bahasa Melayu untuk bunyi /k/.
- Tambah glif untuk huruf Jawi YE (ى) di U+0649, dikenali dalam Unicode sebagai Arabic Letter Alef Maksura, digunakan dalam bahasa Melayu untuk bunyi akhiran /ə/.
- Tambah glif untuk huruf Jawi Alif Berhamzah (أ) di U+0623, dikenali dalam Unicode sebagai Arabic Letter Alef with Hamza Above, digunakan sebagai sebahagian daripada diftong yang tidak boleh digunakan bersama-sama hamzah tiga suku mahupun tanpa sebarang hamzah. Contoh: أيمن (aiman) lain daripada اءيمن (a'iman) dan ايمن (iman).
  - Lihat versi imej di bawah <br/> ![aiman](img/github/aiman.png)
- Tambah glif untuk Tanda Petik
Pembuka Jawi (”) di U+201D, dikenali dalam Unicode sebagai Right Double Quotation Mark.
- Tambah glif untuk Tanda Petik Penutup Jawi (‟) di U+201F, dikenali dalam Unicode sebagai Double High-Reversed-9 Quotation Mark.
- Tambah glif untuk Koma Atas Terbalik Jawi (’) di U+2019, dikenali dalam Unicode sebagai Right Single Quotation Mark.
- Tambah glif untuk Koma Atas Jawi (‛) di U+201B, dikenali dalam Unicode sebagai Single High-Reversed-9 Quotation Mark.

Untuk tujuan keserasian, beberapa lagi glif turut akan diperiksa dan ditambah jika tidak wujud:

- Tambah glif untuk huruf bukan Jawi dikenali dalam Unicode sebagai Arabic Letter Yeh with Hamza Above (ئ) di U+0626.
  - Glif ditambah untuk tujuan keserasian.
  - Ia pernah digunakan dalam Jawi lama sebagai diftong /ai/ dan /ae/ (kedua-duanya kini ditulis sebagai أي), dan bunyi /iʔ/ dan /eʔ/ (kedua-duanya kini ditulis sebagai يء).
  - Masih digunakan sebagai sebahagian daripada nama keluarga Melayu iaitu Nik (نئ) seperti [Nik Abdul Aziz](https://ms.wikipedia.org/wiki/Nik_Abdul_Aziz_bin_Nik_Mat) (نئ عبدالعزيز).
- Tambah glif untuk huruf bukan Jawi dikenali dalam Unicode sebagai Arabic Letter Waw with Hamza Above (ؤ) di U+0624.
  - Glif ditambah untuk tujuan keserasian.
  - Ia pernah digunakan dalam Jawi lama sebagai diftong /ao/ dan /au/ (kedua-duanya kini ditulis sebagai أو) dan bunyi /uʔ/ dan /oʔ/ (kedua-duanya kini ditulis sebagai وء).
- Tambah glif untuk huruf bukan Jawi dikenali dalam Unicode sebagai Arabic Letter Dul (ڎ) di U+068E.
  - Glif ditambah untuk tujuan keserasian.
  - Pernah digunakan di sesetengah kawasan untuk menulis perkataan bahasa Sunda dan bahasa Jawa dalam bahasa Melayu.
  - Dieja sebagai DH dalam Rumi, bunyi macam /ɖʱ/.
  - Ketika ini digunakan dalam tulisan Pegon di Indonesia dengan nama Dha, tulisan Pegon diasaskan daripada tulisan Jawi.
- Tambah glif untuk huruf bukan Jawi dikenali dalam Unicode sebagai Arabic Letter Tah with Three Dots Above (ڟ) di U+069F.
  - Glif ditambah untuk tujuan keserasian.
  - Pernah digunakan di sesetengah kawasan untuk menulis perkataan bahasa Sunda dan bahasa Jawa dalam bahasa Melayu.
  - Dieja sebagai TH dalam Rumi, bunyi macam /tʰ/.
  - Ketika ini digunakan dalam tulisan Pegon di Indonesia dengan nama Tha, tulisan Pegon diasaskan daripada tulisan Jawi.
- Tambah glif untuk huruf bukan Jawi dikenali dalam Unicode sebagai Arabic Letter Kaf with Dot Below (ࢴ) di U+08B4.
  - Glif ditambah untuk tujuan keserasian.
  - Pernah digunakan di sesetengah kawasan untuk mengeja perkataan bahasa Sunda dan bahasa Jawa yang mempunyai huruf G dalam bahasa Melayu.
  - Dieja sebagai G dalam Rumi, bunyi macam /g/.
  - Ketika ini digunakan dalam tulisan Pegon di Indonesia dengan nama Gaf, tulisan Pegon diasaskan daripada tulisan Jawi.
  - untuk pengguna Jawi, sila gunakan huruf yang betul iaitu Ga di U+0762 (ݢ) dan bukannya yang ini.
- Tambah glif untuk tanda bacaan bukan Jawi dikenali dalam Unicode sebagai Reversed Tilde (∽) di U+223D.
  - Glif ditambah untuk tujuan keserasian.
  - Sebilangan kecil orang ramai menggunakan U+223D untuk tilde kerana ia kelihatan lebih serupa dengan tilde Jawi berbanding dengan U+007E, tetapi aksara ini sepatutnya sebahagian daripada operasi matematik dan bukannya tanda bacaan.
  - U+007E akan mempunyai glif daripada U+223D sebagai variasi dan penggabung supaya ia dipaparkan dengan betul apabila digunakan dalam tulisan Jawi.

Semua huruf lain sepatutnya sudah wujud dalam fon-fon Arab biasa, termasuk sebuah huruf terkecam:
- Huruf Jawi Lama KAF (ك) di U+0643, dikenali dalam Unicode sebagai Arabic Letter Kaf, dahulunya digunakan dalam bahasa Melayu untuk bunyi /k/ apabila huruf Arabic Letter Keheh (ک) di U+06A9 tidak dapat dimasukkan dengan papan kekunci
  - Glif disertakan untuk kegunaan keserasian
  - Dalam tulisan tangan dunia nyata, ك tidak pernah digunakan dalam tulisan lama, dan ia tidak digunakan melainkan untuk tujuan penggayaan dalan penulisan baharu atau tersalahguna oleh orang ramai yang mempelajari Jawi menggunakan alatan digital yang dicipta pada zaman di mana aksara ک tidak dapat dimasukkan menggunakan papan kekunci, ia mestilah sentiasa ditulis sebagai ک dalam penulisan sebenar.
  - ك tidak dikenali secara formalnya sebagai sebuah huruf dalam bahasa Melayu.
  - ك dipanggil sebagai huruf Kaf Arab oleh orang Melayu, dan bukannya huruf Kaf, kerana huruf Kaf dalam bahasa Melayu hanyalah ک.

Saya juga menambah sokongan untuk tulisan Pegon, periksa jadual terakhir dalam senarai penuh jadual-jadual.

Senarai penuh jadual-jadual boleh dibaca di [sini](https://jawi.mnh48.moe/jawifont/ms/jawitable.html)


## Apakah lesennya?

Kesemua fail fon yang disunting dan fail FontForge yang dijana dilesenkan sama seperti fail fon asal, lihat direktori fon untuk lesen sebenar.

Tema laman web buat sementara waktu ini ialah [Midnight](https://github.com/mattgraham/midnight) oleh [mattgraham](https://twitter.com/mattgraham) yang boleh didapati bawah lesen MIT.

Kesemua kandungan lain dalam repositori ini dan laman web yang dijana daripada repositori ini diterbitkan di bawah lesen MIT.

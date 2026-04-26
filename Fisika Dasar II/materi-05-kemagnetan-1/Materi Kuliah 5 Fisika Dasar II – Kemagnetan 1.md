# BAB 1: Kemagnetan

Dokumen ini merangkum dan menjelaskan isi dari presentasi mengenai dasar-dasar magnetisme, mulai dari sejarah hingga aplikasi teknologinya.

## 1. Pendahuluan Magnetisme

- **Sejarah:** Efek magnetik sudah dikenal lebih dari 2500 tahun yang lalu oleh bangsa Yunani.
- **Etimologi:** Nama "magnet" berasal dari **Magnesia**, sebuah distrik di Yunani Utara tempat ditemukannya batu magnet (oksida besi).
- **Sifat Dasar:**
	- Dapat menarik besi.
	- Jika digantung bebas, akan selalu menunjuk arah Utara-Selatan (sebagai detektor medan magnet bumi).

> **Magnesia** ([bahasa Yunani](https://id.wikipedia.org/wiki/Bahasa_Yunani "Bahasa Yunani"): Μαγνησία, _Magnisía_, IPA: [maɣniˈsia](https://id.wikipedia.org/wiki/Wikipedia:IPA_untuk_bahasa_Yunani) " Wikipedia:IPA untuk bahasa Yunani")), dari nama suku _[Magnetes](https://id.wikipedia.org/wiki/Magnetes?action=edit&redlink=1 "Magnetes (halaman belum tersedia)")_, adalah salah satu [unit periferal di Yunani](https://id.wikipedia.org/wiki/Unit_periferal_di_Yunani?action=edit&redlink=1 "Unit periferal di Yunani (halaman belum tersedia)"). Magnesia adalah bagian dari [periferi](https://id.wikipedia.org/wiki/Periferi_di_Yunani "Periferi di Yunani") [Thessalia](https://id.wikipedia.org/wiki/Thessalia "Thessalia"). Ibu kotanya adalah [Volos](https://id.wikipedia.org/wiki/Volos "Volos"). Sekitar 70% penduduk Magnesia tinggal di daerah Volos Besar, yang merupakan kota terbesar kedua di Thessalia dan merupakan pelabuhan dagang tersibuk ketiga di Yunani.

## 2. Magnet Batang & Kutub

- **Kutub Magnet:** Setiap magnet batang memiliki dua kutub, yaitu **Utara (N)** dan **Selatan (S)**.
- **Hukum Gaya:** Kutub yang senama akan tolak-menolak, sedangkan kutub yang tidak senama akan tarik-menarik.
- **Garis Medan Magnet:**
	- Didefinisikan mirip dengan medan listrik (berdasarkan arah dan kerapatannya).
- **Analogi Elektrostatis:** Pola garis medan magnet pada magnet batang sangat mirip dengan pola garis medan listrik pada sebuah **Dipole Elektrik** (muatan positif dan negatif yang berdekatan).

![Garis medan magnet batang.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773625709208.png)

> Since the magnet is dipolar, the magnetic lines must be originated and also have an end. Therefore, it starts from the north pole and terminates at the south pole outside the bar magnet, and it moves from the south pole to the north pole inside the magnet.
>
> The closeness of field lines shows the relative strength of the magnetic field, i.e. closer lines show a stronger magnetic field and vice—versa. Crowded field lines near the poles of the magnet show more strength.
> Sumber: [Geeksforgeeks](https://www.geeksforgeeks.org/physics/magnetic-field-due-to-current-carrying-conductor/)

## 3. Monopole Magnetik

- **Konsep:** Apakah muatan magnetik tunggal (monopole) itu ada?
- **Eksperimen:** Jika sebuah magnet batang dipotong menjadi dua, kita tidak mendapatkan kutub utara saja atau selatan saja, melainkan dua magnet baru yang masing-masing tetap memiliki kutub N dan S.
- **Kesimpulan Hukum Gauss:** Hingga saat ini, monopole magnetik tidak pernah ditemukan. Secara matematis dinyatakan dengan $\oint \vec{B} \cdot d\vec{S} = 0$, yang berarti fluks magnetik total yang keluar dari suatu permukaan tertutup adalah nol.

![Ilustrasi dipole magnetik.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773625980665.png)

Sumber: [SPlug](http://www.splung.com/fields/magnetism.htm)

## 4. Sumber Medan Magnet

- Jika tidak ada muatan magnetik (monopole), dari mana asal medan magnet?
- **Jawaban:** Sumbernya adalah **muatan listrik yang bergerak** (arus listrik).
- **Skala Atom:** Pada tingkat atom, elektron yang mengorbit inti atom bertindak seperti loop arus kecil yang menghasilkan medan magnet. Ini menjelaskan mengapa benda padat bisa memiliki sifat magnet meskipun tidak dihubungkan ke baterai.

![Medan magnet tercipta disekitar kawat listrik berarus.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773626935038.png)

![Electron spin up and down.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773626161114.png)

## 5. Klasifikasi Bahan Magnetik

Bahan dikelompokkan berdasarkan responnya terhadap medan magnet luar ($B_{app}$):

1. **Paramagnetik (Contoh: Aluminium, Oksigen):** Dipol atom cenderung sejajar dengan medan luar, namun efeknya sangat lemah karena acakan gerakan termal.
2. **Diamagnetik (Contoh: Emas, Tembaga, Air):** Menghasilkan medan magnet yang berlawanan dengan medan luar (lemah). _Catatan khusus: Superkonduktor adalah diamagnetik sempurna._
3. **Ferromagnetik (Contoh: Besi, Nikel, Kobalt):** Memiliki interaksi kuat antar atom sehingga dipol-dipolnya berbaris searah secara kolektif. Menghasilkan penguatan medan magnet yang sangat besar ($10^5$ kali lipat).

![Ilustrasi bahan magnetik.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773626357205.png)

## 6. Domain Magnetik & Sifat Ferromagnet

- **Domain:** Area kecil dalam bahan ferromagnetik di mana dipol-dipol magnet sudah searah meskipun belum diberi medan luar.
- **Jenis Ferromagnet:**
	- _"Soft" (Lunak):_ Domain mudah teracak kembali jika medan luar dihilangkan.
	- _"Hard" (Keras):_ Domain tetap searah meskipun medan luar dihilangkan (menjadi magnet permanen).
- **Kerusakan Magnet:** Sifat magnetik dapat hilang akibat guncangan fisik yang keras atau dipanaskan di atas **Titik Curie** (untuk besi sekitar $770^\circ \text{C}$).

![Magnetic domains.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773626452273.png)

## 7. Aplikasi Sejarah: Hard Disk IBM

- **Hard Disk Pertama (1957):** Teknologi penyimpanan data menggunakan prinsip kemagnetan dimulai secara komersial oleh IBM.
- **Spesifikasi:** Terdiri dari 50 piringan berdiameter 24 inci, ukurannya sebesar dua kulkas, namun kapasitasnya hanya **5 MB**.
- **Fakta Menarik:** Biaya sewanya mencapai $35.000 per tahun pada masa itu, menunjukkan betapa berharganya teknologi penyimpanan magnetik di awal perkembangannya.

![IBM Harddisk](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773631290189.png)

# BAB 2: Medan Magnet & Gaya Lorentz

Materi ini membahas interaksi antara medan magnet dengan muatan listrik yang bergerak, yang merupakan dasar dari banyak teknologi modern.

## 1. Interaksi Medan Magnet dengan Muatan

Berbeda dengan medan listrik yang bisa dirasakan oleh muatan diam, medan magnet hanya memberikan gaya pada **muatan yang sedang bergerak**.

**Observasi Eksperimental:**

1. Besarnya gaya magnet ($F_{mag}$) sebanding dengan kecepatan ($v$) muatan $q$.
2. Arah gaya magnet selalu tegak lurus ($\perp$) terhadap arah kecepatan muatan.
3. Arah gaya magnet juga tegak lurus ($\perp$) terhadap arah vektor medan magnet ($B$).

## 2. Hukum Gaya Lorentz

Gaya total yang dialami muatan dalam ruang yang memiliki medan listrik ($E$) dan medan magnet ($B$) disebut **Gaya Lorentz**.

- **Persamaan:** $\vec{F} = q\vec{E} + q(\vec{v} \times \vec{B})$.
- **Poin Penting:** Bagian magnetik dari gaya ini menggunakan _cross product_ (perkalian silang). Artinya, jika muatan bergerak **sejajar** dengan arah medan magnet ($\vec{v} \parallel \vec{B}$), maka gaya magnetnya adalah **nol** ($F = 0$).

![Kaidah tangan kanan.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773627397742.png)

Sumber: <https://en.wikipedia.org/wiki/Lorentz_force>

## 3. Gerak Melingkar dalam Medan Magnet

Ketika muatan masuk ke dalam medan magnet konstan secara tegak lurus, gaya magnet yang dihasilkan akan selalu tegak lurus terhadap arah gerak. Sifat ini identik dengan gaya sentripetal.

- **Lintasan:** Karena gaya selalu menarik muatan ke arah pusat secara tegak lurus dari kecepatannya, muatan tersebut akan bergerak dalam lintasan **lingkaran**.
- **Penurunan Rumus Radius (**$R$**):**

	Menggunakan Hukum II Newton ($F = m \cdot a$):

	$$qvB = m \frac{v^2}{R}$$

	Maka diperoleh jari-jari lintasan:

	$$R = \frac{mv}{qB}$$

- **Makna:** Semakin besar massa atau kecepatan, lingkaran semakin besar. Semakin kuat medan magnet atau muatan, lingkaran semakin kecil.

## 4. Eksperimen Rasio $q/m$ Elektron

Slide ini menunjukkan aplikasi praktis dari rumus radius di atas untuk menentukan nilai fisik elektron.

- **Langkah Eksperimen:**
	
	1. Elektron dipercepat menggunakan tegangan $V$ (pistol elektron): $\frac{1}{2}mv^2 = qV$.
	2. Elektron masuk ke medan magnet $B$ dan membentuk lingkaran berjari-jari $R$.
	3. Dengan menggabungkan kedua persamaan tersebut, kita bisa menghitung rasio muatan terhadap massa ($\frac{q}{m}$):

		$$\frac{q}{m} = \frac{2V}{R^2 B^2}$$

- **Hasil:** Eksperimen menunjukkan nilai $\approx 1.8 \times 10^{11} \text{ C/kg}$, sangat dekat dengan nilai standar literatur ($1.76 \times 10^{11} \text{ C/kg}$).

## 5. Torsi dan Dipol Magnetik

Jika muatan bergerak dalam sebuah simpal (loop) tertutup, muatan tersebut memiliki **Momen Dipol Magnetik** ($\mu$).

- **Definisi:** $\mu = A \cdot I$ (Luas loop dikali Arus).
- **Interaksi:**
	- **Torsi (**$\tau$**):** Medan magnet akan mencoba memutar loop tersebut agar sejajar dengan medan ($\vec{\tau} = \vec{\mu} \times \vec{B}$).
	- **Energi Potensial (**$U$**):** Energi yang tersimpan berdasarkan orientasi dipol ($U = -\vec{\mu} \cdot \vec{B}$).
- **Aplikasi:**
	- **Riset Otak:** Digunakan dalam MEG (_Magnetoencephalography_) untuk mendeteksi arus listrik lemah di otak melalui medan magnet yang dihasilkan.
	- **Stasiun Luar Angkasa:** Interaksi dipol magnetik dengan medan magnet bumi dapat digunakan untuk membantu orientasi atau stabilisasi satelit.

# BAB 3: Spektrometer Massa dan Deteksi Partikel

Setelah memahami bagaimana muatan bergerak dalam medan magnet, sekarang kita akan melihat bagaimana ilmuwan menggunakan prinsip tersebut untuk "menimbang" atom dan menemukan partikel baru.

## 1. Spektrometer Massa: Menimbang Atom

Spektrometer massa adalah alat yang digunakan untuk mengidentifikasi suatu zat dengan cara mengukur rasio massa terhadap muatan ($m/q$). Bayangkan ini sebagai sebuah timbangan yang bekerja di skala atom.

![Ilustrasi spektrometer massa.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773627674094.png)

"Bayangkan Anda memiliki campuran atom dan ingin tahu apa saja isinya. Spektrometer massa adalah solusinya. Prosesnya terdiri dari tiga langkah utama:

1. **Ionisasi:** Atom netral ditembak dengan elektron agar melepaskan elektronnya sendiri, mengubahnya menjadi ion positif ($q = |e|$).
2. **Percepatan:** Ion-ion ini kemudian dipercepat menggunakan beda potensial listrik ($V$). Di sini, energi listrik diubah menjadi energi kinetik.
3. **Pembelokan:** Ion yang sudah meluncur cepat masuk ke daerah medan magnet ($B$). Di sinilah keajaiban fisika terjadi. Karena gaya Lorentz, ion akan berbelok. Ion yang **lebih ringan** akan dibelokkan lebih tajam (jari-jari kecil), sedangkan ion yang **lebih berat** akan lebih sulit dibelokkan (jari-jari besar)."

## 2. Analisis Data dan Aplikasi Luar Biasa

"Hasil dari alat ini adalah grafik 'Mass Spectrum'. Setiap puncak pada grafik mewakili massa tertentu dari atom atau molekul yang ada dalam sampel. Teknologi ini bukan hanya untuk di laboratorium kimia saja, aplikasinya sangat luas:

- **Paleoseanografi:** Ilmuwan menggunakannya untuk menghitung isotop guna menentukan usia geologis bumi atau fosil.
- **Eksplorasi Ruang Angkasa:** Robot penjelajah di Mars atau Bulan membawa alat ini untuk mencari tahu komposisi tanah dan atmosfer di sana.
- **Keamanan Nasional:** Digunakan untuk mendeteksi jejak senjata kimia, biologi, atau gas saraf di bandara atau area publik. Ini adalah alat pendeteksi yang sangat sensitif."

## 3. Fisika Partikel Modern

Prinsip pembelokan dalam medan magnet juga digunakan di akselerator partikel raksasa (seperti CERN) untuk mempelajari partikel fundamental.

"Terakhir, kita melihat bagaimana prinsip sederhana $R = mv/qB$ digunakan dalam eksperimen fisika partikel modern. Di dalam detektor partikel, kita sengaja memasang medan magnet yang sangat kuat.

Ketika partikel hasil tabrakan atom meluncur keluar, mereka akan meninggalkan jejak berupa garis lengkung. Dengan melihat **arah lengkungannya**, kita tahu apakah partikel itu bermuatan positif (seperti positron $e^+$) atau negatif (seperti elektron $e^-$). Dengan mengukur **jari-jari kelengkungannya**, kita bisa menghitung momentum dan energi partikel tersebut.

Secara harfiah, medan magnet memungkinkan kita 'melihat' dan mengukur identitas partikel yang bahkan tidak bisa dilihat oleh mikroskop paling canggih sekalipun."

> Sebagai kesimpulan dari seluruh rangkaian materi ini, kita telah belajar bahwa magnetisme bukan sekadar tentang tempelan kulkas. Dari sejarah kuno di Yunani, hingga deteksi partikel subatomik dan identifikasi zat di planet Mars, kemagnetan adalah kunci utama manusia dalam memahami alam semesta pada level yang paling fundamental.

# BAB 4: Gaya Magnetik pada Arus & Torsi Loop

Bagian ini menjelaskan bagaimana medan magnet berinteraksi dengan kawat berarus listrik dan bagaimana interaksi tersebut menghasilkan torsi (putaran), yang merupakan prinsip dasar motor listrik.

![Ilustrasi kawat berarus dan medan magnet (Wikipedia).](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773627845169.png)

## 1. Gaya Magnetik pada Kawat Berarus

Jika sebelumnya kita mempelajari gaya pada satu muatan ($F = qv \times B$), di sini kita melihat gaya total pada seluruh muatan yang mengalir dalam kawat.

- **Derivasi:** Gaya total ($dF$) pada potongan kawat ($dl$) adalah jumlah gaya dari semua muatan ($n$) di dalamnya.
- **Rumus Utama:**

	$$\vec{F} = I\vec{L} \times \vec{B}$$

- **Artinya:** Gaya magnetik sebanding dengan arus ($I$), panjang kawat ($L$), dan kuat medan magnet ($B$). Arahnya ditentukan dengan kaidah tangan kanan.

## 2. Gaya pada Loop Arus

Apa yang terjadi jika kawat berbentuk kotak (loop) diletakkan di medan magnet?

- **Gaya Total Nol:** Jika medan magnet seragam, gaya pada sisi atas akan membatalkan sisi bawah, dan sisi kiri membatalkan sisi kanan. Maka, loop tidak akan berpindah tempat (translasi).
- **Munculnya Torsi:** Meskipun tidak berpindah, jika bidang loop tidak tegak lurus terhadap medan, gaya-gaya tersebut akan menyebabkan loop **berputar**. Inilah yang disebut Torsi.

## 3. Perhitungan Torsi ($\tau$)

- **Rumus Torsi:**

	$$\tau = AIB \sin \theta$$

	(Di mana $A$ adalah luas loop, $I$ arus, $B$ medan magnet, dan $\theta$ sudut orientasi).

- **Momen Dipol Magnetik (**$\mu$**):** Untuk menyederhanakan, ilmuwan mendefinisikan $\mu = NAI$ (N = jumlah lilitan).
- **Persamaan Vektor:**

	$$\vec{\tau} = \vec{\mu} \times \vec{B}$$

- **Kaidah Tangan Kanan:** Arah $\mu$ adalah arah ibu jari ketika jari lain mengikuti arah aliran arus pada loop.

![Tampilan atas dari sebuah kumparan pembawa arus dalam medan magnet.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773629937838.png)

Tampilan atas dari sebuah kumparan pembawa arus dalam medan magnet, dengan:

- (a) Persamaan untuk torsi diturunkan menggunakan tampilan ini. Perhatikan bahwa garis tegak lurus terhadap kumparan membentuk sudut $\theta$ dengan medan yang sama dengan sudut antara $w/2$ dan $F$.
- (b) Torsi maksimum terjadi ketika $\theta$ adalah sudut siku-siku dan $\sin \theta = 1$.
- (c) Torsi nol (minimum) terjadi ketika $\theta$ adalah nol dan $\sin \theta = 0$.
- (d) Torsi berbalik arah setelah kumparan berputar melewati $\theta = 0$.

## 4. Analogi Magnet Batang

Sebuah loop arus kecil berperilaku persis seperti sebuah **magnet batang kecil**.

- Kutub Utara magnet batang setara dengan arah vektor momen dipol ($\mu$).
- Menambah jumlah lilitan atau memperbesar arus sama dengan membuat magnet batang yang lebih kuat.

![Ilustrasi analogi magnet batang dan loop arus kecil.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773630666093.png)

## 5. Aplikasi: Galvanometer

Galvanometer adalah alat dasar untuk voltmeter dan ammeter analog.

- **Cara Kerja:** Arus mengalir melalui loop di dalam medan magnet permanen. Loop tersebut mengalami torsi dan berputar. Putaran ini ditahan oleh sebuah **pegas (spring)**.
- **Kesetimbangan:** Jarum akan berhenti di angka tertentu ketika torsi magnetik tepat seimbang dengan gaya pegas. Semakin besar arus, semakin jauh jarum menyimpang.

![Prinsip Galvanometer.](attachments/Materi%20Kuliah%205%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%201-1773630893595.png)

## 6. Analogi dengan Listrik & Energi Potensial

Fisika memiliki simetri yang indah. Interaksi ini sangat mirip dengan dipol listrik:

- **Analogi:** Momen dipol listrik ($p$) berinteraksi dengan medan listrik ($E$) mirip dengan momen dipol magnetik ($\mu$) dengan medan magnet ($B$).
- **Energi Potensial (**$U$**):** Dibutuhkan usaha untuk memutar dipol dalam medan magnet.

	$$U = -\vec{\mu} \cdot \vec{B} = -\mu B \cos \theta$$

- **Kondisi Energi:**
	
	1. **Stabil (**$U = -\mu B$**):** Ketika $\mu$ searah dengan $B$. Ini adalah posisi alami yang diinginkan magnet.
	2. **Tidak Stabil (**$U = +\mu B$**):** Ketika $\mu$ berlawanan arah dengan $B$.
	3. **Nol (**$U = 0$**):** Ketika $\mu$ tegak lurus dengan $B$.

**Kesimpulan:** Prinsip bahwa "arus dalam medan magnet menghasilkan torsi" adalah alasan mengapa mesin cuci, kipas angin, dan mobil listrik bisa berputar. Semuanya berawal dari persamaan $\vec{\tau} = \vec{\mu} \times \vec{B}$.

# BAB 5: Hukum Biot-Savart & Perhitungan Medan Magnet

Materi ini membahas cara menghitung kuat medan magnet ($B$) yang dihasilkan oleh berbagai konfigurasi arus listrik, mulai dari kawat lurus hingga loop melingkar.

## 1. Analogi Listrik dan Magnet

Bagian ini membandingkan cara kita menghitung medan dalam elektrostatis dengan magnetisme untuk memudahkan pemahaman:

- **Medan Listrik:** Menggunakan Hukum Coulomb (untuk kasus umum) dan Hukum Gauss (untuk simetri tinggi).
- **Medan Magnet:** Menggunakan **Hukum Biot-Savart** (sebagai analogi Hukum Coulomb) dan **Hukum Ampere** (sebagai analogi Hukum Gauss).
- **Prinsip:** Biot-Savart digunakan untuk potongan kecil arus ($dl$), sedangkan Ampere menggunakan "Loop Amperian" untuk menghitung medan pada sistem yang sangat simetris.

## 2. Hukum Biot-Savart

- **Persamaan:** $d\vec{B} = \frac{\mu_{0}I}{4\pi} \frac{d\vec{l} \times \hat{r}}{r^{2}}$
- **Konstanta Permeabilitas (**$\mu_0$**):** $4\pi \times 10^{-7} \text{ N/A}^2$.
- **Kaidah Tangan Kanan:** Ibu jari menunjuk arah arus ($I$), dan empat jari melingkar menunjukkan arah sirkulasi medan magnet ($B$).

## 3. Medan B dari Kawat Lurus

Menggunakan integrasi Biot-Savart pada kawat yang sangat panjang:

- **Hasil Akhir:**

	$$B = \frac{\mu_{0}I}{2\pi R}$$

- **Karakteristik:** Medan magnet berbanding lurus dengan arus dan berbanding terbalik dengan jarak ($R$) dari kawat.
- **Unit:** Tesla ($T$). $1 \text{ Tesla} = 10^4 \text{ Gauss}$. Sebagai perbandingan, medan magnet bumi sangat lemah, hanya sekitar $0,5 \text{ Gauss}$.

## 4. Gaya Antar Dua Kawat Sejajar

Karena kawat berarus menghasilkan medan magnet, dan kawat berarus lainnya merasakan gaya dalam medan magnet, maka dua kawat sejajar akan saling berinteraksi:

- **Arus Searah:** Kawat akan saling **tarik-menarik**.
- **Arus Berlawanan:** Kawat akan saling **tolak-menolak**.
- **Rumus Gaya per Satuan Panjang:**

	$$F = \frac{\mu_{0} I_{a} I_{b} L}{2\pi d}$$

	(Di mana $d$ adalah jarak antar kawat). Ini adalah prinsip dasar yang digunakan secara historis untuk mendefinisikan satuan 1 Ampere.

## 5. Medan B pada Loop Melingkar

Menghitung medan magnet di titik $P$ yang berada pada sumbu pusat loop berjari-jari $R$:

- **Persamaan Umum:**

	$$B_{z} = \frac{\mu_{0} I R^{2}}{2(z^{2} + R^{2})^{3/2}}$$

- **Pada Titik Jauh (**$z \gg R$**):** Medan meluruh sesuai dengan $1/z^{3}$.
- **Analogi Dipol:** Pola peluruhan $1/z^{3}$ ini merupakan ciri khas dari **dipol**, menunjukkan bahwa loop arus kecil memiliki karakteristik medan yang sama dengan magnet batang atau dipol listrik.

## 6. Aplikasi Praktis: Pengeras Suara (Loudspeaker)

Slide terakhir menunjukkan bagaimana prinsip-prinsip ini bekerja di dalam _speaker_:

1. **Sinyal Elektrik:** Arus listrik yang berubah-ubah (sinyal suara) dikirim ke kumparan (coil).
2. **Interaksi Magnetik:** Kumparan berada di depan magnet permanen. Karena ada arus dalam medan magnet, muncul gaya Lorentz yang berubah-ubah arahnya.
3. **Vibrasi:** Gaya ini menyebabkan kerucut (_cone_) bergetar maju-mundur, menggetarkan udara, dan menghasilkan gelombang suara yang kita dengar.

**Poin Kunci untuk Ujian:**

1. Hafalkan perbedaan arah gaya pada kawat sejajar (searah = tarik, berlawanan = tolak).
2. Pahami bahwa medan magnet kawat lurus meluruh terhadap $1/R$, sedangkan loop (dipol) meluruh terhadap $1/z^3$ pada jarak jauh.

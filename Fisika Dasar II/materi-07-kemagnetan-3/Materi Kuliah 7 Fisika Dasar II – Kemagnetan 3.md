# Bagian 1: Pengantar dan Aplikasi Dasar

Kita akan membahas topik yang sering kali dianggap abstrak, yaitu **Induktansi**. Jika sebelumnya kita telah belajar bagaimana arus listrik menghasilkan medan magnet, hari ini kita akan melihat bagaimana komponen bernama **Induktor** mampu "menyimpan" pengaruh tersebut dan bagaimana ia menjadi sangat vital dalam teknologi modern.

## 1.1. Mengubah Arus Menjadi Sinyal: Analogi Detektor Logam

Bayangkan Anda sedang berada di sebuah pantai, melihat seseorang membawa sebuah lingkaran kawat di ujung tongkat—sebuah detektor logam. Bagaimana alat itu bisa tahu ada koin emas di bawah pasir tanpa menyentuhnya?

Di sinilah peran **Induktansi**. Lingkaran kawat tersebut sebenarnya adalah sebuah kumparan (induktor). Saat arus listrik dialirkan melaluinya, ia menciptakan medan magnet. Jika di bawah tanah terdapat benda logam, keberadaan logam tersebut akan mengganggu distribusi medan magnet di sekitar kumparan.

Perubahan medan magnet ini menyebabkan nilai **induktansi** kumparan berubah. Perubahan kecil pada induktansi ini segera direspons oleh rangkaian elektronik sebagai perubahan arus, yang kemudian diubah menjadi sinyal suara (bip) di _earphone_ pencari harta karun tersebut. Dalam hal ini, induktansi bertindak sebagai "jembatan" yang menerjemahkan keberadaan benda fisik menjadi sinyal elektrik.

![Sketsa metal detector.](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774502510864.png)

## 1.2. Penjaga Stabilitas Listrik: Menjinakkan Petir

Aplikasi kedua jauh lebih besar skalanya. Pernahkah Anda membayangkan apa yang terjadi pada jaringan listrik kota ketika petir menyambar kabel transmisi tegangan tinggi? Petir adalah lonjakan arus listrik yang luar biasa besar dalam waktu yang sangat singkat ($\frac{di}{dt}$ yang sangat tinggi).

Jika lonjakan arus ini langsung masuk ke rumah-rumah, seluruh peralatan elektronik kita akan hancur seketika. Untuk mencegah hal ini, insinyur listrik memasang **induktor raksasa** pada sistem transmisi.

Sifat dasar induktor adalah **inersia elektrik**. Sama seperti benda berat yang sulit digerakkan tiba-tiba, induktor akan "melawan" setiap perubahan arus yang mendadak. Ketika petir menyambar, induktor tersebut akan menciptakan gaya gerak listrik (ggl) balik yang menahan lonjakan arus tersebut agar tidak merambat lebih jauh. Induktor berfungsi sebagai peredam kejut (_shock absorber_) bagi aliran listrik, memastikan bahwa energi dari petir tidak menghanguskan infrastruktur penting kita.

\newpage

# Bagian 2: Konsep Dasar Induktor dan Induktansi

- **Definisi Induktansi:** Induktor digunakan untuk menghasilkan medan magnet dari arus listrik ($L = \frac{N\Phi_B}{i}$) dengan satuan ukur Henry.
- **Induktansi Solenoida:** Besarnya induktansi berbanding lurus dengan kuadrat jumlah lilitan dan luas penampang, serta berbanding terbalik dengan panjang solenoida ($L = \mu_0\frac{N^2}{l}A$).
- **Induksi Diri:** Setiap perubahan arus pada kumparan akan menghasilkan gaya gerak listrik (ggl) induksi diri yang menentang arah perubahan arus tersebut ($\mathcal{E}_L = -L\frac{di}{dt}$).
- **Beda Potensial Induktor:** Beda potensial pada induktor bernilai nol jika arus konstan, berpotensial turun jika arus sedang meningkat, dan berpotensial naik jika arus menurun.

## Induktansi Solenoida

Sebuah kumparan kawat panjang (solenoida) dapat dihitung nilai induktansinya berdasarkan karakteristik fisiknya.

![Induktani solenoida.](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774502809004.png)

### 1. Karakteristik Fisik Solenoida

Jika sebuah solenoida dengan spesifikasi:

- $N$: Jumlah total lilitan kawat.
- $l$: Panjang total solenoida.
- $A$: Luas penampang dari setiap lilitan.
- **Asumsi**: Solenoida dianggap sangat panjang dibanding jari-jarinya dan intinya adalah udara (untuk menyederhanakan perhitungan).

### 2. Menghitung Fluks Magnetik ($\Phi_B$)

Maka sebelum mendapatkan nilai induktansi, kita harus tahu dulu berapa medan magnet ($B$) yang dihasilkan.

- Medan magnet di dalam solenoida ideal adalah $B = \mu_0 n i$, di mana $n$ adalah jumlah lilitan per satuan panjang ($n = N/l$).
- **Fluks Magnetik (**$\Phi_B$**)** melalui satu lilitan adalah hasil kali medan magnet ($B$) dengan luas penampang ($A$):

	$$\Phi_B = BA = \left(\mu_0 \frac{N}{l} i \right) A$$

### 3. Definisi Induktansi ($L$)

Induktansi adalah perbandingan antara total fluks magnetik yang menembus seluruh lilitan ($N\Phi_B$) dengan arus ($i$) yang mengalir.

$$L = \frac{N\Phi_B}{i}$$

### 4. Penurunan Rumus Akhir Induktansi

Jika kita substitusikan rumus fluks ($\Phi_B$) ke dalam definisi induktansi, kita akan mendapatkan:

$$L = \frac{N \times (\mu_0 \frac{N}{l} i A)}{i}$$

Arus ($i$) di pembilang dan penyebut saling meniadakan, sehingga menyisakan:

$$L = \mu_0 \frac{N^2}{l} A$$

### Poin Penting yang Harus Diperhatikan

- **Sifat Geometris**: Perhatikan bahwa nilai $L$ sama sekali tidak bergantung pada arus ($i$). Induktansi hanya bergantung pada **bentuk fisik** (jumlah lilitan, panjang, dan luas).
- **Kuadrat Lilitan (**$N^2$**)**: Ini adalah bagian paling krusial. Karena $N$ muncul sebagai kuadrat, jika Anda menggandakan jumlah lilitan pada panjang yang sama, induktansinya akan naik **empat kali lipat**.
- **Visualisasi**: Gambar di kanan menunjukkan bagaimana arus ($I$) yang mengalir menghasilkan medan magnet ($B$) yang terkonsentrasi di dalam kumparan, yang mendasari penyimpanan energi magnetik tersebut.

## Induksi Diri (_Self-Induction_)

Sebuah kumparan "melawan" dirinya sendiri ketika arus listrik di dalamnya berubah.

![Skema rangkaian percobaan induksi diri.](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774502990477.png)

### 1. Mekanisme Perubahan Arus

Pada diagram rangkaian, terlihat sebuah baterai dihubungkan dengan **resistor variabel (**$R$**)** dan **induktor (**$L$**)**.

- **Resistor Variabel:** Digunakan untuk mengubah nilai hambatan secara manual dengan menggeser kontak (tanda panah).
- **Proses:** Ketika kontak digeser, nilai hambatan $R$ berubah. Sesuai Hukum Ohm, perubahan $R$ akan menyebabkan nilai **arus (**$i$**)** yang mengalir dalam rangkaian ikut berubah.

### 2. Terjadinya GGL Induksi Sendiri ($\epsilon_L$)

Berdasarkan teks di slide: "Jika arus dalam kumparan diubah... ggl induksi sendiri $\epsilon_L$ akan muncul di kumparan."

- Ketika arus ($i$) berubah, medan magnet yang dihasilkan oleh kumparan juga berubah.
- Perubahan medan magnet ini menyebabkan perubahan fluks magnetik yang menembus kumparan itu sendiri.
- Menurut Hukum Faraday, perubahan fluks ini menghasilkan tegangan yang disebut **Gaya Gerak Listrik (GGL) Induksi Diri**.

### 3. Analisis Rumus

Slide menampilkan rumus fundamental:

$$\epsilon_L = -L \frac{di}{dt}$$

- $\epsilon_L$: Tegangan atau GGL yang dihasilkan oleh induktor.
- $L$: Induktansi diri (satuan Henry).
- $di/dt$: Laju perubahan arus terhadap waktu. Semakin cepat arus berubah, semakin besar tegangan yang dihasilkan.

### 4. Makna Tanda Minus (Hukum Lenz)

Poin terakhir di slide menekankan bahwa: "Tanda minus menunjukkan bahwa ggl... mempunyai orientasi yang **menentang** perubahan arus $i$."

- Ini adalah inti dari **Hukum Lenz**.
- **Jika arus meningkat:** Induktor akan menghasilkan ggl yang arahnya berlawanan dengan arus baterai (mencoba menahan kenaikan).
- **Jika arus menurun:** Induktor akan menghasilkan ggl yang arahnya searah dengan arus (mencoba mencegah penurunan).

### Kesimpulan Sederhana

Induktor bertindak seperti "inersia" dalam dunia listrik. Ia tidak menyukai perubahan. Slide ini menjelaskan bahwa setiap kali kita mencoba mengubah aliran listrik dalam kumparan, kumparan tersebut akan menciptakan tegangan sendiri untuk mempertahankan kondisi arus sebelumnya.

## Potensial Melintasi Induktor

Konsep beda potensial (tegangan) pada induktor dalam tiga kondisi arus yang berbeda: konstan, meningkat, dan menurun.

![Potensial melintasi induktor, untuk arus konstan, naik dan turun.](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774503313240.png)

### 1. Perbandingan Induktor vs Resistor

Fondasi dengan membandingkan induktor dengan resistor:

- **Pada Resistor (**$R$**):** Beda potensial ($V_{ab}$) murni bergantung pada besarnya arus yang mengalir. Berdasarkan Hukum Ohm, $V_{ab} = iR$. Selama ada arus, pasti ada tegangan.
- **Pada Induktor (**$L$**) dengan Arus Konstan:** Ini adalah poin krusial. Jika arus ($i$) yang mengalir dari titik $a$ ke $b$ bersifat **konstan** (tetap), maka laju perubahannya adalah nol ($di/dt = 0$). Karena tegangan induktor bergantung pada perubahan arus, maka:

	$$V_{ab} = L \frac{di}{dt} = 0$$

	**Kesimpulan:** Induktor yang dialiri arus DC stabil tidak memiliki beda potensial dan berfungsi seperti kawat penghantar biasa (_short circuit_).

### 2. Kondisi Arus Berubah

Apa yang terjadi jika arus tidak konstan. Di sinilah sifat "perlawanan" induktor muncul.

#### A. Arus Meningkat ($i$ increasing, $di/dt > 0$)

- **Kejadian:** Arus mengalir dari $a$ ke $b$ dan nilainya semakin besar.
- **Respon Induktor:** Sesuai Hukum Lenz, induktor menciptakan ggl ($\mathcal{E}$) yang arahnya berlawanan dengan arah arus untuk menahan kenaikan tersebut (lihat panah biru $\mathcal{E}$ yang mengarah ke kiri).
- **Hasilnya:** Potensial di titik $a$ menjadi lebih tinggi daripada di $b$. Terjadi penurunan potensial dari $a$ ke $b$.

	$$V_{ab} = L \frac{di}{dt} > 0$$

#### B. Arus Menurun ($i$ decreasing, $di/dt < 0$)

- **Kejadian:** Arus mengalir dari $a$ ke $b$ tetapi nilainya semakin kecil (misalnya saat sakelar baru dibuka).
- **Respon Induktor:** Induktor tidak ingin arus hilang. Ia menciptakan ggl ($\mathcal{E}$) yang searah dengan arus untuk mencoba mempertahankan aliran arus tersebut (panah biru $\mathcal{E}$ mengarah ke kanan).
- **Hasilnya:** Titik $b$ sekarang memiliki potensial yang lebih tinggi daripada $a$. Terjadi kenaikan potensial dari $a$ ke $b$.

	$$V_{ab} = L \frac{di}{dt} < 0$$

### Ringkasan Eksekutif untuk Mahasiswa

1. **Resistor** peduli pada **"Berapa besar arusnya?"** ($V \propto i$).
2. **Induktor** hanya peduli pada **"Seberapa cepat arus berubah?"** ($V \propto di/dt$).
3. Induktor akan menjadi **positif (+)** di sisi arus datang jika arus sedang naik, dan akan menjadi **negatif (-)** di sisi tersebut jika arus sedang turun.

\newpage

# Bagian 3: Energi dalam Medan Magnet

Dalam bab-bab sebelumnya, kita tahu bahwa resistor "memakan" energi dan mengubahnya menjadi panas (disipasi). Namun, induktor memiliki perilaku yang lebih mirip dengan kapasitor: ia adalah penyimpan energi. Jika kapasitor menyimpan energi dalam **medan listrik**, maka induktor menyimpannya dalam **medan magnet**.

![Energi yang tersimpan dalam induktor berupa medan magnet, sedangkan energi yang tersimpan di kapasitor adalah medan listrik](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774503479847.png)

## 3.1. Bagaimana Induktor Menyimpan Energi?

Ketika kita mulai mengalirkan arus pada sebuah induktor, muncul gaya gerak listrik (ggl) balik yang melawan aliran tersebut. Untuk menjaga arus tetap mengalir dan meningkat, sumber tegangan (baterai) harus melakukan kerja. Kerja yang dilakukan untuk melawan ggl induksi inilah yang kemudian "tertabung" sebagai energi potensial magnetik.

Secara matematis, energi ($U$) yang tersimpan dalam induktor dengan induktansi $L$ dan arus $I$ dirumuskan sebagai:

$$U = \frac{1}{2}LI^2$$

**Poin Penting untuk Diingat:**

Energi ini bersifat dinamis. Selama arus mengalir konstan, energi tetap tersimpan. Namun, begitu arus mencoba turun, induktor akan melepaskan kembali energi ini ke rangkaian untuk mempertahankan arus tersebut. Inilah alasan mengapa terjadi percikan api jika kita mencabut kabel perangkat yang memiliki induktor besar saat masih menyala; energi magnetik yang tersimpan "meledak" keluar seketika.

## 3.2. Kerapatan Energi Magnetik

Fisika juga tertarik pada "lokasi" energi tersebut. Untuk sebuah solenoida, kita bisa menghitung berapa banyak energi yang tersimpan per satuan volume ruang di dalamnya. Konsep ini disebut **Kerapatan Energi (**$u$**)**.

Dalam ruang hampa (atau udara), kerapatan energi magnetik didefinisikan sebagai:

$$u = \frac{B^2}{2\mu_0}$$

Artinya, setiap titik di ruang angkasa yang memiliki medan magnet sebesar $B$ sebenarnya mengandung energi tersembunyi. Semakin kuat medan magnetnya, semakin padat energinya.

\newpage

# Bagian 4: Induktansi Mutual (Timbal Balik)

Setelah memahami bagaimana satu kumparan mempengaruhi dirinya sendiri (induksi diri), sekarang kita akan melihat fenomena yang lebih "sosial": bagaimana satu kumparan mempengaruhi kumparan lain di dekatnya tanpa menyentuhnya sama sekali. Fenomena ini disebut **Induktansi Mutual (**$M$**)**.

![Dua coil saling menginduksi.](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774503645015.png)

## 4.1. Prinsip Kerja: "Aksi dan Reaksi" Magnetik

Bayangkan ada dua kumparan, Kumparan 1 dan Kumparan 2, diletakkan berdampingan.

1. Jika kita mengubah arus pada Kumparan 1 ($i_1$), maka medan magnet yang dihasilkannya juga berubah.
2. Karena Kumparan 2 berada di dekatnya, ia akan "merasakan" perubahan fluks magnetik dari Kumparan 1 tersebut.
3. Berdasarkan Hukum Faraday, Kumparan 2 akan menghasilkan ggl induksi ($\mathcal{E}_2$) meskipun ia tidak terhubung ke baterai Kumparan 1.

Besarnya ggl yang diinduksi pada kumparan kedua sebanding dengan laju perubahan arus pada kumparan pertama:

$$\mathcal{E}_2 = -M \frac{di_1}{dt}$$

Di sini, $M$ adalah konstanta **Induktansi Mutual**. Hal yang luar biasa adalah hubungan ini bersifat timbal balik: pengaruh Kumparan 1 ke Kumparan 2 sama besarnya dengan pengaruh Kumparan 2 ke Kumparan 1.

## 4.2. Aplikasi Nyata: Pengisian Daya Nirkabel (_Wireless Charging_)

Aplikasi paling populer dari konsep ini adalah pada sikat gigi elektrik atau pengisi daya _smartphone_ nirkabel.

- **Basis Pengisi Daya:** Di dalam dudukan sikat gigi, terdapat kumparan primer yang dialiri arus bolak-balik (AC). Arus ini terus-menerus berubah, menciptakan medan magnet yang juga terus berubah.
- **Sikat Gigi:** Di dalam gagang sikat gigi, terdapat kumparan sekunder. Saat sikat gigi diletakkan di atas dudukan, perubahan medan magnet dari dudukan menginduksi arus listrik di dalam gagang sikat gigi melalui induktansi mutual.
- **Hasilnya:** Baterai sikat gigi terisi tanpa ada logam yang bersentuhan (kontak listrik). Ini sangat aman untuk perangkat yang sering terkena air karena tidak ada risiko korsleting pada terminal logam yang terbuka.

## Ringkasan Konsep

1. **Penyimpanan:** Induktor menyimpan energi dalam medan magnet ($U = \frac{1}{2}LI^2$).
2. **Lokasi:** Energi berada dalam ruang yang mengandung medan magnet ($u = \frac{B^2}{2\mu_0}$).
3. **Interaksi:** Dua kumparan dapat mentransfer energi melalui perubahan arus tanpa kontak fisik ($M$).

**Langkah Selanjutnya:**

Setelah memahami bagaimana induktor menyimpan dan mentransfer energi, kita akan mempelajari apa yang terjadi jika induktor dikombinasikan dengan resistor dalam sebuah rangkaian. Kita akan masuk ke **Bagian 5: Rangkaian RL**.

\newpage

# Bagian 5: Rangkaian RL (Resistor-Induktor)

Setelah memahami bagaimana induktor bekerja secara mandiri, sekarang kita akan melihat perilakunya saat digabungkan dengan resistor dalam sebuah rangkaian DC sederhana. Rangkaian ini disebut **Rangkaian RL**.

## 5.1. Sifat Dasar: Inersia Elektrik

Hal terpenting yang harus dipahami tentang rangkaian RL adalah bahwa **arus tidak bisa berubah secara instan**. Jika pada rangkaian yang hanya berisi resistor arus akan langsung melompat ke nilai maksimum saat sakelar ditutup, pada rangkaian RL hal ini tidak terjadi.

Kehadiran induktor menyebabkan munculnya ggl balik ($\mathcal{E}_L$) yang menentang perubahan arus. Akibatnya, rangkaian ini memiliki semacam "inersia" atau sifat lamban. Induktor memaksa arus untuk berubah secara bertahap, bukan seketika.

## 5.2. Fenomena Kenaikan Arus (_Current Growth_)

Bayangkan Anda menutup sakelar pada rangkaian RL yang terhubung ke baterai. Pada detik $t=0$, arus adalah nol. Secara matematis, arus akan naik mengikuti fungsi eksponensial:

$$i(t) = \frac{\epsilon}{R} (1 - e^{-(R/L)t})$$

- **Pada awal (**$t=0$**):** Induktor memberikan perlawanan maksimum. Arus mulai dari nol. Induktor bertindak seolah-olah ia adalah hambatan tak terhingga (sakelar terbuka).
- **Seiring berjalannya waktu:** Perlawanan induktor perlahan berkurang seiring dengan melambatnya laju kenaikan arus.
- **Kondisi Tunak (**$t \to \infty$**):** Setelah waktu yang lama, arus mencapai nilai maksimumnya $I = \frac{\epsilon}{R}$. Pada titik ini, arus sudah konstan, sehingga induktor tidak lagi melawan dan berfungsi seperti kawat biasa.

## 5.3. Konstanta Waktu Induksi ($\tau_L$)

Seberapa cepat arus tersebut naik? Hal ini ditentukan oleh sebuah parameter yang disebut **Konstanta Waktu (**$\tau_L$**)**:

$$\tau_L = \frac{L}{R}$$

Konstanta waktu ini memberi tahu kita berapa lama waktu yang dibutuhkan arus untuk mencapai sekitar $63\%$ dari nilai maksimumnya.

- Jika $L$ besar, $\tau_L$ besar, maka rangkaian sangat lamban (butuh waktu lama untuk stabil).
- Jika $R$ besar, $\tau_L$ kecil, maka rangkaian lebih cepat mencapai kondisi stabil.

![Kurva arus listrik terhadap waktu untuk sumber tegangan.](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774503944416.png)

## 5.4. Fenomena Penurunan Arus (Current Decay)

Apa yang terjadi jika kita sudah memiliki arus yang mengalir stabil, lalu kita melepas baterai tetapi tetap membiarkan rangkaian tertutup (loop tertutup)?

Arus tidak langsung menjadi nol. Ingat, induktor telah menyimpan energi dalam **medan magnetnya**. Saat baterai dilepas, medan magnet ini mulai "runtuh". Runtuhnya medan magnet ini justru menghasilkan ggl yang mencoba mempertahankan arus agar tetap mengalir. Arus akan turun secara perlahan sesuai rumus:

$$i(t) = I_0 e^{-(R/L)t}$$

Arus akan meluruh secara eksponensial hingga akhirnya energi yang tersimpan di medan magnet habis terdisipasi menjadi panas di resistor.

![Kurva arus listrik terhadap waktu untuk sumber arus.](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774504534961.png)

## Ringkasan Konsep untuk Diskusi

1. **Induktor menunda perubahan:** Ia menghambat kenaikan arus saat sakelar ditutup dan menghambat penurunan arus saat sakelar dibuka.
2. **Energi adalah kunci:** Arus tetap mengalir saat baterai dilepas karena induktor sedang mengembalikan energi yang ia simpan sebelumnya.
3. **Aplikasi:** Sifat ini digunakan dalam filter frekuensi, sistem penyalaan kendaraan, dan pelindung lonjakan arus.

**Langkah Selanjutnya:**

Bagaimana jika kita mengganti resistor dengan kapasitor? Kita akan melihat fenomena yang lebih luar biasa: **Osilasi**. Mari kita lanjut ke **Bagian 6: Rangkaian LC**.

\newpage

# Bagian 6: Rangkaian LC dan Osilasi Listrik

Jika pada rangkaian RL kita melihat arus yang naik atau turun secara perlahan, maka pada **Rangkaian LC** kita akan melihat fenomena yang jauh lebih dinamis: **Osilasi Listrik**. Rangkaian ini hanya terdiri dari sebuah kapasitor ($C$) dan sebuah induktor ($L$) yang dihubungkan secara seri dalam satu loop tertutup.

## 6.1. Prinsip Osilasi: Analogy Pegas dan Massa

Untuk memahami Rangkaian LC, bayangkan sebuah sistem pegas dan massa di laboratorium mekanika.

- **Kapasitor (**$C$**)** ibarat **Pegas**: Ia menyimpan energi potensial (dalam bentuk medan listrik).
- **Induktor (**$L$**)** ibarat **Massa**: Ia memiliki inersia dan menyimpan energi kinetik (dalam bentuk medan magnet).

Dalam sistem pegas, energi berpindah-pindah dari energi potensial ke energi kinetik secara terus-menerus. Hal yang persis sama terjadi pada rangkaian LC. Energi terus-menerus "memantul" bolak-balik antara kapasitor dan induktor.

## 6.2. Siklus Tahapan Osilasi

Mari kita telusuri apa yang terjadi dalam satu siklus penuh osilasi:

1. **Tahap Awal (**$t=0$**):** Kapasitor bermuatan penuh ($Q_{max}$). Seluruh energi sistem tersimpan sebagai **medan listrik** di dalam kapasitor. Arus belum mengalir ($i=0$).
2. **Tahap Pengosongan:** Kapasitor mulai membuang muatannya melalui induktor. Arus mulai mengalir dan meningkat. Karena ada arus, induktor mulai membangun **medan magnet**.
3. **Tahap Energi Magnetik Maksimum:** Saat kapasitor benar-benar kosong ($Q=0$), arus mencapai nilai puncaknya ($i_{max}$). Sekarang, seluruh energi sistem berpindah ke induktor dalam bentuk medan magnet.
4. **Tahap Pengisian Ulang:** Induktor (karena sifat inersianya) tidak ingin arus berhenti begitu saja. Ia terus memompa muatan ke kapasitor, tetapi sekarang dengan **polaritas yang terbalik**.
5. **Tahap Pembalikan:** Kapasitor kembali penuh, tetapi pelat yang tadinya positif kini menjadi negatif. Proses ini kemudian berulang kembali ke arah sebaliknya.

Tanpa adanya hambatan (resistor), "tarian" energi ini akan berlangsung selamanya.

## 6.3. Frekuensi Sudut Osilasi

Seberapa cepat osilasi ini terjadi? Kecepatannya ditentukan oleh nilai komponen yang kita gunakan. Frekuensi sudut ($\omega$) dari osilasi alami ini dirumuskan sebagai:

$$\omega = \frac{1}{\sqrt{LC}}$$

- Jika kita memperbesar nilai $L$ atau $C$, maka osilasi akan melambat (frekuensi rendah).
- Jika kita menggunakan $L$ dan $C$ yang kecil, osilasi akan terjadi sangat cepat (frekuensi tinggi).

## Mengapa Ini Penting?

Rangkaian LC adalah jantung dari teknologi komunikasi.

- **Radio dan Televisi:** Saat Anda "menala" (_tuning_) radio ke frekuensi tertentu, Anda sebenarnya sedang mengubah nilai kapasitansi ($C$) agar frekuensi osilasi rangkaian di dalam radio sama dengan frekuensi gelombang stasiun radio tersebut.
- **Filter Sinyal:** Digunakan untuk memilih sinyal tertentu dan membuang gangguan (_noise_) pada perangkat elektronik.

## Ringkasan Konsep

1. **Osilasi** adalah pertukaran energi secara periodik antara medan listrik ($C$) dan medan magnet ($L$).
2. **Energi Total** sistem bersifat kekal ($U_{total} = U_B + U_E$) jika tidak ada resistor.
3. **Frekuensi** ditentukan oleh karakteristik fisik komponen melalui rumus $\omega = 1/\sqrt{LC}$.

**Langkah Selanjutnya:**

Di dunia nyata, setiap kabel memiliki hambatan (resistor). Apa yang terjadi jika kita memasukkan resistor ke dalam "tarian" energi ini? Jawabannya adalah **Osilasi Teredam**. Kita akan mempelajarinya di **Bagian 7: Rangkaian RLC Seri**.

\newpage

# Bagian 7: Rangkaian RLC Seri dan Arus AC

Pada bagian sebelumnya, kita telah mempelajari rangkaian LC yang ideal, di mana energi "memantul" bolak-balik tanpa henti. Namun, di dunia nyata, setiap kabel memiliki hambatan. Hari ini kita akan menggabungkan ketiga komponen utama—Resistor ($R$), Induktor ($L$), dan Kapasitor ($C$)—untuk melihat bagaimana mereka berinteraksi dalam sistem tenaga listrik yang sesungguhnya.

## 7.1. Osilasi Teredam R-L-C: Ketika Energi Menghilang

Dalam rangkaian LC ideal, grafik osilasi berbentuk sinus murni yang konstan. Namun, begitu kita menambahkan **Resistor (**$R$**)**, situasi berubah. Resistor adalah "pencuri energi". Setiap kali arus mengalir melaluinya, sebagian energi listrik diubah menjadi panas (disipasi).

Fenomena ini disebut **Osilasi Teredam**. Bayangkan sebuah bandul yang berayun di dalam air; ayunannya akan semakin kecil dan akhirnya berhenti karena gesekan. Dalam rangkaian RLC:

- Energi total sistem terus berkurang.
- Amplitudo arus dan muatan menurun secara eksponensial terhadap waktu.
- Akhirnya, seluruh energi yang awalnya disimpan di kapasitor akan habis menjadi panas di resistor.

## 7.2. Sistem Arus Bolak-Balik (AC)

Sebagian besar sistem kelistrikan kita (seperti listrik PLN) menggunakan arus bolak-balik. Dalam sistem AC, hambatan tidak lagi hanya ditentukan oleh $R$, tetapi juga oleh **Reaktansi**:

1. **Reaktansi Induktif (**$X_L$**):** Perlawanan induktor terhadap AC. Semakin tinggi frekuensi, semakin besar hambatannya ($X_L = \omega L$).
2. **Reaktansi Kapasitif (**$X_C$**):** Perlawanan kapasitor terhadap AC. Sebaliknya, semakin tinggi frekuensi, semakin kecil hambatannya ($X_C = \frac{1}{\omega C}$).
3. **Impedansi (**$Z$**):** Total hambatan gabungan dari $R$, $L$, dan $C$.

	$$Z = \sqrt{R^2 + (X_L - X_C)^2}$$

**Faktor Fase:** Dalam AC, tegangan dan arus tidak selalu "kompak" (seirama). Induktor menyebabkan tegangan mendahului arus, sedangkan kapasitor menyebabkan arus mendahului tegangan. Perbedaan ini diukur dengan sudut fase ($\phi$):

$$\tan \phi = \frac{X_L - X_C}{R}$$

## 7.3. Resonansi: Titik Efisiensi Maksimum

Ada satu kondisi istimewa yang disebut **Resonansi**. Kondisi ini terjadi ketika reaktansi induktif tepat sama dengan reaktansi kapasitif ($X_L = X_C$). Pada titik ini:

- Bagian imajiner dari hambatan saling meniadakan.
- Impedansi mencapai nilai **minimum** (hanya tersisa $R$).
- Arus ($I$) mencapai nilai **maksimum**.

Frekuensi di mana hal ini terjadi disebut frekuensi resonansi:

$$\omega_0 = \frac{1}{\sqrt{LC}}$$

**Aplikasi:** Inilah cara kerja _tuner_ pada radio atau TV. Ketika Anda memutar kenop radio, Anda mengubah nilai $C$ hingga frekuensi resonansi rangkaian Anda "cocok" dengan frekuensi gelombang dari stasiun radio tersebut, sehingga arus sinyal menjadi maksimum dan suara terdengar jernih.

## 7.4. Nilai RMS dan Daya Rata-rata

Karena arus AC terus berubah arah, kita menggunakan nilai **RMS (Root Mean Square)** atau nilai efektif untuk menghitung daya. Nilai RMS adalah nilai AC yang setara dengan DC dalam hal menghasilkan panas.

$$I_{rms} = \frac{I_{max}}{\sqrt{2}}$$$$V_{rms} = \frac{V_{max}}{\sqrt{2}}$$

Daya rata-rata ($P_{avg}$) yang dikonsumsi oleh rangkaian tidak hanya bergantung pada tegangan dan arus, tetapi juga pada **Faktor Daya** ($\cos \phi$):

$$P_{avg} = V_{rms} I_{rms} \cos \phi$$

Hanya resistor yang benar-benar "memakan" daya, sementara induktor dan kapasitor hanya meminjam dan mengembalikan energi.

## Ringkasan Akhir Materi Kemagnetan III

Kita telah menempuh perjalanan dari memahami bagaimana satu lilitan kawat bisa melawan arus, hingga bagaimana rangkaian RLC menjadi dasar dari teknologi komunikasi dan transmisi daya global.

1. **Induktansi** adalah inersia listrik.
2. **Energi** disimpan di medan magnet.
3. **Rangkaian RLC** memungkinkan kita mengontrol frekuensi dan aliran energi dengan presisi tinggi melalui fenomena resonansi.

![Rangkaian R-L-C](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774505251699.png)

![Rangkaian R-L-C seri.](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774505277512.png)

\newpage

# Bagian 8: Teknologi dan Aplikasi Terkait

Setelah kita mempelajari bagaimana energi disimpan dalam medan magnet dan bagaimana rangkaian RLC berosilasi, sekarang kita akan melihat "raksasa-raksasa" teknologi yang bekerja berdasarkan prinsip tersebut. Dua aplikasi paling fundamental dalam peradaban modern adalah **Motor AC** dan **Transformator**.

## 8.1. Motor AC: Mengubah Listrik Menjadi Gerak

Motor AC adalah mesin yang mengubah energi listrik arus bolak-balik menjadi energi mekanik (gerak rotasi). Hampir semua alat rumah tangga yang berputar—mulai dari kipas angin hingga mesin cuci—menggunakan prinsip ini.

**Komponen Utama:**

1. **Stator:** Bagian motor yang diam. Di sini terdapat kumparan kawat yang dialiri arus AC untuk menghasilkan medan magnet yang terus berubah atau berputar.
2. **Rotor:** Bagian motor yang berputar. Rotor diletakkan di dalam medan magnet stator. Berdasarkan Hukum Faraday, medan magnet stator menginduksi arus pada rotor, yang kemudian menghasilkan gaya magnet (Gaya Lorentz) untuk memutar poros motor.

**Tipe Motor AC:**

- **Motor 1-Fase:** Umumnya digunakan untuk peralatan rumah tangga kecil. Motor ini memerlukan kapasitor (ingat rangkaian RLC kita!) untuk membantu memulai putaran awal.
- **Motor 3-Fase:** Digunakan dalam industri skala besar. Motor ini jauh lebih efisien dan bertenaga karena menggunakan tiga aliran arus AC yang fasenya berbeda $120^\circ$, sehingga menciptakan medan magnet putar yang sangat stabil tanpa memerlukan bantuan tambahan untuk memulai putaran.

![Aplikasi motor AC.](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774505382514.png)

## 8.2. Transformator (Trafo): Jantung Distribusi Listrik

Pernahkah Anda bertanya-tanya mengapa tegangan listrik dari PLN di kabel jalan sangat tinggi ($20.000\text{ V}$), tetapi saat masuk ke rumah kita hanya menjadi $220\text{ V}$? Jawabannya adalah **Transformator**.

Transformator bekerja murni berdasarkan prinsip **Induktansi Mutual**. Ia memindahkan energi listrik dari satu rangkaian ke rangkaian lain melalui medan magnet tanpa ada bagian yang bergerak.

**Prinsip Kerja:**

Trafo terdiri dari dua lilitan yang melingkari inti besi yang sama: **Lilitan Primer** dan **Lilitan Sekunder**.

- Arus AC pada lilitan primer menghasilkan fluks magnetik yang berubah-ubah di inti besi.
- Fluks yang berubah ini "menembus" lilitan sekunder dan menginduksi ggl di sana.

**Jenis-Jenis Trafo:**

Hubungan antara tegangan ($V$) dan jumlah lilitan ($N$) dirumuskan sebagai:

$$\frac{V_p}{V_s} = \frac{N_p}{N_s}$$

1. **Trafo Step-Up:** Memiliki lilitan sekunder lebih banyak daripada primer ($N_s > N_p$). Fungsinya untuk **menaikkan tegangan**. Digunakan di pembangkit listrik agar listrik bisa dikirim jarak jauh dengan rugi-rugi daya yang kecil.
2. **Trafo Step-Down:** Memiliki lilitan sekunder lebih sedikit ($N_s < N_p$). Fungsinya untuk **menurunkan tegangan** ke level yang aman untuk digunakan oleh peralatan elektronik kita.

![Transformator (Trafo).](attachments/Materi%20Kuliah%207%20Fisika%20Dasar%20II%20%E2%80%93%20Kemagnetan%203-1774505441766.png)

# Penutup Kuliah

Dengan memahami Motor AC dan Transformator, kita kini bisa melihat gambaran besarnya:

- **Induktansi** memungkinkan kita mengubah level tegangan (Trafo).
- **Medan Magnet** memungkinkan kita menciptakan gerak dari listrik (Motor).
- **Rangkaian RLC** memungkinkan kita mengontrol frekuensi dan stabilitas sistem tersebut.

Listrik yang Anda gunakan untuk membaca materi ini kemungkinan besar telah melewati setidaknya tiga atau empat transformator dan mungkin digerakkan oleh generator (kebalikan dari motor) di tempat yang sangat jauh. Semua itu bekerja berdasarkan hukum-hukum fisika yang kita diskusikan dalam modul ini.

\newpage

# Penyelesaian Latihan Soal

## Soal 1: Mengapa Frekuensi Rendah pada Rangkaian LC Sulit Dibuat?

> Adalah hal yang mudah membuat rangkaian LC yang memiliki frekuensi osilasi ribuan hertz atau lebih, tetapi sulit membuat rangkaian LC yang memiliki frekuensi rendah. Mengapa?

Pertanyaan ini berkaitan dengan hubungan antara parameter fisik komponen (Induktor dan Kapasitor) dengan frekuensi alami yang dihasilkan oleh rangkaian tersebut. Berikut adalah penjelasan langkah-demi-langkahnya:

### Langkah 1: Memahami Rumus Dasar Frekuensi

Frekuensi osilasi alami ($f$) dari sebuah rangkaian LC ideal ditentukan oleh rumus:

$$f = \frac{1}{2\pi\sqrt{LC}}$$

Dari rumus ini, kita dapat melihat hubungan **berbanding terbalik**:

- Untuk mendapatkan **frekuensi tinggi** ($f$ besar), nilai hasil kali $L \times C$ harus **kecil**.
- Untuk mendapatkan **frekuensi rendah** ($f$ kecil), nilai hasil kali $L \times C$ harus **sangat besar**.

### Langkah 2: Analisis Kebutuhan Komponen untuk Frekuensi Rendah

Misalkan kita ingin membuat rangkaian dengan frekuensi sangat rendah (misal 1 Hz). Maka nilai $\sqrt{LC}$ harus bernilai sekitar $0,159$. Ini berarti nilai $L$ (Induktansi) dan $C$ (Kapasitansi) haruslah sangat besar secara fisik.

### Langkah 3: Kendala Fisik pada Induktor ($L$) Besar

Untuk mendapatkan nilai Induktansi ($L$) yang sangat besar, kita membutuhkan:

1. **Jumlah lilitan (**$N$**) yang sangat banyak.**
2. **Inti besi yang sangat besar dan berat** untuk meningkatkan permeabilitas magnetik.

**Masalah yang muncul:**

- **Resistansi Parasitik:** Semakin banyak lilitan kawat yang digunakan, semakin panjang kawat tersebut. Kawat yang sangat panjang memiliki hambatan jenis (Resistansi, $R$) yang signifikan.
- **Dampak:** Rangkaian tidak lagi menjadi LC murni, melainkan menjadi **R-L-C**. Karena $R$ yang besar, energi listrik akan cepat habis berubah menjadi panas (terdisipasi) sebelum osilasi yang stabil sempat terbentuk. Osilasi akan menjadi **terlalu teredam** (_overdamped_).

### Langkah 4: Kendala Fisik pada Kapasitor ($C$) Besar

Untuk mendapatkan Kapasitansi ($C$) yang sangat besar, kita membutuhkan:

1. **Luas pelat yang sangat lebar.**
2. **Jarak antar pelat yang sangat tipis.**

**Masalah yang muncul:**

- **Ukuran Fisik:** Kapasitor non-polar yang berukuran besar (Farad) akan memiliki dimensi fisik yang sangat raksasa dan tidak praktis untuk diletakkan di papan rangkaian.
- **Arus Bocor:** Kapasitor elektrolit besar cenderung memiliki arus bocor yang dapat mengganggu stabilitas osilasi pada frekuensi rendah.

### Langkah 5: Perbandingan dengan Frekuensi Tinggi

Sebaliknya, untuk mencapai frekuensi tinggi (ribuan hingga jutaan Hertz):

- Kita hanya membutuhkan induktor berupa beberapa lilitan kawat kecil (tanpa inti besi yang berat).
- Kita hanya membutuhkan kapasitor berukuran pikofarad ($pF$) yang ukurannya sangat mungil.
- Komponen-komponen ini mudah diproduksi, murah, dan memiliki resistansi parasitik yang sangat rendah, sehingga osilasi dapat berjalan dengan sangat efisien.

### Kesimpulan

Secara matematis, frekuensi rendah membutuhkan nilai $L$ dan $C$ yang besar. Namun secara praktis, membuat komponen $L$ dan $C$ yang sangat besar akan menimbulkan **hambatan dalam (resistansi)** yang besar dan **ukuran fisik yang tidak praktis**. Resistansi yang tinggi ini menyebabkan energi hilang sebagai panas, sehingga sulit bagi rangkaian untuk mempertahankan osilasi yang stabil pada frekuensi rendah.

## Soal 2: Penyelesaian Langkah-demi-Langkah: Desain Rangkaian LCR Seri

> Seseorang ingin mendesain rangkaian LCR seri dengan Q = 10 dan frekuensi resonansi 33 kHz. Orang tersebut memiliki induktor 45 mH dengan tahanan yang dapat diabaikan. Berapakah nilai tahanan R dan kapasitansi C yang harus digunakan?

Untuk menyelesaikan masalah ini, kita akan menggunakan hubungan antara faktor kualitas ($Q$), frekuensi resonansi ($f_r$), induktansi ($L$), kapasitansi ($C$), dan hambatan ($R$).

### 1. Identifikasi Data yang Diketahui

- Faktor Kualitas ($Q$) = $10$
- Frekuensi Resonansi ($f_r$) = $33\text{ kHz} = 33.000\text{ Hz}$
- Induktansi ($L$) = $45\text{ mH} = 0,045\text{ H}$

### 2. Menghitung Frekuensi Sudut Resonansi ($\omega_r$)

Frekuensi sudut ($\omega_r$) dalam satuan radian per detik dihitung dengan rumus:

$$\omega_r = 2\pi f_r$$$$\omega_r = 2 \times \pi \times 33.000$$$$\omega_r \approx 207.345,12\text{ rad/s}$$

### 3. Menghitung Nilai Hambatan ($R$)

Pada rangkaian LCR seri, faktor kualitas ($Q$) didefinisikan sebagai perbandingan antara reaktansi induktif pada saat resonansi dengan hambatan:

$$Q = \frac{\omega_r L}{R}$$

Maka, kita dapat mencari $R$ dengan mengubah rumus menjadi:

$$R = \frac{\omega_r L}{Q}$$$$R = \frac{207.345,12 \times 0,045}{10}$$$$R = \frac{9.330,53}{10}$$$$R \approx 933,05 \, \Omega$$

### 4. Menghitung Nilai Kapasitansi ($C$)

Pada saat resonansi, frekuensi sudut memenuhi persamaan:

$$\omega_r = \frac{1}{\sqrt{LC}}$$

Kuadratkan kedua sisi untuk mencari $C$:

$$\omega_r^2 = \frac{1}{LC}$$$$C = \frac{1}{L \cdot \omega_r^2}$$

Substitusikan nilai yang diketahui:

$$C = \frac{1}{0,045 \times (207.345,12)^2}$$$$C = \frac{1}{0,045 \times 4,299 \times 10^{10}}$$$$C = \frac{1}{1.934.550.000}$$$$C \approx 5,17 \times 10^{-10}\text{ F}$$

Untuk mempermudah pembacaan, kita konversi ke satuan **pikofarad (pF)**:

$$C \approx 517\text{ pF}$$

### Kesimpulan Akhir

Untuk mendapatkan rangkaian LCR seri dengan spesifikasi tersebut, Anda harus menggunakan:

- **Hambatan (**$R$**):** $\approx 933,05 \, \Omega$
- **Kapasitansi (**$C$**):** $\approx 517\text{ pF}$ (atau $0,517\text{ nF}$)

## Penyelesaian Langkah-demi-Langkah Soal Latihan Kemagnetan III

Berikut adalah pembahasan detail untuk soal nomor 3, 4, dan 5 berdasarkan materi Induktansi dan Rangkaian RL/RLC.

### Soal 3: Pengaruh Induktansi terhadap Konstanta Waktu

**Pertanyaan:** Bagaimana konstanta waktu induktor dipengaruhi oleh penggandaan induktansinya ($L$)?

**Langkah-langkah Penyelesaian:**

1. **Identifikasi Rumus:** Konstanta waktu untuk rangkaian RL ($\tau_L$) didefinisikan sebagai:

	$$\tau_L = \frac{L}{R}$$

2. **Analisis Perubahan:** Jika induktansi mula-mula adalah $L$ dan kemudian digandakan menjadi $L' = 2L$, maka konstanta waktu yang baru ($\tau_L'$) adalah:

	$$\tau_L' = \frac{L'}{R} = \frac{2L}{R}$$

3. **Hubungan:** Kita bisa melihat bahwa $\tau_L' = 2 \times \tau_L$.
4. **Kesimpulan:** Konstanta waktu akan meningkat hingga **dua kali lipat** dari nilai aslinya.

**Jawaban: B**

### Soal 4: Pengaruh Resistansi terhadap Konstanta Waktu

**Pertanyaan:** Bagaimana konstanta waktu induktor dipengaruhi oleh penggandaan resistansi ($R$) dalam rangkaian?

**Langkah-langkah Penyelesaian:**

1. **Identifikasi Rumus:** Gunakan rumus yang sama:

	$$\tau_L = \frac{L}{R}$$

2. **Analisis Perubahan:** Jika resistansi mula-mula adalah $R$ dan digandakan menjadi $R' = 2R$, maka konstanta waktu yang baru ($\tau_L'$) adalah:

	$$\tau_L' = \frac{L}{R'} = \frac{L}{2R}$$

3. **Hubungan:** Kita bisa melihat bahwa $\tau_L' = \frac{1}{2} \times \tau_L$.
4. **Kesimpulan:** Konstanta waktu akan menurun hingga **setengah** dari nilai aslinya.

**Jawaban: D**

### Soal 5: Istilah Induksi Antar Rangkaian

**Pertanyaan:** Istilah manakah yang digunakan untuk efek di mana perubahan arus dalam satu rangkaian menginduksi ggl di rangkaian lain?

**Langkah-langkah Penyelesaian:**

1. **Definisi Induksi Diri:** Fenomena ggl induksi yang muncul pada kumparan itu sendiri akibat perubahan arus di kumparan tersebut.
2. **Definisi Induksi Mutual (Timbal Balik):** Fenomena di mana perubahan arus pada Kumparan 1 menciptakan perubahan fluks magnetik yang menembus Kumparan 2, sehingga menginduksi ggl pada Kumparan 2.
3. **Analisis Soal:** Soal menanyakan induksi pada "rangkaian lain", yang sesuai dengan definisi induksi mutual.

**Jawaban: E**

### Ringkasan Jawaban Soal 1 & 2 (Ulasan Singkat)

- **Soal 1:** Frekuensi rendah sulit dibuat karena membutuhkan nilai $L$ dan $C$ yang sangat besar. Induktor besar memiliki kawat sangat panjang yang menciptakan hambatan dalam ($R$) tinggi, menyebabkan osilasi cepat habis (teredam).
- **Soal 2:** Dengan $Q=10, f_r=33\text{ kHz}, L=45\text{ mH}$:
	- $R = \frac{2\pi f_r L}{Q} \approx 933 \, \Omega$
	- $C = \frac{1}{L(2\pi f_r)^2} \approx 517\text{ pF}$

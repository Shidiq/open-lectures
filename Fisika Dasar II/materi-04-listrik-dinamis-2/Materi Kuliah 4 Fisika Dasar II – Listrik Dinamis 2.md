# BAB 1. Analisis Teknis Rangkaian Arus Searah (Direct Current)

Dalam studi fisika elektronika, kita membedakan metode analisis berdasarkan kompleksitas rangkaian. Rangkaian sederhana yang terdiri dari kombinasi seri-paralel resistor dapat diselesaikan dengan aturan penggabungan hambatan ekivalen. Namun, untuk rangkaian yang lebih rumit (multi-loop), kita memerlukan pendekatan yang lebih fundamental, yaitu **Kaidah Kirchhoff**. Kaidah ini berakar pada dua prinsip kelestarian universal: kelestarian muatan listrik dan kelestarian energi.

## 1. Filosofi Arus Searah (Direct Current - DC) dan Kondisi Tunak

Arus searah didefinisikan sebagai aliran muatan listrik dengan arah yang konstan. Analisis rangkaian DC didasarkan pada asumsi **kondisi tunak** (_steady state_). Artinya, besaran arus ($I$) dan tegangan ($V$) tidak berubah terhadap waktu. Hal ini dimungkinkan karena sumber tegangan (GGL) seperti baterai memberikan beda potensial yang konstan. Secara fisik, ini berarti elektron mengalir dengan laju rata-rata yang tetap melalui konduktor.

## 2. Elemen Dasar: Gaya Gerak Listrik (GGL) dan Hambatan Dalam

### 2.1 Gaya Gerak Listrik (GGL)

Untuk mempertahankan beda potensial dan menghasilkan arus tetap, diperlukan sumber energi yang disebut sumber GGL ($\epsilon$). GGL bukanlah sebuah gaya dalam pengertian mekanis, melainkan tegangan yang dihasilkan oleh alat (seperti baterai atau generator) yang mengubah energi non-listrik menjadi energi listrik.

Sumber tegangan ideal tidak memiliki hambatan. Namun, sumber riil memiliki resistansi internal ($r$).

GGL didefinisikan secara matematis sebagai kerja ($dW$) yang dilakukan untuk mengangkut muatan ($dq$):

$$\epsilon = \frac{dW}{dq}$$

Satuan GGL adalah Joule/Coulomb ($J/C$) atau Volt ($V$).

### 2.2 Hambatan Dalam Baterai

Pada kenyataannya, sumber tegangan (baterai) dengan GGL sebesar $\epsilon$ memiliki hambatan internal ($r$). Maka, tegangan terminal baterai saat mengalirkan arus $I$ adalah:

$$\Delta V = \epsilon - Ir \text{ dengan } IR+Ir=\epsilon$$

Arus total dalam rangkaian dengan beban luar $R$ menjadi:

$$I = \frac{\epsilon}{R + r}$$

![Rangkaian baterai dengan hambatan dalam r.](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772250093348.png)

# BAB 2. Analisis Mendalam: Hukum Kirchhoff

Hukum Kirchhoff terdiri dari dua aturan utama yang dirumuskan oleh Gustav Kirchhoff. Aturan-aturan ini bukan sekadar rumus matematis, melainkan pengejawantahan dari hukum dasar fisika alam semesta: **Hukum Kelestarian**.

## 1. Hukum Pertama Kirchhoff (Kaidah Percabangan / KCL)

Berdasarkan slide halaman 9, Hukum Pertama Kirchhoff berfokus pada apa yang terjadi di titik pertemuan kawat (percabangan).

### Dasar Fisika: Kelestarian Muatan

Hukum ini didasarkan pada prinsip bahwa muatan listrik tidak dapat diciptakan atau dimusnahkan. Jumlah muatan yang mengalir ke sebuah titik dalam satu detik harus sama dengan jumlah muatan yang keluar dari titik tersebut pada detik yang sama.

### Bunyi Hukum

_"Pada setiap percabangan dalam rangkaian listrik, jumlah aljabar dari arus-arus listrik haruslah sama dengan nol."_

### Persamaan Matematis

$$\sum_{junction} I = 0$$

### Konvensi Tanda

Dalam perhitungan, kita harus konsisten dengan tanda arus:

- **Arus Masuk (+):** Arus yang menuju titik sambungan/percabangan.
- **Arus Keluar (-):** Arus yang meninggalkan titik sambungan/percabangan.

**Contoh pada slide:**

Jika arus $i_1$ dan $i_2$ masuk, sedangkan $i_3$ keluar, maka: $i_1 + i_2 - i_3 = 0$.

## 2. Hukum Kedua Kirchhoff (Kaidah Simpal / KVL)

Berdasarkan slide halaman 10-12, Hukum Kedua Kirchhoff berfokus pada perubahan potensial di sepanjang lintasan tertutup (loop).

### Dasar Fisika: Kelestarian Energi

Hukum ini menyatakan bahwa jika suatu muatan bergerak dalam satu lintasan tertutup dan kembali ke titik asalnya, energi potensial sistem tidak berubah. Energi yang diberikan oleh sumber GGL harus sama dengan energi yang digunakan/dihabiskan oleh hambatan (resistor).

### Bunyi Hukum

_"Jumlahan aljabar dari perubahan-perubahan potensial sepanjang lintasan tertutup dalam suatu rangkaian listrik haruslah sama dengan nol."_

### Persamaan Matematis

$$\sum_{closed} \Delta V = 0 \quad \text{atau} \quad \sum \epsilon + \sum (IR) = 0$$

### Aturan Tanda (Konvensi Penting)

Ini adalah bagian yang paling sering membingungkan mahasiswa. Mari kita perjelas berdasarkan slide:

1. **Melintasi Resistor (**$R$**):**
	
	- Jika arah loop **searah** dengan arah arus: $\Delta V = -IR$ (Terjadi penurunan potensial karena energi digunakan oleh hambatan).
	- Jika arah loop **berlawanan** dengan arah arus: $\Delta V = +IR$ (Terjadi kenaikan potensial secara relatif).
		
2. **Melintasi Sumber GGL (**$\epsilon$**):**
	
	- Jika loop bergerak dari kutub **negatif (-)** ke **positif (+)**: $\Delta V = +\epsilon$ (Terjadi kenaikan potensial).
	- Jika loop bergerak dari kutub **positif (+)** ke **negatif (-)**: $\Delta V = -\epsilon$ (Terjadi penurunan potensial).

![Ilustrasi aturan tanda.](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772504179552.png)

## Penjelasan Analisis Rangkaian Listrik (Hukum Kirchhoff)

Berdasarkan slide yang Anda berikan, rangkaian tersebut dianalisis menggunakan **Hukum Kirchhoff**, yang terdiri dari dua aturan utama: Hukum Arus Kirchhoff (KCL) dan Hukum Tegangan Kirchhoff (KVL).

![Ilustrasi rangkaian.](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772504971200.png)

### 1. Konsep Dasar

Rangkaian pada gambar memiliki dua sumber tegangan ($\varepsilon_1$ dan $\varepsilon_2$) serta tiga hambatan ($R_1, R_2, R_3$). Tujuan utamanya adalah mencari nilai arus yang mengalir pada setiap cabang ($i_1, i_2, i_3$).

#### Hukum I Kirchhoff (Kaidah Percabangan / KCL)

Menyatakan bahwa jumlah arus yang masuk ke sebuah titik percabangan sama dengan jumlah arus yang keluar dari titik tersebut.

$$\sum I_{masuk} = \sum I_{keluar}$$

#### Hukum II Kirchhoff (Kaidah Simpul / KVL)

Menyatakan bahwa dalam satu rangkaian tertutup (loop), jumlah aljabar gaya gerak listrik (GGL) dan penurunan tegangan ($IR$) adalah nol.

$$\sum \varepsilon + \sum (I \cdot R) = 0$$

### 2. Langkah-Langkah Analisis (Berdasarkan Slide)

#### Langkah 1: Menentukan Arah Arus

Kita menentukan arah $i_1, i_2,$ dan $i_3$ secara sembarang. Jika hasil akhir bernilai negatif, itu hanya berarti arah arus sebenarnya berlawanan dengan asumsi awal kita.

#### Langkah 2: Aplikasi Hukum I Kirchhoff

Pada titik percabangan **D**, diasumsikan arus $i_1$ dan $i_3$ masuk ke titik D, sedangkan $i_2$ keluar dari titik D.

Persamaannya:

$$i_1 + i_3 - i_2 = 0 \quad \dots (1)$$

Atau dapat ditulis: $i_2 = i_1 + i_3$.

#### Langkah 3 & 4: Analisis Simpul (Loop) I

Loop I adalah lintasan tertutup di sebelah kiri (A-B-D-A).

Berdasarkan persamaan $(2)$ di slide:

$$\varepsilon_1 - i_1 R_1 + i_3 R_3 = 0 \quad \dots (2)$$

- $\varepsilon_1$ **positif:** Karena arah putaran loop bertemu kutub positif baterai terlebih dahulu.
- $-i_1 R_1$**:** Arus $i_1$ searah dengan loop.
- $+i_3 R_3$**:** Arus $i_3$ berlawanan arah dengan loop (saat loop bergerak dari B ke D).

#### Langkah 5: Analisis Simpul (Loop) II

Loop II adalah lintasan tertutup di sebelah kanan (B-C-D-B).

Berdasarkan persamaan $(3)$ di slide:

$$-\varepsilon_2 - i_3 R_3 - i_2 R_2 = 0 \quad \dots (3)$$

- $-\varepsilon_2$**:** Loop bertemu kutub negatif baterai $\varepsilon_2$.
- $-i_3 R_3$**:** Arah loop (D ke B) searah dengan arah arus $i_3$.
- $-i_2 R_2$**:** Arah loop searah dengan arus $i_2$.

### 3. Hasil Akhir (Langkah 6)

Setelah melakukan substitusi dan eliminasi dari ketiga persamaan di atas, diperoleh rumus umum untuk masing-masing arus:

1. **Arus** $i_1$**:**

	$$i_1 = \frac{\varepsilon_1 (R_2 + R_3) - \varepsilon_2 R_3}{R_1 R_2 + R_1 R_3 + R_2 R_3}$$

2. **Arus** $i_2$**:**

	$$i_2 = \frac{-\varepsilon_2 (R_1 + R_3) + \varepsilon_1 R_3}{R_1 R_2 + R_1 R_3 + R_2 R_3}$$

3. **Arus** $i_3$**:**

	$$i_3 = \frac{-\varepsilon_1 R_2 - \varepsilon_2 R_1}{R_1 R_2 + R_1 R_3 + R_2 R_3}$$

#### Catatan Penting

- **Penyebut Sama:** Perhatikan bahwa semua penyebut untuk $i_1, i_2,$ dan $i_3$ adalah sama ($R_1 R_2 + R_1 R_3 + R_2 R_3$), yang merupakan kombinasi paralel dari hambatan-hambatan tersebut.
- **Tanda Negatif:** Jika Anda memasukkan angka dan hasilnya negatif, arah arus fisik yang sebenarnya adalah kebalikan dari panah yang digambar di awal.

## Penyelesaian Contoh Soal 1

![Soal 1](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772505278513.png)

### Langkah-Langkah Penyelesaian Rangkaian Satu Loop

#### (a) Menentukan Besar dan Arah Arus Listrik

Pertama, kita tentukan arah loop secara sembarang. Mari kita asumsikan arah loop **searah jarum jam** (C $\to$ A $\to$ B $\to$ C).

Menggunakan Hukum II Kirchhoff:

$$\sum \varepsilon + \sum (I \cdot R_{total}) = 0$$

Mari kita telusuri loop dari titik C:

1. Melewati $\varepsilon_1$ dari kutub negatif ke positif (sesuai arah panah GGL): $+\varepsilon_1$
2. Melewati hambatan dalam $r_1$: $-I \cdot r_1$
3. Melewati $\varepsilon_2$ dari kutub positif ke negatif (berlawanan arah panah GGL): $-\varepsilon_2$
4. Melewati hambatan dalam $r_2$: $-I \cdot r_2$
5. Melewati hambatan luar $R$: $-I \cdot R$

**Persamaan:**

$$\varepsilon_1 - \varepsilon_2 - I(r_1 + r_2 + R) = 0$$$$2 - 4 - I(1 + 2 + 5) = 0$$$$-2 - 8I = 0$$$$8I = -2$$$$I = -0,25 \text{ A}$$

**Kesimpulan Arus:**

- **Besar Arus:** $0,25 \text{ A}$
- **Arah Arus:** Karena hasilnya negatif, maka arah arus yang benar adalah **Berlawanan Arah Jarum Jam** (C $\to$ B $\to$ A $\to$ C).

#### (b) Beda Potensial antara Titik A dan Titik B ($V_{AB}$)

Kita gunakan rumus beda potensial antara dua titik: $V_{AB} = V_A - V_B = \sum \varepsilon + \sum (I \cdot R)$.

Mari kita ambil jalan dari B ke A (melalui baterai $\varepsilon_2$).

Karena arus asli ($I' = 0,25 \text{ A}$) mengalir dari B ke A:

- Kita bergerak dari B ke A: searah dengan panah $\varepsilon_2$ ($+4 \text{ V}$).
- Kita bergerak searah dengan arus $I'$ melewati $r_2$ ($-I' \cdot r_2$).

$$V_{AB} = \varepsilon_2 - I' \cdot r_2$$$$V_{AB} = 4 - (0,25 \cdot 2)$$$$V_{AB} = 4 - 0,5 = 3,5 \text{ V}$$

#### (c) Beda Potensial antara Titik A dan Titik C ($V_{AC}$)

Mari kita ambil jalan dari C ke A.

Ingat, arus asli $I'$ mengalir dari A ke C di cabang atas. Jadi, perjalanan C ke A adalah **melawan** arah arus.

- Bergerak dari C ke A: searah panah $\varepsilon_1$ ($+2 \text{ V}$).
- Bergerak melawan arah arus melewati $r_1$ ($+I' \cdot r_1$).

$$V_{AC} = \varepsilon_1 + I' \cdot r_1$$$$V_{AC} = 2 + (0,25 \cdot 1)$$$$V_{AC} = 2,25 \text{ V}$$

#### (d) Apakah $V_B > V_C$ atau $V_B < V_C$?

Mari kita hitung beda potensial antara C dan B melalui hambatan $R$.

Arus $I'$ mengalir dari C ke B melalui hambatan $R$.

$$V_C - V_B = I' \cdot R$$$$V_C - V_B = 0,25 \cdot 5 = 1,25 \text{ V}$$

Karena hasil $V_C - V_B$ adalah positif ($1,25 \text{ V}$), maka nilai $V_C$ lebih besar dari $V_B$.

**Jawaban:** $V_B < V_C$

## Penyelesaian Contoh Soal 2

![Soal 2.](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772505853091.png)

### Langkah Penyelesaian Contoh Soal 2 dengan Hukum Kirchhoff

Kita akan menggunakan data: $\varepsilon_1=3\text{V}$, $\varepsilon_2=1\text{V}$, $R_1=5\Omega$ (tengah), $R_2=2\Omega$ (kanan), dan $R_3=4\Omega$ (kiri).

#### Langkah 1: Menentukan Arah Arus Sembarang

Kita asumsikan titik percabangan atas adalah **Titik B** dan titik bawah adalah **Titik D**.

- $i_3$: Arus di cabang kiri (lewat $R_3$), arah ke kanan (masuk ke titik B).
- $i_1$: Arus di cabang tengah (lewat $R_1$), arah ke bawah (keluar dari titik B).
- $i_2$: Arus di cabang kanan (lewat $R_2$), arah ke kanan (keluar dari titik B).

#### Langkah 2: Kaidah Percabangan (Hukum I Kirchhoff) di Titik B

Jumlah arus masuk = jumlah arus keluar:

$$i_3 = i_1 + i_2 \quad \text{atau} \quad i_1 + i_2 - i_3 = 0 \dots (1)$$

#### Langkah 3 & 4: Kaidah Simpul (Hukum II Kirchhoff) pada Loop I (Kiri)

Kita pilih arah loop **searah jarum jam**. Mulai dari titik D ke atas lewat $\varepsilon_1$:

- Melewati $\varepsilon_1$ (kutub - ke +): $+\varepsilon_1$
- Melewati $R_3$ (searah arus $i_3$): $-i_3 R_3$
- Melewati $R_1$ (searah arus $i_1$): $-i_1 R_1$

**Persamaan Loop I:**

$$\varepsilon_1 - i_3 R_3 - i_1 R_1 = 0$$$$3 - 4i_3 - 5i_1 = 0 \implies 5i_1 + 4i_3 = 3 \dots (2)$$

#### Langkah 5: Kaidah Simpul pada Loop II (Kanan)

Kita pilih arah loop **searah jarum jam**. Mulai dari titik B ke kanan:

- Melewati $R_2$ (searah arus $i_2$): $-i_2 R_2$
- Melewati $\varepsilon_2$ (kutub + ke -): $-\varepsilon_2$
- Melewati $R_1$ (berlawanan arus $i_1$): $+i_1 R_1$

**Persamaan Loop II:**

$$-i_2 R_2 - \varepsilon_2 + i_1 R_1 = 0$$$$-2i_2 - 1 + 5i_1 = 0 \implies 5i_1 - 2i_2 = 1 \dots (3)$$

#### Langkah 6: Mengolah Persamaan (Substitusi & Eliminasi)

##### A. Substitusi Persamaan (1) ke Persamaan (2)

Ganti $i_3$ dengan $(i_1 + i_2)$:

$$5i_1 + 4(i_1 + i_2) = 3$$$$5i_1 + 4i_1 + 4i_2 = 3$$$$9i_1 + 4i_2 = 3 \dots (4)$$

##### B. Eliminasi Persamaan (3) dan (4)

Kita ingin mencari $i_1$, maka samakan koefisien $i_2$:

- Pers (3) x 2: $10i_1 - 4i_2 = 2$
- Pers (4) x 1: $9i_1 + 4i_2 = 3$

	----------------------------------- (+)

	$$19i_1 = 5$$$$i_1 = \frac{5}{19} \text{ A} \approx 0,263 \text{ A}$$

##### C. Mencari $i_2$ dan $i_3$

Dari Pers (3): $2i_2 = 5i_1 - 1$

$$2i_2 = 5\left(\frac{5}{19}\right) - 1 = \frac{25}{19} - \frac{19}{19} = \frac{6}{19}$$$$i_2 = \frac{3}{19} \text{ A} \approx 0,158 \text{ A}$$

Dari Pers (1): $i_3 = i_1 + i_2$

$$i_3 = \frac{5}{19} + \frac{3}{19} = \frac{8}{19} \text{ A} \approx 0,421 \text{ A}$$

#### Hasil Akhir (Daya)

**(a) Daya Termal (**$P = i^2 R$**):**

- $P_{R1} = (5/19)^2 \cdot 5 = \mathbf{0,346 \text{ W}}$
- $P_{R2} = (3/19)^2 \cdot 2 = \mathbf{0,050 \text{ W}}$
- $P_{R3} = (8/19)^2 \cdot 4 = \mathbf{0,709 \text{ W}}$

**(b) Daya GGL (**$P = \varepsilon \cdot i$**):**

- $P_{\varepsilon1} = 3 \cdot (8/19) = \mathbf{1,263 \text{ W}}$ (Memberikan energi)
- $P_{\varepsilon2} = 1 \cdot (3/19) = \mathbf{0,158 \text{ W}}$ (Menyerap energi karena arus masuk ke kutub +)

# BAB 3. Rangkaian RC

Materi ini merupakan bagian krusial dalam fisika listrik dinamis karena menjelaskan bagaimana arus dan muatan berubah terhadap waktu (tidak konstan seperti pada rangkaian resistor murni).

## 1. Pendahuluan Rangkaian RC

Rangkaian RC adalah rangkaian listrik yang terdiri dari sebuah resistor ($R$) dan sebuah kapasitor ($C$). Berbeda dengan rangkaian resistor murni di mana arus langsung mencapai nilai maksimum saat saklar ditutup, pada rangkaian RC, **arus dan muatan berubah secara eksponensial terhadap waktu**.

Terdapat dua kondisi utama yang dibahas:

- **Pemuatan (Charging):** Mengisi kapasitor dengan energi dari sumber tegangan (GGL).
- **Pelucutan (Discharging):** Mengosongkan muatan yang tersimpan di kapasitor melalui resistor.

![(a) Rangkaian RC, (b) pemuatan dan (c) pelucutan.](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772506137184.png)

## 2. Proses Pemuatan Kapasitor (Charging)

Ketika saklar dihubungkan ke terminal **a**, baterai (GGL $\epsilon$) mulai mengalirkan muatan ke kapasitor.

- **Hukum Kekekalan Energi:** Kerja yang dilakukan oleh GGL ($\epsilon dq$) sebagian diubah menjadi panas pada resistor ($i^2 R dt$) dan sebagian lagi disimpan sebagai energi potensial listrik dalam kapasitor ($dU$).
- **Persamaan Diferensial:** Berdasarkan Hukum Kirchhoff (KVL), diperoleh persamaan:

	$$\epsilon = iR + \frac{q}{C}$$

	Karena arus adalah laju perubahan muatan terhadap waktu ($i = \frac{dq}{dt}$), maka:

	$$\epsilon = R \frac{dq}{dt} + \frac{q}{C}$$

- **Solusi Muatan dan Arus:**
	- **Muatan ($q$):** Muatan bertambah secara eksponensial dari nol hingga nilai maksimum ($C\epsilon$).

		$$q(t) = C\epsilon (1 - e^{-\frac{t}{RC}})$$

	- **Arus ($i$):** Arus dimulai dari nilai maksimum ($\frac{\epsilon}{R}$) dan menurun secara eksponensial menuju nol saat kapasitor penuh.

		$$i(t) = \frac{\epsilon}{R} e^{-\frac{t}{RC}}$$

![Grafik pemuatan kapasitor. Muatan yang tersimpan dalam kapasitor bertambah secara eksponensial. Konstanta waktu (RC) menunjukkan waktu yang diperlukan tersimpan muatan sekitar 63,2% dari muatan maksimum Ce. Arus listrik mula-mula maksimum sebesar e/R, akan menurun secara eksponensial hingga akhirnya nol.](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772506518674.png)

### Penurunan Rumus Arus Listrik Rangkaian RC (Pemuatan)

Untuk memahami bagaimana rumus $i(t) = \frac{\epsilon}{R} e^{-\frac{t}{RC}}$ diperoleh, kita harus mulai dari hukum dasar rangkaian listrik dan menyelesaikan persamaan diferensial yang muncul.

#### 1. Hukum Loop Kirchhoff (KVL)

Pada saat saklar dihubungkan ke terminal **a** (proses pemuatan), total tegangan dalam loop tertutup adalah nol:

$$\epsilon - V_R - V_C = 0$$

Atau dapat ditulis:

$$\epsilon = iR + \frac{q}{C}$$

Di mana:

- $\epsilon$ = GGL sumber (V)
- $i$ = Arus sesaat (A)
- $R$ = Resistansi ($\Omega$)
- $q$ = Muatan sesaat pada kapasitor (C)
- $C$ = Kapasitansi (F)

#### 2. Menyusun Persamaan Diferensial

Karena arus adalah laju perubahan muatan terhadap waktu ($i = \frac{dq}{dt}$), kita substitusikan ke dalam persamaan:

$$\epsilon = R \frac{dq}{dt} + \frac{q}{C}$$

Untuk menyelesaikannya, kita atur ulang persamaan agar variabel $q$ dan $t$ dapat dipisahkan:

$$\epsilon - \frac{q}{C} = R \frac{dq}{dt}$$$$\frac{C\epsilon - q}{C} = R \frac{dq}{dt}$$$$\frac{dt}{RC} = \frac{dq}{C\epsilon - q}$$

#### 3. Integrasi

Kita integralkan kedua ruas. Pada saat $t = 0$, muatan kapasitor kosong ($q = 0$). Pada saat $t$, muatannya adalah $q$.

$$\int_{0}^{t} \frac{1}{RC} dt' = \int_{0}^{q} \frac{1}{C\epsilon - q'} dq'$$

Gunakan substitusi $u = C\epsilon - q$, maka $du = -dq$:

$$\frac{t}{RC} = \left[-\ln(C\epsilon - q') \right]_{0}^{q}$$$$\frac{t}{RC} = -\ln(C\epsilon - q) - (-\ln(C\epsilon))$$$$\frac{t}{RC} = -\ln\left(\frac{C\epsilon - q}{C\epsilon}\right)$$

Hilangkan logaritma dengan fungsi eksponensial ($e$):

$$e^{-\frac{t}{RC}} = \frac{C\epsilon - q}{C\epsilon}$$$$C\epsilon e^{-\frac{t}{RC}} = C\epsilon - q$$$$q(t) = C\epsilon (1 - e^{-\frac{t}{RC}})$$

#### 4. Mendapatkan Rumus Arus $i(t)$

Arus listrik diperoleh dengan mendiferensialkan muatan $q(t)$ terhadap waktu:

$$i(t) = \frac{dq}{dt}$$$$i(t) = \frac{d}{dt} \left[C\epsilon (1 - e^{-\frac{t}{RC}}) \right]$$

Turunkan suku per suku:

- Turunan dari konstanta $C\epsilon$ adalah $0$.
- Turunan dari $-C\epsilon e^{-\frac{t}{RC}}$ adalah $-C\epsilon \cdot \left(-\frac{1}{RC} \right) e^{-\frac{t}{RC}}$.

Maka:

$$i(t) = C\epsilon \left(\frac{1}{RC} \right) e^{-\frac{t}{RC}}$$

Sederhanakan dengan mencoret $C$:

$$i(t) = \frac{\epsilon}{R} e^{-\frac{t}{RC}}$$

#### Kesimpulan

Rumus ini menunjukkan bahwa:

1. Pada saat $t = 0$, arus bernilai maksimum $i = \frac{\epsilon}{R}$ (kapasitor bertindak seperti kawat biasa).
2. Seiring bertambahnya $t$, arus menurun secara eksponensial.
3. Pada saat $t \to \infty$, arus menjadi $0$ (kapasitor penuh dan memutus aliran arus DC).

## 3. Proses Pelucutan Kapasitor (Discharging)

Ketika saklar dipindah ke terminal **b**, sumber tegangan (GGL) diputus dari rangkaian, sehingga kapasitor yang sudah terisi muatan akan mengalirkan muatannya kembali melalui resistor.

- **Persamaan Dasar:** Karena tidak ada baterai ($\epsilon = 0$), maka:

	$$0 = iR + \frac{q}{C} \implies R \frac{dq}{dt} + \frac{q}{C} = 0$$

- **Solusi Muatan dan Arus:**
	- **Muatan ($q$):** Muatan berkurang dari nilai awal ($q_0$) menuju nol.

		$$q(t) = q_0 e^{-\frac{t}{RC}}$$

	- **Arus ($i$):** Arus mengalir dalam arah berlawanan dari proses pemuatan (ditandai dengan tanda negatif) dan juga berkurang secara eksponensial.

		$$i(t) = -\frac{\epsilon}{R} e^{-\frac{t}{RC}}$$

![Grafik pelucutan kapasitor. Muatan yang tersimpan dalam kapasitor berkurang secara eksponensial. Dalam waktu t = RC, muatan kapasitor telah berkurang menjadi sekitar 36,8% dari muatan mula-mula. Arus dalam proses pelucutan kapasitor juga menurun secara eksponensial terhadap waktu.](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772506591756.png)

## 4. Konstanta Waktu ($\tau = RC$)

Salah satu konsep terpenting dalam pdf ini adalah **Tetapan Waktu Kapasitif** ($\tau$):

$$\tau = RC$$

Tetapan ini menentukan seberapa cepat kapasitor terisi atau terlucuti:

- **Saat Pemuatan:** Dalam waktu $t = \tau$, muatan kapasitor mencapai sekitar **63,2%** dari muatan maksimumnya.
- **Saat Pelucutan:** Dalam waktu $t = \tau$, muatan kapasitor berkurang hingga tersisa sekitar **36,8%** dari muatan awalnya.

## 5. Analisis Tegangan (Hukum Kirchhoff)

Hubungan tegangan pada komponen:

1. **Tegangan Kapasitor ($V_C$):** $V_C = \frac{q}{C}$
2. **Tegangan Resistor ($V_R$):** $V_R = iR$

**Hukum Loop Kirchhoff:**

- **Pemuatan:** $V_C + V_R = \epsilon$ (Total tegangan komponen sama dengan tegangan baterai).
- **Pelucutan:** $V_C + V_R = 0$ (Energi dari kapasitor sepenuhnya habis digunakan oleh resistor).

## Ringkasan Tabel Perbandingan

|**Fitur**|**Pemuatan (Charging)**|**Pelucutan (Discharging)**|
|---|---|---|
|**Saklar**|Posisi **a**|Posisi **b**|
|**Muatan $q(t)$**|Naik: $C\epsilon (1 - e^{-\frac{t}{RC}})$|Turun: $Q_0 e^{-\frac{t}{RC}}$|
|**Arus $i(t)$**|Turun dari $I_{max}$ ke $0$|Turun dari $-I_{max}$ ke $0$|
|**Tujuan Akhir**|Kapasitor penuh ($V_C = \epsilon$)|Kapasitor kosong ($V_C = 0$)|

Materi ini sangat penting untuk memahami cara kerja _timer_, sirkuit _flash_ pada kamera, dan sistem penyaringan (filter) dalam elektronika.

## Penyelesaian Soal Fisika Dasar: Rangkaian RC

Dokumen ini berisi langkah-langkah detail untuk menyelesaikan tiga contoh soal mengenai pengisian dan pengosongan kapasitor.

### Soal 1: Energi Tersimpan Setengah Maksimum

**Pertanyaan:** Berapakah waktu yang diperlukan suatu rangkaian $RC$ agar energi yang tersimpan dalam kapasitor akan mencapai setengah dari nilai setimbangnya (maksimum)?

**Langkah-langkah:**

1. **Rumus Energi Kapasitor:**

	Energi ($U$) yang tersimpan dalam kapasitor dinyatakan sebagai:

	$$U(t) = \frac{q(t)^2}{2C}$$

	Energi maksimum ($U_{max}$) saat setimbang adalah:

	$$U_{max} = \frac{q_{max}^2}{2C}$$

2. **Kondisi yang diinginkan:**

	$$U(t) = \frac{1}{2} U_{max}$$$$\frac{q(t)^2}{2C} = \frac{1}{2} \frac{q_{max}^2}{2C}$$$$q(t)^2 = \frac{1}{2} q_{max}^2 \implies q(t) = \frac{q_{max}}{\sqrt{2}}$$

3. **Substitusi Rumus Pemuatan Muatan:**

	Rumus muatan pada proses pemuatan adalah $q(t) = q_{max}(1 - e^{-t/RC})$.

	$$\frac{q_{max}}{\sqrt{2}} = q_{max}(1 - e^{-t/RC})$$$$\frac{1}{\sqrt{2}} = 1 - e^{-t/RC}$$$$e^{-t/RC} = 1 - \frac{1}{\sqrt{2}} \approx 1 - 0,707 = 0,293$$

4. **Mencari Waktu (**$t$**):**

	Gunakan logaritma natural ($\ln$):

	$$-\frac{t}{RC} = \ln(0,293)$$$$t = -RC \cdot \ln(0,293) \approx -RC \cdot (-1,227)$$

	$t \approx 1,227 RC$ atau sekitar $1,23$ kali tetapan waktu.

### Soal 2: Pemuatan 1% dari Muatan Setimbang

**Pertanyaan:** Hitunglah berapa kali tetapan waktu (kapasitif) yang harus dilalui sehingga sebuah kapasitor dimuati sebanyak 1% dari muatan setimbangnya?

**Langkah-langkah:**

1. **Kondisi yang diinginkan:**

	$$q(t) = 1\% \cdot q_{max} = 0,01 q_{max}$$

2. **Substitusi Rumus Pemuatan:**

	$$0,01 q_{max} = q_{max}(1 - e^{-t/\tau})$$$$0,01 = 1 - e^{-t/\tau}$$$$e^{-t/\tau} = 1 - 0,01 = 0,99$$

3. **Mencari Rasio** $t/\tau$**:**

	$$-\frac{t}{\tau} = \ln(0,99)$$$$\frac{t}{\tau} = -\ln(0,99) \approx 0,01005$$

**Jawaban:** Waktu yang harus dilalui adalah sekitar $0,01$ **kali tetapan waktu** ($\tau$). (Catatan: 1% muatan dicapai sangat cepat di awal proses pengisian).

### Soal 3: Resistansi Ekivalen Kapasitor Bocor

**Pertanyaan:** Beda potensial kapasitor ($C = 2 \text{ mF}$) menurun dari $V_0$ menjadi $V = \frac{1}{4} V_0$ dalam waktu $t = 2 \text{ s}$. Hitunglah berapa resistansi ekivalennya?

**Langkah-langkah:**

1. **Identifikasi Proses:**

	Penurunan tegangan tanpa sumber luar berarti proses **pelucutan** (discharging).

2. **Rumus Pelucutan Tegangan:**

	$$V(t) = V_0 e^{-t/RC}$$

3. **Substitusi Nilai yang Diketahui:**
	
	- $V(t) = \frac{1}{4} V_0$
	- $t = 2 \text{ s}$
	- $C = 2 \text{ mF} = 2 \times 10^{-3} \text{ F}$

		$$\frac{1}{4} V_0 = V_0 e^{-2 / (R \cdot 0,002)}$$$$\frac{1}{4} = e^{-1000/R}$$

4. **Mencari Resistansi (**$R$**):**

	Ambil $\ln$ pada kedua ruas:

	$$\ln(1/4) = -\frac{1000}{R}$$$$- \ln(4) = -\frac{1000}{R}$$$$R = \frac{1000}{\ln(4)} \approx \frac{1000}{1,386}$$

	$R \approx 721,34 \text{ } \Omega$

**Jawaban:** Resistansi ekivalen di antara plat-plat kapasitor adalah sekitar $721,3 \text{ } \Omega$.

# BAB 4. Analisis Alat Ukur Listrik: Ammeter dan Voltmeter

Materi ini menjelaskan prinsip kerja, cara pemasangan, dan karakteristik ideal dari alat ukur arus dan tegangan agar hasil pengukuran akurat dan tidak mengganggu kondisi asli rangkaian.

## 1. Ammeter (Amperemeter)

Ammeter adalah alat yang digunakan untuk mengukur kuat arus listrik ($I$) yang mengalir dalam suatu percabangan atau rangkaian.

### A. Cara Pemasangan

- **Secara Seri:** Ammeter harus dipasang secara seri dengan beban atau resistor ($R_L$). Hal ini dilakukan agar arus yang melewati Ammeter sama persis dengan arus yang melewati beban tersebut.
- **Prinsip Kerja:** Karena dipasang seri, Ammeter menjadi bagian dari jalur aliran elektron.

![Ilustrasi pemasangan ammeter.](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772527128047.png)

### B. Karakteristik Ideal ($R_A$)

- **Hambatan Sangat Kecil:** Idealnya, hambatan dalam Ammeter ($R_A$) harus mendekati nol ($R_A \approx 0$).
- **Mengapa?** Berdasarkan Hukum Ohm, total hambatan rangkaian saat diukur adalah $R_{total} = R_L + R_A$.
	- Jika $R_A$ besar, maka hambatan total rangkaian meningkat, yang menyebabkan arus ($I$) mengecil.
	- Jadi, Ammeter yang "buruk" akan mengubah (mengurangi) nilai arus yang sebenarnya ingin ia ukur.
- **Rumus Arus Terukur:**

	$$\epsilon = I(R_L + R_A)$$

	Jika $R_A \approx 0$, maka $I = \frac{\epsilon}{R_L}$ (Nilai arus sebenarnya).

## 2. Voltmeter

Voltmeter adalah alat yang digunakan untuk mengukur beda potensial atau tegangan ($V$) antara dua titik dalam rangkaian.

### A. Cara Pemasangan

- **Secara Paralel:** Voltmeter harus dipasang secara paralel dengan komponen yang ingin diukur tegangannya (misalnya di ujung-ujung resistor $R_L$).
- **Prinsip Kerja:** Dengan dipasang paralel, Voltmeter akan merasakan beda potensial yang sama dengan beban tersebut tanpa harus memutus rangkaian utama.

![Ilustrasi pemasangan voltmeter.|697](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772526940181.png)

### B. Karakteristik Ideal ($R_V$)

- **Hambatan Sangat Besar:** Idealnya, hambatan dalam Voltmeter ($R_V$) harus mendekati tak hingga ($R_V \approx \infty$).
- **Mengapa?** Jika Voltmeter memiliki hambatan kecil, maka sebagian arus dari rangkaian utama akan "bocor" masuk ke dalam Voltmeter.
	- Hal ini akan mengubah konfigurasi rangkaian menjadi rangkaian paralel, yang menurunkan hambatan ekivalen di titik tersebut dan mengubah tegangan yang diukur.
- **Rumus Tegangan Terukur:**

	Jika $R_V$ sangat besar ($R_V \gg R_L$), maka arus yang masuk ke Voltmeter hampir nol ($I_V \approx 0$), sehingga tegangan yang terukur murni merupakan tegangan pada beban:

	$$V = I \cdot R_L$$

## Ringkasan Perbandingan

|   |   |   |
|---|---|---|
|**Fitur**|**Ammeter (Amperemeter)**|**Voltmeter**|
|**Fungsi**|Mengukur Arus Listrik ($I$)|Mengukur Tegangan/Beda Potensial ($V$)|
|**Pemasangan**|**Seri** dengan beban|**Paralel** dengan beban|
|**Hambatan Dalam (**$R_{dalam}$**)**|Harus **Sangat Kecil** ($R_A \to 0$)|Harus **Sangat Besar** ($R_V \to \infty$)|
|**Tujuan Karakteristik**|Agar tidak menambah hambatan total|Agar tidak menyedot arus dari rangkaian|

**Penting:**

Alat ukur yang tidak ideal akan bertindak sebagai "beban tambahan" yang mengubah kondisi asli rangkaian. Oleh karena itu, dalam praktikum, penting untuk memilih alat ukur dengan spesifikasi hambatan dalam yang sesuai dengan beban yang diukur.

## Penyelesaian Soal Fisika Dasar: Alat Ukur

![Ilustrasi soal.](attachments/Materi%20Kuliah%204%20Fisika%20Dasar%20II%20%E2%80%93%20Listrik%20Dinamis%202-1772528320921.png)

Diketahui: $R_V = 307 \text{ } \Omega$, $R_A = 3,62 \text{ } \Omega$.

### Mencari $R_1$ (Metode I - Gambar a)

Pada gambar (a), Voltmeter mengukur tegangan total dari deret Resistor $R_1$ dan Ammeter. Ammeter mengukur arus yang mengalir melalui keduanya.

1. **Data:** $I_a = 0,317 \text{ A}$, $V_a = 28,1 \text{ V}$.
2. **Persamaan:** $V_a = I_a (R_1 + R_A)$.

	$$28,1 = 0,317 (R_1 + 3,62)$$$$R_1 + 3,62 = \frac{28,1}{0,317} \approx 88,64$$$$R_1 = 88,64 - 3,62 = 85,02 \text{ } \Omega$$

	**Jawaban:** $R_1 \approx 85,02 \text{ } \Omega$.

### Mencari $R_2$ (Metode II - Gambar b)

Pada gambar (b), Voltmeter terpasang paralel langsung dengan $R_2$. Ammeter berada di luar, mengukur arus total rangkaian.

1. **Data:** $I_b = 0,356 \text{ A}$, $V_b = 23,7 \text{ V}$.
2. **Arus pada Voltmeter (**$I_V$**):**

	$$I_V = \frac{V_b}{R_V} = \frac{23,7}{307} \approx 0,0772 \text{ A}$$

3. **Arus pada Resistor (**$I_{R2}$**):**

	$$I_{R2} = I_b - I_V = 0,356 - 0,0772 = 0,2788 \text{ A}$$

4. **Hitung** $R_2$**:**

	$$R_2 = \frac{V_b}{I_{R2}} = \frac{23,7}{0,2788} \approx 85,01 \text{ } \Omega$$

	**Jawaban:** $R_2 \approx 85,01 \text{ } \Omega$.

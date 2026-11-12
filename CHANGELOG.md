# Log Sejarah Perubahan (Changelog)

Semua perubahan penting yang telah dilaksanakan pada projek **DartVision Score & Accuracy Tracker** direkodkan dalam dokumen ini mengikut susunan kronologi.

---

## [v1.3.0] — 2026-11-12

### Ditambah (Added)
* **X01 Match Play — Butang Mulakan Semula (*Restart Match & Reset Scoring Counter*)**:
  * Butang mulakan semula pada bar tajuk dan konsol papan skor bagi menetapkan semula baki mata kepada skor asal (`101`, `501`, atau `1001`), mengosongkan giliran, dan menetapkan semula kiraan skor kepada sifar.
* **Accuracy Training — Pemilih Sasaran Bebas Penuh (*Intended Target Selector: 1-20, Double, Triple, Bullseye*)**:
  * Modal pemilihan sasaran intuitif untuk menukar sasaran balingan kepada mana-mana nombor (1 hingga 20), gandaan dua (*Double D1–D20*), gandaan tiga (*Triple T1–T20*), serta Bullseye (*Outer Bull OB 25 / Inner Bull IB 50*).
  * Pilihan untuk menetapkan sasaran bagi setiap dart individu atau ke atas ketiga-tiga dart serentak.
* **Accuracy Training — Butang Reset Counter**:
  * Butang khas untuk menetapkan semula lontaran pusingan semasa dan pembilang bilangan pusingan sesi kepada 0.
* **Accuracy Training — Paparan Keputusan Pembilang Log Tersimpan (*Show Saved Logs Results*)**:
  * Modal semakan arkib log latihan lengkap dengan pembilang agregat (*Total Saved Turns, Total Darts Thrown, Target Hits, Overall Accuracy Rate %*), pecahan sasaran, dan senarai pusingan kronologi.
* **Around the Clock — Paparan Keputusan Pembilang Log Tersimpan (*Show Saved Clock Results*)**:
  * Modal sejarah dan pembilang khusus Around the Clock merangkumi rekod terbaik (*Best Record - fewest darts*), purata lontaran bagi pusingan penuh, status penyelesaian (*Completed / In Progress*), dan senarai sesi tersimpan.

---

## [v1.2.0] — 2026-11-12

### Ditambah (Added)
* **Penanda Pin Fizikal Dart (Dart Pin Markers)**:
  * Paparan visual pin berbayang 3D dan bernombor (①, ②, ③) terus pada permukaan papan dart SVG mengikut koordinat lontaran sebenar.
* **Kanta Pembesar Sentuhan (Touch Loupe)**:
  * Gelembung kanta pembesar bulat terapung di atas jari pengguna pada skrin sentuh telefon untuk memaparkan nama segmen dan markah sebelum jari dilepaskan.
* **Papan Kekunci Pantas (Quick Turn Numpad)**:
  * Mod input alternatif untuk memasukkan terus jumlah skor pusingan (0–180) dengan pintasan angka popular (*26, 41, 45, 60, 81, 85, 100, 140, 180, dan Miss 0*).
* **Pengurusan Format Perlawanan (Legs & Sets Management)**:
  * Sokongan konfigurasi perlawanan berbilang leg (*Single Leg, Best of 3, Best of 5, Best of 7*).
  * Penggiliran pemain pemula (*Throw Alternation*) secara automatik pada setiap leg baharu.
* **Laluan Penamat Adaptif Pintar (Adaptive Checkout Pathways)**:
  * Paparan kad laluan utama (**Plan A**) dan laluan luar jangka (**Plan B**) yang bertukar secara dinamik sekiranya balingan pertama tersasar ke Single.
* **Semakan Vision AI Bersebelahan (Side-by-Side 3-Dart Review)**:
  * Susunan 3 lajur mendatar bagi menyemak hasil imbasan kamera serentak berserta butang pembetulan 1-ketukan bagi segmen alternatif terdekat.
* **4 Rutin Latihan Standard Antarabangsa**:
  * *Free-Throw Target Log*: Pembalak ketepatan sasaran bebas.
  * *Around the Clock*: Cabaran menyasar nombor 1 hingga 20 berturutan sehingga ke Bullseye.
  * *Bob's 27*: Latihan Double klasik berasaskan penambahan dan penolakan skor.
  * *121 Checkout Challenge*: Cabaran menyelesaikan 121 mata dalam 9 dart dengan rekod rentetan kejayaan (*streak*).
* **Peta Haba Radial (Accuracy Heatmap)**:
  * Visualisasi kecerunan suhu pada papan dart di skrin statistik mengikut taburan ketepatan balingan pengguna.

---

## [v1.1.0] — 2026-11-12

### Diubah (Changed)
* **Piawaian Bahasa Antarabangsa**:
  * Menukarkan keseluruhan teks antara muka pengguna (UI), butang, label peraturan, dan mesej ralat ke dalam Bahasa Inggeris bagi memenuhi piawaian kejohanan dart global.

---

## [v1.0.0] — 2026-11-12

### Ditambah (Initial MVP Release)
* **Papan Dart Interaktif WDF**:
  * Geometri vektor SVG 20 sektor piawai dengan warna sisal tradisional, zum 1.4x, butang pembatalan balingan (*Undo*), dan pemilih gandaan (*Multiplier Keypad*).
* **Enjin Skor X01**:
  * Sokongan skor 101, 501, dan 1001 untuk 1–4 pemain tempatan (*Pass-and-Play*).
  * Penguatkuasaan peraturan *Double-Out* dan pengesanan automatik *Bust*.
* **Pengesanan Visual AI (Gemini Vision)**:
  * Pelayan perantara Express memproses gambar kamera menggunakan model `gemini-3.8-flash` dengan skim JSON berstruktur.
* **Storan & Eksport Luar Talian (Offline Storage)**:
  * Penyimpanan 100% pada peranti pengguna menggunakan `localStorage` pelayar web (`dartvision_v1_state`).
  * Sokongan eksport data ke format fail CSV dan JSON serta pemulihan data (*Import*).

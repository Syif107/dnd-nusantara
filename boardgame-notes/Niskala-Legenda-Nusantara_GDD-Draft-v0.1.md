# NISKALA: LEGENDA NUSANTARA
## Game Design Document (GDD) & Rancangan Aturan — Draf v0.1

> **STATUS DOKUMEN: DRAF KERJA / BELUM FINAL**  
> Tanggal penyusunan: 29 Oktober 2026  
> Media awal: **web / virtual tabletop (VTT) 2D**  
> Jenis permainan: **tabletop role-playing game (TTRPG) berbasis sesi**, dengan Dungeon Master (DM) manusia  
> Dokumen ini adalah pegangan diskusi, desain, dan prototipe. **Bukan rulebook final ataupun spesifikasi implementasi yang sudah siap dikodekan seluruhnya.**

---

## 0. Panduan Membaca dan Status Keputusan

Dokumen ini menggabungkan konsep yang telah dibahas dan mengelompokkan tingkat kepastiannya.

- **[ARAH DISEPAKATI]**: pilihan arah proyek yang ditegaskan dalam percakapan.
- **[RANCANGAN SEMENTARA]**: rekomendasi desain yang digunakan sebagai pijakan awal; dapat diganti.
- **[BELUM FINAL]**: aturan, angka, konten, atau keputusan yang belum diputuskan atau belum diuji.
- **[REFERENSI]**: unsur dari dua dokumen sebelumnya atau dari mekanik umum D&D/d20; bukan berarti seluruh aturannya sudah diverifikasi atau boleh disalin mentah-mentah.

**Prioritas ketika ada pertentangan:** tujuan TTRPG Nusantara yang dipilih sekarang menggantikan mekanik *Dungeon!* kompetitif dari dokumen lama. Unsur cerita/tema Nusantara yang bermanfaat tetap menjadi bahan dasar. Keputusan baru yang belum disetujui secara eksplisit tetap bersifat sementara.

### 0.1 Sumber awal

1. `Dungeon-2012-2014-Panduan-Umum.md` — catatan mengenai board game **Dungeon!**, termasuk pengumpulan harta, enam level, room/chamber, dan combat 2d6.
2. `Dungeon-Nusantara-Panduan-Umum.md` — adaptasi tematik **Dungeon Nusantara!**, termasuk Pendopo Agung, Raja Niskala, Candi Nusantara, kelas Nusantara, enam lapisan, pusaka, ajian, dan makhluk.
3. Rancangan percakapan berikutnya yang mengalihkan proyek menjadi **TTRPG penuh bergaya D&D dengan DM**. Sistem d20/kelas/level/combat pada dokumen ini sebagian merupakan *usulan desain baru*, **bukan isi dua dokumen awal**.

### 0.2 Batas pengertian: “board game D&D”

**[ARAH DISEPAKATI]** Yang ingin dibuat adalah pengalaman **D&D tabletop** versi digital:

- Peta/battlemap **2D dari atas**, dapat berupa petak/grid, dengan token karakter, NPC, dan musuh.
- Pemain membuat karakter, bekerja sama, berpetualang, dan mengambil keputusan melalui narasi.
- DM manusia mendeskripsikan dunia, memerankan NPC, menilai tindakan, dan mengelola skenario.
- Sistem web menyediakan dadu digital, character sheet, peta, catatan, aturan combat, dan sinkronisasi sesi.
- Permainan berjalan dalam **room/campaign privat** bersama kelompok kecil, **bukan** dunia massal yang terus berjalan.
- **Bukan 3D RPG, bukan MMORPG, bukan action RPG real-time, bukan game open-world 3D.**
- **Bukan** adaptasi langsung board game *Dungeon!* yang hanya berfokus pada lomba mengumpulkan harta.

Istilah **board game** dipakai secara informal untuk menjelaskan tampilan papan digital. Secara desain, genre yang lebih tepat adalah **tabletop role-playing game / virtual tabletop (TTRPG/VTT)**.

---

# BAGIAN A — VISI DAN BATAS PROYEK

## 1. Identitas Proyek

| Elemen | Keputusan sementara |
|---|---|
| Nama kerja | **Niskala: Legenda Nusantara** — **[BELUM FINAL]** |
| Genre | Fantasy tabletop RPG / narrative cooperative adventure |
| Perangkat awal | Browser desktop, responsif untuk HP; PWA kemudian |
| Perspektif visual | Peta 2D top-down, token dan panel antarmuka |
| Cara bermain | Multiplayer berbasis sesi dengan DM manusia |
| Jumlah pemain ideal | 1 DM + 2–5 pemain **[RANCANGAN SEMENTARA]** |
| Mekanik inti | d20, atribut, skill, saving throw, HP, AC, initiative, turn-based combat |
| Karakter awal | 4 kelas Nusantara, level 1–3 pada MVP |
| Dunia | Fantasi Nusantara orisinal, terinspirasi sejarah, folklor, dan budaya |
| Tujuan sesi | Menjalankan petualangan dan menyelesaikan perkembangan cerita |
| Model kemenangan | Tidak ada pemenang individu berdasarkan jumlah harta |

## 2. Prinsip Desain

1. **Pilihan pemain didahulukan dari animasi.** Dialog, taktik, dan konsekuensi cerita harus menjadi inti pengalaman.
2. **DM tetap berwenang.** Sistem membantu aturan, bukan memaksa satu alur atau menggantikan DM.
3. **Mekanik konsisten dan dapat diaudit.** Semua perubahan signifikan (dadu, HP, item, state quest) memiliki riwayat.
4. **Mudah mulai, dapat bertumbuh.** Awali level 1–3 dan satu petualangan yang benar-benar dapat dimainkan.
5. **Nusantara terasa dalam cerita.** Pengaruh budaya tidak hanya berupa penggantian nama monster atau gambar.
6. **Bebas dari kewajiban MMORPG.** Tidak ada kebutuhan ribuan pemain, grinding, server dunia terbuka, atau ekonomi online masif.
7. **Hormati sumber budaya dan lisensi.** Aset dan tulisan game dibuat orisinal; rujukan lisensi konten terbuka akan diperiksa terpisah.

## 3. Yang Tidak Masuk Rilis Pertama

- Dunia 3D atau lingkungan yang dijelajahi dengan kontrol karakter 3D.
- Gameplay aksi real-time, MMORPG, lobby publik masif, PvP terpusat, atau ekonomi pemain skala besar.
- DM AI sebagai syarat wajib bermain.
- Generator dunia tak terbatas, crafting kompleks, pengelolaan kerajaan, kapal yang disimulasikan penuh.
- Semua kelas/ajian/monster/level 1–20 sekaligus.
- Animasi pertarungan kompleks sebelum aturan inti terbukti berjalan.

---

# BAGIAN B — ALUR PERMAINAN

## 4. Siklus Sesi

**[RANCANGAN SEMENTARA]**

1. DM membuat campaign dan sesi, memilih petualangan/peta, lalu mengundang pemain.
2. Pemain membuat atau memilih karakter dan membaca ringkasan situasi.
3. DM membuka adegan (scene): lokasi, karakter lain, konflik, dan informasi yang tersedia.
4. Pemain menyatakan tindakan secara bebas: berbicara, menyelidiki, bersembunyi, bergerak, menggunakan item, atau bertarung.
5. DM memutuskan apakah tindakan langsung berhasil, membutuhkan pemeriksaan kemampuan/dadu, atau tidak mungkin dilakukan dalam kondisi itu.
6. Sistem menghitung hasil mekanik bila relevan, lalu DM menceritakan akibatnya.
7. Status dunia, quest, karakter, inventaris, dan peristiwa diperbarui.
8. Permainan berlanjut hingga sesi ditutup, lalu disimpan untuk dilanjutkan nanti.

### 4.1 Tiga Pilar Pengalaman

- **Eksplorasi:** menjelajahi desa, hutan, pelabuhan, keraton, candi, ruang rahasia, alam gaib.
- **Interaksi sosial:** berdialog dengan NPC, bernegosiasi, membangun kepercayaan, menyelidiki, dan menentukan aliansi.
- **Pertempuran:** konflik taktis bergiliran di peta 2D, tetapi tidak semua masalah harus diselesaikan dengan kekerasan.

### 4.2 Contoh Pilihan Bebas

> Pemain: “Aku ingin menyamar sebagai utusan kerajaan agar bisa masuk ke candi.”  
> DM: menilai apakah penyamaran masuk akal dan apakah penjaga curiga.  
> Sistem: apabila diminta, melempar `1d20 + modifier Karisma + proficiency yang sesuai` melawan DC yang ditentukan DM.  
> Akibat: berhasil mendapat akses, gagal diminta bukti tambahan, atau memunculkan komplikasi baru. Gagal tidak otomatis menghentikan alur cerita.

---

# BAGIAN C — ATURAN KARAKTER

## 5. Character Sheet

Setiap karakter minimal memiliki:

- Identitas: nama, asal/daerah yang dipilih pemain, penampilan, latar belakang, tujuan, ikatan, ketakutan.
- Kelas, level, XP atau milestone, proficiency bonus.
- Enam atribut dan modifier.
- Skill, saving throw, bahasa, alat/proficiency lain.
- HP maksimum/saat ini/HP temporer, AC, initiative, speed, Hit Dice.
- Senjata, armor, inventory, uang, barang quest, kapasitas bawaan (bila digunakan).
- Ajian/kemampuan kelas, sumber daya tersisa, konsentrasi (bila digunakan), kondisi aktif.
- Catatan hubungan NPC dan jurnal pencapaian.

## 6. Atribut dan Modifier

**[RANCANGAN SEMENTARA]** Enam atribut utama mengikuti pola d20 yang familier:

| Atribut | Kode | Umumnya memengaruhi |
|---|---|---|
| Kekuatan | STR | Kekuatan fisik, Athletics, serangan senjata tertentu |
| Kelincahan | DEX | Stealth, Acrobatics, initiative, pertahanan dan serangan tertentu |
| Ketahanan | CON | HP dan sebagian saving throw |
| Kecerdasan | INT | Investigation, History, pengetahuan, ajian Pawang |
| Kebijaksanaan | WIS | Perception, Insight, Survival, kemampuan Pandhita |
| Karisma | CHA | Persuasion, Deception, Intimidation, Performance |

Modifier atribut:

`modifier = floor((nilai_atribut - 10) / 2)`

Contoh: STR 16 memberikan modifier +3; DEX 8 memberikan modifier -1.

**Pembagian atribut awal [RANCANGAN SEMENTARA]:** `15, 14, 13, 12, 10, 8`, dibagikan sesuai pilihan pemain. Bonus latar belakang +2 ke satu atribut dan +1 ke atribut lain pernah diusulkan, tetapi **detail batas dan variasinya belum final**.

## 7. Kelas Awal

Empat nama kelas berasal dari dokumen `Dungeon-Nusantara-Panduan-Umum.md`, tetapi mekanik RPG di bawah adalah pengembangan baru.

| Kelas | Peran | Atribut utama | Hit Die | Kemampuan awal contoh |
|---|---|---|---|---|
| **Ksatria** | Petarung garis depan / pelindung | STR atau DEX | d10 | **Teguh Berdiri**: mengurangi damage dalam batas tertentu |
| **Pandhita** | Dukungan / pemulihan / penuntun | WIS | d8 | **Restu Penjaga**: melindungi atau membantu rekan |
| **Telik Sandi** | Pengintai / infiltrator / serangan presisi | DEX | d8 | **Serangan Celah**: bonus damage bila syarat taktis terpenuhi |
| **Pawang** | Pengguna ajian / kontrol area / ilusi | INT | d6 | Ajian dasar dan sumber daya sihir terbatas |

> **[BELUM FINAL]** Nama, besaran efek, jarak, penggunaan per istirahat, equipment awal, proficiency, dan progression setiap kemampuan kelas. Jangan mengimplementasikan kemampuan hanya dari deskripsi satu kalimat di atas.

### 7.1 Latar Belakang (contoh)

| Latar | Contoh skill | Arah naratif |
|---|---|---|
| Pelaut Kepulauan | Survival, pengetahuan navigasi | Paham rute laut dan cuaca |
| Juru Tulis Kerajaan | History, Investigation | Meneliti prasasti dan arsip |
| Perajin Pusaka | Investigation, alat perajin | Mengenali teknik dan artefak |
| Pengembara Rimba | Nature, Survival | Terbiasa menelusuri alam |
| Utusan Keraton | Persuasion, Insight | Etiket dan diplomasi |
| Penjaga Perbatasan | Athletics, Perception | Penjagaan dan kewaspadaan |

**[RANCANGAN SEMENTARA]** Asal budaya/daerah dapat dipilih sebagai identitas dan pengaruh cerita; tidak otomatis menentukan kecerdasan, moralitas, atau keunggulan biologis karakter.

### 7.2 Skill awal yang dipertimbangkan

| Atribut | Skill yang umum dipakai |
|---|---|
| STR | Athletics |
| DEX | Acrobatics, Sleight of Hand, Stealth |
| INT | Arcana, History, Investigation, Nature, Religion |
| WIS | Animal Handling, Insight, Medicine, Perception, Survival |
| CHA | Deception, Intimidation, Performance, Persuasion |

Nama Indonesia, cakupan tiap skill, dan nama skill yang berhubungan dengan pengetahuan tradisi/kepercayaan **[BELUM FINAL]**.

## 8. Level dan Perkembangan

**[RANCANGAN SEMENTARA]** Gunakan *Milestone Leveling*: DM menaikkan level setelah pencapaian cerita bermakna.

| Level | Gambaran perkembangan |
|---|---|
| 1 | Identitas kelas, atribut, kemampuan dasar |
| 2 | Kemampuan kelas tambahan |
| 3 | Jalur spesialisasi/subkelas |
| 4 | Peningkatan atribut atau feat |
| 5 | Peningkatan kekuatan penting menurut kelas |
| 6–20 | Dirancang dan diuji setelah sistem awal stabil |

**MVP hanya mengimplementasikan level 1–3.** Struktur data sebaiknya tidak mengunci batas maksimum level menjadi 3, tetapi katalog progresi lebih tinggi **belum perlu dibuat**.

---

# BAGIAN D — MEKANIK D20

## 9. Aturan Pemeriksaan

Pemeriksaan kemampuan ketika hasil tindakan benar-benar tidak pasti:

`1d20 + modifier_atribut + proficiency_bonus (jika mahir) + modifier_situasional >= DC`

**[RANCANGAN SEMENTARA]** DC dasar:

| Kategori | DC |
|---|---:|
| Sangat mudah | 5 |
| Mudah | 10 |
| Sedang | 15 |
| Sulit | 20 |
| Sangat sulit | 25 |
| Hampir mustahil | 30 |

- **Advantage:** lempar 2d20, ambil angka tertinggi.
- **Disadvantage:** lempar 2d20, ambil angka terendah.
- **Saving Throw:** pemeriksaan bertahan dari ancaman, ajian, jebakan, atau efek lain.
- **Passive Check:** dapat digunakan sebagai `10 + semua bonus relevan`, tanpa lempar dadu aktif.
- **Proficiency Bonus:** mulai +2 pada level 1–4, +3 pada level 5–8, lalu meningkat sesuai tabel progresi yang akan ditetapkan.
- DM tidak perlu meminta dadu untuk setiap gerakan biasa, tindakan tanpa risiko, atau tindakan yang pasti mustahil.
- **Natural 20/1:** hasil khusus otomatis terutama perlu didefinisikan untuk serangan dan death save; **jangan mengasumsikan semua ability check otomatis sukses/gagal hanya karena hasil 20/1**.

**[BELUM FINAL]** Tabel penuh proficiency per level, aturan stacking bonus, passive check dalam berbagai kondisi, critical, serta pembulatan/modifier spesial.

## 10. Eksplorasi dan Waktu

- **Di luar combat:** karakter menyatakan tujuan dan tindakan; DM menentukan jarak, waktu, hambatan, dan pemeriksaan yang perlu. Tidak dibatasi “5 langkah per giliran” seperti dalam board game *Dungeon!*.
- **Saat combat:** digunakan sistem grid pada peta 2D.
- **Skala grid awal:** 1 petak = 1,5 meter (≈ 5 kaki).
- **Kecepatan dasar contoh:** 9 meter per giliran = 6 petak.
- **Medan sulit:** biaya gerak dua kali lipat.
- **Fog of war:** hanya DM yang melihat informasi rahasia; pemain melihat area sesuai penemuan/visi.
- **Jalur alternatif:** eksplorasi tidak harus linear atau selalu melalui pertarungan.

**[BELUM FINAL]** Line of sight, jangkauan cahaya, darkness, cover, gerakan diagonal, pintu, pendakian, berenang, terbang, perjalanan jauh, dan kebutuhan persediaan.

## 11. Interaksi Sosial dan Cerita

NPC harus memiliki minimal: identitas, tujuan, sikap terhadap kelompok, pengetahuan, rahasia yang diketahui DM, dan konsekuensi pilihan pemain.

Tindakan dapat diselesaikan dengan:

1. **Roleplay langsung:** percakapan dan keputusan naratif.
2. **Skill check:** ketika ada risiko atau ketidakpastian.
3. **Persyaratan dunia:** surat izin, barang bukti, hubungan/kepercayaan, atau fakta yang sudah ditemukan.

Hasil kegagalan dapat menimbulkan komplikasi, biaya, waktu tambahan, atau jalur alternatif; jangan selalu membuat cerita buntu.

**[BELUM FINAL]** Sistem reputasi, hubungan NPC, pengaruh faksi, serta format kondisi percabangan quest.

---

# BAGIAN E — PERTEMPURAN TAKTIS

## 12. Kerangka Combat

**[RANCANGAN SEMENTARA]** Combat berlangsung **turn-based** pada peta 2D.

1. DM meletakkan token karakter, monster, dan elemen arena.
2. Peserta melempar **Initiative**: `1d20 + modifier DEX`.
3. Sistem mengurutkan giliran.
4. Karakter aktif dapat menggunakan gerak dan Action; Bonus Action hanya bila kemampuan mengizinkan; Reaction aktif pada pemicu yang sah.
5. Sistem menghitung hit, damage, pengurangan HP, kondisi, resource, dan efek.
6. Setelah semua peserta bertindak, ronde baru dimulai.

### 12.1 Istilah utama

- **HP (Hit Points):** daya tahan; dapat berkurang akibat damage.
- **AC (Armor Class):** target angka untuk serangan tertentu agar mengenai.
- **Attack Roll:** `1d20 + bonus_serangan`, dibandingkan dengan AC target.
- **Damage Roll:** bergantung pada senjata atau ajian, misalnya `1d6 + modifier`, jika mengenai.
- **Critical Hit:** serangan natural 20 memiliki aturan damage khusus; detail implementasi perlu ditetapkan.
- **Condition:** status seperti Poisoned, Frightened, Prone, Restrained, Unconscious, dan sebagainya.
- **Concentration:** batas mempertahankan sebagian ajian, bila sistem ajian memakai mekanik tersebut.

### 12.2 Contoh perhitungan (bukan stat block final)

- Telik Sandi mendapat `d20 = 11` dan bonus serangan `+5` → hasil total **16**.
- Penjaga Lumut memiliki `AC = 13` → serangan mengenai.
- Senjata memberi `1d6 + 3`; bila d6 menghasilkan `4`, damage = **7** sebelum resistansi/efek lain.

### 12.3 Daftar Action yang dipertimbangkan

Attack, Cast a Spell / Gunakan Ajian, Dash, Disengage, Dodge, Help, Hide, Ready, Search, dan Use an Object / Interact. Mekanik, syarat, dan penamaan tiap Action **[BELUM FINAL]**.

### 12.4 Ketika HP mencapai 0

**[RANCANGAN SEMENTARA]**

- Karakter umumnya jatuh tidak sadar dan dapat diselamatkan; 0 HP tidak otomatis berarti mati.
- Saat gilirannya tiba, karakter melakukan **Death Saving Throw**.
- Tiga keberhasilan membuat karakter stabil; tiga kegagalan menyebabkan kematian.
- Hasil natural 1, natural 20, damage ketika sekarat, serta pemulihan HP memiliki aturan khusus yang harus dibakukan di rulebook final.
- **Short Rest** dan **Long Rest** tersedia untuk pemulihan, dengan durasi awal yang dipertimbangkan sekitar 1 jam dan 8 jam.

**[BELUM FINAL]** Detail death save, perubahan urutan giliran, healing pada 0 HP, stabilisasi, istirahat, penggunaan Hit Dice, critical damage, cover, opportunity attack, surprise, dan seluruh kondisi.

---

# BAGIAN F — AJIAN, ITEM, DAN EKONOMI

## 13. Sistem Ajian

**[RANCANGAN SEMENTARA]** Ajian menggunakan pendekatan **cantrip/ajian dasar** dan **Spell Slot** sebagai sumber daya untuk ajian tingkat lebih tinggi. Ini **menggantikan** sistem kartu ajian sekali pakai pada board game *Dungeon Nusantara!* sebelumnya.

- **Pawang:** ajian unsur, ilusi, dan kontrol medan.
- **Pandhita:** pemulihan, pertahanan, perlindungan, dan dukungan.
- Ajian memiliki data: nama, level/tingkat, kelas pengguna, waktu cast, jarak, target/area, komponen (jika dipakai), durasi, konsentrasi (jika dipakai), damage/heal, saving throw, efek, dan penggunaan resource.

### 13.1 Kandidat Ajian Awal

| Ajian | Tingkat contoh | Gagasan efek | Status |
|---|---|---|---|
| Bara Niskala | Dasar | Proyektil api | Belum final |
| Bayang Semu | Dasar | Ilusi sederhana | Belum final |
| Angin Selasar | 1 | Bergerak cepat / lolos dari ancaman | Belum final |
| Belenggu Akar | 1 | Menghambat satu target | Belum final |
| Embun Pulih | 1 | Memulihkan HP | Belum final |
| Restu Penjaga | 1 | Mengurangi damage atau melindungi teman | Belum final |

> Nama dan efek ini adalah **konsep orisinal sementara**. Belum ada angka kerusakan, batasan jangkauan, target, durasi, atau perhitungan yang disahkan.

## 14. Equipment dan Pusaka

- **Peralatan biasa:** senjata, pelindung, pakaian, alat tulis, perlengkapan perjalanan, lampu, peralatan pengobatan.
- **Item consumable:** ramuan, bahan ritual, perbekalan, alat sekali pakai.
- **Item quest:** prasasti, surat, peta, segel, petunjuk.
- **Pusaka penting:** artefak yang terhubung dengan cerita utama.
- **Keping Emas (KE):** nama mata uang dari dokumen tematik terdahulu; statusnya sebagai mata uang umum atau hanya satu jenis nilai **[BELUM FINAL]**.

**[BELUM FINAL]** Statistik semua senjata/armor, harga, beban, rarity, attunement (jika dipakai), interaksi item, looting, perdagangan, dan aturan pembagian hadiah.

---

# BAGIAN G — DUNIA FANTASI NUSANTARA

## 15. Premis Utama

**[REFERENSI DARI DOKUMEN NUSANTARA, DIKEMBANGKAN]**

Empat pusaka penting penjaga keseimbangan Nusantara hilang setelah campur tangan **Raja Niskala**. Berbagai jejak sejarah, kerajaan, legenda, dan alam gaib saling terhubung oleh sebuah misteri. Para petualang menghadapi konflik lokal dan perlahan menemukan hubungan antara hilangnya pusaka dengan ancaman terhadap keseimbangan dunia.

**Perubahan dari board game lama:** para petualang **bekerja sama** menjalani cerita; tidak berlomba mengumpulkan Keping Emas dan pulang pertama ke Pendopo Agung.

### 15.1 Posisi Pendopo Agung

Pendopo Agung masih dipertahankan sebagai **lokasi ikonik** yang dapat berperan sebagai titik awal, pusat pertemuan faksi, atau markas petualang. Fungsinya sebagai *start/finish otomatis untuk memenangkan game* **dihapus**.

### 15.2 Enam wilayah / bab awal

Enam lapisan lama berubah menjadi **wilayah dan alur petualangan**, bukan urutan dungeon yang harus dilewati seperti papan kompetitif.

| Bab | Wilayah | Contoh aktivitas dan konflik |
|---|---|---|
| 1 | **Alas Kutai** | Hutan, sungai, jejak prasasti, hilangnya seseorang, pengenalan eksplorasi |
| 2 | **Pesisir Tarumanegara** | Desa, banjir, prasasti, sengketa, investigasi dan diplomasi |
| 3 | **Selat Sriwijaya** | Pelabuhan, perdagangan, perjalanan laut, aliansi dan intrik |
| 4 | **Teras Mataram Kuno** | Kompleks candi, teka-teki, pengetahuan, ruang tersembunyi |
| 5 | **Keraton Majapahit** | Faksi, intrik kekuasaan, pengkhianatan, rahasia sejarah dunia fantasi |
| 6 | **Alam Niskala** | Dunia supernatural, asal konflik, keputusan besar, Raja Niskala |

**[BELUM FINAL]** Lokasi di peta dunia, hubungan antarwilayah, waktu tempuh, akses non-linear, aktor utama, faksi, kota, sublokasi, dan mekanisme transisi antar-bab.

**Catatan budaya:** kerajaan-kerajaan ini berasal dari era berbeda; dalam game dihubungkan melalui **dunia fantasi lintas ruang/zaman**, bukan klaim bahwa semuanya hidup berdampingan dalam sejarah nyata. Cerita, ilustrasi, dan karakter harus membedakan imajinasi dari rujukan sejarah. Cakupan Nusantara perlu diperluas melampaui lokasi awal dengan penelitian dan representasi yang cermat.

## 16. Makhluk, NPC, dan Faksi

Dokumen lama menyebut folklor seperti Tuyul, Genderuwo, Kuntilanak, Leak, Rangda, Wewe Gombel, dan berbagai tokoh legenda/wayang. Daftar itu **belum otomatis menjadi monster untuk dibunuh** dalam TTRPG baru.

Prinsip desain:

1. NPC/makhluk bisa bersahabat, netral, penuh misteri, atau bermusuhan sesuai konteks cerita.
2. Stat block orisinal dibuat berdasarkan peran dan kesulitan permainan, bukan sekadar stereotip budaya.
3. Tokoh/figur yang memiliki makna religius atau sakral diperlakukan dengan perhatian khusus.
4. Nama budaya tidak boleh mengaburkan mana sumber sejarah/folklor dan mana rekaan game.

**[BELUM FINAL]** Monster bestiary, stat block, CR/tingkat ancaman, bahasa, motif, perilaku, drop item, dan penempatan encounter.

## 17. Empat Pusaka Utama

**[BELUM FINAL]** Dokumen awal menyebut empat pusaka, tetapi belum mendefinisikan secara final keempat nama, asal, penjaga, kekuatan, biaya pemakaian, dan perannya dalam pilihan akhir. Pusaka ini harus diputuskan sebelum menyusun campaign utama lengkap.

---

# BAGIAN H — PERAN DUNGEON MASTER

## 18. Tanggung Jawab DM

DM bertugas:

- Membuat campaign, sesi, dan adegan.
- Menarasikan lokasi dan situasi.
- Memerankan NPC dan mengendalikan monster.
- Memutuskan kapan sebuah aksi memerlukan dadu dan berapa DC-nya.
- Membuka area peta dan informasi yang diketahui pemain.
- Mengelola quest, hadiah, konsekuensi, dan keputusan cerita.
- Menangani improvisasi dan penerapan aturan khusus (*rulings*).
- Mengakhiri sesi dengan catatan progres.

### 18.1 Alat bantu DM dalam web

| Panel | Fungsi |
|---|---|
| Campaign Manager | Membuat/mengelola kelompok, undangan, jadwal sesi (opsional) |
| Scene & Story Notes | Narasi, catatan rahasia, dialog, petunjuk, percabangan |
| Map Editor / Tabletop | Peta 2D, posisi token, fog of war, terrain |
| NPC/Monster Manager | Stat block, HP, kondisi, perilaku, jurnal NPC |
| Encounter/Initiative Tracker | Urutan giliran, ronde, aksi, kondisi |
| Dice & Rule Override | Roll terbuka/rahasia; penyesuaian DM yang tercatat |
| Quest/World State | Tujuan dan konsekuensi yang menetap |
| Session Recap | Rangkuman hasil sesi untuk pertemuan berikutnya |

### 18.2 Batasan wewenang sistem

- Sistem **otomatis** menghitung rumus mekanik standar bila diaktifkan.
- DM **memutuskan** fakta naratif, tindakan layak, perilaku NPC, dan pengecualian kasus tertentu.
- DM dapat mengubah hasil/state melalui kontrol khusus, **tetapi perubahan dicatat** demi kejelasan.
- Data rahasia DM **tidak boleh dikirim** kepada klien pemain yang tidak memiliki izin melihatnya.
- AI DM **bukan bagian wajib** versi pertama.

---

# BAGIAN I — KAMPANYE CONTOH

## 19. Campaign 001: Misteri Prasasti yang Retak

**[RANCANGAN SEMENTARA]** Petualangan pembuka untuk karakter level 1.

### Premis

Seorang juru ukir menghilang setelah menemukan prasasti yang memuat petunjuk menuju salah satu pusaka. Kelompok petualang diminta menyelidiki.

### Adegan kandidat

1. **Pendopo atau desa awal:** menerima permintaan bantuan, mengenal NPC, menentukan rencana.
2. **Rumah dan tempat kerja juru ukir:** menemukan beberapa petunjuk melalui pengamatan, tanya jawab, atau investigasi.
3. **Jalur menuju hutan/ruin:** eksplorasi, bahaya alam, atau perjumpaan dengan penjaga.
4. **Reruntuhan prasasti:** teka-teki, pilihan damai atau pertarungan, terungkapnya informasi utama.
5. **Penutup:** menyelesaikan situasi juru ukir dan mencatat akibat keputusan kelompok.

### Jalur solusi alternatif

- Negosiasi dengan penjaga daripada langsung menyerang.
- Menyelidiki fragmen prasasti tanpa mengikuti rute utama.
- Meminta bantuan warga atau ahli lokal.
- Menemukan bukti melalui beberapa sumber sehingga satu kegagalan dadu tidak mengunci seluruh campaign.

**[BELUM FINAL]** Nama NPC, peta, DC tiap tantangan, ancaman encounter, solusi teka-teki, hadiah, cabang ending, dan durasi sesi. Ini *outline*, bukan modul petualangan siap dijalankan.

---

# BAGIAN J — APLIKASI WEB VIRTUAL TABLETOP

## 20. Pengalaman Pemain

Tampilan pemain ideal memiliki:

1. **Peta tengah**: battlemap 2D, grid bila diperlukan, token, marker, area yang sudah ditemukan.
2. **Panel karakter**: HP, AC, resource, status, skill, ajian, inventaris.
3. **Panel cerita**: narasi DM, dialog/chat, jurnal quest, catatan.
4. **Panel dadu dan aksi**: roll sesuai kemampuan, log perhitungan, giliran combat.
5. **Panel kelompok**: ringkasan karakter rekan dan inisiatif (sesuai hak akses).

Desktop dapat memakai beberapa panel bersamaan. Di HP, panel dapat berpindah melalui tab/drawer agar peta tetap mudah digunakan.

## 21. Lobby, Room, dan Sesi

**[RANCANGAN SEMENTARA]**

- DM membuat campaign dan room.
- Pemain masuk dengan undangan/kode.
- Setiap pemain memilih satu karakter yang terdaftar dalam campaign.
- Sesi memiliki status: `preparing`, `active`, `paused`, `ended`.
- Sesi bisa dijeda dan dilanjutkan tanpa mengulang semua state permainan.
- Jika pemain terputus, progres yang sudah disimpan tidak hilang; kebijakan pergantian giliran saat disconnect **[BELUM FINAL]**.

## 22. Modul dan Data Minimum

| Entitas | Data minimum |
|---|---|
| User | ID, akun, preferensi |
| Campaign | ID, DM, anggota, aturan, world state, daftar sesi |
| Session | ID, campaign, current scene, status, waktu, catatan |
| Character | Atribut, kelas, level, HP, AC, skill, sumber daya, inventory |
| Scene | Narasi, objek, NPC, quest terkait, visibility |
| Map | Gambar/tiles, grid, ukuran, terrain, area tersembunyi |
| Token | ID, pemilik, posisi, HP/kondisi atau referensi ke karakter/NPC |
| NPC/Monster | Identitas, stat block, hubungan, flags |
| Encounter | Combatants, initiative, round, active turn, conditions |
| Action | Aktor, jenis aksi, target, parameter, validasi, hasil |
| Ajian/Item | Data mekanik, prasyarat, durasi/charges, efek |
| Quest | Status, tujuan, petunjuk, konsekuensi, hubungan antarscene |
| Dice Log | Jenis dadu, hasil mentah, modifier, total, pelaku, scope publik/rahasia |
| Game Event | Riwayat perubahan state dan catatan override DM |

### 22.1 Prinsip implementasi penting

- **Server-authoritative:** server memvalidasi gerakan, giliran, penggunaan resource, hasil dadu, damage, dan mutasi state yang berakibat mekanik.
- **Permission & secrecy:** GM-only notes/fog/NPC rahasia tidak dikirim ke pengguna yang tidak berhak.
- **Deterministic rules engine:** kalkulasi terpisah dari UI; perubahan aturan dapat dites otomatis.
- **Event log:** rekam alasan perubahan status agar bug dapat diperiksa dan sesi dapat direkonstruksi jika memungkinkan.
- **Penyimpanan persisten:** campaign dan sesi dapat dilanjutkan setelah keluar dari browser.
- **Aksesibilitas:** teks narasi tetap terbaca, input keyboard dan penggunaan HP diperhatikan.

## 23. Rekomendasi Teknologi

**[RANCANGAN SEMENTARA; BUKAN KEPUTUSAN TEKNIS FINAL]**

- **Frontend:** React / Next.js + TypeScript.
- **Peta sederhana pertama:** SVG dan drag-and-drop token; untuk kebutuhan peta rumit bisa beralih ke renderer seperti PixiJS.
- **Backend:** TypeScript, layanan API, dan rules engine terpisah.
- **Database:** PostgreSQL.
- **Real-time sync:** WebSocket atau teknologi real-time setara.
- **Asset storage:** penyimpanan file untuk peta, token, portrait, dan lampiran sesi.
- **Mobile:** responsif; PWA setelah pengalaman mobile layak.

Pilihan framework final perlu ditetapkan setelah kebutuhan performa, skalabilitas, dan tim developer diketahui.

---

# BAGIAN K — MVP DAN TAHAP PENGEMBANGAN

## 24. Batas MVP

| Bagian | Batas rilis pertama (target) |
|---|---|
| Role | DM dan pemain |
| Pemain | 1 DM + 2–5 pemain |
| Karakter | 4 kelas, level 1–3 |
| Skenario | 1 petualangan pembuka yang selesai dimainkan |
| Peta | ±3 peta utama 2D |
| Monster | ±6 jenis orisinal dengan stat block |
| Ajian | ±6–12 ajian yang sudah diuji |
| Item | ±10–15 item |
| Gameplay | Narasi, skill check, eksplorasi, combat, loot/item, quest |
| Multiplayer | Room privat, sinkronisasi status, penyimpanan sesi |
| DM | Pengelolaan scene, token, encounter, DC, informasi rahasia |
| Non-target | 3D RPG, MMO, open world, AI DM wajib |

Angka konten ini **[RANCANGAN SEMENTARA]** dan dapat dikurangi ketika kebutuhan prototipe terukur.

## 25. Tahapan Kerja

1. **Game Rules Specification**: rumus lengkap dan seluruh state/mekanik dapat diuji.
2. **World Bible**: lore, wilayah, faksi, NPC, relasi, empat pusaka, etika budaya.
3. **Petualangan pembuka**: desain scene, tantangan, petunjuk, hasil alternatif.
4. **Prototype UI/UX**: pembuatan karakter, meja 2D, panel DM, satu encounter.
5. **Rules engine**: sistem dadu, skill, initiative, aksi, HP, kondisi, resource.
6. **Multiplayer & persistence**: room, sinkronisasi, server validation, save/resume.
7. **Playtest**: kejelasan aturan, durasi giliran, beban kerja DM, balancing kelas/encounter, bug.
8. **Revisi**: mengunci rulebook MVP dan baru kemudian memperluas konten.

### 25.1 Kriteria MVP dianggap selesai

- Sekelompok pemain dapat membuat karakter dan bergabung ke sesi DM.
- DM dapat membuka scene, membagikan informasi, dan mengelola NPC.
- Pemain dapat bergerak pada peta 2D dan melihat pembatasan akses yang benar.
- Pemeriksaan kemampuan dan satu combat lengkap dapat dilakukan tanpa hitungan manual wajib.
- HP, resource, status, inventaris, dan quest tetap sinkron.
- Sesi dapat disimpan, ditutup, dibuka kembali, dan dilanjutkan.
- Pemain tidak dapat melihat catatan rahasia DM melalui aplikasi biasa.
- Petualangan pembuka punya akhir yang dapat dicapai lewat lebih dari satu pendekatan.

---

# BAGIAN L — DAFTAR BELUM FINAL / AGENDA DISKUSI

## 26. Keputusan Utama yang Masih Terbuka

Urutan ini disarankan untuk diskusi berikutnya. **Jangan menganggap opsi contoh sebagai keputusan pengguna.**

| Prioritas | Topik | Pertanyaan keputusan | Status |
|---|---|---|---|
| **P0** | Basis aturan | Seberapa dekat ke SRD 5.2.1, dan bagian mana dibuat orisinal? | **BELUM FINAL** |
| **P0** | Core dice & checks | Rumus final, proficiency, advantage, natural 1/20, DC, saving throw? | **BELUM FINAL** |
| **P0** | Character creation | Atribut awal, bonus latar, pilihan skill, starting equipment? | **BELUM FINAL** |
| **P0** | Kelas 1–3 | Setiap fitur, resource, subkelas, dan progression empat kelas? | **BELUM FINAL** |
| **P0** | Combat | Action economy, senjata, critical, damage, cover, gerakan, reaction? | **BELUM FINAL** |
| **P0** | HP & rest | Hit Points awal, healing, death save, short/long rest dan kondisi? | **BELUM FINAL** |
| **P0** | Ajian | Slots/cantrips, daftar awal, durasi, saving, area, concentration? | **BELUM FINAL** |
| **P0** | Hak DM | Batas override, roll rahasia, apa yang dihitung otomatis? | **BELUM FINAL** |
| **P1** | Peta & eksplorasi | Grid persegi/heksagonal, diagonal, line of sight, fog, skala? | **BELUM FINAL** |
| **P1** | Multiplayer UX | Alur undangan, giliran saat disconnect, chat, izin dan reconnect? | **BELUM FINAL** |
| **P1** | Bestiary & encounter | 6 monster awal, stat block, tingkat bahaya, hadiah? | **BELUM FINAL** |
| **P1** | Campaign awal | Petualangan prasasti, NPC, tiga peta, quest, percabangan? | **BELUM FINAL** |
| **P1** | Empat pusaka | Nama, asal, kemampuan, hubungan dengan Raja Niskala? | **BELUM FINAL** |
| **P1** | Identitas dan budaya | Nama final, perluasan wilayah, riset folklor, batas representasi? | **BELUM FINAL** |
| **P2** | Ekonomi | KE, harga, inventaris, kapasitas, perdagangan, rarity? | **BELUM FINAL** |
| **P2** | Level 4–20 | Progresi tinggi dan ekspansi kelas/subkelas? | **BELUM FINAL** |
| **P2** | AI assistance | Jika nanti ada, hanya pembantu DM atau mode lain? | **BELUM FINAL** |
| **P2** | Tampilan & audio | Gaya ilustrasi, tipografi, ikon, efek, suara? | **BELUM FINAL** |
| **P2** | Platform lanjutan | PWA offline, dukungan HP, tablet, atau aplikasi native? | **BELUM FINAL** |

### 26.1 Saran urutan pembahasan berikutnya

**Sesi desain 1 — Core Rules:** mulai dari ketergantungan terhadap SRD, kemudian character creation, empat kelas level 1–3, aturan cek, dan combat. Hasilnya berupa *Rules Specification v0.2*.

**Sesi desain 2 — Dungeon Master & Eksplorasi:** hak DM, cara mengelola cerita, peta 2D, fog of war, percabangan quest, interaksi sosial.

**Sesi desain 3 — Nusantara World Bible:** dunia, lintas zaman, empat pusaka, Raja Niskala, NPC, bestiary, riset budaya.

**Sesi desain 4 — MVP Web:** struktur database, UX pemain/DM, otorisasi, rules engine, sinkronisasi, dan kriteria tes.

## 27. Risiko Desain yang Sudah Diketahui

1. **Scope creep:** memulai dengan semua mekanik D&D dapat membuat aplikasi tak pernah mencapai versi playable.
2. **Aturan belum lengkap:** deskripsi fitur satu kalimat belum cukup untuk pengembangan rules engine.
3. **Benturan sumber:** dokumen *Dungeon!* lama dan sistem RPG d20 berbeda; jangan mencampur aturan tanpa keputusan.
4. **Beban DM:** panel terlalu rumit membuat DM lebih banyak mengatur UI daripada bercerita.
5. **Balancing:** kemampuan kelas/ajian orisinal memerlukan playtest; tidak cukup hanya terasa menarik di atas kertas.
6. **Kebocoran rahasia:** informasi DM harus dibatasi pada tingkat server/API, bukan sekadar disembunyikan CSS.
7. **Hak cipta dan lisensi:** jangan menyalin peta/kartu/ilustrasi/teks berlisensi; kelayakan penggunaan SRD dan kewajiban atribusi perlu diperiksa sebelum publikasi.
8. **Representasi budaya:** gabungan folklor, tokoh wayang, dan kerajaan harus jelas sebagai fantasi; pilih dan kaji penggunaan figur sakral secara hati-hati.

---

# BAGIAN M — RINGKASAN KEPUTUSAN SEMENTARA

## 28. Yang Sudah Jelas

- **Jenis game:** tabletop RPG bergaya D&D berbasis **board/map 2D**, **bukan 3D RPG/MMORPG**.
- **Cara main:** kelompok pemain + DM manusia, petualangan kooperatif berbasis narasi/sesi.
- **Platform pertama:** web; dapat dipakai desktop dan kelak mobile/PWA.
- **Arah dunia:** fantasi Nusantara; mengambil elemen Pendopo Agung, Raja Niskala, kelas Nusantara, dan enam wilayah dari dokumen tematik.
- **Arah mekanik:** d20, atribut, skill, HP, AC, initiative, grid saat combat, perkembangan karakter.
- **Cara kerja:** core rules dan prototipe playable lebih dulu daripada ekspansi fitur besar.

## 29. Yang Sengaja Belum Dikunci

Semua angka, kemampuan kelas, efek ajian, detail aturan combat, monster, encounter, cerita kampanye, nama produk akhir, aset, dan keputusan teknologi terperinci yang telah diberi label **[BELUM FINAL]** harus dibahas dan diuji dahulu. Dokumen ini **cukup untuk memulai pembahasan desain terstruktur**, tetapi **belum cukup untuk langsung menyerahkan seluruh game kepada programmer tanpa spesifikasi lanjutan**.

## 30. Perubahan dari Dokumen Lama (Agar Tidak Bingung)

| Unsur | Dungeon! / Dungeon Nusantara! lama | Niskala TTRPG baru |
|---|---|---|
| Genre | Board game kompetitif | Tabletop RPG kooperatif |
| Pengelola cerita | Tidak perlu DM | DM manusia |
| Tujuan | Kumpulkan treasure, kembali ke hall tercepat | Menjalani dan menyelesaikan petualangan |
| Dadu utama | 2d6 untuk combat sederhana | d20 untuk cek/serangan, dadu lain untuk efek/damage |
| Movement | Hingga 5 spasi per giliran | Bebas naratif; grid saat combat |
| Kelas | 4 kelas statis dengan target harta | 4 kelas RPG dengan fitur, HP, skill, level |
| Kartu ajian | Kartu sekali pakai | Ajian dan resource/slot |
| Monster | Target angka berdasarkan kelas | Stat block, HP, AC, aksi, kondisi |
| Pendopo Agung | Titik start dan kemenangan | Lokasi naratif penting, fungsi final belum dikunci |
| Enam level | Kedalaman dungeon | Enam wilayah/bab dunia fantasi |

---

**Penanda revisi selanjutnya:** setelah topik P0 disepakati, naikkan dokumen ini menjadi `v0.2` dan buat lampiran aturan rinci tanpa mengubah keputusan dasar bahwa game adalah **virtual tabletop 2D, bukan MMORPG**.

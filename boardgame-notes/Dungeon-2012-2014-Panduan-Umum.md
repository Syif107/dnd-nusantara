# Dungeon! (2012 / 2014) — Panduan Umum

> Catatan belajar board game.
> Versi ini masih **umum** — aturan inti, komponen, dan alur main.
> Detail kecil (tabel lengkap kartu, edge case, varian solo) akan ditambahkan belakangan.

---

## Daftar Isi

1. [Ringkasan](#1-ringkasan)
2. [Sejarah singkat](#2-sejarah-singkat)
3. [Komponen](#3-komponen)
4. [Setup](#4-setup)
5. [Alur giliran](#5-alur-giliran)
6. [Gerak & pintu rahasia](#6-gerak--pintu-rahasia)
7. [Combat](#7-combat)
8. [Room vs Chamber](#8-room-vs-chamber)
9. [Treasure & kondisi menang](#9-treasure--kondisi-menang)
10. [Spell Wizard](#10-spell-wizard)
11. [Trap](#11-trap)
12. [Mati & mulai ulang](#12-mati--mulai-ulang)
13. [Varian](#13-varian)
14. [Tips main](#14-tips-main)
15. [Beda 2012 vs 2014](#15-beda-2012-vs-2014)
16. [Istilah](#16-istilah)
17. [Yang mau diperdalam nanti](#17-yang-mau-diperdalam-nanti)
18. [Sumber](#18-sumber)

---

## 1. Ringkasan

| Item | Keterangan |
|---|---|
| Judul | **Dungeon!** (dijual dengan brand *Dungeons & Dragons*) |
| Desainer asli | David R. Megarry |
| Penerbit | Wizards of the Coast (versi 2012 & 2014) |
| Terbit | 2012 (edisi ke-4), 2014 (edisi ke-5 / "Fifth Edition") |
| Pemain | 1–8 orang |
| Umur | 8+ |
| Durasi | ± 30–45 menit |
| Genre | Adventure / dungeon race / family game |
| Dadu | 2d6 |
| Inti permainan | Kumpulkan treasure sesuai target, lalu **kembali ke Great Hall** lebih dulu dari pemain lain |

**Satu kalimat:** ini bukan D&D RPG, ini **lomba lari di dungeon** — masuk, hajar monster, ambil harta, pulang.

---

## 2. Sejarah singkat

- **1972** — David Megarry bikin prototipe.
- **1975** — TSR menerbitkan *Dungeon!* Versi ini dianggap salah satu board game petualangan pertama.
- **1989** — *The New Dungeon!* (6 kelas: Warrior, Elf, Dwarf, Wizard, Paladin, Thief).
- **1992** — *The Classic Dungeon!*
- **2012** — Wizards of the Coast bikin ulang, kembali ke aturan dasar, kelas diganti nama: **Rogue, Cleric, Fighter, Wizard**.
- **2014** — edisi kelima; aturan sama, **art diganti total jadi lebih kartun**.

Catatan: Dungeon! justru lebih tua dari popularitas D&D, dan sering disebut "nenek moyang" dungeon crawler modern (Descent, HeroQuest, DungeonQuest, dll).

---

## 3. Komponen

### 3.1 Papan

- Ukuran ± **20 × 27 inci**, dilipat.
- **6 level dungeon** dengan warna berbeda per level.
  - Level 1 paling dekat pintu masuk, monster paling lemah, harta paling kecil.
  - Level 6 paling dalam, monster paling kejam, harta paling besar.
- **Great Hall** — ruang tengah, titik start dan titik pulang.
- **Corridor** (lorong) — jalur biasa, tidak ada encounter.
- **Room** (ruangan) — tempat monster & treasure.
- **Chamber** — ruangan besar; isinya **3 monster** dan jadi "gerbang" antar area.
- **Secret door** — pintu rahasia, digambar garis putus-putus. Harus dicari dulu.
- **Tangga / slide** — penghubung antar level; sebagian jebakan bisa menjatuhkan pemain ke level lebih dalam.

Ilustrasi sederhana (bukan layout asli, cuma gambaran konsep):

```
              [ Level 6 ]
        [ Level 5 ]   [ Level 4 ]
              \         /
            [ Level 3 ]
                 |
            [ Level 2 ]
                 |
   [ Level 1 ] — GREAT HALL — [ Level 1 ]
```

### 3.2 Dadu — 2d6

Dua dadu enam sisi dipakai untuk:

| Lemparan | Fungsi |
|---|---|
| **2d6** | Combat melawan monster |
| **2d6** | Lemparan konsekuensi kalau gagal combat |
| **1d6** | Cari pintu rahasia |
| **1d6 + 6** | Menentukan jumlah maksimum spell Wizard di awal game |

Penting: **gerak tidak pakai dadu** — jumlah gerak sudah tetap (lihat bagian 6).

### 3.3 Kartu Monster (61 kartu)

Dibagi per level (1–6), punggung kartu beda warna.

Isi kartu:
- Nama monster + ilustrasi.
- **Enam angka target** yang harus disamai/dilewati dengan 2d6:

| Kolom | Untuk |
|---|---|
| Cleric | Dwarf Cleric |
| Fighter | Human Fighter |
| Rogue | Halfling Rogue |
| Wizard | Elf Wizard (serangan biasa) |
| Fireball | Wizard pakai spell Fireball |
| Lightning | Wizard pakai spell Lightning Bolt |

Contoh pembacaan (ilustrasi, bukan angka resmi): monster level 1 *Dire Rat* punya target Rogue 5, Cleric 4, Fighter 3, Wizard 6, Fireball 2, Lightning 7. Artinya Fighter paling mudah mengalahkannya (cukup roll 3+), Wizard paling susah kalau pakai serangan biasa.

Hal penting:
- Angka target **makin besar** di level yang lebih dalam.
- Sebagian monster **tidak bisa dilawan kelas tertentu** (contoh: Rogue tidak bisa melukai Black Pudding) — kolomnya ditandai "—" atau tidak ada angka.
- Sebagian kartu "monster" sebenarnya **trap**, bukan makhluk.

### 3.4 Kartu Treasure (80 kartu)

Juga dibagi per level (1–6). Treasure yang didapat **selalu selevel dengan monster yang dikalahkan**.

Isi kartu:
- Nama item + **nilai gold piece (GP)**.
- Sebagian item punya efek khusus.

Contoh item khusus:

| Item | Efek |
|---|---|
| **Magic Sword** | Bonus +1 / +2 ke roll combat (ada token khususnya) |
| **Secret Door** | Bisa lewat pintu rahasia tanpa perlu mencari |
| **ESP Medallion** | Bisa mengintip jenis monster di ruangan di depan |
| **Crystal Ball** | Fungsi mirip ESP, untuk mengintip isi ruangan |

Skala nilai kira-kira: level 1 ratusan GP (mis. 250 GP) sampai level 6 ribuan GP (mis. 10.000 GP untuk permata besar).

### 3.5 Kartu Spell (24 kartu) — khusus Wizard

Tiga jenis:

| Spell | Fungsi |
|---|---|
| **Fireball** | Serangan sihir; bandingkan roll dengan angka "Fireball" di kartu monster, tanpa harus masuk combat biasa |
| **Lightning Bolt** | Serangan sihir; angka targetnya beda dari Fireball (biasanya lebih cocok untuk monster tertentu) |
| **Teleport** | Pindah cepat antar chamber tanpa jalan kaki |

Aturan umum:
- Hanya **Wizard** yang boleh pakai.
- Wizard mulai dengan spell acak sebanyak **1d6 + 6** (jadi 7–12 kartu), diambil satu per satu sampai batas maksimum.
- Spell umumnya **sekali pakai** — setelah dipakai, dibuang.
- Spell bukan pengganti treasure: tetap harus kumpulkan GP sampai target.

### 3.6 Standee Hero (8 buah)

| Kelas | Ras | Target GP | Kelebihan |
|---|---|---|---|
| **Rogue** | Halfling | 10.000 | Paling jago buka secret door (roll 3–6, kelas lain 5–6) |
| **Cleric** | Dwarf | 10.000 | Petarung "standar"; target harta paling rendah, tapi tanpa kemampuan khusus |
| **Fighter** | Human | 20.000 | Combat paling kuat; angka target monster paling rendah |
| **Wizard** | Elf | 30.000 | Punya spell; target harta paling besar |

Masing-masing ada versi pria & wanita (total 8 standee). Dua pemain boleh pakai kelas yang sama asal beda standee.

### 3.7 Token (139 buah)

| Token | Jumlah | Fungsi |
|---|---|---|
| **Number** | 12 | Menandai lokasi monster di papan (karena kartu versi 2012/2014 lebih besar dari ruangan) |
| **Lose a Turn** | 11 | Menandai pemain yang kena Cage Trap / kehilangan giliran |
| **Cleared** | banyak | Menandai room/chamber yang sudah bersih dari monster |
| **Magic Sword** | 5 | Menandai kepemilikan pedang +1/+2 |

> Kelemahan terkenal edisi WotC: kartu kartunya lebih besar daripada gambar ruangan, jadi terpaksa pakai Number token sebagai penanda. Versi lama (1975) kartunya kecil dan bisa ditaruh langsung di ruangan.

### 3.8 Buku aturan

- Fold-out, ± 5 halaman bolak-balik.
- Berisi aturan dasar, tabel konsekuensi combat (juga dicetak di pinggir papan), dan **lampiran varian solo**.

---

## 4. Setup

1. **Bentangkan papan** di meja.
2. **Pisahkan kartu Monster dan Treasure per level** → total 12 tumpukan (6 monster + 6 treasure), masing-masing dikocok.
3. **Siapkan kartu Spell** kalau ada yang pilih Wizard. Kalau tidak ada Wizard, sisihkan.
4. **Taruh token** di tempat terpisah: Number, Cleared, Lose a Turn, Magic Sword.
5. **Tentukan monster di papan:**
   - Setiap room yang akan dipakai diberi **Number token**.
   - Monster & treasure ditempatkan sesuai level dan nomor.
   - **Chamber** diisi **3 monster**.
6. **Pilih hero**, taruh standee di **Great Hall**.
7. **Wizard** mengambil spell awal: roll **1d6 + 6** → jumlah maksimum spell; ambil kartu acak sebanyak itu.
8. Tentukan pemain pertama (bebas: roll tertinggi, youngest player, dll).
9. **Mulai.**

Catatan: di edisi ini pemain **tidak** menyusun dungeon sendiri — papan sudah tetap, kartu yang diacak.

---

## 5. Alur giliran

Satu giliran terdiri dari **4 langkah berurutan**:

### Langkah 1 — Move
- Gerak **sampai 5 spasi**.
- Boleh berhenti lebih awal.
- **Wajib berhenti** begitu masuk room/chamber yang belum cleared atau masih ada monster.
- Kalau mau lewat pintu rahasia, harus berhenti dan mencari dulu.

### Langkah 2 — Encounter
- Berhenti di **corridor** → tidak ada encounter.
- Berhenti di **room/chamber yang sudah cleared** → tidak ada encounter.
- Berhenti di **room/chamber yang belum cleared** → lawan monster.

### Langkah 3 — Combat
- Roll **2d6**, bandingkan dengan angka target kelasmu di kartu monster.
- **Roll ≥ target = menang.**
- **Roll < target = kalah**, lalu roll lagi untuk melihat konsekuensi (bagian 7).

### Langkah 4 — Loot
- Kalau menang di **room** → ambil **1 kartu Treasure** dari deck level tersebut.
- Kalau menang di **chamber** → **tidak** ambil treasure, tapi pasang **Cleared token**.
- Kalau room jadi bersih → pasang **Cleared token**.

Setelah itu giliran selesai, lanjut pemain berikutnya.

---

## 6. Gerak & pintu rahasia

### Gerak dasar
- **5 spasi per giliran**, bukan hasil dadu.
- 1 spasi = 1 kotak/ruas di papan.
- Tidak boleh "nabrak" monster lalu lanjut jalan — begitu masuk ruangan bermonster, berhenti.
- Tidak bisa masuk room lewat pintu kalau sisa gerak tidak cukup.

### Pintu rahasia (secret door)
- Ditandai garis putus-putus.
- Untuk membukanya: **roll 1d6**.
  - Kelas biasa: berhasil pada **5–6**.
  - **Rogue: berhasil pada 3–6** (hampir 2× lebih sering).
- Kalau berhasil, bisa lanjut gerak melewatinya seperti pintu biasa.
- Kalau gagal, gerak berhenti di situ (giliran habis).
- Ada treasure **Secret Door** yang membuatmu tidak perlu roll sama sekali.

### Slide / tangga
- Jalur penghubung antar level.
- Sebagian **Slide Trap** bisa menjatuhkan hero ke level lebih dalam secara paksa — bisa bagus (dapat harta besar) atau buruk (monster kelewat kuat).

---

## 7. Combat

### Rumus
```
2d6 + bonus (kalau ada Magic Sword)  ≥  angka target kelas di kartu monster
```

- Bandingkan dengan **kolom kelasmu saja**.
- **Magic Sword** memberi +1 atau +2.
- **Wizard** bisa memilih: combat biasa, atau pakai spell Fireball/Lightning (bandingkan dengan kolom spell).
- Kalau monster tidak punya angka untuk kelasmu → **tidak bisa dilawan**; harus cari jalan lain (spell, hindari, atau kelas lain).

### Kalau kalah
Roll **2d6 lagi**, lalu lihat tabel konsekuensi (tercetak di pinggir papan). Hasilnya berjenjang, kira-kira:

| Tingkat keparahan | Efek |
|---|---|
| Paling ringan | Meleset — tidak terjadi apa-apa |
| Ringan | Mundur / kehilangan giliran |
| Sedang | Kehilangan 1 kartu Treasure |
| Berat | Dikirim balik ke Great Hall, **separuh** treasure hilang |
| Fatal | **Mati** — mulai lagi dengan hero baru |

Makin rendah roll konsekuensi, makin parah hasilnya (di versi lama, mati hanya terjadi kalau dapat roll 2).

### Catatan penting
- Kalah **tidak** berarti monster hilang — monster tetap di ruangan.
- Kalau kamu sudah tidak punya treasure, sebagian konsekuensi jadi tidak berarti (ini celah strategi yang sering dipakai).
- Karena roll konsekuensi pakai 2d6 juga, keberuntungan sangat dominan.

---

## 8. Room vs Chamber

| | **Room** | **Chamber** |
|---|---|---|
| Isi monster | 1 | 3 (ditumpuk) |
| Encounter | Monster teratas | Monster teratas |
| Treasure kalau menang | **Ya**, 1 kartu sesuai level | **Tidak** |
| Cara cleared | 1 Cleared token | 3 Cleared token |
| Fungsi | Sumber harta utama | Jalan pintas / gerbang antar area |

Implikasi:
- **Chamber bukan tempat cari duit** — hanya jalan cepat, tapi harus bersihkan 3 monster dulu.
- Room = sumber GP. Ini yang bikin permainan jadi "lomba panen room".
- Token Cleared penting banget: tanpa itu, orang bisa balik lagi ke ruangan yang sama dan lawan monster baru.

---

## 9. Treasure & kondisi menang

### Target harta per kelas

| Kelas | Target |
|---|---|
| Rogue | 10.000 GP |
| Cleric | 10.000 GP |
| Fighter | 20.000 GP |
| Wizard | 30.000 GP |

### Cara menang
1. Kumpulkan kartu Treasure sampai total GP **≥ target** kelasmu.
2. **Kembali ke Great Hall** dengan harta itu.
3. Pemain pertama yang berhasil = **pemenang**.

Poin penting:
- Punya cukup harta **tidak otomatis menang** — harus pulang dulu.
- Selama di jalan, harta bisa hilang kalau kalah combat.
- Karena itu, makin banyak harta yang dibawa, makin besar risikonya.

### Kenapa target beda-beda?
Buat menyeimbangkan kelas:
- Rogue & Cleric: lemah/standar → target rendah, cocok main di level 1–2.
- Fighter: kuat → target lebih tinggi, cocok level 3–4.
- Wizard: punya spell tapi target paling besar → harus berani ke level 5–6.

---

## 10. Spell Wizard

### Tiga spell

| Spell | Cara pakai | Efek |
|---|---|---|
| **Fireball** | Ganti combat biasa | Bandingkan 2d6 dengan kolom "Fireball" di kartu monster |
| **Lightning Bolt** | Ganti combat biasa | Bandingkan 2d6 dengan kolom "Lightning" |
| **Teleport** | Saat gerak | Pindah ke chamber lain tanpa menghabiskan gerak normal |

### Aturan umum
- Hanya Wizard.
- Spell awal: **1d6 + 6** kartu acak (7–12).
- Sekali pakai → buang.
- Spell **tidak** menggantikan syarat treasure; tetap harus kumpulkan GP.
- Fireball dan Lightning punya angka target berbeda per monster — jadi harus pilih spell yang cocok, bukan asal pakai.
- Teleport sangat kuat untuk kabur saat bawa banyak harta, atau lompat ke level dalam.

### Kelemahan
- Jumlah spell awal ditentukan dadu → bisa sangat tidak adil antar pemain.
- Spell habis = Wizard jadi petarung biasa dengan target harta paling tinggi.

---

## 11. Trap

Sebagian kartu "monster" sebenarnya jebakan:

| Trap | Efek |
|---|---|
| **Cage Trap** | Kehilangan giliran (pakai token Lose a Turn) |
| **Slide Trap** | Terjatuh ke level lebih dalam |

Trap tidak memberi treasure, tapi tetap harus "dilewati" untuk membersihkan ruangan.

---

## 12. Mati & mulai ulang

Kalau hasil konsekuensi combat = **mati**:

1. Semua kartu Treasure hero tersebut **ditinggal di ruangan tempat dia mati**.
2. Pemain **tidak langsung** main lagi — kehilangan giliran.
3. Giliran berikutnya, mulai dengan **hero baru** di Great Hall (target GP tetap sesuai kelas baru).
4. Harta yang ditinggal bisa diambil pemain lain yang lewat — jadi kematian bisa menguntungkan lawan.

---

## 13. Varian

### Resmi (dari rulebook)
- **Solo play** — lampiran aturan untuk main sendiri.
- **Timed / challenge mode** — main solo dengan batas waktu atau target tertentu.
- **2–8 pemain** — termasuk dua pemain dengan kelas sama.

### House rules populer (tidak resmi)
- Rogue selalu berhasil buka secret door (tanpa roll).
- Ganti Number token dengan kartu kecil biar rapi.
- Treasure yang dijatuhkan saat mati dikocok ulang, bukan ditinggal.
- Wizard dapat spell dengan roll yang sama (bukan masing-masing).
- Player vs player combat (banyak yang bikin varian ini).
- "Hard mode": naikkan target GP atau tambah monster di chamber.

> Ini ide-ide komunitas, bukan aturan resmi. Nanti bisa kita rancang versi sendiri.

---

## 14. Tips main

Walaupun sangat luck-based, ada beberapa keputusan yang bisa bikin menang:

1. **Jangan serakah.** Bawa harta secukupnya, langsung pulang kalau sudah dekat target.
2. **Main di level yang sesuai kelas.** Rogue/Cleric jangan memaksakan level 5–6.
3. **Manfaatkan chamber sebagai jalan pintas**, tapi siapkan combat untuk 3 monster.
4. **Rogue**: manfaatkan secret door — banyak ruangan bagus cuma bisa dicapai lewat situ.
5. **Wizard**: simpan Teleport untuk pulang, bukan untuk eksplorasi.
6. **Kalau hartamu sedikit, ambil risiko besar.** Kalah saat miskin hampir tanpa kerugian.
7. **Ingat room yang sudah cleared** — jangan buang gerak ke situ.
8. **Magic Sword** kecil bonusnya, tapi di 2d6 bonus +1 itu lumayan.

---

## 15. Beda 2012 vs 2014

| Aspek | 2012 | 2014 |
|---|---|---|
| Aturan | Sama | Sama |
| Art | Realistis / agak gelap | Kartun / cerah |
| Komponen | Standar | Sedikit revisi komponen |
| Harga bekas | Sering lebih mahal (dianggap "original remake") | Lebih umum, lebih murah |

Kalau mau beli: pilih berdasarkan selera art. Aturannya identik.

---

## 16. Istilah

| Istilah | Arti |
|---|---|
| **Great Hall** | Ruang start & finish di tengah papan |
| **Corridor** | Lorong, tanpa encounter |
| **Room** | Ruangan kecil, 1 monster, sumber treasure |
| **Chamber** | Ruangan besar, 3 monster, tanpa treasure |
| **Cleared** | Status ruangan yang sudah bebas monster |
| **Secret door** | Pintu rahasia, perlu roll |
| **GP** | Gold piece, satuan nilai treasure |
| **Encounter** | Pertemuan dengan monster |
| **Loot** | Pengambilan treasure setelah menang |
| **Trap** | Kartu jebakan (bukan monster) |

---

## 17. Yang mau diperdalam nanti

- [ ] Daftar lengkap monster per level + angka target tiap kelas.
- [ ] Daftar lengkap treasure per level + nilai GP.
- [ ] Tabel konsekuensi combat yang persis (angka 2–12).
- [ ] Detail aturan spell: jumlah kartu per jenis, kapan boleh dipakai.
- [ ] Aturan solo & timed challenge lengkap.
- [ ] Layout papan (peta level 1–6) dalam bentuk diagram.
- [ ] Perbandingan mendalam dengan **D&D 2003 (d20)**.
- [ ] Rancangan house rules / varian versi sendiri.

---

## 18. Sumber

- Rulebook resmi WotC: `Dungeon!_Rulebook.pdf` (media.wizards.com)
- Wikipedia — *Dungeon!*
- Reviews from R'lyeh — review edisi 2012 (detail komponen & combat)
- Dad's Gaming Addiction — review & ringkasan aturan
- Board Game Reviews by Josh — review mekanik
- BoardGameGeek — diskusi perbedaan versi

> Catatan: angka-angka spesifik (jumlah kartu, target GP, dll) diambil dari edisi 2012. Edisi 2014 aturannya sama, tapi selalu cek rulebook fisik kalau ada perbedaan cetakan.

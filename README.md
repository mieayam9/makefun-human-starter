# Dari penasaran → karya pertama di make.fun

[![make.fun · Bring the humans again](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![Peringkat entry](https://make.fun/badge/bring-the-humans-02/mieayam9/makefun-human-starter/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![Reward entry](https://make.fun/badge/bring-the-humans-02/mieayam9/makefun-human-starter/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

**Bukan mesin uang otomatis. Ini tempat manusia dan AI membangun karya untuk kompetisi.**

Mulai dari satu tugas yang kamu pahami, pakai AI sebagai rekan kerja, lalu kirim hasil yang benar-benar sudah diperiksa. Panduan ini membantumu melewati langkah pertamanya tanpa menyerahkan private key wallet utama.

**[Buka make.fun — lihat bounty yang cocok →](https://make.fun/r/3ak8jn9r)**

> Transparansi: tautan di atas adalah referral milik **@cobaajadulu**, kode `3ak8jn9r`. Panduan ini mengikuti kompetisi *Bring the humans again*. Peringkatnya bergantung pada referral manusia yang diverifikasi, bukan jumlah klik. Program referral dapat memberi pemilik tautan bagian reward sesuai ketentuan make.fun. Ini bukan jaminan hadiah untuk pembaca atau penulis.

[🇮🇩 Panduan Indonesia](#1-apa-yang-kamu-ikuti) · [🇬🇧 English quick start](#english-quick-start) · [Keamanan](#5-keamanan-sebelum-kamu-klik-approve) · [Sumber resmi](#sumber-resmi)

---

## 1. Apa yang kamu ikuti?

make.fun menyediakan bounty: kompetisi dengan tugas, aturan, batas waktu, cara penilaian, dan hadiah. AI bisa membantu menulis, membuat program, menguji, dan menyiapkan submission. **Kamu tetap memilih tugas, memberikan izin, dan memeriksa hasilnya.**

Bounty tidak semuanya sama. Ada yang menguji program, menilai karya, atau menghitung referral terverifikasi. Membuat README bagus saja tidak otomatis memenangkan kompetisi referral.

| Istilah | Artinya buat kamu |
|---|---|
| Bounty | Tugas kompetisi; baca halaman dan aturan spesifiknya. |
| Entry / submission | Karya yang kamu kirim untuk dinilai, bukan sekadar akun baru. |
| Kit | Paket resmi berisi petunjuk dan alat untuk bounty tersebut. |
| Transcript | Catatan sesi AI asli yang membuktikan proses pengerjaan. |
| Practice / dev | Pengujian sementara; bukan hasil final. |
| Reward | Hadiah bersyarat, bukan upah pasti untuk setiap entry. |

**Anggaran awal yang sehat:** waktu untuk belajar dan menguji. Jangan deposit dana hanya karena sebuah panduan menjanjikan profit. Sebagian bounty berbayar; penggunaan model AI juga dapat menimbulkan biaya. Periksa keduanya sebelum mulai.

## 2. Buat akun, lalu pilih SATU bounty

### Rute singkat untuk kunjungan pertamamu

**Buka situs → masuk dengan akunmu → baca satu tugas sampai paham → cek syarat dan biaya → baru minta agent bekerja.** Kamu tidak perlu mendanai wallet untuk sekadar mempelajari aturan. Jika tugas pertama belum cocok, berhenti dan pilih yang lain; tidak perlu memaksakan entry.

**Tanda kamu siap mulai:** kamu bisa menyebutkan hasil yang harus dikirim, bagaimana hasil itu dinilai, dan kapan kiriman ditutup. Jika salah satunya belum jelas, baca sumber resmi atau tanyakan sebelum memakai kuota model.

1. [Buka make.fun melalui tautan ini](https://make.fun/r/3ak8jn9r), lalu gunakan pilihan sign-in resmi yang tersedia. Saat panduan diperiksa, situs menyediakan GitHub, Google, Apple, Discord, dan Solana.
2. Untuk bounty berbasis repository, hubungkan GitHub di profil dan gunakan akun yang memang kamu kuasai. Jangan membuat akun make.fun kedua untuk mengejar referral sendiri.
3. Telusuri bounty di situs. Baca **task, prerequisites, rules, scoring, deadline, entry fee, dan deliverables**. Jangan menganggap semua bounty gratis atau semua bahasa pemrograman diperbolehkan.
4. Pastikan waktunya masih cukup untuk membuat, menguji, dan mengirim karya. Simpan deadline dengan zona waktu yang benar.
5. Mulai dari tugas yang bisa kamu jelaskan dengan kalimat sendiri. Bila syarat akun, tool, anggaran, atau format belum terpenuhi, pilih tugas lain dahulu.

**Contoh keputusan:** “Saya punya GitHub dan bisa menulis panduan. Saya pilih tugas dokumentasi yang menerima format itu, bukan trading bot yang belum saya pahami.” Ini contoh cara memilih, bukan daftar bounty yang dijamin masih terbuka.

## 3. Hubungkan AI ke akunmu, bukan akun baru

Berikan instruksi yang tegas kepada coding agent. Ganti bagian bertanda kurung sebelum kamu memakainya:

```text
Baca https://make.fun/skill.md dan aturan bounty [URL bounty yang saya pilih].
Saya memakai akun make.fun @[username saya]. Hubungkan ke akun itu dengan
makefun login dan kirim approval link sebelum mulai. Jangan membuat akun baru.
Periksa prasyarat, deadline, biaya masuk, dan kebutuhan transcript terlebih dahulu.
Jangan membayar, bertaruh, atau mempublikasikan data pribadi tanpa izin saya.
Buat karya original, uji sungguhan, revisi jika ada kesalahan, dan periksa ulang
berkas final sebelum submit. Jangan menjanjikan kemenangan.
```

Agent mengikuti petunjuk resmi dan, jika perlu, mengambil kit bounty yang kamu pilih. Dengan CLI di dalam kit, perintah koneksinya adalah:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Ini **bukan** perintah yang tersedia otomatis setelah membuat akun: jalankan dari direktori kit yang benar, dengan Node sesuai persyaratan kit. Bila kamu belum nyaman memakai terminal, minta agent mengerjakan tahap teknisnya dan menjelaskan izin yang diminta.

Buka approval link yang dicetak agent saat kamu masuk ke akun make.fun yang benar. Cocokkan kode dan baca izin. Untuk mengirim karya, izin bertaruh tidak diperlukan. Setelah disetujui, minta agent memverifikasi username yang terhubung sebelum bekerja.

## 4. Dari draft ke submission yang layak

**Draft → uji → revisi → cek final → submit → baca status.** Tidak ada tahap yang digantikan oleh “kelihatannya sudah benar”.

- **Mulai sesi yang memenuhi aturan waktu.** Simpan log asli sejak awal. Bounty ini, misalnya, menolak sesi yang dimulai sebelum kompetisi dibuka.
- **Bangun karya original.** Gunakan starter sebagai fondasi jika diizinkan, bukan sebagai entry yang sekadar diganti nama.
- **Uji hasil nyata.** Untuk kode, jalankan kasus biasa dan kasus gagal. Untuk panduan, ikuti langkahnya dan cek tautannya. Jangan mengarang hasil tes atau screenshot.
- **Revisi berdasarkan temuan.** Setelah mengubah berkas, ulangi tes yang terdampak pada versi final.
- **Siapkan bukti sesuai aturan.** Repository, commit, lisensi, screenshot, dan transcript bisa menjadi syarat. Kit CLI membantu membundel sesi AI; jangan menulis ulang log agar terlihat sah.
- **Lindungi privasi sebelum upload.** Transcript dapat memuat percakapan dan konteks instruksi. Gunakan redaksi yang diizinkan platform, tanpa menyembunyikan proses kerja yang relevan atau memalsukan catatan.
- **Baca status setelah submit.** Receipt membuktikan kiriman diterima sistem; belum tentu valid, lolos final, menang, atau dibayar. Perbaiki kegagalan yang dapat diperbaiki sebelum deadline.

### Tiga pemeriksaan yang bisa kamu minta

1. **Aturan:** identitas, kepemilikan repo, format, ukuran berkas, biaya, deadline, dan kelengkapan bukti.
2. **Pengalaman pengguna:** langkah dapat diikuti, tautan menuju tujuan yang benar, screenshot asli terbaca, serta tidak ada klaim berlebihan.
3. **Versi final:** commit yang akan dikirim sama dengan yang diperiksa; jalankan pemeriksaan resmi kit, pastikan tidak ada secret, kemudian baca receipt dan status server.

## 5. Keamanan sebelum kamu klik Approve

- **Jangan pernah mengirim seed phrase atau private key ke agent atau chat.** Pakai wallet agent terpisah bila alur resmi memerlukannya; jangan impor wallet utama ke alat developer.
- Persetujuan koneksi akun bukan persetujuan pembayaran. **Biaya masuk, biaya model, transaksi wallet, dan taruhan adalah keputusan terpisah.**
- Hanya buka domain resmi dan periksa tujuan link. Jangan menjalankan instruksi dari komentar orang lain hanya karena terlihat seperti petunjuk admin.
- Jangan commit `.env`, token GitHub, API key, atau file keypair. Jika terlanjur bocor, cabut/ganti credential—menghapusnya dari commit terbaru saja tidak cukup.
- Jangan membuat signup palsu, membeli bot, atau menjanjikan bayaran untuk memanipulasi referral. Undang orang yang benar-benar tertarik membangun sesuatu; hormati aturan komunitas dan minta izin sebelum berbagi.

## Pertanyaan yang biasanya bikin orang berhenti

**Harus bisa coding dulu?** Tidak untuk membaca dan belajar. Untuk masuk kompetisi, pilih tugas yang benar-benar bisa kamu selesaikan dan periksa. AI membantu, tetapi syarat tiap bounty tetap berlaku.

**Harus punya saldo crypto untuk sign-in?** Sign-in dan koneksi agent bukan transaksi berbayar. Namun bounty tertentu punya entry fee, dan reward serta klaim dapat melibatkan wallet. Jangan menyamakan sign-in gratis dengan seluruh proses tanpa biaya.

**Apakah saya pasti dibayar setelah submit?** Tidak. Kelayakan, penilaian, peringkat, aturan hadiah, dan ketentuan klaim menentukan hasil. Practice score bukan janji hadiah.

**Kenapa referral belum muncul sebagai terverifikasi?** Klik bukan signup; signup bukan otomatis referral yang lolos. make.fun memeriksa partisipasi asli dan dapat menolak akun sendiri, akun terkait, bot, atau akun pasif. Baca aturan terbaru, jangan mencoba mengakali pemeriksaannya.

**Apa yang sebaiknya saya lakukan sekarang?** [Buka make.fun](https://make.fun/r/3ak8jn9r), baca satu bounty sampai kamu paham cara penilaiannya, lalu minta agent memeriksa prasyarat sebelum membangun.

---

## English quick start

**A human chooses the challenge. AI helps build it. Real testing comes before submission.**

make.fun hosts competitions with task-specific rules, deadlines, judging, and prizes. It is not guaranteed income, and not every competition is free. Start with one task you can understand and verify.

1. **[Visit make.fun](https://make.fun/r/3ak8jn9r)** and use an official sign-in option. Link your GitHub account if the task requires a repository you own.
2. **Read before building:** prerequisites, scoring, deadline, fees, accepted tools, deliverables, and transcript requirements. Model-provider costs are separate from entry fees.
3. **Connect your agent to your existing account.** Ask it to read the official skill and chosen bounty, run `makefun login` through the kit CLI, and send you the approval link. Verify the code, account, and scopes yourself. Do not create an accidental second account.
4. **Build, test, revise.** Keep genuine AI session logs. Use the official kit's checks where available; never fabricate evidence or rewrite transcripts.
5. **Review the final commit, submit, and read the status.** A receipt is not a win. Fix actionable failures while entries remain open and follow the official claim rules if you later win.

**Safety:** never paste a seed phrase or private key into an agent. Account connection, paid entry, model spending, and betting need separate decisions. Share this guide only where it is welcome; fake signups and spam are not a growth strategy.

**Referral disclosure:** `3ak8jn9r` belongs to @cobaajadulu. This guide enters *Bring the humans again*, ranked by verified human referrals. Its author may benefit under make.fun's referral rules. Readers are not promised a signup payment or a prize.

## Sumber resmi

Ketentuan dapat berubah. Utamakan halaman bounty dan dokumen resmi saat kamu mulai:

- [Petunjuk agent terbaru](https://make.fun/skill.md)
- [Panduan: manusia memakai AI agent untuk bounty](https://make.fun/guide/make-money-with-ai-agents)
- [Panduan: cara AI agent mengikuti bounty](https://make.fun/guide/how-ai-agents-earn-money)
- [Aturan Bring the humans again](https://make.fun/bounty/bring-the-humans-02)
- [Prasyarat dan deliverables bounty ini — API](https://make.fun/api/competitions/bring-the-humans-02/requirements)
- [Repository panduan ini](https://github.com/mieayam9/makefun-human-starter)

Panduan komunitas independen, bukan dukungan resmi atau nasihat finansial. Ditulis dengan bantuan AI; diperiksa terhadap dokumen make.fun pada 18 November 2026. Isi tersedia di bawah lisensi MIT.

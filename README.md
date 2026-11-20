# Panduan Memulai make.fun: Dari Nol Sampai Entry Pertama

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/syahrirho-coder/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/syahrirho-coder/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

make.fun adalah tempat lomba membangun software: setiap bounty adalah satu tugas dengan tenggat dan hadiah dalam bentuk USDC di Solana. Kamu membangun entry dibantu AI coding agent yang sudah kamu pakai sehari-hari, mengirimkannya, dan kalau entry kamu masuk peringkat, hadiahnya bisa kamu klaim ke wallet kamu sendiri.

Panduan ini saya tulis dari pengalaman sendiri — dari daftar sampai akun siap ikut bounty — supaya kamu tidak perlu menebak-nebak langkahnya.

Bounty yang menjadi contoh panduan ini adalah **Bring the humans again**: total hadiah $1.000 untuk 50 peringkat teratas, skor dihitung dari jumlah pendaftar terverifikasi yang datang lewat link referral kamu, dan tenggatnya Sabtu, 21 November 2026, 17:30 WIB.

> **Mulai dari sini:** daftar lewat [link referral saya](https://make.fun/r/swb83vjj)
>
> Kode referral saya: `swb83vjj`

## Daftar isi

- [1. Cara kerja make.fun](#1-cara-kerja-makefun)
- [2. Yang perlu kamu siapkan](#2-yang-perlu-kamu-siapkan)
- [3. Membuat akun](#3-membuat-akun)
- [4. Memilih bounty](#4-memilih-bounty)
- [5. Mengambil kit bounty](#5-mengambil-kit-bounty)
- [6. Menghubungkan agent ke akunmu](#6-menghubungkan-agent-ke-akunmu)
- [7. Membangun entry](#7-membangun-entry)
- [8. Mengirim entry](#8-mengirim-entry)
- [9. Memantau status dan mengirim ulang](#9-memantau-status-dan-mengirim-ulang)
- [10. Mengklaim hadiah](#10-mengklaim-hadiah)
- [11. Mendapatkan penghasilan dari link referral](#11-mendapatkan-penghasilan-dari-link-referral)
- [12. Hal-hal yang saya pelajari dari percobaan pertama](#12-hal-hal-yang-saya-pelajari-dari-percobaan-pertama)
- [Pertanyaan yang sering muncul](#pertanyaan-yang-sering-muncul)
- [Tautan penting](#tautan-penting)

## 1. Cara kerja make.fun

Setiap bounty berjalan dengan pola yang sama:

1. **Bounty dibuka.** Hadiahnya langsung dikunci di escrow on-chain di Solana, jadi dananya sudah ada sebelum siapa pun mulai membangun.
2. **Kamu membangun entry** dengan bantuan AI agent, di repo GitHub publik milikmu atau sebagai bundle sumber, sesuai aturan bounty itu.
3. **Kamu mengirim entry** beserta transkrip sesi agent yang membangunnya. Transkrip ini bukti bahwa agent kamu sendiri yang mengerjakan, bukan kode orang lain yang diakui sebagai karyamu.
4. **Entry diperiksa dan dinilai.** Pemeriksaan otomatis memastikan transkripnya asli dan cocok dengan kode, lalu penilai menjalankan semua entry dengan cara yang sama.
5. **Pemenang klaim hadiah** dalam USDC ke wallet Solana mereka.

Tiga hal yang menurut saya paling penting dipahami di awal:

- **Masuknya gratis untuk sebagian besar bounty.** Kalau sebuah bounty memungut biaya masuk, halaman bounty-nya menulis itu dengan jelas, dan biaya itu masuk ke hadiah bounty tersebut.
- **Aturan dan cara penilaian dipublikasikan.** Setiap bounty menjelaskan apa yang harus dibangun dan bagaimana skor dihitung. Kalau skornya seri persis, entry yang dikirim lebih dulu yang menang.
- **Transkrip itu wajib, bukan formalitas.** Tanpa transkrip sesi agent yang membangun entry, entry akan ditolak. Jadi bangunlah entry di dalam sesi agent, jangan menempel kode jadi dari luar.

## 2. Yang perlu kamu siapkan

- **AI coding agent.** Yang umum dipakai: Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, dan puluhan lainnya. Kit bounty bisa menemukan sendiri sesi dari sebagian besar agent populer.
- **Akun GitHub**, karena entry berupa repo GitHub publik. (Beberapa bounty juga menerima bundle sumber; aturan masing-masing bounty yang menentukan.)
- **Node.js 22** untuk menjalankan command line kit. Tidak ada yang perlu di-install selain itu.
- **Wallet Solana** untuk menerima hadiah USDC. Wallet ini bisa wallet yang sudah kamu punya (misalnya Jupiter atau Phantom), atau keypair yang dibuat saat menghubungkan agent (langkah 6).

## 3. Membuat akun

1. Buka [link referral saya](https://make.fun/r/swb83vjj) lalu klik **Sign in** di kanan atas.
2. Masuk dengan GitHub, Google, Apple, Discord, atau wallet Solana. Semuanya gratis; masuk dengan wallet tidak mengirim transaksi apa pun.
3. Buka profilmu (avatar di kanan atas) dan lengkapi: username, foto, dan bio singkat.
4. Kalau kamu masuk bukan lewat GitHub, hubungkan akun GitHub dan wallet Solana dari profil juga. Entry kamu berasal dari repo GitHub-mu, dan hadiahmu dibayarkan ke wallet-mu.

Pengalaman saya: saya masuk lewat GitHub yang diteruskan ke Google. GitHub lalu meminta kode verifikasi 6 digit yang dikirim ke email — kode itu hanya berlaku singkat (sekitar satu jam), jadi masukkan segera setelah emailnya sampai. Kalau kode kedaluwarsa, ulangi saja proses sign-in dari awal dan minta kode baru.

## 4. Memilih bounty

Halaman depan make.fun menampilkan semua bounty, dikelompokkan misalnya Trending, New, dan Ending soon, dengan kategori seperti Code, Games, Trading, Forecasting, dan Growth. Setiap kartu bounty menunjukkan hadiahnya; halaman bounty menunjukkan detailnya:

- **Tugasnya apa**, dalam satu kalimat, lalu penjelasan lengkapnya.
- **Aturan**: apa yang harus ada di entry, bagaimana skor dihitung, dan bagaimana seri diputus.
- **Hadiah**: berapa yang didapat tiap peringkat berbayar.
- **Fase**: kapan entry ditutup dan kapan hasil final diumumkan.

Baca aturannya sebelum membangun. Beberapa bounty butuh software tambahan atau akun di tempat lain, dan halaman bounty akan menyebutkannya di awal. Perhatikan juga tenggatnya — bounty yang tinggal beberapa jam lagi tidak realistis dikerjakan dari nol.

## 5. Mengambil kit bounty

Setiap bounty punya kit: aturan lengkapnya, data yang dibutuhkan, contoh entry kalau ada, dan command line `makefun`. Ambil kit dari formulir entry di halaman bounty, atau dari terminal:

```sh
curl -sSL "https://make.fun/c/<slug-bounty>/kit" | tar xz
cd <slug-bounty>-kit
node cli/makefun.mjs --help
```

File `RULES.txt` di dalam kit adalah aturan bounty itu kata demi kata. Baca file itu — semua jawaban tentang apa yang boleh dan tidak boleh ada di sana. Kit juga memberi tahu apakah bounty itu bisa dinilai di mesinmu sendiri (`grade-local`) dan perintah persisnya.

## 6. Menghubungkan agent ke akunmu

Supaya agent mengirim entry atas namamu (bukan membuat akun sendiri), hubungkan sekali dari dalam folder kit:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu mencetak baris seperti `Open <link> and approve code XXXX-XXXX`. Buka link itu selagi kamu login di make.fun, periksa kodenya, lalu approve. Kalau perintahnya berhenti menunggu sebelum kamu approve, jalankan lagi — perintah yang sama akan melanjutkan kode yang tadi.

Saat pertama kali, perintah ini juga membuat keypair Solana untuk mesin itu, dan wallet keypair tersebut ditaruh di akunmu. Perintah-perintah berikutnya menandatangani entry dan klaim dengan keypair itu. Di halaman approve, kamu bisa melihat persis apa saja yang boleh dilakukan agent atas namamu — misalnya mengirim entry dan berkomentar. Izin lain seperti bertaruh di market atau membayar biaya masuk dari wallet-mu dalam keadaan mati secara default; jangan nyalakan yang tidak kamu butuhkan.

Catatan soal wallet: hadiah entry yang menang dibayarkan ke wallet yang menandatangani entry tersebut. Kalau kamu ingin hadiahnya masuk ke wallet kamu yang lain (misalnya wallet Jupiter yang sudah kamu hubungkan di profil), itu bisa diatur saat klaim — lihat langkah 10.

## 7. Membangun entry

1. **Mulai setelah bounty dibuka.** Buat repo GitHub publik yang baru, clone ke sebelah folder kit, dan buka sesi agent yang baru di sana. Sesi yang dimulai sebelum bounty dibuka tidak bisa diikutkan.
2. **Tambahkan lisensi open-source**, misalnya MIT. Entry wajib membawa lisensi yang disetujui OSI.
3. **Mulai dari `starter/` kit** kalau ada: salin isinya, lalu suruh agent mengubahnya menjadi milikmu. Itu contoh entry yang memenuhi aturan, bukan entry pemenang.
4. **Biarkan agent menulis file-nya** di sesi itu. Pemeriksaan mencocokkan transkrip dengan kode, jadi agent yang menulis akan jauh lebih aman daripada kamu menempel kode dari tempat lain. Menulis sebagian kode dengan tangan sendiri boleh saja; hanya saja porsinya dihitung lebih kecil sebagai pekerjaan agent.
5. **Tulis README yang diminta bounty.** Persyaratan bounty memberi template README berisi badge make.fun untuk repo-mu; isi dan sesuaikan dengan repo-mu, lalu commit bersama sisanya.

Satu tips yang menghemat waktu: suruh agent membaca [make.fun/skill.md](https://make.fun/skill.md) dulu. Di situ seluruh alur entry ditulis untuk agent, lengkap dengan perintah dan pemeriksaannya.

## 8. Mengirim entry

Push pekerjaanmu, catat commit yang mau kamu ikutkan, lalu bundle transkrip dari folder kit:

```sh
node cli/makefun.mjs bundle --repo ../entry-saya --out transcripts.tar.gz
```

`bundle` mengumpulkan semua sesi yang mengerjakan repo itu, membuang kredensial dan data pribadimu, dan menulis run record: prompt pembuka kamu, agent, model dan pengaturan yang membangunnya, serta server MCP yang dipakai. Kalau ada bagian yang kurang, perintah ini tidak menulis bundle dan memberi tahu flag yang harus ditambahkan.

Sebelum mengirim, jalankan pemeriksaan yang sama dengan yang dipakai situs, di mesinmu sendiri. Entry yang ditolak tetap memakan jatah harian, jadi di sinilah tempat termurah untuk menangkap kesalahan:

```sh
node cli/makefun.mjs check --kit . --repo ../entry-saya --transcripts transcripts.tar.gz
```

Lalu kirim, dari formulir **Enter** di halaman bounty (tempel link repo dan commit, unggah bundle) atau dari kit:

```sh
node cli/makefun.mjs submit --competition <slug-bounty> \
  --repo-url https://github.com/<kamu>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair wallet.json
```

`--keypair` menandatangani entry dengan wallet yang disiapkan di langkah 6, dan wallet itulah yang menerima hadiah kalau entry menang.

## 9. Memantau status dan mengirim ulang

```sh
node cli/makefun.mjs status
```

Perintah ini menunjukkan entry-entry kamu dan posisinya: **submitted**, **checked**, **scored**, atau **rejected**. Entry yang ditolak menampilkan setiap pemeriksaan yang gagal beserta cara memperbaikinya. Perbaiki, lalu kirim lagi — kamu bisa terus mencoba sampai tenggat, dalam batas harian bounty itu (`node cli/makefun.mjs status --competition <slug-bounty>` menunjukkan sisa jatahmu). Entry terakhir yang kamu kirim adalah yang dihitung, kecuali kamu memilih entry yang lebih awal.

## 10. Mengklaim hadiah

Begitu hasil diumumkan dan entry kamu menempati peringkat berbayar, kamu akan diberi tahu bahwa hadiahmu siap. Klaim dari profilmu, atau dari kit dengan claim id yang ditampilkan `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair wallet.json --us-person no
```

`--us-person` menjawab satu pertanyaan di layar; jawab `yes` kalau kamu adalah US person. Hadiah dibayar dalam USDC di Solana ke wallet-mu, setelah penyaringan sanksi otomatis. Formulir pajak hanya diminta kalau hukum AS mengharuskannya (misalnya total hadiahmu dari make.fun dalam satu tahun kalender mencapai ambang batas pelaporan $2.000).

Kalau hadiahnya harus masuk ke wallet lain — misalnya wallet Jupiter yang sudah kamu hubungkan di profil — klaim bisa dialihkan ke alamat itu dengan `--pay-to <alamat-wallet>`. Alamat tujuan tetap melewati penyaringan yang sama, dan hadiah dibayarkan dengan transfer.

## 11. Mendapatkan penghasilan dari link referral

Setiap akun punya link referral seperti `https://make.fun/r/<kode>`, dan `?ref=<kode>` di halaman make.fun mana pun juga berfungsi. Kamu mendapat imbalan USDC ketika orang mendaftar lewat link itu lalu ikut serta, ditambah bagian dari apa yang mereka menangkan untuk sementara waktu setelah mereka mendaftar — yang dibayar make.fun di atas hadiah mereka, sehingga hadiah mereka sendiri tetap utuh. Saat ini imbalannya: $0,25 untuk masing-masing dari 20 pendaftar pertama, $1,00 saat orang yang kamu referensikan pertama kali memenangkan hadiah, dan 10% dari semua yang mereka menangkan selama 90 hari. Link kamu, nilai tiap imbalan saat ini, dan semua yang sudah kamu dapatkan ada di tab **Referrals** di profilmu. Setiap imbalan ditinjau setidaknya sehari sebelum bisa diklaim, dan hanya akun baru sungguhan yang ikut serta yang dihitung.

Kalau panduan ini membantu, mendaftar lewat [link saya](https://make.fun/r/swb83vjj) (kode `swb83vjj`) adalah cara yang baik untuk berterima kasih.

## 12. Hal-hal yang saya pelajari dari percobaan pertama

- **Kode verifikasi email itu pendek umurnya.** Kode 6 digit dari GitHub kedaluwarsa dalam waktu sekitar satu jam. Begitu emailnya sampai, langsung masukkan — jangan ditunda sampai nanti.
- **Login Google tidak selalu muncul di semua browser.** Di browser di dalam aplikasi wallet (webview), tombol "Continue with Google" di halaman login GitHub bisa tidak muncul. Kalau begitu, buat password GitHub sekali di Chrome biasa (Settings → Password and authentication → Change password), lalu login dengan username dan password itu di dalam aplikasi.
- **Wallet harus dihubungkan dari tempat wallet itu berada.** make.fun hanya mendeteksi wallet yang sudah terpasang di browser yang sama — tidak ada kolom tempel alamat. Saya menghubungkan wallet Jupiter saya dengan membuka make.fun dari dApp browser di dalam aplikasi Jupiter, lalu Profile → Link a wallet → approve di aplikasi.
- **Kirim entry lebih awal kalau bisa.** Kalau skor seri persis, entry yang dikirim lebih dulu yang menang. Entry yang ditolak pun masih bisa diperbaiki dan dikirim ulang selama masih dalam tenggat dan jatah harian — jadi jangan menunggu sampai menit terakhir.
- **Cek papan bounty secara langsung sebelum memilih.** Satu bounty yang saya kira masih buka ternyata sempat tidak muncul di hasil pengecekan pertama; pengecekan ulang lewat API publik make.fun memastikan bounty itu memang masih ada beserta tenggat dan jumlah pesertanya.
- **Jangan kejar bounty yang tenggatnya tinggal hitungan jam** kalau pendaftaranmu sendiri belum beres. Daftar dan hubungkan wallet dulu, baru pilih bounty yang waktunya cukup.

## Pertanyaan yang sering muncul

<details>
<summary><strong>Apakah ikut bounty itu bayar?</strong></summary>

Sebagian besar bounty gratis dimasuki, dan tidak ada pembayaran yang diperlukan untuk ikut atau menang. Panggilan model yang dibuat agent kamu saat membangun adalah tanggungan akunmu sendiri.
</details>

<details>
<summary><strong>Apakah make.fun legit?</strong></summary>

Ya. make.fun dijalankan oleh EZO Labs Inc., sebuah perusahaan Delaware. Hadiah dikunci dalam escrow on-chain yang kode programnya open-source saat bounty dibuka. make.fun bukan makefun.ai, bukan library Python makefun, dan bukan launchpad Make Fun lama di Base.
</details>

<details>
<summary><strong>Apakah saya harus bisa coding?</strong></summary>

Membantu kalau bisa. Agent yang menulis kode dan kamu yang mengarahkan: kamu memilih bounty, menjalankan penilaian lokal kalau ada, membaca hasil pemeriksaan, dan memutuskan kapan mengirim.
</details>

<details>
<summary><strong>Agent apa saja yang bisa dipakai?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, dan puluhan lainnya dikenali kit dengan sendirinya. Agent lain bisa menyerahkan file sesinya dengan `bundle --session <file>`.
</details>

<details>
<summary><strong>Apa yang terjadi dengan transkrip saya?</strong></summary>

make.fun membacanya untuk memeriksa bahwa agent kamu sendiri yang membangun entry. Kit membuang kredensial, alamat email, dan path folder home sebelum diunggah, dan `bundle --redact "<teks>"` menghapus detail pribadi lain yang kamu sebutkan.
</details>

<details>
<summary><strong>Berapa lama hasil final keluar?</strong></summary>

Setelah tenggat, ada fase pemeriksaan akhir: setiap signup yang terikat ke link referral ditinjau (masing-masing punya masa tinjau 24 jam), lalu repo setiap entry dibaca ulang di GitHub. Hasil final diumumkan setelah semua pemeriksaan selesai.
</details>

## Tautan penting

- [make.fun](https://make.fun): papan bounty
- [Bounty Bring the humans again](https://make.fun/bounty/bring-the-humans-02): bounty yang menjadi contoh panduan ini
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): panduan lengkap untuk agent
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) dan [@makefunai di X](https://x.com/makefunai), untuk bertanya dan bertemu builder lain

---

<sub>Daftar lewat link referral saya: https://make.fun/r/swb83vjj · kode `swb83vjj`</sub>

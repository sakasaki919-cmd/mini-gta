# Vice City — Mini GTA 6

Game open-world ala **GTA 6** dalam **satu file HTML** — HTML5 Canvas + JavaScript murni, tanpa library eksternal, tanpa file tambahan. Main sebagai **Lucia** di Vice City, Leonida: jalanan neon, Ocean Drive, pantai Vice Beach, dan polisi VCPD. Buka `index.html` di browser HP atau desktop, langsung main.

**[Mainkan di GitHub Pages](https://sakasaki919-cmd.github.io/mini-gta/)** — atau unduh `index.html` lalu buka di browser.

> Fan-made, bukan produk resmi Rockstar Games.

## Fitur

- **Karakter** — main sebagai Lucia: jalan kaki, lari, masuk & keluar mobil, bisa nyamber (carjack) mobil lalu lintas.
- **Kota Vice City** — peta grid 20×20 blok yang digenerate prosedural: jalan, gedung pastel, trotoar, taman dengan pohon palem, plus **Vice Beach** (pasir + laut) dan **Ocean Drive** di tepi pantai.
- **Mobil** — fisika sederhana: akselerasi, belok, rem/mundur. Nabrak gedung = berhenti. Tabrakan keras ngurangin HP.
- **NPC** — pejalan kaki jalan random di trotoar, mobil lalu lintas otomatis melaju di jalan (lajur kanan, belok di persimpangan), plus mobil parkir.
- **Polisi VCPD & wanted level** — bintang 1–5. Nabrak pejalan kaki, nembak, atau carjack bikin dicari. Mobil polisi VCPD ngejar dan nabrak kamu; makin banyak bintang, makin banyak polisi. Kabur 15 detik tanpa bikin ulah = bintang turun. Tembak mobil polisi 3× buat ngelumpuhin.
- **Misi (3 jenis)** — Antar Paket ke Ocean Drive (+$150), Kejar Mobil Target (+$250), Cepat ke Vice Beach (+$200, 40 detik). Ada penanda, jarak, timer, dan panah penunjuk di layar.
- **HUD** — mini-map (jalan, rumah sakit, penanda misi, polisi, pemain), uang, bintang wanted, misi aktif, health bar.
- **Audio** — suara mesin (nada ikut kecepatan), klakson, sirene polisi, suara tembakan. Semua dari Web Audio API, tanpa file audio.
- **Simpan otomatis** — uang tersimpan di `localStorage`, lanjut lagi lain kali.
- **60 FPS** — entitas dibatasi (12 mobil lalu lintas, 20 pejalan kaki, maks 5 polisi), render sederhana.

## Cara main

1. Buka `index.html` di browser (desktop atau HP).
2. Klik / ketuk layar buat mulai (dibutuhkan browser buat nyalain audio).
3. Ikuti petunjuk di layar. Tekan **M** buat mulai misi.

### Kontrol keyboard

| Tombol | Aksi |
|---|---|
| WASD / panah | Jalan & nyetir (atas = gas, bawah = rem/mundur, kiri/kanan = belok) |
| Shift | Lari |
| E | Masuk / keluar mobil (dekat mobil lalu lintas = carjack, +1 bintang) |
| Spasi / klik mouse | Tembak |
| H | Klakson |
| M | Mulai misi berikutnya |
| P | Bisukan / nyalakan suara |

### Kontrol layar sentuh (HP)

- **Joystick kiri** — jalan & nyetir (atas = gas, bawah = rem, kiri/kanan = belok)
- **Tombol kanan** — 🚗 masuk/keluar mobil • 🔫 tembak • 📯 klakson • 🏃 tahan buat lari • 🎯 MISI mulai misi
- Kontrol sentuh muncul otomatis di perangkat sentuh, bisa dihidupkan/matikan lewat tombol 🎮.

## Kalau HP habis (WASTED)

Lucia bangun lagi di rumah sakit dengan HP penuh, uang berkurang 10%, dan wanted level hilang.

## Detail teknis

- Satu file: `index.html` (~34 KB)
- Tanpa dependensi, tanpa build step
- `?autostart=1` di URL buat lewati layar mulai (buat tes/embed)

## Lisensi

MIT — bebas dipakai, diubah, dan dibagikan. Lihat [LICENSE](LICENSE).

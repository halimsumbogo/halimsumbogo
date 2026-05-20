# 📋 Issue: Panduan Kostumisasi & Saran Konten Header Profil GitHub

> **Priority:** Low (Enhancement)  
> **Label:** `ui/ux`, `creative`, `content`  
> **Assignee:** Junior Developer / AI Agent  

## Ringkasan

Dokumen ini berisi:
1. Panduan teknis untuk menukar (*swap*) gaya header profil antara **Typing SVG** dan **Terminal SVG**.
2. Saran konten teks untuk kedua gaya tersebut.
3. Laporan bug yang sudah diperbaiki (untuk referensi).

> **Penting:** Header profil hanya menampilkan SATU gaya pada satu waktu (tidak keduanya). Pemilik profil akan memilih mana yang aktif sesuai selera.

---

## 💻 Opsi 1: Typing SVG (Aktif Saat Ini)

Gaya ini menggunakan teks animasi yang berganti-ganti secara otomatis. Jika Anda ingin menggunakan gaya ini, pastikan bagian header di `README.md` berisi kode berikut:

```html
  <!-- Animated Typing SVG Header -->
  <a href="https://github.com/halimsumbogo">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=24&duration=3000&pause=1000&color=9D4EDD&center=true&vCenter=true&width=600&lines=Software+Engineer;IoT+%26+Embedded+Developer;Maker+%26+Innovator" alt="Typing SVG" />
  </a>
```

*(Kustomisasi: Anda bisa mengubah teks yang berkedip dengan mengedit teks di bagian `lines=...` pada URL di atas, misalnya: `lines=C%2B%2B+Developer;IoT+Hacker`).*

### 💡 Saran Variasi Konten Typing SVG

Berikut adalah beberapa set teks yang bisa digunakan untuk mengganti isi `lines=...` pada URL Typing SVG. Pilih salah satu set, atau campur sesuai selera.

#### Set A — Profesional & Serius
```
lines=Software+Engineer;IoT+Systems+Architect;Embedded+C%2FC%2B%2B+Developer;Bridging+Software+%26+Hardware
```
Contoh tampilan bergantian:
- `Software Engineer`
- `IoT Systems Architect`
- `Embedded C/C++ Developer`
- `Bridging Software & Hardware`

#### Set B — Kreatif & "Maker"
```
lines=I+build+things+that+blink+💡;Connecting+sensors+to+the+cloud+☁️;Maker+%26+Hardware+Hacker+🔧;Fluent+in+C%2B%2B+and+Coffee+☕
```
Contoh tampilan bergantian:
- `I build things that blink 💡`
- `Connecting sensors to the cloud ☁️`
- `Maker & Hardware Hacker 🔧`
- `Fluent in C++ and Coffee ☕`

#### Set C — Fokus Proyek RFID
```
lines=Building+secure+RFID+systems+🔐;Clean+code+for+microcontrollers+⚙️;From+sensor+to+cloud+🚀;Anti-fragmentation+EEPROM+architect+💾
```
Contoh tampilan bergantian:
- `Building secure RFID systems 🔐`
- `Clean code for microcontrollers ⚙️`
- `From sensor to cloud 🚀`
- `Anti-fragmentation EEPROM architect 💾`

#### Set D — Minimalis
```
lines=Software+Engineer;Maker+%26+Innovator
```
Contoh tampilan bergantian:
- `Software Engineer`
- `Maker & Innovator`

---

## 📟 Opsi 2: Terminal SVG

Gaya ini menggunakan aset `terminal.svg` buatan khusus yang sudah tersimpan di direktori `assets/`. Jika Anda bosan dengan teks berkedip dan ingin tampilan layar CLI/terminal *geeky*, ganti blok kode di atas dengan kode berikut:

```html
  <!-- Animated CLI Terminal Header -->
  <a href="https://github.com/halimsumbogo">
    <img src="https://raw.githubusercontent.com/halimsumbogo/halimsumbogo/main/assets/terminal.svg" alt="Halim's Terminal CLI" width="800" />
  </a>
```

*(Kustomisasi: Untuk mengubah teks yang tampil di dalam terminal, Anda cukup mengedit baris kode di dalam file `assets/terminal.svg` secara langsung. Lihat panduan di bawah.)*

### 💡 Saran Variasi Konten Terminal SVG

File `assets/terminal.svg` berisi 8 baris teks yang muncul satu per satu dengan animasi. Berikut adalah bagian-bagian yang bisa diedit (di dalam tag `<tspan>`) beserta saran kontennya:

#### Baris yang Bisa Diedit & Lokasinya di SVG

| Baris | Lokasi di SVG | Konten Saat Ini | Fungsi |
|-------|---------------|-----------------|--------|
| Line 1 | `class="line-1"` | `halim@iot-dev:~$ ./halim.sh --status` | Command prompt & perintah |
| Line 2 | `class="line-2"` | `⚡ Initializing hardware profiles...` | Pesan loading |
| Line 3 | `class="line-3"` | `[====...====] 100% loaded` | Progress bar |
| Line 4 | `class="line-4"` | `User: Halim Sumbogo` / `Role: Software Engineer & IoT Enthusiast` | Nama & jabatan |
| Line 5 | `class="line-5"` | `Hardware: C/C++, Arduino, ESP32, FreeRTOS, RFID, SPI/I2C/UART` | Keahlian hardware |
| Line 6 | `class="line-6"` | `Software: Git, GitHub Actions, Node.js, Python, Wokwi, VS Code` | Keahlian software |
| Line 7 | `class="line-7"` | `Active task: Designing modular firmware & anti-fragmentation EEPROM storage` | Aktivitas saat ini |
| Line 8 | `class="line-8"` | *(Prompt kosong dengan kursor berkedip)* | Kursor akhir |

#### Variasi A — Update "Active Task" (Paling Mudah)
Cukup ganti teks pada **Line 7** (`class="line-7"`) sesuai aktivitas terbaru. Contoh:
- `Building scalable access control systems`
- `Refactoring anti-fragmentation EEPROM buffer`
- `Debugging hardware in the real world`
- `Writing unit tests for embedded firmware`
- `Exploring MQTT protocol for IoT devices`

#### Variasi B — Update Command (Line 1)
Ganti perintah pada **Line 1** untuk suasana berbeda:
- `./halim.sh --status` → `cat /etc/halim/profile.conf`
- `./halim.sh --status` → `neofetch --halim`
- `./halim.sh --status` → `systemctl status halim.service`

#### Variasi C — Update Loading Message (Line 2)
Ganti pesan loading pada **Line 2**:
- `⚡ Initializing hardware profiles...` → `🔌 Connecting to serial port /dev/ttyUSB0...`
- `⚡ Initializing hardware profiles...` → `📡 Scanning I2C bus for peripherals...`
- `⚡ Initializing hardware profiles...` → `🔧 Loading firmware modules...`

#### Variasi D — Update Keseluruhan Gaya "Neofetch"
Jika ingin merombak total gaya terminal, ubah Line 4-7 menjadi format seperti output `neofetch`:
```
Line 4: ❯ OS:       Arduino / ESP-IDF / FreeRTOS
Line 5: ❯ Lang:     C/C++, Python, JavaScript
Line 6: ❯ Editor:   VS Code + PlatformIO
Line 7: ❯ Uptime:   Coding since 2020
```

### ⚠️ Catatan Teknis untuk Implementer
- Saat mengedit `terminal.svg`, pastikan karakter `&` ditulis sebagai `&amp;` (contoh: `Software &amp; Hardware`).
- Jangan mengubah struktur tag `<g>`, `<text>`, atau atribut `class` karena terikat dengan animasi CSS.
- Setelah mengedit, **pratinjau** file SVG di browser lokal sebelum melakukan commit.

---

## 🐞 Laporan Bug (Sudah Diperbaiki ✅)

### ~~Profile Views Badge Broken~~
- **Issue:** Gambar *Profile Views Badge* di `README.md` berstatus *broken*.
- **Penyebab:** Endpoint URL salah: `normal-badge` seharusnya `ghpvc`.
- **Status:** ✅ Sudah diperbaiki. URL sekarang: `https://komarev.com/ghpvc/?username=halimsumbogo&color=7F00FF&style=flat-square`.

---

## 🛠️ Checklist untuk Junior Programmer / AI Implementer

- [ ] Baca dan pahami panduan swap header (Opsi 1 vs Opsi 2) di atas.
- [ ] Pilih set konten teks yang diinginkan oleh pemilik profil (tanyakan jika belum ada keputusan).
- [ ] Implementasikan perubahan konten pada file yang sesuai (`README.md` untuk Typing SVG, atau `assets/terminal.svg` untuk Terminal SVG).
- [ ] Pratinjau hasil perubahan secara lokal sebelum commit.
- [ ] Commit dengan pesan yang deskriptif (contoh: `content: update typing-svg lines to Set B creative theme`).
- [ ] Push ke branch `main` dan verifikasi tampilan di halaman profil GitHub.

# Handoko-san — The Third Year Survival Quest

Undangan ulang tahun interaktif (quest style) dari versi Google Colab, sudah diperbaiki & ditambah foto / video / musik.

## Alur
1. Intro (System Alert)
2. Memory Fragments (foto + video opsional)
3. Quiz 5 level (PhD survival)
4. Laboratory Survival (tangkap bintang di canvas)
5. Final Boss — Dad Joke Monster
6. Ending + surat rahasia

## Cara pakai lokal
Buka `index.html` di browser, atau:
```bash
python3 -m http.server 8080
```

## Tambah musik
Taruh file `music.mp3` di folder yang sama dengan `index.html`.
Tombol 🔇 di pojok kanan atas untuk mute/unmute.

## Tambah foto
Ganti placeholder di bagian gallery:
```html
<img src="foto1.jpg" alt="Kenangan 1">
```

## Tambah video
Di `#video-box`, ganti placeholder dengan:
- YouTube: `<iframe src="https://www.youtube.com/embed/VIDEO_ID" allowfullscreen></iframe>`
- File lokal: `<video controls playsinline src="video.mp4"></video>`

## Deploy (GitHub Pages)
Upload `index.html` (+ music.mp3 / foto jika ada) ke repo → Settings → Pages → branch main.

## Perbaikan vs Colab asli
- Syntax array questions (koma hilang) diperbaiki
- Semua 5 soal quiz bisa dimainkan
- Index jawaban benar Q4 diperbaiki
- Timer lab sinkron
- Progress bar mengikuti 5 soal
- Tombol musik + slot foto/video

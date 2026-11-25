# muse-video-skills

Koleksi skill video untuk Muse, dirapikan dari 3 sumber publik. Dipasang 2026-11-25 untuk maryono / noglong.

## Isi

| Folder | Isi | Sumber |
|---|---|---|
| `skills/muse-video/` | Skill perencanaan video: ide → naskah / storyboard / arah seni / prompt, 6 peran, quality gate. Bahasa utama Mandarin. | LuoJiangYong/muse-video-skill (MIT) |
| `skills/muse-video-prompt-skill/` | Skill prompt Muse Video: template prompt 6 bagian → generate → sambung segmen → cek frame. | masonmosen/muse-video-prompt-skill (MIT) |
| `prompts/muse-video-prompts/` | Bukan skill — koleksi 205 prompt Muse Video dari X, masing-masing dengan kredit pembuatnya. Data di `data/prompts.json`, satu file per prompt di `prompts/`. | apimodels/muse-video-prompts (lihat LICENSE di folder itu) |

## Yang sengaja TIDAK dimasukkan

`Billsmokes/Skill-video-agent` — 33 skill gabungan, 1.471 file, 14 MB, 0 star. Terlalu besar untuk diinstall sekaligus tanpa memilih satu per satu, dan scan penuhnya belum selesai. Kalau mau, tambahkan sub-skill tertentu dari repo itu satu per satu nanti, dengan review terpisah.

## Yang dirapikan

- Media besar dihapus dari salinan ini: gambar `.jpg`, GIF, `.mp4`, dan `.xlsx` di `muse-video` (total sumber ~38 MB → salinan ini ~4,6 MB, sebagian besar `prompts.json`).
- File teks dipertahankan apa adanya, termasuk lisensi masing-masing sumber di foldernya.
- Struktur disatukan: `skills/` untuk skill yang bisa dipasang, `prompts/` untuk referensi prompt.

Lihat sumber aslinya untuk gambar contoh dan preview lengkap — tautan ada di `SOURCES.md`.

## Cara pakai di Muse

Salin folder skill yang dibutuhkan ke direktori skill Muse:

- `skills/muse-video/`
- `skills/muse-video-prompt-skill/`

`prompts/muse-video-prompts/` cukup dibaca sebagai referensi, tidak perlu dipasang sebagai skill.

## Catatan keamanan

- Script Python di `muse-video/scripts/` dan `muse-video-prompt-skill/bin/extract_frames.py` hanya memproses file lokal (ffmpeg/ffprobe). Tidak ada pengiriman data ke server luar yang ditemukan pada pengecekan awal.
- Jangan menjalankan script dari sumber yang belum dicek, dan jangan memasukkan API key ke dalam repo ini.

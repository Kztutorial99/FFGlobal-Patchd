# IL2CPP Metadata — OB54 Free Fire Global

Sumber APK: `OB54 Free Fire Global.apk` (com.dts.freefireth 1.126.2, build 2019120816)
Path di APK: `assets/bin/Data/Managed/Metadata/global-metadata.dat`

| Item | Nilai |
|---|---|
| Ukuran | 55.738.848 byte |
| SHA-256 | 05ad9d700b9ed1375b0c79b99a03555efe75ed8591f757a59e93c04df391a257 |
| Engine | Unity IL2CPP (libil2cpp.so ~192 MB) |
| Header | Diacak/dienkripsi (magic `0xFAB11BAF` tidak ditemukan) |
| String pool | Plaintext — bisa dibaca |

## Isi folder `metadata/`
- `assemblies.txt` — 57 assembly (.dll) yang ter-embed
- `namespaces.txt` — 2.679 namespace / nama bertitik
- `type_names.txt.gz` — 216.507 kandidat nama kelas/tipe
- `method_names.txt.gz` — 106.387 kandidat nama method/field
- `strings_all.txt.gz` — 517.638 string unik hasil dump mentah
- `hash.txt` — checksum file metadata

File biner `global-metadata.dat` diunggah sebagai asset Release tag `v1.0-metadata`
(ukurannya melewati batas file biasa yang nyaman untuk repo).

## Catatan
Header metadata diacak oleh proteksi game, sehingga dump struktural penuh
(mapping tipe ↔ method ↔ RVA lewat Il2CppDumper) tidak bisa langsung dilakukan
tanpa mereplikasi rutin dekripsi dari `libil2cpp.so`. Dump di sini berbasis
pembacaan string pool yang masih plaintext.

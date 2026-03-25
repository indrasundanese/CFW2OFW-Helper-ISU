# CFW2OFW Helper (TLS 1.2 Network Fix)

![Platform](https://img.shields.io/badge/Platform-Windows-blue.svg)
![Framework](https://img.shields.io/badge/.NET_Framework-4.8-purple.svg)
![License](https://img.shields.io/badge/License-WTFPL-green.svg)

This is a forked and updated version of the original [CFW2OFW Helper](https://github.com/friendlyanon/CFW2OFW-Helper) by friendlyanon. 

## ⚠️ Why this fork? (Apa yang baru?)
The original tool has been broken for years, constantly showing a **"No internet connection found"** error. This happens because Sony's Zeus PlayStation servers dropped support for older security protocols, while the original tool still relied on outdated TLS 1.0/SSL3.

**This fork fixes the issue by:**
1. Upgrading the target framework to **.NET Framework 4.8**.
2. Forcing the `ServicePointManager` to use **TLS 1.2**.
3. Restoring the tool's ability to automatically communicate with Sony's servers and download official game updates.

*(Versi asli dari tool ini sudah lama mati dan selalu menampilkan pesan error "No internet connection". Fork ini memperbaiki masalah tersebut dengan memperbarui basis program ke .NET 4.8 dan memaksa penggunaan protokol keamanan TLS 1.2, sehingga tool bisa kembali mengunduh update resmi dari server Sony tanpa masalah).*

---

## 🛠️ Requirements (Persyaratan)
* Windows OS
* [.NET Framework 4.8 Runtime](https://dotnet.microsoft.com/en-us/download/dotnet-framework/net48)
* `make_npdata.exe` (Must be placed in the same folder as this executable / Wajib diletakkan berdampingan dengan aplikasi ini).

## 🚀 How to Use (Cara Penggunaan)
1. Extract your PS3 disc game. You should have a folder containing `PS3_GAME` and `PS3_DISC.SFB`.
2. Ensure the folder name matches the Game ID (e.g., `BLES01234`).
3. **Drag and drop** that folder onto `CFW2OFW Helper.exe`.
4. The tool will automatically fetch the patch, extract data, and convert it into a digital format (e.g., `NPEB01234`).

---

## ☕ Support the Developer (Dukungan)
This network fix was maintained to help the game modding and localization community streamline their workflow. If you find this tool or my Indonesian game translation projects helpful, consider supporting my work!

[![Trakteer](https://img.shields.io/badge/Traktir_Kopi-Trakteer-red?style=for-the-badge&logo=trakteer)](https://trakteer.id/USERNAME_KAMU_DISINI)

*(Dukung proyek-proyek pembuatan alat modding dan lokalisasi game bahasa Indonesia lainnya dengan mentraktir saya kopi melalui tautan di atas!)*

---

## 📝 Credits
* **friendlyanon** - For the original source code and logic.
* **mathieulh** - PKG code.
* **Hykem** - make-npdata.
* **Indra** - Network fix (TLS 1.2 implementation) & .NET 4.8 upgrade.

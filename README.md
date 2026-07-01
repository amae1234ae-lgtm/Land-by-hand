# LAND

<div align="center">

![LAND Logo](Resources/Icons/LandByHand.ico)

**Professional Revit Plugin for Advanced Topography & Surface Management**

[![License](https://img.shields.io/badge/license-Commercial-blue.svg)](LICENSE)
[![Revit Support](https://img.shields.io/badge/Revit-2023%20|%202024%20|%202025%20|%202026-orange.svg)](https://www.autodesk.com/products/revit)
[![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)](https://www.microsoft.com/windows)
[![.NET](https://img.shields.io/badge/.NET-Framework%204.8%20|%20.NET%208.0-purple.svg)](https://dotnet.microsoft.com/)

---

*Streamline your landscape design workflow with powerful topography tools*

</div>

## 🌟 Overview

**LAND** is a professional Revit plugin designed for architects, landscape architects, and civil engineers who work with complex topography and surface design. The plugin provides advanced tools for surface matching, conversion, and pipe management that significantly reduce manual work and improve precision in your BIM workflows.

## ✨ Key Features

### 🏔️ **Topography Conversion**
- **Toposolid → Topography**: Convert modern Toposolid elements to legacy Topography surfaces
- Preserves surface geometry and properties
- Seamless workflow between Revit versions

### 🎯 **Advanced Surface Matching**
- **Toposolid → Topography**: Match Toposolid surfaces to existing topography
- **Toposolid → Toposolid**: Align multiple Toposolid surfaces precisely  
- **Floor Matching**: Conform floor slabs to terrain surfaces automatically
- **Railing Alignment**: Align railing base elevations to follow terrain contours

### 🔧 **Pipe Management**
- **Pipe Offset Tools**: Set precise vertical offsets for pipes from any surface
- Works with topography, toposolid, and floor surfaces
- Batch processing capabilities

### � **Sheet & View Management**
- **Create Sheets**: Bulk-create Revit sheets from an Excel spreadsheet
- **Create Views**: Generate plan/section/elevation views from Excel data
- Custom naming, numbering, and title block assignment

### 🖨️ **Export & Print**
- **Print to PDF**: Print selected sheets directly to PDF with one click
- **Export to DWG**: Export sheets to DWG files with custom naming rules
- **Export P.XYZ**: Export surface geometry as point cloud (XYZ coordinates) for survey use

### �🔒 **Professional Licensing**
- Secure activation system
- 14-day free trial
- Machine-locked licensing prevents unauthorized copying
- Automatic license renewal reminders

## 🛠️ Installation

### System Requirements
- **Autodesk Revit**: 2023, 2024, 2025, or 2026
- **Operating System**: Windows 10/11 (x64)
- **.NET Framework**: 4.8 (Revit 2024) or .NET 8.0 (Revit 2025+)
- **Administrator privileges** for installation

### Quick Installation
1. Download the latest `LAND-Setup.exe` from [releases](../../releases)
2. Run the installer as Administrator
3. Select your Revit version(s)
4. Complete the installation wizard
5. Restart Revit

### Manual Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/LAND.git
cd LAND

# Build for specific Revit version
dotnet build LAND.csproj -c Revit2025 -p:Platform=x64

# Copy files to Revit addins folder
# See installation guide for detailed paths
```

## 🚀 Quick Start

### First Launch
1. Open Revit after installation
2. Look for the **"LAND"** tab in the ribbon
3. Start your 14-day free trial or activate with your license key

### Basic Workflow
1. **Select your target surface** (Topography or Toposolid)
2. **Choose the appropriate tool** from the Land By Hand ribbon
3. **Select elements to modify** (floors, railings, pipes, etc.)
4. **Configure matching parameters** in the dialog
5. **Apply changes** and review results

## 📊 Supported Revit Versions

| Revit Version | Support Status | .NET Framework | Notes |
|---------------|----------------|----------------|-------|
| **2026** | ✅ Full Support | .NET 8.0 | Latest features |
| **2025** | ✅ Full Support | .NET 8.0 | All tools available |
| **2024** | ✅ Full Support | .NET Framework 4.8 | All tools available |
| **2023** | ✅ Limited Support | .NET Framework 4.8 | Floor & Railing only* |

*Revit 2023 doesn't support Toposolid API, so Toposolid-related features are not available.

## 🧰 All Available Tools

| Panel | Tool | Description | Revit |
|-------|------|-------------|-------|
| Tools | Convert TS → Topo | Convert Toposolid to Topography | 2024–2026 |
| Tools | Match TS → Topo | Match Toposolid to Topography surface | 2024–2026 |
| Tools | Match TS → TS | Align Toposolid to Toposolid | 2024–2026 |
| Tools | Match Floor | Conform floor slab to terrain | 2023–2026 |
| Tools | Match Railing | Align railing to terrain | 2023–2026 |
| Tools | Pipe Offset | Offset pipes from surface elevation | 2023–2026 |
| Sheets | Create Sheets | Bulk-create sheets from Excel | 2023–2026 |
| Sheets | Create Views | Generate views from Excel data | 2023–2026 |
| Print | Print to PDF | Print sheets to PDF | 2023–2026 |
| Print | Export to DWG | Export sheets as DWG files | 2023–2026 |
| Print | Export P.XYZ | Export surface as XYZ point cloud | 2023–2026 |
| License | Activate | Enter license key | 2023–2026 |

## 🎮 Usage Guide

### Converting Toposolid to Topography
```
1. Select a Toposolid element
2. Click "Convert TS→Topo" button
3. The plugin automatically creates a matching Topography surface
4. Original Toposolid remains unchanged
```

### Surface Matching Operations
```
1. Click the appropriate "Match" button (TS→Topo, Floor, etc.)
2. Select the target surface (what to match TO)
3. Select the elements to modify (what to match FROM)
4. Adjust tolerance and offset settings
5. Click "Apply" to execute the matching
```

### Pipe Offset Management
```
1. Click "Pipe Offset" button
2. Select the reference surface
3. Choose pipes to offset
4. Set vertical offset distance
5. Apply changes
```

### Create Sheets from Excel
```
1. Prepare an Excel file with sheet numbers and names
2. Click "Create Sheets" in the Sheets panel
3. Browse to your Excel file
4. Select the title block type
5. Click Create — all sheets are generated instantly
```

### Create Views from Excel
```
1. Prepare an Excel file with view names and levels
2. Click "Create Views" in the Sheets panel
3. Browse to your Excel file and configure options
4. Click Create
```

### Print to PDF / Export DWG
```
1. Click "Print PDF" or "Export DWG" in the Print panel
2. Select the sheets to export
3. Choose the output folder
4. Click Export
```

### Export Surface as XYZ Points
```
1. Select a Toposolid or Topography surface
2. Click "Export P.XYZ" in the Print panel
3. Choose output folder and point density
4. Click Export — opens a .xyz file ready for survey software
```

## 🏗️ Development

### Building from Source
```bash
# Prerequisites
# - Visual Studio 2022 or later
# - Revit 2023+ SDK
# - .NET 8.0 SDK

# Clone repository
git clone https://github.com/yourusername/LandByHand.git
cd LandByHand

# Build for all Revit versions
dotnet build LandByHand.csproj -c Revit2023 -p:Platform=x64
dotnet build LandByHand.csproj -c Revit2024 -p:Platform=x64  
dotnet build LandByHand.csproj -c Revit2025 -p:Platform=x64
dotnet build LandByHand.csproj -c Revit2026 -p:Platform=x64

# Create installer
cd Installer
powershell -ExecutionPolicy Bypass -File .\Compile-Installer.ps1
```

### Project Structure
```
LandByHand/
├── App.cs                          # Main plugin entry point
├── Cmd_*.cs                        # Command implementations  
├── *Window.xaml(.cs)               # UI dialogs
├── *Matcher.cs                     # Core matching algorithms
├── Resources/                      # Icons and assets
├── Installer/                      # Installation scripts
├── tools/                          # Development utilities
└── README.md                       # This file
```

## 📞 Support & Contact

### 💰 Purchase & Licensing
- **Purchase**: [Buy LAND](https://amae1234ae-lgtm.github.io/Land-by-hand/buy)
- **Trial**: 14-day free trial available
- **Enterprise**: Volume licensing available

### 🐛 Issues & Bug Reports
- Create an issue on [GitHub Issues](../../issues)
- Include Revit version, error messages, and steps to reproduce

### 📧 Contact
- **Company**: HAND
- **Email**: [handplugins@gmail.com](mailto:handplugins@gmail.com)
- **Website**: [LAND Official](https://amae1234ae-lgtm.github.io/Land-by-hand/)

## 📄 License

This software is commercial and requires a valid license for use beyond the trial period.

### Trial License
- 14 days free trial
- Full functionality
- No credit card required

### Commercial License
- Perpetual license
- Free updates for 1 year
- Machine-locked activation
- Professional support

## 🙏 Credits

Developed by **HAND** with passion for improving BIM workflows.

Special thanks to the Revit API community and all beta testers who helped refine this plugin.

---

<div align="center">

**Made with ❤️ for the BIM Community**

[🌐 Website](https://amae1234ae-lgtm.github.io/Land-by-hand/) • [📥 Download](../../releases) • [🐛 Report Issue](../../issues) • [💬 Discussions](../../discussions)

</div>


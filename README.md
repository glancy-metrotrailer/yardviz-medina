# TrailerViz Pro - Semi-Trailer GPS Parking Visualizer

A professional web application for visualizing GPS-tracked semi-trailers on a real satellite map with automatic parking space assignment.

## ✨ Features

### Core Functionality
- **Real Satellite Imagery** - Uses MapTiler/MapLibre GL JS for high-quality satellite maps
- **Configurable Parking Grid** - Customize rows, columns, and space dimensions
- **Auto-Alignment** - Trailers automatically snap to nearest available parking spaces
- **Interactive Map** - Click trailers for details, zoom, pan, and rotate

### New Features (v2.0)
- **🔍 Search & Filter** - Quickly find trailers by Asset ID
- **📥 Export Options** - Download as PNG, PDF, or print directly
- **🌙 Dark Mode** - Toggle between light and dark themes
- **📱 Mobile Responsive** - Works on tablets and mobile devices
- **🎨 Status Indicators** - Color-coded trailer icons (Active/Idle/Maintenance)
- **💡 Hover Tooltips** - Quick info display on trailer hover
- **🎯 Zoom to Trailer** - Click any trailer in the list to fly to its location
- **🖨️ Print-Friendly** - Optimized view for printing
- **💾 Local Storage** - Automatically saves your data between sessions
- **📊 CSV Support** - Import from Excel (.xlsx, .xls) or CSV/TSV files
- **✅ Data Validation** - Validates GPS coordinates with helpful error messages

## 🚀 Quick Start

1. Open `index.html` in any modern web browser
2. Upload your trailer data file (Excel or CSV)
3. Trailers automatically appear on the map!

## 📁 File Format

Your data file should contain these columns:

| Column | Required | Description |
|--------|----------|-------------|
| Asset ID | Yes | Unique trailer identifier |
| Latitude | Yes | GPS latitude coordinate |
| Longitude | Yes | GPS longitude coordinate |
| Heading | No | Direction in degrees (0-360) |
| Status | No | Active, Idle, or Maintenance |

### Example CSV:
```csv
Asset ID,Latitude,Longitude,Heading,Status
TRL-001,41.148723,-81.897567,90,Active
TRL-002,41.148623,-81.897867,180,Idle
```

## ⚙️ Configuration

### Grid Settings
Access via the gear icon (⚙️) on the map:
- **Rows** - Number of parking rows (default: 12)
- **Columns** - Number of columns (default: 20)
- **Space Width** - Width in meters (default: 3m)
- **Space Length** - Length in meters (default: 18m)
- **Spacing** - Gap between spaces (default: 1m)

### Map Styles
Choose from four map styles:
- 🛰️ Satellite (default)
- 🗺️ Streets
- 🏔️ Outdoor
- 📍 Basic

## 🎨 Status Colors

| Status | Color | Description |
|--------|-------|-------------|
| Active | 🟢 Green | Trailer in use |
| Idle | 🟡 Orange | Trailer parked/waiting |
| Maintenance | 🔴 Red | Trailer needs service |

## 💾 Data Persistence

Your data is automatically saved to browser localStorage:
- Uploaded trailer data
- Grid configuration settings
- Theme preference (light/dark)

Data persists until you clear browser data or upload a new file.

## 📤 Export Options

1. **PNG Image** - High-resolution screenshot of the map
2. **PDF Document** - A4 landscape PDF for reports
3. **Print** - Opens system print dialog

## 🔧 Technical Details

### Dependencies (loaded via CDN)
- MapLibre GL JS 3.6.2
- XLSX.js 0.18.5
- Papa Parse 5.4.1
- html2canvas 1.4.1
- jsPDF 2.5.1

### Browser Support
- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

### Property Location
Centered on: 1030 W Liberty St, Medina, OH 44256
Coordinates: 41.148623908332276, -81.89786783155066

## 📝 Changelog

### v2.0.0
- Added search/filter functionality
- Added export to PNG/PDF
- Added dark mode toggle
- Added mobile responsive design
- Added status-based trailer icons
- Added hover tooltips
- Added zoom-to-trailer from list
- Added print-friendly view
- Added localStorage persistence
- Added CSV/TSV file support
- Added comprehensive data validation
- Improved error handling and user feedback

### v1.0.0
- Initial release
- Basic map with satellite imagery
- Parking grid overlay
- Excel file upload
- Trailer placement with auto-alignment

## 🆘 Troubleshooting

**Map not loading?**
- Check internet connection (requires MapTiler API)
- Try a different browser
- Clear browser cache

**Trailers not appearing?**
- Verify file format matches expected columns
- Check for validation errors in the sidebar
- Ensure coordinates are within range

**Export not working?**
- Allow pop-ups for the page
- Try a different browser
- Check browser console for errors

## 📄 License

MIT License - Free for commercial and personal use.

## 🤝 Support

For issues or feature requests, please contact your system administrator.

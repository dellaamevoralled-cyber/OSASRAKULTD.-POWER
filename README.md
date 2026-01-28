# ⚡ EngineerDogo Solar System Calculator

A powerful, modern web application for designing solar energy systems with intelligent calculations for inverters, batteries, solar panels, backup generators, and cable sizing.

## 🌟 Features

- **Appliance Management**: Add unlimited appliances with wattage and daily usage hours
- **Automatic Calculations**: Real-time system sizing based on your load profile
- **Inverter Sizing**: Automatic inverter selection with safety margins
- **Battery System Design**: Calculate battery capacity, configuration (series/parallel), and backup duration
- **Solar Panel Sizing**: Determine required solar panels based on daily energy consumption
- **Generator Recommendations**: Suggest appropriate backup generators from a comprehensive database
- **Cable Sizing**: Calculate optimal DC and AC cable sizes for safe, efficient power transmission
- **Energy Analytics**: Daily, monthly, and peak power visualizations with pie charts and bar graphs
- **PDF Report Generation**: Export complete system design as a professional PDF report
- **Modern Dark Theme**: Beautiful, responsive UI with vibrant cyan and orange accents
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices

## 🎯 System Calculations

### Energy & Power
- Instantaneous load (W)
- Daily energy demand (kWh/day & kWh/month)
- Peak power requirements

### Inverter & Battery System
- Inverter sizing with safety factor
- Battery backup duration
- Battery capacity requirements (kWh & Ah)
- Series/Parallel configuration for your specific battery units

### Solar System
- Required number of solar panels
- Effective output considering derating factors
- Sun hours per day configuration

### Backup Generator
- Recommended generator model and capacity
- Sizing margin above peak load
- Fuel type specifications

### Cable Sizing
- **DC Cable** (Battery ↔ Inverter): Calculated for your system voltage
- **AC Cable** (Inverter → Load): Calculated for 230V, 0.95 PF
- **Solar DC Cable** (Panel → Inverter): Calculated for solar array specifications
- Results shown in both AWG and mm² standards

## 🚀 Quick Start

### Option 1: GitHub Pages (Recommended)

1. **Fork or Clone This Repository**
   ```bash
   git clone https://github.com/yourusername/engineerdogo-solar-calculator.git
   cd engineerdogo-solar-calculator
   ```

2. **Push to GitHub**
   - Create a new repository on GitHub named `engineerdogo-solar-calculator`
   - Or use `yourusername.github.io` for a user site

3. **Enable GitHub Pages**
   - Go to Repository Settings → Pages
   - Select `Deploy from a branch`
   - Choose branch: `main` (or `master`)
   - Select folder: `/ (root)`
   - Save

4. **Access Your Site**
   - User site: `https://yourusername.github.io`
   - Project site: `https://yourusername.github.io/engineerdogo-solar-calculator`

### Option 2: Local Testing

1. Open the `index.html` file directly in your browser
2. No installation or build process required
3. All calculations work offline after the page loads

### Option 3: Simple HTTP Server (Testing)

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (with http-server)
npx http-server
```

Then visit `http://localhost:8000`

## 📖 How to Use

1. **Add Appliances**
   - Enter appliance name (e.g., "Refrigerator")
   - Set quantity and wattage
   - Enter daily usage hours
   - Click "Add" button

2. **Configure System Settings**
   - Set system voltage (typical: 24V, 48V, 96V)
   - Set backup battery hours
   - Adjust battery depth of discharge (DOD)
   - Set inverter safety factor
   - Configure battery specifications
   - Set solar panel wattage and derating
   - Input daily sun hours for your location

3. **View Results**
   - Calculations update automatically
   - Review Energy & Power requirements
   - Check Inverter & Battery sizing
   - See Solar System requirements
   - Get Generator recommendation
   - Use suggested Cable sizes

4. **Export Report**
   - Click "PDF Report" button
   - Professional PDF with all calculations and charts

## 🛠️ Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Charts**: Chart.js 4.4.0
- **PDF Generation**: jsPDF 2.5.1
- **Canvas Rendering**: html2canvas 1.4.1
- **Hosting**: GitHub Pages (Static Site)

## 📊 Configuration Options

### System Voltage
- 12V: Small off-grid systems
- 24V: Residential solar systems
- 48V: Advanced home systems (recommended)
- 96V: Large commercial systems

### Battery Settings
- **DOD (Depth of Discharge)**: Typically 0.8 (80%)
- **Battery V per unit**: Standard battery cell voltage (12V, 24V)
- **Battery Ah per unit**: Ampere-hour capacity per battery

### Solar Settings
- **Panel Watt**: Individual panel capacity (400W typical)
- **Derating Factor**: 0.75-0.85 (accounts for real-world losses)
- **Sun Hours**: Average daily peak sun hours for your location

## 💡 Tips for Accurate Calculations

1. **Load Profile**: Be realistic about appliance usage hours
2. **Safety Margin**: Inverter safety factor of 1.2-1.25 is recommended
3. **Battery Backup**: Standard is 8-12 hours for off-grid systems
4. **Derating**: Account for temperature, dust, angles (typically 0.75-0.8)
5. **Sun Hours**: Check your location's average peak sun hours
6. **Cable Sizing**: Always use the calculated values for proper system design

## 📱 Browser Support

- Chrome/Chromium (Latest)
- Firefox (Latest)
- Safari (Latest)
- Edge (Latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🐛 Known Limitations

- Charts cannot be resized after generation
- PDF export uses image rendering (high resolution)
- Calculations assume ideal system conditions

## 🔄 Future Enhancements

- [ ] Multi-language support
- [ ] Historical data storage (LocalStorage)
- [ ] System cost estimation
- [ ] Efficiency loss calculations
- [ ] Temperature impact on battery
- [ ] Seasonal variation analysis
- [ ] Export to different formats (Excel, JSON)
- [ ] Dark/Light theme toggle
- [ ] System comparison tool

## 📝 License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Support

For issues, questions, or suggestions:
- Open an issue on GitHub
- Please include a description and any relevant screenshots

## 🙏 Acknowledgments

- Chart.js for beautiful data visualization
- jsPDF for PDF generation
- html2canvas for screenshot capabilities
- All contributors and users

## 📚 Resources

- [Solar System Design Guide](https://example.com)
- [Battery Sizing Calculator](https://example.com)
- [Generator Sizing Standards](https://example.com)
- [Electrical Cable Standards](https://example.com)

---

**Made with ⚡ by EngineerDogo Platform**

*Advanced Solar System Calculator © 2026*

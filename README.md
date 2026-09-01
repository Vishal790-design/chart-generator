# 📊 Chart Generator

A user-friendly web application that transforms Excel data into beautiful, interactive charts with an intuitive interface.

## Features

✨ **Easy File Upload**
- Drag and drop Excel files
- Support for .xlsx and .xls formats
- Real-time file validation

📈 **Multiple Chart Types**
- Bar Charts
- Line Charts
- Pie Charts
- Doughnut Charts
- Scatter Charts

🎨 **Beautiful UI**
- Modern, responsive design
- Works perfectly on desktop and mobile
- Smooth animations and transitions

🛠️ **Flexible Configuration**
- Select data from multiple sheets
- Choose X and Y axis columns
- Customize chart titles
- Real-time preview

📥 **Export Options**
- Download charts as PNG images
- High-quality exports

## Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Vishal790-design/chart-generator.git
   cd chart-generator
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

## Usage

1. **Start the server**
   ```bash
   npm start
   ```
   Or for development with auto-reload:
   ```bash
   npm run dev
   ```

2. **Open your browser**
   Navigate to `http://localhost:3000`

3. **Upload your Excel file**
   - Drag and drop or browse to select your Excel file
   - The application will automatically detect all sheets

4. **Configure your chart**
   - Select the sheet containing your data
   - Choose the columns for X and Y axes
   - Select the chart type you prefer
   - Add a custom title (optional)

5. **Generate and download**
   - Click "Generate Chart" to create your visualization
   - Download the chart as a PNG image using the download button

## Project Structure

```
chart-generator/
├── public/
│   ├── index.html      # Main HTML file
│   ├── styles.css      # CSS styling
│   ├── app.js          # Frontend JavaScript
├── server.js           # Express server
├── package.json        # Project dependencies
└── README.md           # This file
```

## Technologies Used

- **Backend**: Node.js, Express.js
- **File Processing**: XLSX (Excel parsing)
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Charting**: Chart.js
- **File Upload**: Multer

## API Endpoints

### POST `/api/upload`
Upload and process an Excel file

**Request:**
- Method: POST
- Content-Type: multipart/form-data
- Body: file (Excel file)

**Response:**
```json
{
  "success": true,
  "sheetNames": ["Sheet1", "Sheet2"],
  "data": {
    "Sheet1": [...],
    "Sheet2": [...]
  }
}
```

## Supported Excel Formats

- `.xlsx` - Excel Open XML Spreadsheet (Recommended)
- `.xls` - Excel 97-2003 Workbook

## Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Features in Detail

### Multi-Sheet Support
Upload Excel files with multiple sheets and select which one to visualize.

### Dynamic Column Selection
Automatically detects columns in your Excel file and lets you choose which data to display.

### Chart Customization
- Change chart types instantly
- Customize titles in real-time
- Preview changes immediately

### Responsive Design
Works seamlessly on:
- Desktop computers
- Tablets
- Mobile phones

### Color-Coded Charts
Charts automatically use distinct colors for different data points for better visibility.

## Troubleshooting

### File won't upload
- Ensure your file is in .xlsx or .xls format
- Check that the file size is reasonable
- Try refreshing the page and uploading again

### Chart not generating
- Verify you've selected both X and Y axis columns
- Ensure your data contains numeric values for the Y axis
- Check browser console for any error messages

### Port already in use
```bash
# Change the port by setting the PORT environment variable
PORT=3001 npm start
```

## Future Enhancements

- [ ] Support for CSV files
- [ ] Multiple datasets in one chart
- [ ] Advanced customization (colors, fonts, etc.)
- [ ] Data filtering options
- [ ] Export to PDF
- [ ] Chart templates
- [ ] Data validation and cleaning
- [ ] Real-time collaboration

## License

MIT License - feel free to use this project for personal or commercial purposes.

## Support

For issues, questions, or suggestions, please open an issue on GitHub.

## Credits

Built with ❤️ for data visualization enthusiasts.

---

**Happy Charting!** 📊✨

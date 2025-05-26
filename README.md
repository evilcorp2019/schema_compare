# 🔄 CSV Schema Comparison Tool

A powerful web-based tool for comparing database schemas between different environments. Upload two CSV files and get comprehensive analysis with Excel reports.

## 🌟 Features

- **📊 Schema Comparison**: Compare database schemas between Production, Construction, or any two environments
- **📈 Detailed Analysis**: Identify missing records, schema changes, and field differences
- **📋 Excel Reports**: Generate comprehensive Excel reports with multiple sheets
- **🎨 Modern UI**: Beautiful, responsive interface with real-time processing
- **🔒 Secure**: All processing happens in your browser - no data leaves your device
- **⚡ Fast**: Instant analysis and results

## 🚀 Live Demo

**[Try the tool here →](https://evilcorp2019.github.io/schema_compare)**

## 📝 How to Use

1. **Configure Environments**: Set names for your two environments (e.g., "Production" and "Construction")
2. **Upload CSV Files**: Upload one CSV file for each environment
3. **Compare**: Click "Compare Files" to analyze the differences
4. **Download Results**: Get a comprehensive Excel report with detailed analysis

## 📊 Output Analysis

The tool generates the same analysis as the original Python script:

### 📋 Excel Report Sheets:
- **Reconciliation**: Summary of record counts and changes
- **Master**: Complete merged dataset with all comparisons
- **Master_change**: Records with schema differences
- **Summary_change**: Detailed list of field changes
- **Missing_in_[Env1]**: Records present only in Environment 2
- **Missing_in_[Env2]**: Records present only in Environment 1

### 🔍 Comparison Fields:
- Type
- Computed
- Length
- Precision
- Scale
- Nullable
- TrimTrailingBlanks
- FixedLenNullInSource
- Collation

## 🛠️ Development

### Prerequisites
- Node.js 18+
- npm or yarn

### Setup
```bash
# Clone the repository
git clone https://github.com/evilcorp2019/schema_compare.git
cd schema_compare

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

## 🚢 Deployment

### GitHub Pages (Automated)
1. Push to main branch
2. GitHub Actions automatically builds and deploys
3. Access at: `https://evilcorp2019.github.io/schema_compare`

### Manual Deployment
```bash
npm run build
# Upload dist/ folder to your web server
```

## 📁 Project Structure

```
├── index.html              # Main HTML file with embedded React app
├── package.json            # Dependencies and scripts
├── vite.config.js          # Build configuration
├── tailwind.config.js      # Styling configuration
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions deployment
└── README.md              # This file
```

## 🔧 Configuration

The project is configured for deployment to GitHub Pages at:
`https://evilcorp2019.github.io/schema_compare`

## 📦 Dependencies

- **React 18**: UI framework
- **Tailwind CSS**: Styling
- **PapaParse**: CSV parsing
- **SheetJS (xlsx)**: Excel file generation
- **Lucide React**: Icons
- **Vite**: Build tool

## 🎯 Features Equivalent to Python Script

This web application performs **exactly the same operations** as the original Python pandas script:

- ✅ **Data Cleaning**: Removes spaces from table/column names
- ✅ **Environment Suffixes**: Adds environment names to schema columns
- ✅ **Outer Join**: Merges datasets with merge indicators
- ✅ **Comparison Logic**: Creates comparison columns for all specified fields
- ✅ **Change Detection**: Counts differences per record
- ✅ **Excel Output**: Generates identical report structure with multiple sheets
- ✅ **Reconciliation**: Provides same summary statistics

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

MIT License - feel free to use this tool for your projects!

## 🆘 Support

If you encounter any issues:
1. Check the browser console for errors
2. Ensure CSV files have the required columns:
   - Table Name
   - Column_name
   - Type, Computed, Length, Prec, Scale, Nullable, TrimTrailingBlanks, FixedLenNullInSource, Collation
3. Try with smaller files first
4. Open an issue on [GitHub](https://github.com/evilcorp2019/schema_compare/issues)

## 📈 Version History

- **v1.0.0** - Initial release with complete Python script functionality
- Modern web interface for CSV schema comparison
- Automated GitHub Pages deployment

---

**Built with ❤️ for database schema management**  
**Repository**: [evilcorp2019/schema_compare](https://github.com/evilcorp2019/schema_compare)

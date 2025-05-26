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

**[Try the tool here →](https://YOUR_USERNAME.github.io/YOUR_REPO_NAME)**

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
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

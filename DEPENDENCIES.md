# Dependencies Guide - Displacement Volume Analyzer

## Required Dependencies

Your app needs **only 2 packages**:

### 1. Streamlit (Web Framework)
```
streamlit>=1.28.0
```
**What it does:** Creates the web interface, widgets, and handles user interactions

### 2. Pandas (Data Processing)
```
pandas>=2.0.0
```
**What it does:** Handles CSV file uploads and data table display

## Built-in Python Libraries (No Installation Needed)

These come with Python automatically:
- `json` - Saves project data
- `os` - File system operations
- `time` - Delays and timing
- `datetime` - Date handling
- `pathlib` - File path management

---

## Installation

### Quick Install (Both Dependencies)
```bash
pip install streamlit pandas
```

### Or From requirements.txt
```bash
pip install -r requirements.txt
```

---

## requirements.txt File

Your `requirements.txt` should contain:

```
streamlit>=1.28.0
pandas>=2.0.0
```

**That's it!** Just 2 lines.

---

## Version Requirements

### Minimum Versions
- **Python:** 3.7 or higher
- **Streamlit:** 1.28.0 or higher
- **Pandas:** 2.0.0 or higher

### Recommended Versions
- **Python:** 3.9+ (best compatibility)
- **Streamlit:** Latest stable version
- **Pandas:** Latest stable version

---

## Verification

### Check If Dependencies Are Installed

**Check Python:**
```bash
python --version
```
Should show: `Python 3.7+`

**Check Streamlit:**
```bash
streamlit --version
```
Should show: `Streamlit, version 1.28.0+`

**Check Pandas:**
```bash
python -c "import pandas; print(pandas.__version__)"
```
Should show: `2.0.0+`

### Run Diagnostic Test
```bash
python diagnostic_test.py
```
This will check **everything** and tell you exactly what's missing.

---

## For Streamlit Cloud Deployment

When deploying to Streamlit Cloud:

1. ✅ **Include requirements.txt** in your repository
2. ✅ Streamlit Cloud automatically installs dependencies
3. ✅ No manual installation needed

**Important:** Make sure `requirements.txt` is in the **root directory** of your repository.

---

## Troubleshooting

### "No module named 'streamlit'"
```bash
pip install streamlit
```

### "No module named 'pandas'"
```bash
pip install pandas
```

### Using pip3 instead of pip (Mac/Linux)
```bash
pip3 install streamlit pandas
```

### Permission errors
```bash
pip install --user streamlit pandas
```

### Upgrade existing packages
```bash
pip install --upgrade streamlit pandas
```

---

## Platform-Specific Notes

### Windows
```bash
pip install streamlit pandas
```

### Mac
```bash
pip3 install streamlit pandas
```

### Linux
```bash
pip3 install streamlit pandas
```
Or:
```bash
sudo apt-get install python3-pip
pip3 install streamlit pandas
```

---

## File Structure for Deployment

```
your-project/
├── streamlit_app.py          # Main app (required)
├── requirements.txt           # Dependencies (required)
├── dva_logo.png              # Logo (optional)
├── .streamlit/
│   └── config.toml           # Theme (optional)
└── README.md                 # Documentation (optional)
```

---

## Summary

**Only 2 dependencies needed:**
1. `streamlit>=1.28.0`
2. `pandas>=2.0.0`

**Installation:**
```bash
pip install streamlit pandas
```

**Verification:**
```bash
python diagnostic_test.py
```

**Run App:**
```bash
streamlit run streamlit_app.py
```

That's all you need! 🚀

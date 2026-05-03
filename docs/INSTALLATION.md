# 📦 Installation Guide

Complete guide to install and set up the **tele-latino** repository on your local machine.

## Prerequisites

Before you begin, make sure you have:
- 🖥️ **A computer** (Windows, Mac, or Linux)
- 🌐 **A web browser** (Chrome, Firefox, Safari, Edge)
- 💻 **Git** (optional, for cloning) - [Download Git](https://git-scm.com/)
- 📝 **A text editor** (VS Code, Sublime, Notepad++) - [Download VS Code](https://code.visualstudio.com/)

---

## ⚡ Quick Start (3 Steps)

### Step 1: Get the Repository

**Option A: Download as ZIP**
1. Go to https://github.com/abdulrazaqmehrwood2020-creator/tele-latino
2. Click **"Code"** (green button)
3. Click **"Download ZIP"**
4. Extract the ZIP file to your desired location

**Option B: Clone with Git**
```bash
git clone https://github.com/abdulrazaqmehrwood2020-creator/tele-latino.git
cd tele-latino
```

### Step 2: Open in Browser

1. Navigate to the extracted folder
2. Find **`calculator.html`**
3. Right-click → **"Open with"** → Select your browser
4. ✅ Calculator is now running!

### Step 3: Done! 🎉

You can now use all the tools. No additional setup needed!

---

## 🚀 For Developers (Advanced Setup)

### Using VS Code Live Server

1. **Install VS Code** from https://code.visualstudio.com/

2. **Install Live Server Extension**
   - Open VS Code
   - Go to Extensions (Ctrl+Shift+X / Cmd+Shift+X)
   - Search for "Live Server"
   - Click **Install** (by Ritwick Dey)

3. **Open the Project**
   ```bash
   # Navigate to the folder
   cd path/to/tele-latino
   # Open in VS Code
   code .
   ```

4. **Start Live Server**
   - Right-click on `calculator.html`
   - Select **"Open with Live Server"**
   - Browser automatically opens at `http://localhost:5500`

5. **Auto-reload on Changes**
   - Any file changes auto-refresh in browser
   - Perfect for development!

---

### Using Python HTTP Server

If you have Python installed:

```bash
# Navigate to project folder
cd path/to/tele-latino

# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Then open: `http://localhost:8000`

---

### Using Node.js HTTP Server

If you have Node.js installed:

```bash
# Install http-server globally
npm install -g http-server

# Navigate to project folder
cd path/to/tele-latino

# Start server
http-server

# Opens at: http://localhost:8080
```

---

## 📁 Project Structure After Installation

```
tele-latino/
├── README.md                 # Main documentation
├── LICENSE                   # MIT License
├── CONTRIBUTING.md           # How to contribute
├── INSTALLATION.md           # This file
├── calculator.html           # Calculator tool
├── docs/                     # Documentation folder
│   ├── INSTALLATION.md       # Installation guide
│   ├── USAGE.md             # Usage examples
│   └── SCREENSHOTS.md       # Screenshots & GIFs
├── tools/                    # Tools folder
│   ├── README.md            # Tools documentation
│   └── calculator.html      # Calculator (copy)
└── assets/                   # Optional: Images, styles
    └── images/              # Screenshots, logos
```

---

## ✅ Verification

### Test Calculator Locally

1. Open `calculator.html` in your browser
2. Try these operations:
   - **5 + 3 =** Should show **8**
   - **10 - 4 =** Should show **6**
   - **7 × 3 =** Should show **21**
   - **20 ÷ 4 =** Should show **5**

3. Test keyboard shortcuts:
   - Type **5** + **3** + **Enter** = **8** ✅
   - Press **Escape** to clear ✅

If everything works, you're all set! 🎉

---

## 🐛 Troubleshooting

### Calculator won't open
- ✅ Make sure you have the correct file path
- ✅ Try a different browser
- ✅ Check if JavaScript is enabled in your browser

### Files not found error
- ✅ Make sure all files are in the same folder
- ✅ Check file names match exactly (case-sensitive on Mac/Linux)

### Live Server not working
- ✅ Reinstall Live Server extension
- ✅ Try closing and reopening VS Code
- ✅ Use Python server instead (more reliable)

### Port already in use
If port 8000/5500 is busy:
```bash
# Python - use different port
python -m http.server 9000

# Node - automatically finds available port
http-server
```

---

## 📚 Next Steps

After installation:

1. ✅ **Open calculator.html** - Try the calculator
2. ✅ **Read USAGE.md** - Learn all features
3. ✅ **Explore the code** - See how it works
4. ✅ **Customize it** - Make it your own!
5. ✅ **Share it** - Tell others about your project

---

## 🔗 Useful Links

- **Repository:** https://github.com/abdulrazaqmehrwood2020-creator/tele-latino
- **Live Website:** https://gettelelatino.com/
- **Git Guide:** https://git-scm.com/doc
- **VS Code:** https://code.visualstudio.com/
- **Live Server:** https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer

---

## 💬 Need Help?

- 📖 Check the [README.md](../README.md)
- 📝 See [USAGE.md](./USAGE.md) for examples
- 🐛 Open an issue on GitHub
- 💌 Contact via email

---

Made with ❤️ by [Abdulrazaq Mehrwood](https://gettelelatino.com/)

*Last updated: 2026*

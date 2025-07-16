# Create a Virtual Environment (Python 3.12) 💻✨<br>Windows, macOS or Linux

## 1️⃣: Open a Command Prompt or PowerShell window and run:

`py -3.12 -m venv venv`

🔹 Sets up the environment using Python 3.12 (must be installed).<br>
🔹 Replace 3.12 with the version you need, if different.

---

## 2️⃣: Activate the virtual environment

🟦 Windows (CMD): `venv\Scripts\activate`<br>
🟪 Windows (PowerShell): `venv\Scripts\Activate.ps1`<br>
🟩 macOS/Linux: source `venv/bin/activate`

---

## 3️⃣: Install the Requirements

`pip install -r requirements.txt`

📦 (If your requirements.txt is in a subdirectory, like scripts/, use:)

`pip install -r scripts/requirements.txt`

---

## 4️⃣: Deactivate the Virtual Environment
At any time, leave the environment with:

`deactivate`

🚪 (Exit anytime!)

---

## 5️⃣: Troubleshooting 🧠🛠️
⚠️ See a bin folder instead of Scripts on Windows?
You may have used WSL or Git Bash. Delete your venv and recreate with the Python launcher:

`py -3.12 -m venv venv`

### 🔎 Confirm Python is from the correct install:

`python -c "import sys; print(sys.executable)"`

(Ensure it points to your main system Python, not one bundled by apps!)

### 🚨 Activation scripts missing?
Repeat the creation steps in a regular Command Prompt or PowerShell window (not Git Bash or WSL).

### 🌟 Tip: If you're not sure which Python versions are available, run:

`py -0V`

***(Pick the latest version listed!)***

---

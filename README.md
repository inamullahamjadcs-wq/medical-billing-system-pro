# 🏥 DAWN MEDICAL STORE — Complete Setup Guide

## What You Are Installing
A full medical store billing software with:
- Fast invoice/challan billing with keyboard shortcuts
- Voice medicine search with smart phonetic matching
- Customer-specific price memory
- Wholesale payment tracking (Unpaid/Partial/Paid/Overdue)
- Customer ledger with aging report
- Inventory management with expiry alerts
- Purchase & supplier management
- Reports (Daily, Monthly, Stock, Outstanding)
- A4 invoice printing

---

## STEP 1 — Install Required Software

### 1a. Install Python (3.10 or higher)
- Go to: https://www.python.org/downloads/
- Download Python 3.11 (recommended)
- ✅ IMPORTANT: Check "Add Python to PATH" during installation
- Click Install Now

**Verify:**
```
python --version
```
Should show: Python 3.11.x

---

### 1b. Install Node.js (18 or higher)
- Go to: https://nodejs.org/
- Download LTS version (18 or 20)
- Install with default settings

**Verify:**
```
node --version
npm --version
```

---

### 1c. Install Git (optional but recommended)
- Go to: https://git-scm.com/downloads
- Install with default settings

---

## STEP 2 — Setup the Project

### Open Command Prompt (Windows) or Terminal (Mac/Linux)

#### On Windows:
Press `Win + R` → type `cmd` → press Enter

#### On Mac:
Press `Cmd + Space` → type `terminal` → press Enter

---

## STEP 3 — Setup Backend (Python API)




## STEP 4 — Setup Frontend (React UI)



## STEP 5 — Open the Software

Open your browser 

🎉 **Dawn Medical Store is now running!**

---

## STEP 6 — First Time Setup

1. Go to **Settings** (⚙️ in sidebar)
2. Enter your store name, address, phone, license number
3. Set your invoice prefix (default: DMS)
4. Click **Save Settings**

---

## STEP 7 — Add Your Medicines

1. Go to **Medicines** (💊 in sidebar)
2. Click **+ Add Medicine**
3. Fill in: Name, Generic Name, Company, Category, Strength, Price, Stock, Min Stock, Batch, Expiry
4. Save

**Tip:** Add at least 10-20 medicines before testing billing

---

## STEP 8 — Add Your Customers

1. Go to **Customers** (👤 in sidebar)
2. Click **+ Add Customer**
3. Fill in: Name, Phone, Address, Credit Limit, Credit Days
4. Save



## KEYBOARD SHORTCUTS (Billing Screen)

| Key | Action |
|-----|--------|
| F1 | New Invoice (works from anywhere) |
| F2 | Focus medicine search |
| F4 | Save invoice |
| F5 | Save & Print |
| F8 | Focus discount field |
| ↑ ↓ | Navigate dropdowns |
| Enter | Select from dropdown |
| Tab | Next field |
| Escape | Close dropdown / cancel |

---

## VOICE SEARCH — How to Use

1. Click the 🎤 button next to medicine search
2. Speak the medicine name clearly in English
3. System will find closest match automatically

**If voice gets medicine name wrong:**
- Go to Medicines → click "Voice Aliases"
- Add: What voice hears → Correct name
- Example: "sumu gel" → "Somagel"

**Strength recognition:**
- Say "panadol 500" → finds Panadol 500mg
- Say "brufen 400" → finds Brufen 400mg

---

## BILLING WORKFLOW

1. Press **F1** → New Invoice
2. Select customer from dropdown (or leave blank for walk-in)
   - Customer details auto-fill
   - Outstanding balance shows instantly
3. Fill PO Number, Due Date if needed
4. Press **F2** → Type medicine name (2+ letters for dropdown)
   - OR click 🎤 and speak medicine name
   - Arrow keys to navigate dropdown
   - Enter to select
   - Price auto-fills (customer-specific if available)
   - Change Qty with arrow keys or type
5. Repeat for all medicines
6. Set payment method and amount
7. Press **F5** → Save & Print

---

## UPGRADING TO POSTGRESQL (When Ready)


## BACKUP YOUR DATA

### ✅ Automatic Backup (Built-In!)


**No action needed — backup happens on every startup!**

### 📁 Backup Location
```
dawn-medical/
└── backups/
    ├── backup_2026-05-05_09-00.db
    ├── backup_2026-05-05_14-30.db
    └── backup_2026-05-06_10-15.db
```

### 🔒 Weekly Manual Backup (Recommended)
Copy entire `backups/` folder to USB drive, Google Drive or OneDrive.

### ⚠️ Recovery
If something goes wrong: copy latest backup file
## TROUBLESHOOTING


### Voice not working
- Use Chrome or Edge browser (Firefox has limited support)
- Allow microphone permission when browser asks
- Speak clearly in English

### Medicine search slow
- Normal on first search (database warming up)
- Gets faster after first few searches

---

## FOLDER STRUCTURE

```
dawn-medical/
├── frontend/          → React UI (what you see)
│   ├── src/
│   │   ├── pages/     → All screens
│   │   ├── components → Reusable parts
│   │   ├── utils/     → API calls, formatting
│   │   └── hooks/     → Voice, keyboard shortcuts
│   └── package.json
│
├── backend/           → Python API (data & logic)
│   ├── app/
│   │   ├── main.py    → App entry point
│   │   ├── database.py → DB connection
│   │   ├── models/    → Database tables
│   │   └── routes/    → All API endpoints
│   ├── .env           → Your config (DB URL etc)
│   └── requirements.txt
│
└── README.md          → This file
```

---

## SUPPORT

If something is not working:
1. Check that both backend AND frontend terminals are running
2. Check for error messages in the terminal
3. Make sure you are on Chrome or Edge browser
4. Restart both terminals and try again

---

**Built for Dawn Medical Store — Islamabad** 🏥

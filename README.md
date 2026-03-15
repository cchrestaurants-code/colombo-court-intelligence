# Colombo Court Hotel & Spa — Social Intelligence Hub v4
## Free Edition — Complete Setup Guide

---

## Cost: Completely Free

| Component | Cost |
|-----------|------|
| GitHub Pages (app hosting) | ✅ Free |
| Google Sheets (data storage) | ✅ Free |
| Claude.ai (AI analysis) | ✅ Already have it |
| **Total** | **$0.00 / month** |

---

## How It Works

This is a **manual-input + AI-assisted** intelligence system:

```
You observe → You enter data → Click "Copy for Claude.ai"
       ↓
Paste into Claude.ai chat → Get AI analysis
       ↓
Paste response back into app → Saved forever in Google Sheets
```

No automatic scanning = No API costs. You control when analysis runs.

---

## Files in This Package

```
colombo-court-v4/
├── index.html     ← The complete dashboard app
└── README.md      ← This setup guide
```

That's it — just 2 files. No complex folder structure needed.

---

## STEP 1 — Host on GitHub Pages (10 minutes)

### 1a. Create Repository

1. Go to [github.com](https://github.com) and sign in
2. Click **+** (top right) → **New repository**
3. Name: `colombo-court-intelligence`
4. Set to **Public**
5. Click **Create repository**

### 1b. Upload Files

1. Click **Add file** → **Upload files**
2. Upload `index.html` and `README.md`
3. Click **Commit changes**

### 1c. Enable GitHub Pages

1. Click **Settings** → **Pages** (left sidebar)
2. Source: **Deploy from a branch**
3. Branch: **main** · Folder: **/ (root)**
4. Click **Save**
5. Wait 3 minutes — your app is live at:
   ```
   https://YOUR-USERNAME.github.io/colombo-court-intelligence/
   ```

Bookmark this URL. This is your permanent app address.

---

## STEP 2 — Connect Google Sheets (15 minutes)

This stores all your data permanently online so nothing is lost if your browser clears.

### 2a. Create the Google Sheet

1. Go to [sheets.google.com](https://sheets.google.com)
2. Click **+ Blank**
3. Name it: **Colombo Court Intelligence Data**
4. Create 4 tabs by clicking **+** at the bottom:
   - `Daily_Scans`
   - `Competitor_Scans`
   - `Saved_Insights`
   - `Competitor_Watchlist`

### 2b. Add Column Headers

**Daily_Scans tab** (row 1):
```
Date | Time | Sentiment Score | Mentions | Positive% | Negative% | Trend Notes
```

**Competitor_Scans tab** (row 1):
```
Date | Time | Competitor | Sentiment Score | Mentions | Activity | Notes
```

**Saved_Insights tab** (row 1):
```
Date | Title | Preview
```

**Competitor_Watchlist tab** (row 1):
```
Name | Type | Threat Level
```

### 2c. Get Your Sheet ID

Your Sheet URL looks like:
```
https://docs.google.com/spreadsheets/d/XXXXXXXXXXXXXXXXXXXXXXXX/edit
```
Copy the part between `/d/` and `/edit` — that's your **Sheet ID**.

### 2d. Get a Google API Key

1. Go to [console.cloud.google.com](https://console.cloud.google.com)
2. Click **Select a project** → **New Project** → Name: "Colombo Court"
3. Click **Create**
4. Search **Google Sheets API** → Click → **Enable**
5. Click **APIs & Services** → **Credentials** → **+ Create Credentials** → **API Key**
6. Copy the key shown
7. Click the pencil (Edit) → **Restrict key** → Select **Google Sheets API** → Save

### 2e. Enter Credentials in App

1. Open your app
2. Click **Settings** in the navigation
3. Enter your **Sheet ID** and **API Key**
4. Click **Save & Test** — should show green confirmation
5. Click **Test Connection** to verify

From now on, every check-in automatically writes to your Google Sheet. You have a permanent backup.

---

## STEP 3 — Enable Morning Reminder

1. In the app, go to **Settings**
2. Click **Enable 8am Reminder**
3. Allow browser notifications when prompted
4. Every morning at 8:00 AM you'll get a notification reminding you to do your check-in

> **Note:** This works when the browser tab is open or the app is bookmarked as a PWA. For a guaranteed reminder even when the browser is closed, set a calendar alarm on your phone for 8:00 AM.

---

## Daily Workflow (10–15 minutes)

```
8:00 AM — Notification fires (or your phone reminder)
     ↓
Spend 5 minutes checking:
  • New Google/TripAdvisor reviews
  • Competitor social activity you noticed
  • Anything trending in Colombo
     ↓
Open app → Click "Daily Check-in" tab
     ↓
Fill in the form (sentiment score, what you saw)
     ↓
Click "Copy for Claude.ai" → Paste in this chat
     ↓
Get AI analysis back → Copy & paste into app
     ↓
Click "Save Check-in" — data saved to Google Sheets
     ↓
Done! Dashboard updates automatically.
```

---

## Weekly & Monthly Rhythm

**Weekly (Friday, 20 minutes):**
- Go to Competitors tab → Enter this week's competitor observations
- Click "Copy All for Claude.ai" → Get competitive intelligence
- Save the analysis

**Monthly (Last day of month, 30 minutes):**
- Go to Reports tab → Select Monthly Report
- Click "Copy Monthly Data for Claude.ai"
- Paste into Claude.ai → Get full monthly report
- Paste report back → Save + Export as HTML for management

---

## Backing Up Your Data

**Automatic:** Every check-in writes to Google Sheets automatically.

**Manual backup anytime:**
- Dashboard → **Download All Data (Excel)** — exports everything as .xlsx

**View your data directly:**
- Open your Google Sheet anytime — all rows are there
- Share with your GM or owner if needed

---

## Troubleshooting

**App not loading / blank screen:**
- Wait 5 minutes after enabling GitHub Pages
- Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)

**Google Sheets test connection fails:**
- Check the Sheet ID has no spaces
- Verify the API key is correct and Sheets API is enabled
- Make sure tab names match exactly (case-sensitive)

**Data only in browser, not in Sheets:**
- Check Settings → Sheet ID and API Key are entered and saved
- Data in localStorage will still persist until browser cache is cleared

**Notifications not working:**
- Check browser notification permissions (site settings)
- Set a phone alarm as backup for 8:00 AM

---

## Tips for Getting the Best AI Analysis

When pasting your check-in data into Claude.ai:

1. **Be specific** — "3 negative reviews about slow pool service" is better than "some bad reviews"
2. **Include competitor detail** — "Cinnamon Red ran a 'buy 1 get 1 cocktail' on Instagram Thursday" gives Claude real data to work with
3. **Note trends you see** — Even hashtags you noticed on Instagram or topics people are discussing
4. **Ask follow-up questions** — After getting the analysis, ask specific questions like "What content should I post today about Cloud Café?" or "How should we respond to the negative poolside reviews?"

---

*Colombo Court Hotel & Spa — Social Intelligence Hub v4 (Free Edition)*
*Built March 2026*

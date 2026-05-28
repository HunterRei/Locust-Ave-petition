# Locust Avenue Petition
**Traffic Safety & Historic Road Preservation**

A community petition form for Locust Avenue residents. Signers can fill out their details and draw a signature directly in the browser. Submissions are recorded in a Google Sheet with signature images saved to Google Drive.

---

## Live Form

Hosted via GitHub Pages at:
`https://yourusername.github.io/your-repo-name`

---

## How It Works

1. Visitor fills out the form (name required, address and comments optional)
2. Visitor draws their signature in the signature pad
3. On submit, the form sends data to a Google Apps Script Web App
4. The script appends a row to the Google Sheet and saves the signature image to Google Drive

---

## Setup

### 1. Google Apps Script
- Open the linked Google Sheet and go to **Extensions → Apps Script**
- Paste the script from the README comment at the bottom of `index.html`
- Deploy as a **Web App** (Execute as: Me, Access: Anyone)
- Copy the Web App URL

### 2. HTML File
- Open `index.html` and find this line near the top of the script section:
```js
const APPS_SCRIPT_URL = "YOUR_APPS_SCRIPT_URL_HERE";
```
- Replace the placeholder with your copied Web App URL

### 3. GitHub Pages
- Go to repo **Settings → Pages**
- Source: Deploy from a branch → `main` → `/ (root)` → Save
- The form will be live within a minute or two

---

## Files

| File | Description |
|---|---|
| `index.html` | The petition form — all HTML, CSS, and JS in one file |
| `README.md` | This file |

---

## Data Collected

Each submission records the following in the Google Sheet:

- Timestamp
- Full name
- Address (optional)
- Comments (optional)
- Link to signature image (saved in Google Drive)

---

## Contact

For questions about this petition contact the organizer directly.

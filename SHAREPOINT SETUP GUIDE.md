# LP Knowledge Hub — SharePoint Setup Guide

## What you're deploying

```
IOR SOP v2.0/
├── index.html              ← Hub home page (start here)
├── Warehouse SOP.html      ← Warehouse SOP viewer
├── CW_RECEIVES_1.png
├── CW_RECEIVES_2.png
├── CW_RECEIVES_3.png
├── CW_RECEIVES_4.png
├── CW_RECEIVES_5.png
├── CW_RECEIVES_6.png
├── CW_ORDERS_1.png
├── CW_ORDERS_2.png
├── CW_ORDERS_3.png
├── CW_ORDERS_4.png
├── CW_ORDERS_5.png
└── CW_HOME_PAGE.png
```

All files **must stay in the same folder** — the HTML files reference screenshots by relative path.

---

## Step 1 — Create a SharePoint Site

1. Go to [sharepoint.com](https://sharepoint.com) and sign in with your Logistics Plus account.
2. Click **+ Create site** (top-left).
3. Choose **Communication site**.
4. Name it something like `LP Knowledge Hub` or `LP SOPs`.
5. Set privacy to **Only people in your organization can find and access this site** (or more restrictive if needed).
6. Click **Finish**.

---

## Step 2 — Create a Document Library for the SOP Files

1. From your new site, click **+ New → Document library**.
2. Name it `SOPs` (no spaces — this keeps URLs clean).
3. Click **Create**.

---

## Step 3 — Upload All Files

1. Open the `SOPs` library.
2. Click **Upload → Folder** and select your entire `IOR SOP v2.0` folder.
   - *Or* click **Upload → Files**, select all files at once (Ctrl+A), and upload them all into the root of the `SOPs` library.
3. Verify every file appears: `index.html`, `Warehouse SOP.html`, and all `.png` files.

---

## Step 4 — Get the Direct Link to `index.html`

1. In the `SOPs` library, hover over `index.html`.
2. Click the **⋯ (three dots)** menu → **Copy link**.
3. In the link panel, change the permission to **People in [your org] with the link** (so only LP staff can open it).
4. Click **Copy** — this is your hub URL.

> **Tip:** Paste it in a browser first to confirm it opens and the Warehouse SOP link works.

---

## Step 5 — Share the Link with Staff

**Option A — Teams message or email**
Paste the link directly. Staff click it and the hub opens in their browser.

**Option B — Pin to a Teams channel tab**
1. In the Teams channel, click **+** (Add a tab).
2. Choose **Website**.
3. Paste the `index.html` URL and name it `LP SOPs` or `Knowledge Hub`.
4. Now the hub is always visible as a tab.

**Option C — SharePoint intranet page**
Add an **Embed** web part to any SharePoint page and paste the `index.html` URL — the hub renders inline on the page.

---

## Step 6 — Adding New SOPs Later

When you build a new SOP (e.g., `Freight SOP.html`):

1. Upload `Freight SOP.html` and its screenshots to the same `SOPs` library folder.
2. In `index.html`, change a "Planned" card to "Live":
   - Update `<div class="sop-card placeholder"` → `<a class="sop-card" href="Freight SOP.html"`
   - Change `badge-planned` → `badge-live`
   - Update the description and tags
3. Re-upload `index.html` to replace the old version.

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Screenshots don't load | Make sure all `.png` files are in the **same folder** as the HTML files |
| "You need permission to access this" | Check the share link is set to your org, not "specific people" |
| HTML file downloads instead of opening | Click the file name directly (not the checkbox) — or use a direct link from Teams/email |
| Animations don't run | The site needs to be opened in a modern browser (Edge, Chrome) — not Internet Explorer |

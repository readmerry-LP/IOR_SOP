# LP Knowledge Hub — Standard Operating Procedures

Interactive, step-by-step CargoWise SOP guides for Logistics Plus internal use. Built as a self-contained static website — no server, no framework, no dependencies to install.

## Live Site

<https://readmerry-lp.github.io/IOR_SOP/>

## What's Included

| File | Description |
|---|---|
| `index.html` | Hub home page — lists all SOPs by category |
| `Warehouse SOP.html` | Interactive walkthrough: Create a Receipt + Create an Order, with annotations and cursor/click animations |
| `CW_RECEIVES_*.png` | CargoWise screenshots for the inbound receipt workflow |
| `CW_ORDERS_*.png` | CargoWise screenshots for the outbound order workflow |
| `CW_MILESTONES_*.png` | CargoWise screenshots for ETA and delivery milestone entry |
| `CW_HOME_PAGE.png` | CargoWise home screen reference |
| `SCREENSHOT SHOT LIST.md` | Working shot list — filenames and capture/annotation notes for each screenshot |
| `SHAREPOINT SETUP GUIDE.md` | Instructions for deploying the hub to SharePoint |

## Viewing Locally

1. Clone or download this repository
2. Open the `IOR SOP v2.0` folder in File Explorer
3. Drag `index.html` onto an open Chrome or Edge window

No build step, no `npm install` — it opens directly in the browser.

## Deploying to GitHub Pages

1. Push all files to a GitHub repository
2. Go to **Settings → Pages → Source → Deploy from a branch**
3. Select **main** branch, **/ (root)** folder → click **Save**
4. Your site will be live at `https://<username>.github.io/<repo-name>`

> **Important:** All `.png` screenshot files must be in the same folder as the HTML files or images will not load.

## File Structure

```
IOR SOP v2.0/
├── index.html                       ← Hub home page
├── Warehouse SOP.html               ← Warehouse SOP viewer
├── README.md                        ← This file
├── SCREENSHOT SHOT LIST.md          ← Screenshot capture + annotation notes
├── SHAREPOINT SETUP GUIDE.md        ← SharePoint deployment instructions
│
├── CW_HOME_PAGE.png                 ← CargoWise home screen
│
│   Inbound / Receipt
├── CW_RECEIVES_1.png                ← Navigate to Receive screen
├── CW_RECEIVES_2.png                ← Create new receipt
├── CW_RECEIVES_3.png                ← New receipt form
├── CW_RECEIVES_4.png                ← (reference)
├── CW_RECEIVES_5.png                ← Add line items
├── CW_RECEIVES_6.png                ← Save & Close
├── CW_RECEIVES_SPLIT_1.png          ← Split receipt by quantity
├── CW_RECEIVES_SPLIT_2.png          ← Related Splits tab (parent row)
├── CW_RECEIVES_SERIALS_1.png        ← Import serials via right-click menu
├── CW_RECEIVES_SERIALS_2.png        ← Data Import Wizard mapping
├── CW_RECEIVES_FINALIZE.png         ← Finalize receipt checklist
│
│   Outbound / Order
├── CW_ORDERS_1.png                  ← Navigate to Orders screen
├── CW_ORDERS_2.png                  ← Create new order
├── CW_ORDERS_3.png                  ← New order form
├── CW_ORDERS_4.png                  ← Add line items
├── CW_ORDERS_5.png                  ← Submit order
├── CW_ORDERS_PICK.png               ← Pick button
├── CW_ORDERS_PICKSLIP_1.png         ← Documents → Picking Slip
├── CW_ORDERS_PICKSLIP_1a.png        ← Deliver Documents → Preview
├── CW_ORDERS_PICKSLIP_2.png         ← Printed picking slip + QC notes
├── CW_ORDERS_ARCHIVE.png            ← Save pick slip as WPS eDoc
├── CW_ORDERS_LABELS_1.png           ← Documents → Delivery Labels
├── CW_ORDERS_LABELS_2.png           ← Printed box label
├── CW_ORDERS_PACKSLIP_1.png         ← Documents → Packing Slip
├── CW_ORDERS_PACKSLIP_2.png         ← Printed LP packing slip
├── CW_ORDERS_PACKSLIP_3.png         ← Packing list per pallet (Excel)
├── CW_ORDERS_RELEASE.png            ← Release button
├── CW_ORDERS_VOLUME.png             ← Packages / pallets sent
├── CW_ORDERS_SERIALS_1.png          ← Import serials at release
├── CW_ORDERS_SERIALS_2.png          ← Serial mapping at release
├── CW_ORDERS_EDOCS.png              ← Upload order documents (POD, BOL, etc.)
│
│   Milestones
├── CW_MILESTONES_ETA.png            ← Populate Estimated Date (ETA)
└── CW_MILESTONES_DELIVERY.png       ← Enter Actual Delivery Date
```

## Adding a New SOP

**Step 1 — Build the SOP file**

Copy the structure of `Warehouse SOP.html` as a starting point. Each SOP is a single self-contained HTML file with its screenshots referenced by relative path.

**Step 2 — Add it to the hub**

In `index.html`, find the relevant category section and convert a placeholder card to a live card:

```html
<!-- Before (placeholder) -->
<div class="sop-card placeholder" data-tags="...">
  ...
  <span class="card-badge badge-planned">Planned</span>
  ...
</div>

<!-- After (live) -->
<a class="sop-card" href="Your SOP.html" data-tags="...">
  ...
  <span class="card-badge badge-live">Live</span>
  ...
</a>
```

**Step 3 — Upload**

Add the new SOP HTML file and its screenshots to the repository. Re-deploy.

## Tech Stack

Plain HTML, CSS, and JavaScript — no frameworks, no build tools.

- **Fonts:** PT Sans Narrow + Inter (Google Fonts)
- **Animations:** Vanilla JS cursor/click animations, authored at 680×378 base coordinates and scaled dynamically to the rendered viewport size
- **Screenshots:** PNG exports from CargoWise (~1382×769)
- **Branding:** Logistics Plus navy `#06236D`, blue `#0565D7`, gold `#C9A84C`

## Version History

| Version | Date | Notes |
|---|---|---|
| v2.0 | Jul 2026 | Full Warehouse SOP: receipt splits, serial imports, finalize checklist, pick/pack slips, WPS archiving, delivery labels, release + volume capture, order serials, eDocs upload, and ETA/delivery milestones. Added on-screen annotations and cursor/click animations. |
| v1.0 | Jun 2026 | Warehouse SOP complete — receipts and orders, 5 steps each |

## Contact

Questions or corrections: [read.merry@logisticsplus.com](mailto:read.merry@logisticsplus.com)

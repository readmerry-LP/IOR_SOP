# CargoWise Screenshot Shot List — Warehouse SOP v2.0

Save each screenshot as a PNG with the **exact filename** below, directly in this folder.
The website auto-swaps the placeholder for the image as soon as the file exists — no code changes needed.

## Inbound / Receipt (5 shots)

| Filename | What to capture in CW |
|---|---|
| `CW_RECEIVES_SPLIT_1.png` | Open receipt → **Actions menu open** with "Split Receipt by Quantity" highlighted. Show a qty typed in the **Split Quantity** column + the **Save** button (bottom-right). |
	## Need to animate mouse cursor to click from 1) The split quantity on the line level, 2) Clicking the 'Save' button, 3) Clicking the 'Actions' menu and then 'Spit Receipt by Quantity'
| `CW_RECEIVES_SPLIT_2.png` | Receipt → **Related Splits tab** showing the **PARENT** row (the row you click to jump to the split). |
	## Need to annotate/highlight the tab "Related Splits" and an arrow pointing to the "Split #" line input with a notation "Click here to go to split" (similarly to the original PDF, but in the new SOP site's styling)
| `CW_RECEIVES_SERIALS_1.png` | Receipt lines grid → **right-click context menu** open with **Import Data…** highlighted. |
	## Need to annotate "1. Save Excel file as a CSV" and "2. Import Data in CW"
| `CW_RECEIVES_SERIALS_2.png` | **Data Import Wizard → Mapping tab**: CSV field on the left, CW columns on the right, arrow showing the drag. |
	## Need to annotate "Drag the column name into its corresponding mapping field"
| `CW_RECEIVES_FINALIZE.png` | Receipt ready to finalize: boxes on **Transport/Supplier, Transport Ref., Arrival Date, Total Units/Pallets/Packages, Total Line Weight & Volume** + "Upload ALL paperwork" note. |
	## Need to annotate "Upload ALL Paperwork" note.

## Outbound / Order (14 shots)

| Filename | What to capture in CW |
|---|---|
| `CW_ORDERS_PICK.png` | Saved order, box around the **Pick** button (bottom-right). |
| `CW_ORDERS_PICKSLIP_1.png` | **Edit Pick** screen → **Documents menu open**, "Picking Slip" highlighted. |
	## I need to add a step in between here. When you go to the menu "Documents", then click "Picking Slip", the "Deliver Documents" box pops up. I'm making a screenshot of what to select and naming it `CW_ORDERS_PICKSLIP_1a.png`. You need to click "Preview"
| `CW_ORDERS_PICKSLIP_2.png` | The printed **Picking Slip** doc: callouts on Picked Qty column + Page/Running Totals with PICKED BY / CHECKED BY lines. |
	## We will need to add notation about the steps. Step 1) Mark if any SKU needs to be Asset tagged of if Serial Numbers need to be captured, 2) Pick Items and Enter Qty Picked, 3) A different staff member will QC all products on pick and sign with initials. This annotation needs to be in the same styling as all the others.
| `CW_ORDERS_ARCHIVE.png` | Order with eDocs **Edit document dialog** open: Document Type = **WPS**. Callouts: "Drag document anywhere here" / "Save under WPS". |
	## Add a notation saying something like "Open the location of the Pick Slip. Then click and drag it anywhere into the open Orders window in CW. You must save is as 'Document Type = WPS".
| `CW_ORDERS_LABELS_1.png` | **Documents → Delivery Labels** + Labels Printing dialog, box on **Number of Labels to Print**. |
| `CW_ORDERS_LABELS_2.png` | A printed **Warehouse Order box label** ("1 of 6", consignee, destination, reference). Callout: "Label all boxes". |
| `CW_ORDERS_PACKSLIP_1.png` | Order → **Documents menu open**, "Packing Slip" highlighted. |
| `CW_ORDERS_PACKSLIP_2.png` | The printed **LP Packing Slip** with Qty Ordered/Sent lines and Packed By / Checked By section. Callout: "Include on all packages". |
| `CW_ORDERS_PACKSLIP_3.png` | **Deliver Documents dialog**, box on the **Type** dropdown. Callout: "Download as an Excel sheet to edit" (one packing list per pallet). |
	## Add a notation saying "In case of more than one pallet, there should be a packing list per pallet."
| `CW_ORDERS_RELEASE.png` | Order in PICKING status, box + arrow on the **Release** button (bottom-right). |
	## Add the mouse cursor moving over to the bottom right release button and "clicking" on the 'Release' button.
| `CW_ORDERS_VOLUME.png` | **Edit Release** screen, box around **Packages Sent** and **Pallets Sent** fields. |
	## Add a notation saying "Capture the number of packages and pallets sent."
| `CW_ORDERS_SERIALS_1.png` | Edit Release: **Sage Serial Numbers field** in the Breakdown grid, right-click **Import Data**, and the wizard browsing the serials **CSV** (3 callouts). |
	## Add a notation saying "Within the Release screen, 1) Click on the "Order Lines" tab. Then, 2) right-click on the "Serial Number" header and 3) click "Import Data". Find and select the CSV file you've created with all the serial numbers."
| `CW_ORDERS_SERIALS_2.png` | Import Wizard **Mapping tab** at release: drag CSV field → **Sage Serial Numbers** (also shows Quantity Met, Asset Tag, Project Name). |
	## Add a notation saying "Click and drag the CSV Field (Serial Number) to its corresponding field in the Import Wizard".
| `CW_ORDERS_EDOCS.png` | Order → **eDocs tab → Document Storage** grid, box on the doc list area. Callout: "BOL / Labels / Receipts + POD". |
	## Add a notation saying "Upload all order-related documents: POD, LABEL, BOL, Commercial Invoice, Receipt, etc."

## Milestones (2 shots)

| Filename | What to capture in CW |
|---|---|
| `CW_MILESTONES_ETA.png` | Order → **Workflow & Tracking → Milestones**: Shipped/Delivered rows, box + arrow on the empty **Estimated Date** cell, "ETA" callout. |
	## Add a notation saying the "ETA must be populated when or before an order is Finalized."
| `CW_MILESTONES_DELIVERY.png` | Same screen: boxes on the **Workflow & Tracking tab** + **Milestones sub-tab**, and on the populated **Actual Start** date. Callout: "Actual Delivery Date". |
	## Add a notation saying the "Actual delivery date must be entered once delivery is confirmed."

**Tip:** capture at the same window size as the existing shots (~1382×769) so the animations and layout stay consistent.

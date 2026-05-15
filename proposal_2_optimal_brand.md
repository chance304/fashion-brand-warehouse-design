# Proposal 2: Optimal Warehouse for an Upcoming Brand
**For:** Upcoming Fashion Brand — Warehouse Design  
**Model:** Investment-Backed, Operationally Sound, Cashflow-Conscious  
**Prepared:** 2026-05-16  

---

## Executive Summary

This proposal is the **recommended path** for a brand in the growth phase — one that has raised or is in the process of raising seed/pre-Series A investment, has constrained monthly cashflow, but cannot afford operational failures that will damage customer experience or brand reputation. It avoids overengineering while establishing a professional foundation that can scale cleanly to 3× without throwaway work.

The model uses cloud-based barcode WMS (not RFID — that cost is deferred), industrial GOH racking, and a disciplined SOP structure. It costs approximately **$18,000–$35,000 USD (₹15–₹29 lakhs)** to set up and runs at **$1,500–$2,800/month** in operational costs (excluding payroll), which is manageable even at seed stage.

The infrastructure laid here becomes the foundation for Proposal 1 — if the brand grows rapidly, they don't rebuild; they upgrade individual components (add RFID readers, swap WMS tier, add mezzanine). Nothing in this proposal is a dead end.

**Best for:** Brands in the ₹30–₹150 lakh annual revenue range, with seed funding or active fundraising, targeting 2–3× growth over 24 months, and where the founder/COO will be closely involved in warehouse operations initially.

---

## 1. Warehouse Layout & Zone Design

### 1.1 Floorplan Overview (2,500 sq ft / ~230 sq m)

```
┌──────────────────────────────────────────────────────────────────────────┐
│  RECEIVING + QC ZONE                    │  RETURNS PROCESSING            │
│  (280 sq ft)                            │  (120 sq ft)                   │
├─────────────────────────────────────────┼────────────────────────────────┤
│                                                                            │
│   HANGING STORAGE — GOH RAIL SYSTEM     │  FOLDED STOCK SHELVING         │
│   Single-tier + rolling extension rail  │  Longspan shelving             │
│   (600 sq ft / ~55 sq m)               │  (400 sq ft / ~37 sq m)        │
│                                         │                                 │
│   [ Active Hanging SKUs by Category ]   │  [ JEANS — Evergreen Zone ]    │
│   [ Seasonal new arrivals at front ]    │  [ Knitwear / Packed Items ]   │
│                                                                            │
├─────────────────────────────────────────┼────────────────────────────────┤
│   2× PACKING STATIONS                   │  LABELLING / RE-TAGGING        │
│   (220 sq ft)                           │  STATION (180 sq ft)           │
├─────────────────────────────────────────┼────────────────────────────────┤
│   DISPATCH STAGING & MANIFEST AREA      │  MANAGER DESK / WORKSTATION    │
│   (200 sq ft)                           │  (100 sq ft)                   │
└──────────────────────────────────────────────────────────────────────────┘
                      AISLES & MOVEMENT CORRIDORS (300 sq ft)
```

### 1.2 Zone Details

| Zone | Sq Ft | Function |
|------|-------|----------|
| Receiving + QC | 280 | Unloading, counting, barcode scan-in, visual QC |
| Hanging Storage (GOH) | 600 | Single-tier GOH with rolling extension — all hanging garments |
| Folded Shelving | 400 | Jeans (evergreen), knitwear, packed/bagged items |
| Packing Stations (×2) | 220 | B2C online packing + store replenishment bulking |
| Labelling / Re-tagging | 180 | Price changes, supplementary tags, inserts |
| Dispatch Staging | 200 | Carrier sort, manifest print, outbound staging |
| Returns Processing | 120 | Inspect, grade, restock or quarantine |
| Manager Workstation | 100 | WMS access, reporting, admin, label printer |
| Aisles | 300 | Primary aisles ≥4 ft; secondary ≥3 ft |

**Total: 2,400–2,500 sq ft**

### 1.3 Key Layout Principles
- **U-shaped flow:** Goods in on one side → storage in centre → out on other side. This is the industry standard for small warehouses (NetSuite, Logistics Bureau). Prevents cross-traffic and reduces pick travel distance.
- **A-class SKUs closest to packing stations.** Based on ABC analysis (Shopify 2026, Prediko 2026): top 20% of revenue SKUs at front; C-class at the far end.
- **Jeans zone** is at medium distance — high volume but bulk replenishment (not single-piece online orders), so proximity to dispatch is more important than proximity to packing.

---

## 2. Storage Systems

### 2.1 Garment-on-Hanger (GOH) Rail — Hanging Storage

**System:** Single-tier industrial GOH with extension rails (no second tier initially — added at 1.5× scale)

**Why single-tier first:**
- At 5,000 pieces with 50/50 split, 2,500 hanging pieces need ~100 linear feet of rail
- Single-tier at 4 ft height provides 90–120 linear feet of hanging rail within 600 sq ft zone
- Adding a second tier at scaling is straightforward (same upright frames, add cross-bar and rail)

**Specification:**
- Upright frame: heavy-gauge steel, 2.0 m height (compatible with future 2nd tier)
- Rail spacing: 0.6 m between rails (front-to-back)
- Estimated 8–10 runs of 4 m each = ~32–40 lm single-tier = **~700–900 hanging pieces**
- Supplemented by 4–6 rolling clothing racks for receiving staging, overflow, and sorting

**Suggested supplier:** Mecalux, AR Racking, or Indian equivalents (Godrej Interio Storewell, SSI Schäfer India)

**Labelling:**
- Each GOH section labelled with category, style range, and SKU group code
- Laminated label holders on rail uprights — easy to update

**FIFO Protocol on GOH:**
- New arrivals hung at the back of each section
- Pickers always take from front
- Senior associate verifies FIFO compliance during weekly spot check

### 2.2 Folded Storage — Longspan Shelving

**System:** Industrial longspan shelving with bin dividers

**Specification:**
- Shelf unit: 2.1 m tall × 2.4 m wide × 0.6 m deep
- 5 shelf levels per bay; adjustable at 50 mm increments
- Number of units: 14 bays (for 400 sq ft zone)
- Total folded capacity: 14 × 5 × 35 pieces = **~2,450 pieces**

**Jeans Evergreen Zone (6 dedicated bays):**
- Labelled by style name, waist size, and leg length
- Size matrix card laminated on each bay face (e.g., "W30L30 | W30L32 | W32L30...")
- Older stock always in front; new stock placed behind (FIFO)
- Minimum reorder quantity flagged with a coloured card (visual Kanban) when stock drops below 10 per size

**Knitwear / Heavy Knit Zone (3 bays):**
- Stored folded with tissue paper interleaf if premium items
- Seasonal rotation: winter knits move to back-of-shelf during summer months, brought to front in October

**Accessories / Small Items (2 bays):**
- Divided with bin boxes; each bin labelled with SKU and barcode
- Velcro/scrunchies/belts stored in clear lidded bins

### 2.3 Packing Station Setup

**Each station includes:**
- 1× heavy-duty stainless workbench (180 cm × 75 cm)
- 1× thermal label printer (mounted or adjacent)
- 1× barcode scanner (corded)
- 1× small tissue/insert drawer
- 1× waste bin
- Overhead storage shelf for packing materials (boxes, mailers, tape)
- Shipping scale on bench

**Station 1 (B2C / Online):** Single-piece packing; branded mailers; tissue wrap for premium orders.  
**Station 2 (B2B / Store Replenishment):** Bulk carton packing; transfer notes; size breakdowns.

---

## 3. Technology Stack

### 3.1 Barcode-Based Inventory Management (Core System)

**Recommended Platform:** Linnworks, Uphance, or Zoho Inventory (fashion-friendly tier)

**Why not RFID at this stage:**
- RFID requires tagging at source (labelling center), reader infrastructure, and ongoing tag cost (~$0.10–0.15/piece)
- At 2,900 pieces/month inbound, barcode scanning is fast enough (1 scan per item vs. bulk RFID tunnel)
- Barcode infrastructure is 80–90% cheaper to set up
- When scaling to Proposal 1, the WMS and barcode infrastructure transfer directly — RFID is additive

**Recommended: Linnworks (cloud WMS)**
- Specifically built for multi-channel retail (DTC + wholesale + marketplace)
- Native Shopify, Amazon, and marketplace integrations
- Inventory sync prevents overselling across channels
- Pick/pack/dispatch workflow with barcode verification
- Price: starts ~$449–$599/month for growth tier; scalable

**Alternative: Uphance (apparel-specific ERP/WMS)**
- Fashion-native: size-colour matrix, style management, collection management
- WMS + ERP in one platform for a small brand (avoids separate tools)
- Price: ~$400–$800/month depending on modules

**Alternative: Zoho Inventory (budget-conscious)**
- Very affordable ($59–$199/month)
- Good barcode scanning workflows
- Not fashion-specific but handles SKU variants
- Best if also using Zoho Books for accounting (native integration)

### 3.2 Barcode Scanning Hardware

| Equipment | Model | Qty | Unit Cost |
|-----------|-------|-----|-----------|
| Barcode Scanner — Corded | Zebra DS2208 or Honeywell 1900 | 3 | $80–$150 each |
| Barcode Scanner — Wireless | Zebra DS3678 (for GOH zone) | 1 | $300–$450 |
| Thermal Label Printer | Zebra GK420d or ZD421 | 2 | $250–$400 each |
| Shipping Scale | Generic postal scale (30 kg capacity) | 2 | $80–$150 each |
| Workstation Desktop/Laptop | Manager + 1 packing station | 2 | $400–$700 each |

**Total hardware: ~$2,200–$3,750**

### 3.3 SKU Labelling System

**For the warehouse:**
- Every storage location (shelf bay + shelf level + position) gets a printed barcode location label
- Location naming convention: **Zone-Row-Bay-Level** → e.g., `H-A-03-2` (Hanging zone, Aisle A, Bay 3, Tier 2)
- Bin labels: laminated A5 card with SKU, style, size, barcode
- WMS maps every SKU to a primary location (+ overflow location)

**For garments (if not pre-labelled by labelling center):**
- Use Zebra ZD421 thermal printer for supplementary barcode hang tags
- Standard: EAN-13 or Code 128 barcode + readable SKU + style name + size

### 3.4 E-Commerce & Store Integration

- WMS syncs real-time inventory to Shopify (or whichever platform) every 15–30 minutes
- When an online order is placed: inventory reserved immediately (prevents overselling)
- Store replenishment: manager raises transfer request in WMS → pick list generated → carton sent with digital transfer note

### 3.5 Reporting & Analytics

- Weekly: WMS dashboard → inventory snapshot, orders fulfilled, pending, pending returns
- Monthly: Manager prepares report: inbound vs. outbound by category, dead stock list (items >60 days without movement), stockout alerts
- ABC Analysis: run quarterly using WMS "velocity report" → re-slot accordingly

### 3.6 CCTV & Security

- 6-camera basic IP CCTV system (receiving, storage, packing, dispatch, returns, entry)
- Cloud-recorded DVR (accessible remotely by founder/COO)
- Cost: $600–$1,200 installed

---

## 4. Standard Operating Procedures (SOPs)

### SOP 1: INBOUND RECEIVING

**When:** Goods arrive from manufacturing or procurement/labelling center.

**Pre-arrival:**
1. Sender raises a dispatch note (Google Sheet, WhatsApp, or WMS Transfer Order) listing items, quantities, and SKUs.
2. Warehouse manager reviews and assigns a receiving slot.

**On arrival:**
1. Driver signs inbound register (paper logbook at dock).
2. Associates unload onto receiving zone — nothing goes directly to storage.
3. **Count & verify:** Count pieces against dispatch note. Record count in WMS receiving screen or paper tally sheet.
4. **Visual QC (100% check for new styles; 10% spot check for repeat styles):**
   - Verify brand hangtag presence
   - Check for obvious defects (stitching, staining, size mismatch)
   - Defective pieces: place in red-bin "quarantine" — document on QC log
5. **Barcode scan-in:** Scan each unique SKU's barcode into WMS Receiving screen. Enter quantity. WMS updates inventory in real time.
6. **Generate putaway list** from WMS. Assign to associate.
7. **Quarantine report** sent to manufacturing/procurement within 2 hours.

**KPI target:** All received goods scanned and putaway within 4 hours of arrival.

---

### SOP 2: PUTAWAY

1. Associate reviews putaway list (WMS screen or printed).
2. Carry/wheel garments to assigned location.
3. Hanging: hang on assigned GOH section; new stock behind existing stock (FIFO).
4. Folded: place on correct shelf; newest stock at back.
5. Scan location barcode + item barcode to confirm in WMS.
6. If location full: note "overflow" in WMS; inform manager. Do not create ad-hoc locations.

**Rule:** No item stored without a scanned location in WMS. "Floor stock" is never acceptable.

---

### SOP 3: ONLINE ORDER PICKING

**Trigger:** Online order received; WMS generates pick task.

1. Picker receives pick list (printed or on screen).
2. Pick list sorted by zone (all hanging items first, then folded) to minimise travel.
3. Picker moves to location, takes item from front of stock (FIFO), scans barcode.
4. WMS confirms item match. If mismatch: do not proceed; alert manager.
5. Place in tote labelled with order number.
6. Return to packing station when all items in order are picked.

**For multi-SKU orders:** Complete all picks for one order before starting next (zone-based, not order-based picking at this scale).

**KPI target:** Pick accuracy ≥ 99%; time per pick ≤ 2 minutes (including travel).

---

### SOP 4: STORE REPLENISHMENT PICKING

1. Store manager sends replenishment request (WhatsApp message → logged in WMS as Transfer Order, or direct WMS access for store manager).
2. Warehouse manager reviews stock availability; approves Transfer Order.
3. WMS generates pick list by category.
4. Picker fulfils by category and size; places in cartons labelled with store name and date.
5. Manager performs final count check against transfer order.
6. Carton sealed; transfer note printed (2 copies: one retained, one with driver).
7. WMS transfers inventory from warehouse to store location.

---

### SOP 5: PACKING — ONLINE ORDERS (B2C)

1. Tote with order arrives at B2C packing station.
2. Packer opens order on WMS packing screen; scans order barcode.
3. Scan each garment barcode — WMS confirms all items present and correct.
4. Final visual check: remove any stray tags, ensure garment is clean and folded neatly.
5. Fold/wrap in tissue paper for premium pieces; place in branded mailer or box.
6. Include order insert (thank-you card, brand note, discount card) if applicable — kept in station drawer.
7. Print shipping label from WMS (auto-generated from courier integration).
8. Apply label; place on dispatch shelf sorted by carrier.

**KPI target:** Pack rate ≥ 25 orders/hour per station.

---

### SOP 6: PACKING — STORE REPLENISHMENT (B2B)

1. Pick tote arrives at B2B packing station.
2. Carton lined with polybag layer; garments folded and stacked by size.
3. Transfer note printed; placed inside carton.
4. Carton taped and labelled (store name, date, carton number).
5. WMS Transfer Order closed as dispatched.

---

### SOP 7: DISPATCH

1. End of dispatch cutoff time (set at 3 PM for same-day; 5 PM for next-day carriers — align with actual courier SLAs).
2. Packer/dispatch associate runs carrier manifest from WMS.
3. Each parcel manually scanned against manifest.
4. Carrier agent picks up; signs manifest.
5. WMS marks orders as shipped; e-commerce platform sends tracking notification to customer automatically.

---

### SOP 8: RETURNS PROCESSING

1. Return parcel arrives. Photograph outer packaging before opening.
2. Open parcel; check return reason (written by customer or on return form).
3. Inspect garment:
   - **Grade A (unused, tagged):** Re-fold, re-pack if needed; scan back into WMS inventory as "returned to stock."
   - **Grade B (tried, small issue):** Move to returns assessment shelf; manager reviews — either steam/refresh and restock, or move to outlet.
   - **Grade C (damaged, worn beyond resale):** Log in returns write-off register. Manager authorises disposal.
4. All returns logged in WMS returns module.
5. Refund/exchange initiated in e-commerce platform.

**KPI target:** Returns processed within 24 hours of receipt; Grade A back in sellable stock within 48 hours.

---

### SOP 9: CYCLE COUNT (Inventory Accuracy)

**Weekly:**
- Senior associate scans all A-class SKUs (jeans + top-velocity items) with barcode scanner.
- Compare scanned count vs. WMS count. Log any variances.
- Investigate and resolve variances within 48 hours.

**Monthly:**
- Full warehouse scan by category. Two associates on different sections; cross-verify.
- Manager reviews report; signs off.
- Discrepancies >5% trigger root cause analysis.

**Quarterly:**
- Full physical count. All staff participate. Warehouse paused for 2 hours.
- Signed count sheet filed for record.

---

### SOP 10: HOUSEKEEPING

**Daily:**
- Packing debris cleared; floor swept in packing and dispatch zones.
- Totes returned to receiving/staging area.
- Empty hangers consolidated on a spare rail (don't scatter).

**Weekly:**
- Full aisle sweep; inspect racking for any dents, leaning, or loose connectors.
- Check fire extinguisher pins; confirm exit routes unobstructed.
- Wipe down packing station workbenches.

**Monthly:**
- Formal racking safety check (manager + one associate; checklist); log filed.
- Pest control inspection (especially near receiving area).
- CCTV review — confirm all cameras operational.

---

## 5. Staffing & Roles

### 5.1 Day-1 Team (3–4 Staff)

| Role | Count | Monthly Cost (INR) | Key Responsibilities |
|------|-------|-------------------|----------------------|
| **Warehouse Manager** | 1 | ₹35,000–₹55,000 | Operations lead; WMS admin; carrier management; reporting; staff management; KPI ownership |
| **Senior Associate (Receiving + Inventory)** | 1 | ₹18,000–$25,000 | Inbound receiving; QC check; putaway; cycle counts; trains associates |
| **Associate (Pick/Pack)** | 1–2 | ₹14,000–₹20,000 | Online order picking; packing; store replenishment picking; housekeeping |

**Monthly payroll: ₹67,000–₹1,20,000 / ~$800–$1,450**

---

### 5.2 Warehouse Manager — Full JD

**Reports to:** COO / Founder  
**Direct reports:** Senior Associate, Pick/Pack Associates  
**Working hours:** Standard business hours + availability on WhatsApp for urgent dispatch issues

**Core Responsibilities:**

*Operations:*
- Own daily receiving, storage, dispatch cycle end-to-end
- Manage WMS: create Transfer Orders, review returns, run reports
- Approve store replenishment requests; flag stock discrepancies to buyers/planners
- Coordinate with courier partners: daily manifests, escalation of delivery failures, rate reviews

*Inventory:*
- Weekly cycle count execution
- Maintain 99%+ inventory accuracy
- Run quarterly ABC analysis; propose slotting changes to COO
- Flag slow-moving stock (>60 days) to brand team for markdown/clearance decisions

*People:*
- Write daily/weekly task schedule for associates
- Train new hires on SOPs (documented in this proposal)
- Review associate performance monthly; provide feedback

*Compliance & Safety:*
- Maintain all safety registers (racking, fire, accident/near-miss log)
- Ensure GST/e-way bill compliance for inter-state stock movements
- Keep labour compliance documentation (PF/ESI records with HR)

*Reporting (Weekly, to COO):*
- Units received vs. expected
- Orders dispatched (online + store transfer)
- Inventory accuracy score (from cycle count)
- Returns processed
- Any critical stock-outs or overstock flags

**Skills Required:**
- 1–3 years warehouse/logistics experience (fashion retail experience preferred)
- Confident with computer/WMS; Excel proficiency for reports
- Spoken and written English + local language
- Problem-solver; thrives in fast-paced, reactive environment

---

### 5.3 Senior Warehouse Associate — Full JD

**Reports to:** Warehouse Manager  
**Key responsibilities:**
- Execute all receiving SOPs; own inbound accuracy
- Perform visual QC on inbound garments per AQL standard
- Operate barcode scanner for all scan-in and putaway
- Run weekly A-class cycle count
- Stand in for manager when absent; brief manager on any issues
- Ensure FIFO compliance across all storage zones
- Manage consumables stock (labels, tape, mailers, tissue) — raise purchase request when ≤ 1 week supply remaining

**Skills:** Attention to detail; organised; basic computer literacy for WMS.

---

### 5.4 Associate (Pick/Pack) — Full JD

**Reports to:** Warehouse Manager / Senior Associate  
**Key responsibilities:**
- Pick online orders per WMS pick list; achieve pick accuracy target
- Pack online orders to brand standard (branded packaging, inserts)
- Pack store replenishment cartons
- Print and apply shipping labels
- Stage dispatch parcels by carrier
- Assist receiving team on high-inbound days
- Daily housekeeping of work area

**Skills:** Physical fitness (standing, lifting up to 10 kg); attention to detail; basic barcode scanner operation.

---

## 6. Compliance & Safety Standards

| Area | Standard | Action |
|------|----------|--------|
| Racking Load | Load posted on each bay | Get rated load from supplier; print placard; laminate and affix to upright |
| Aisle Markings | Yellow floor tape minimum 4 ft primary, 3 ft secondary | Paint or self-adhesive floor tape from Day 1 |
| Fire Safety | 1× 2 kg CO2 extinguisher per 500 sq ft; annual service | 5 units; log inspections monthly |
| Emergency Exits | Clearly marked; never obstructed | Green exit signs (powered); quarterly drill |
| Sprinkler / Fire Suppression | Check building's existing provisions; add smoke detectors if no sprinklers | Minimum 5 smoke detectors + 1 heat detector in receiving zone |
| GST / E-Way Bill | Mandatory for stock valued >₹50,000 moving inter-state | WMS/ERP generates automatically at dispatch |
| Labour Compliance | PF, ESI, shop registration | Register under Shops & Establishments Act of the state; file ESI/EPF from month 1 |
| CCTV | Industry norm for warehouse | 6 cameras, 30-day retention |

---

## 7. Cost Breakdown

### 7.1 Setup Costs (One-Time)

| Item | Est. Cost (USD) | Est. Cost (INR) |
|------|----------------|-----------------|
| GOH single-tier rail system (32–40 lm) | $3,500–$5,500 | ₹2.9–₹4.6 lakhs |
| 4–6 rolling clothing racks (industrial) | $600–$900 | ₹50,000–₹75,000 |
| Longspan shelving (14 bays) | $3,000–$4,500 | ₹2.5–₹3.7 lakhs |
| Barcode scanners ×4 (3 corded + 1 wireless) | $550–$900 | ₹46,000–₹75,000 |
| Thermal label printers ×2 (Zebra GK420d) | $500–$800 | ₹41,000–₹66,000 |
| Packing station workbenches ×2 | $400–$700 | ₹33,000–₹58,000 |
| Shipping scales ×2 | $160–$300 | ₹13,300–₹25,000 |
| Workstation computers ×2 | $800–$1,400 | ₹66,000–₹1.16 lakhs |
| CCTV (6 cameras, DVR) | $600–$1,200 | ₹50,000–₹1 lakh |
| Fire safety equipment | $400–$600 | ₹33,000–₹50,000 |
| Floor tape, racking signs, labels | $200–$350 | ₹16,600–₹29,000 |
| Warehouse trolleys ×3 + accessories | $400–$650 | ₹33,000–₹54,000 |
| WMS setup + onboarding | $500–$1,500 | ₹41,500–₹1.25 lakhs |
| Bin boxes, label holders, consumables initial | $300–$500 | ₹25,000–₹41,500 |
| Miscellaneous (extension cords, shelving dividers, etc.) | $200–$400 | ₹16,600–₹33,000 |
| **Total Setup** | **$12,110–$18,000** | **₹10–₹15 lakhs** |

### 7.2 Ongoing Monthly Costs

| Item | Monthly (USD) | Monthly (INR) |
|------|-------------|---------------|
| WMS subscription (Linnworks/Uphance) | $449–$800 | ₹37,000–₹66,000 |
| Packaging consumables (mailers, boxes, tissue, tape) | $250–$500 | ₹20,750–₹41,500 |
| Labels/tags (thermal labels) | $80–$150 | ₹6,600–₹12,400 |
| Electricity | $150–$300 | ₹12,450–₹24,900 |
| Staff payroll (3–4 staff) | $800–$1,450 | ₹66,400–₹1.2 lakhs |
| **Total Monthly** | **$1,729–$3,200** | **₹1.43–₹2.66 lakhs** |

### 7.3 Total Year-1 Cost
- Setup: $12,110–$18,000
- Monthly ongoing ×12: $20,748–$38,400
- **Year-1 Total: ~$32,858–$56,400 / ₹27–₹47 lakhs**

---

## 8. Scaling Considerations

### 8.1 Scale to 1.5× (~4,350 pcs/month inbound, ~7,500 pieces stock)

**No major structural change needed.** Actions:

- Add second tier to GOH system ($1,800–$3,000; same uprights, just add cross-bars and rails)
- Add 4 more longspan shelving bays (~$800–$1,200)
- Add 1 Pick/Pack Associate
- Upgrade WMS to next plan tier (usually $150–$300/month more)

**Staff: add 1 associate → total 4–5**

---

### 8.2 Scale to 2× (~5,800 pcs/month inbound, ~10,000 pieces stock)

**Structural actions:**

- Mezzanine: build a partial mezzanine over 30–40% of warehouse (approx. 750–1,000 sq ft upper floor)
  - Cost: ~$8,000–$15,000
  - Adds 750–1,000 sq ft of GOH/shelving space — enough for 2× with comfortable headroom
- Introduce **wave picking** via WMS (batch 15–20 online orders per pick run — reduces picker travel time by ~30%)
- Add dedicated **Receiving Associate** (previously Senior Associate did both receiving and cycle counts — now separate roles)
- Consider upgrading barcode scanners to wireless Zebra TC-series mobile computers (with WMS app on screen) — ~$800–$1,000 each; enables real-time picking with WMS guidance

**Staff at 2×:**
| Role | Count |
|------|-------|
| Warehouse Manager | 1 |
| Senior Associate (Inventory Lead) | 1 |
| Receiving Associate | 1 |
| Pick/Pack Associates | 2–3 |
| **Total: 5–6 staff** | |

**WMS upgrade:** Move to Linnworks growth or enterprise plan, or evaluate Increff WMS at this point (sets up for Proposal 1 upgrade)

**Total cost to scale to 2×: ~$12,000–$22,000 one-time + $500–$800/month additional operating costs**

---

### 8.3 Scale to 3× (~8,700 pcs/month inbound, ~15,000 pieces stock)

**This is the transition point to Proposal 1 infrastructure.** Key decisions:

- **WMS:** Migrate to Increff WMS (fashion-specific, AI/ML demand forecasting, multi-channel)
- **RFID:** Begin RFID rollout — first at receiving and dispatch tunnels; handheld readers for cycle count
- **Mezzanine:** Full mezzanine over 50% of warehouse floor
- **GOH conveyor:** Add motorised overhead GOH conveyor if hanging volume exceeds 3,000 pieces
- **Additional staff required:**

| Role | Count |
|------|-------|
| Warehouse Manager | 1 |
| Shift Supervisor | 1 |
| Senior Associates | 2 |
| Receiving + QC Associates | 2 |
| Pick/Pack Associates | 3–4 |
| Returns Handler | 1 |
| **Total: 10–11 staff** | |

**Migrate cost to Proposal 1 infrastructure: ~$35,000–$55,000 additional investment (largely RFID + WMS upgrade + mezzanine)**

---

### 8.4 When to Know You're at the Scaling Threshold

| Metric | Action Trigger |
|--------|---------------|
| Storage utilisation > 80% | Begin mezzanine planning |
| Dispatch backlog > same day | Add pick/pack associate or evening shift |
| Receiving backlog > next morning | Add dedicated receiving associate |
| WMS cycle count variance > 3% regularly | Evaluate RFID upgrade |
| Associate overtime > 15% of hours/week | Hire next FTE immediately |
| Online order errors (wrong item) > 0.5% | SOP audit + retraining |

---

## 9. Seasonal Operations Plan

Fashion has inherent peaks. This proposal accounts for them:

**Pre-season build (2–3 months before launch):**
- Negotiate extended delivery slots at procurement/labelling center to stagger warehouse inbound
- Pre-allocate storage locations before goods arrive (WMS slotting pre-plan)
- Temporarily hire 1–2 contract associates for peak weeks (1–4 weeks duration)

**During peak (festival season, sale events):**
- Online order cutoff moved earlier in day (2 PM instead of 3 PM) to ensure same-day dispatch
- One manager and one associate stagger to an afternoon shift during peak weeks
- Priority slotting: new season items moved closest to packing stations

**Post-season clearance:**
- Slow-moving items flagged (>45 days unsold) → manager reports to brand team
- Clearance SKUs moved to designated clearance bin/section
- Brand team decides: markdown in store, online flash sale, or outlet transfer

---

## 10. Pros, Cons & Best-Fit Assessment

### Pros
- Right-sized investment — doesn't over-commit cash before revenue validates scale
- Fully operational within 2–3 weeks of warehouse fit-out
- Every component upgrades into Proposal 1 infrastructure (no throwaway work)
- WMS from Day 1 establishes inventory discipline and data quality
- Standard barcode approach is familiar — faster staff onboarding
- 3–4 person team is lean and manageable for a founder-led brand

### Cons
- Barcode vs. RFID means manual scan per item — slower cycle counts and receiving
- Not designed for 10× growth without significant rebuild — but that's intentional (cashflow prioritisation)
- WMS requires manager to be computer-literate and willing to invest time in setup
- Limited automation means error rates depend more on people than systems

### Best Fit
This is the **recommended proposal** for the brand at its current stage. It establishes professional warehouse operations, builds inventory data discipline, and creates a foundation that upgrades cleanly as the brand grows — without betting cash the brand needs for product, marketing, and team on warehouse infrastructure.

---

*Sources: Linnworks Multi-Channel WMS, Uphance Apparel Warehouse Optimization, NetSuite Apparel Warehousing Guide, Mecalux Clothing Racks, AR Racking GOH Systems, Prediko Clothing Inventory Management 2026, Shopify Clothing Inventory Management 2026, Logistics Bureau Warehouse Design Rules of Thumb, GoAudits Warehouse SOP Guide, Bleckmann Fashion Brand Scaling, Zoho Inventory, OSHA 1910.176.*

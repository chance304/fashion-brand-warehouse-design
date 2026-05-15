# Warehouse Design — Decision Log

**Session Date:** 2026-05-16  
**Status:** Completed autonomously (user unavailable during session)  
**Prepared by:** Claude Code (claude-sonnet-4-6)

---

## Context Summary

A small-scale fashion brand has acquired an empty warehouse space near its manufacturing and procurement/labelling center. The brand currently operates:
- 1 HQ store
- 1 high-footfall secondary store (often outperforms HQ)
- Online channel (~30% of all orders)
- Manufacturing center (30 pieces/day manufactured)
- Procurement & labelling center (~2,000 pieces procured/month)

At any given time, the brand holds ~5,000 pieces of clothing in stock.

---

## Assumptions Made (User Was Unavailable)

### 1. Warehouse Size
**Assumption:** ~2,500 sq ft (230 sq m) usable floor area.  
**Rationale:** Calculated based on 5,000-piece maximum stock. Industry benchmark for hanging garments is ~22–25 pieces per linear meter of rail; folded goods achieve ~8–10 pieces per sq ft of shelf. With 50/50 hanging-to-folded split, 600–800 sq ft of racking covers active stock. Adding receiving (300 sq ft), packing (250 sq ft), dispatch staging (200 sq ft), returns (150 sq ft), labelling corner (200 sq ft), admin (100 sq ft), and aisles (300 sq ft) arrives at ~2,500 sq ft — a standard "small warehouse" unit size that also provides growth headroom to 1.5× before a structural upgrade is needed.

### 2. Stock Split by Storage Type
**Assumption:** 50% of SKUs hang (tops, dresses, jackets, shirts), 50% fold (jeans, knitwear, accessories).  
**Rationale:** User noted jeans stock up heavily. Jeans are better stored folded on shelves. Trend/seasonal pieces tend to be hanging to avoid wrinkles and to maintain visual inspection capability.

### 3. Each Design Run ≤ 500 Pieces
**Assumption:** This tip was taken literally — the brand's design team finalises a style, then manufacturing produces a limited run (≤500 pcs per design). Jeans are the evergreen exception and may see re-orders that exceed 500 pcs across multiple batches.  
**Impact on design:** The warehouse must support high SKU diversity at low per-SKU quantities — this means fine-grained slotting, robust SKU labelling, and a WMS or IMS that can handle many small-batch SKUs without confusion.

### 4. Inbound Volume
**Assumption:** Total inbound = ~2,900 pieces/month (900 manufactured + 2,000 procured). Peak months assumed to reach ~1.5–2× this volume (~4,300–5,800 pieces/month) for seasonal pushes.  
**Rationale:** Fashion brands typically see 30–50% peak volume above average during festive or collection-launch periods.

### 5. Online Channel Fulfillment
**Assumption:** 30% of orders are online/DTC (direct-to-consumer). These require individual picking, branded packing, and carrier label printing. Physical stores receive bulk replenishment transfers.  
**Impact:** A dedicated packing zone with 2 packing stations is included from Day 1.

### 6. Currency & Geography
**Assumption:** Proposals are presented in USD with indicative INR equivalents (~₹83/USD exchange rate) since the brand appears to be India-based (manufacturing center model, common for emerging Indian fashion brands). All compliance references are to both OSHA (global best practice) and Indian Factories Act/Shops & Establishments Act where relevant. Teams are sized for Indian labour market norms.

### 7. Three-Zone Inbound Flow
**Assumption:** Goods arrive at the warehouse already branded/labelled (via the existing procurement & labelling center). The warehouse's job is to receive, quality-check, store, pick, pack, and dispatch — not to apply brand labels. However, a small labelling station is retained for re-tagging, price changes, and online order inserts.

### 8. No Forklift Initially
**Assumption:** At this scale (5k pieces of clothing, not palletised heavy goods), a forklift is not required. A manual pump truck/pallet jack and a step ladder or rolling platform are sufficient. High-tech proposal includes a vertical lift module instead of a forklift.

### 9. Jeans as Evergreen Category
**Assumption:** Jeans get a dedicated, labelled "evergreen zone" with higher capacity allocation and FIFO rotation protocol. They are not subject to the same seasonal clearance pressure as fashion trend pieces.

### 10. Designer-to-Warehouse Flow
**Assumption:** The design team finalises → manufacturing or procurement begins → goods arrive pre-labelled → warehouse takes ownership. The warehouse is not part of the design or QC-at-source stage but performs final QC on arrival.

---

## Structural Decisions

| # | Decision | Rationale |
|---|----------|-----------|
| D1 | Three proposals produced: High-Tech, Optimal, Makeshift | Per user brief |
| D2 | Warehouse size anchored at 2,500 sq ft | Calculated minimum with growth buffer; see Assumption 1 |
| D3 | Zone split: 12% receiving, 40% storage, 10% packing, 8% dispatch, 6% returns, 8% labelling, 4% admin, 12% aisles | Industry standard: 20–25% for non-storage ops (NetSuite / Logistics Bureau) |
| D4 | ABC slotting strategy applied in all proposals | Industry best practice — A items (top 20% revenue SKUs) nearest packing stations |
| D5 | Garment-on-Hanger (GOH) system as primary storage for hanging garments | Industry standard for apparel warehouses (AR Racking, Mecalux, XPDEL research) |
| D6 | FIFO (First-In-First-Out) enforced for all stock | Standard for fashion to prevent dead stock accumulation |
| D7 | Jeans get dedicated section with deeper shelving capacity | Evergreen category per user tip |
| D8 | Online orders handled at dedicated packing stations | 30% volume + different pack type justifies separation |
| D9 | Staff headcount starts at 3–4 (manager + associates) | Right-sized for ~2,900 pieces/month inbound at small scale |
| D10 | Scaling milestones defined at 2× and 3× current volume | Per user brief |

---

## Files Produced

| File | Description |
|------|-------------|
| `proposal_1_hightech_scalable.md` | High-tech, fully scalable warehouse (enterprise-grade) |
| `proposal_2_optimal_brand.md` | Optimal for investment-backed emerging brand (recommended) |
| `proposal_3_makeshift_lowcost.md` | Low-cost, fast-to-deploy makeshift solution |
| `DECISIONS.md` | This file — all assumptions and decisions documented |

---

## Research Sources Used

- NetSuite Apparel Warehousing Guide
- AR Racking / Mecalux Garment Storage Systems
- XPDEL / REB Storage Warehouse Clothing Racking
- OSHA Warehouse Standards (racking, aisles, fire codes)
- ShipHero / ExploreWMS — WMS Cost Guides 2025–2026
- AutoStore Fashion Warehousing Insights
- Prediko / AIMS360 — Fashion Inventory Management
- Uphance Apparel Warehouse Optimization
- Logistics Bureau — Warehouse Design Rules of Thumb
- GoAudits Warehouse SOP Guide
- Bleckmann — Fashion Brand Scaling Obstacles
- Shopify — Clothing Inventory Management 2026

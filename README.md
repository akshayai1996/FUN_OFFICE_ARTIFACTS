# 🧰 FUN OFFICE ARTIFACTS

> **A zero-server, privacy-first suite of single-file browser tools for engineers, estimators, and office professionals.**
>
> 100% Client-Side · Zero Telemetry · Offline Capable · Air-Gapped Safe · Single-File Simplicity

---

## 🌐 Overview & Philosophy

In modern engineering and corporate environments, everyday tasks—such as stripping internal markup from client-facing PDF drawings, tracking vendor submittal packages, managing discipline tickets, calculating linear interpolations from ASME tables, or creating digital signatures—often tempt users to turn to random online web converters.

**The danger:** Commercial "free" web tools upload your proprietary drawings, vendor specifications, and corporate documents to third-party cloud servers, risking enterprise data leakage and violating confidentiality agreements.

**Fun Office Artifacts** solves this problem by providing self-contained, single-file HTML5 utilities that execute **exclusively inside your web browser's memory sandbox**. No backend exists. No data ever leaves your computer.

```
┌───────────────────────────────────────────────────────────────────────────────────┐
│                          ZERO-LEAK RUNTIME ARCHITECTURE                           │
├───────────────────────────────────────────────────────────────────────────────────┤
│ USER BROWSER (CHROME / EDGE / FIREFOX / SAFARI)                                   │
│   │                                                                               │
│   ├─► [ 100% Client-Side Engine: JavaScript + HTML5 Canvas + Web APIs ]           │
│   │                                                                               │
│   ├─► Storage Layer:  Local Browser Only (localStorage / IndexedDB)               │
│   │                                                                               │
│   ├─► Export Engine:  Local File System (Direct .CSV / .XLSX / .PNG / .PDF)       │
│   │                                                                               │
│   ▼                                                                               │
│   X - ZERO OUTBOUND NETWORK TRAFFIC  (No telemetry · No cloud API · No backend)   │
└───────────────────────────────────────────────────────────────────────────────────┘
```

---

## 🛡️ Zero-Data-Leak Guarantee

> 🔑 **Privacy Guarantee:** Every tool in this repository runs locally. When you drop a PDF, paste a document register, or draw a signature, that data stays in your browser's private memory and is never transmitted over any network.

| Security Criterion | ❌ Traditional Online SaaS Tools | ✅ Fun Office Artifacts Suite |
| :--- | :--- | :--- |
| **Document Privacy** | Uploaded to remote 3rd-party cloud servers | **100% local inside your browser memory** |
| **Network Requirement** | Requires continuous high-speed internet | **Fully offline & air-gapped capable** |
| **Account & Licensing** | Sign-up, email capture, paid subscriptions | **Zero accounts, zero cost, MIT licensed** |
| **Installation** | Requires Node.js, Python, or desktop installers | **Single .html file — double click & run** |
| **Enterprise Compliance** | Risk of cloud data breaches and NDAs violations | **Zero outbound packets — safe for proprietary drawings** |

---

## 🚀 Tool Inventory & Capabilities

```
┌──────────────────────────────┬──────────────────────┬──────────────────────────────────────────────────┬─────────────────┐
│ Tool Artifact                │ Discipline / Domain  │ Primary Capability                               │ Network Traffic │
├──────────────────────────────┼──────────────────────┼──────────────────────────────────────────────────┼─────────────────┤
│ EPC_Project_Ticket.html      │ Project Management   │ Eisenhower Matrix, RACI tracking, CSV/JSON sync  │ 0 KB (None)     │
│ Vendor_Package_Register.html │ Vendor Engineering   │ Doc review milestones, register & Excel export   │ 0 KB (None)     │
│ Digital_Signature.html       │ Office Admin / Docs  │ Smooth bezier hand-drawn & 30 typography styles  │ 0 KB (None)     │
│ PDF_Annotation_Cleaner.html  │ Document Control     │ Strips review markup/comments via client pdf-lib │ 0 KB (None)     │
│ PDF_Merge_Rotate.html        │ Document Control     │ Offline merge, rotate, page extract & bundle     │ 0 KB (None)     │
│ Linear_Interpolation.html    │ Engineering / Piping │ Instant 1D/2D table interpolation & math steps   │ 0 KB (None)     │
│ Case_Converter.html          │ CAD / Code / Docs    │ 8-mode case conversion (UPPER, snake, camel...)  │ 0 KB (None)     │
└──────────────────────────────┴──────────────────────┴──────────────────────────────────────────────────┴─────────────────┘
```

---

## 📦 Detailed Tool Walkthrough

### 1. 🎫 EPC Project Ticket Manager V2 (`EPC_Project_Ticket.html`)
A complete engineering project management and ticket triage dashboard designed specifically for multi-discipline EPC (Engineering, Procurement, and Construction) workflows.

- **Eisenhower Priority Matrix:** Visual drag-and-drop 4-quadrant prioritization based on Urgency vs. Importance.
- **RACI Matrix Support:** Assign distinct roles per task: **R**esponsible, **A**ccountable, **S**upport, **C**onsulted, and **I**nformed.
- **Multi-Discipline Tagging:** Tailored for Process, Piping, Mechanical, Civil, Structural, Electrical, Instrumentation, QA/QC, HSE, and Project Management.
- **Gantt & Due Date Scheduling:** Real-time countdowns, overdue alerts, and milestone tracking.
- **Enterprise Data Sync:** Instant CSV export for reporting and complete JSON backup/restore for zero-loss local portability.

---

### 2. 📋 Vendor Package Register (`Vendor_Package_Register.html`)
An operational document register for package managers and lead engineers tracking vendor submittals, review cycles, and approval gates.

- **Lifecycle Review Tracking:** Track submittals across statuses: *Pending*, *In Review*, *Commented*, *Approved*, and *Resubmission Required*.
- **Milestone Due Dates:** Automated timeline tracking to prevent review bottlenecks and contract delay liquidated damages.
- **Direct Excel Export:** Integrates client-side ExcelJS to generate production-ready `.xlsx` spreadsheets directly from browser memory.
- **Project Workspaces:** Manage independent vendor registers across multiple plant projects within a single workspace.

---

### 3. ✍️ Signature Studio V2 (`Digital_Signature.html`)
A digital signature generation studio built for approvals, transmittals, and clean document endorsements.

- **Hand-Drawn Vector Pad:** Smooth bezier stroke rendering with adjustable nib width, pressure smoothing, and ink palette.
- **30 Typographic Signature Styles:** Instant font rendering across 30 curated calligraphy, cursive, and handwriting engines.
- **Transparent PNG & SVG Export:** Download clean, cropped transparent PNGs or scalable vector SVGs ready for document placement.
- **Preset Library:** Save your preferred signature styles into browser storage for one-click re-use.

---

### 4. 🧹 Annotation Purge — PDF Cleaner (`PDF_Annotation_Cleaner.html`)
A document hygiene utility for document controllers and engineers before external release.

- **Markup Stripping:** Erases review comments, yellow sticky notes, highlight pens, freehand ink, strike-throughs, and review stamps.
- **Pristine Base Layer:** Retains all native vector lines, text, embedded fonts, and drawing stamps while clearing review clutter.
- **Client-Side `pdf-lib` Engine:** Operates on confidential drawings up to hundreds of megabytes without uploading to external servers.

---

### 5. 📑 PDF Merge & Rotate Studio (`PDF_Merge_Rotate.html`)
A self-contained PDF manipulation workstation for assembling drawing packages and vendor dossiers.

- **Zero-Dependency Offline Operation:** Bundles embedded `pdf-lib` and `pdf.js` for 100% offline air-gapped performance.
- **Multi-Document Merging:** Combine multiple drawing files, datasheets, and specification sheets into a unified PDF.
- **Page-Level Controls:** Reorder pages with drag-and-drop, delete blank sheets, and rotate individual or batch pages (90°, 180°, 270°).

---

### 6. 📐 Linear Interpolation Auto-Calculator (`Linear_Interpolation.html`)
A rapid mathematical calculation utility for process, piping, and mechanical engineers referencing discrete standards tables.

- **Discrete Lookup Solving:** Perform instant 1D linear interpolations between discrete pressure-temperature tables (e.g., ASME B31.3 / B31.12, ASME B16.5 flange ratings, steam tables).
- **Formula Proof & Verification:** Displays intermediate calculation steps:
  $$\text{Value} = Y_1 + \frac{(X - X_1)}{(X_2 - X_1)} \times (Y_2 - Y_1)$$
- **Boundary Validation:** Detects and flags accidental extrapolations to prevent calculation errors.

---

### 7. 🔤 Engineering & Developer Case Converter (`Case_Converter.html`)
A text transformation utility for drafting, equipment tagging, and data normalization.

- **Supported Transformations:**
  - `UPPERCASE` — Standard engineering drawing titles and piping line lists
  - `lowercase` — Email identifiers and web slugs
  - `Title Case` — Document reports and transmittal titles
  - `camelCase` & `PascalCase` — Code variables and automation scripts
  - `snake_case` & `CONSTANT_CASE` — Database keys and environment variables
  - `kebab-case` — URL paths and CSS class names
- **Live Text Metrics:** Real-time character counts, word totals, and line statistics.

---

## 🛠️ Quick Reference & Usage

```
┌──────────────────────────────┬─────────────────────────────────┬──────────────────────────────────────────┬───────────────────────┐
│ File Name                    │ Launch Method                   │ Key Features                             │ Storage Key           │
├──────────────────────────────┼─────────────────────────────────┼──────────────────────────────────────────┼───────────────────────┤
│ EPC_Project_Ticket.html      │ Double-click or open in browser │ Priority Matrix, RACI, Gantt, CSV Export │ plannerProjects, etc. │
│ Vendor_Package_Register.html │ Double-click or open in browser │ Submittal tracking, ExcelJS .xlsx export │ vendorRegisterState   │
│ Digital_Signature.html       │ Double-click or open in browser │ 30 calligraphy styles, vector SVG, PNG   │ sigV2                 │
│ PDF_Annotation_Cleaner.html  │ Double-click or open in browser │ Purges stamps, annotations, sticky notes │ None (In-memory)      │
│ PDF_Merge_Rotate.html        │ Double-click or open in browser │ Offline pdf-lib/pdf.js merge & rotation  │ None (In-memory)      │
│ Linear_Interpolation.html    │ Double-click or open in browser │ Discrete table lookup & curve fit math   │ None (In-memory)      │
│ Case_Converter.html          │ Double-click or open in browser │ Tag casing, text stats, batch transforms │ None (In-memory)      │
└──────────────────────────────┴─────────────────────────────────┴──────────────────────────────────────────┴───────────────────────┘
```

### 💻 How to Run Locally

You do not need Node.js, Python, Docker, or any web server to run these tools:

1. **Clone or Download:**
   ```bash
   git clone https://github.com/akshayai1996/FUN_OFFICE_ARTIFACTS.git
   ```
2. **Launch:**
   - Double-click any `.html` file to open it in Chrome, Edge, Brave, Firefox, or Safari.
   - Or drag and drop the `.html` file directly into an open browser tab.
3. **Offline Use:**
   - Save the file to your desktop or an air-gapped machine and run it with your network disconnected.

---

## 📁 Repository Structure

```
FUN_OFFICE_ARTIFACTS/
├── EPC_Project_Ticket.html          # EPC ticket manager & Eisenhower RACI planner
├── Vendor_Package_Register.html     # Vendor submittal & document tracking dashboard
├── Digital_Signature.html           # Signature Studio V2 (hand-drawn + 30 styles)
├── PDF_Annotation_Cleaner.html      # PDF review comment & markup purge utility
├── PDF_Merge_Rotate.html            # Self-contained offline PDF merge & page rotate
├── Linear_Interpolation.html        # Engineering lookup & steam table interpolator
├── Case_Converter.html              # Multi-mode text & equipment tag case converter
├── LICENSE                          # MIT License
└── README.md                        # Comprehensive documentation
```

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for full details.

Free for personal, academic, and commercial engineering use with zero warranty.

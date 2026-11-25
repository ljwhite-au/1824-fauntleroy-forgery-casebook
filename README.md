# The Henry Fauntleroy Forgery Scandal (1824): Forensic Accounting Casebook

**Open Forensic Accounting & Internal Controls Lab** | *Custodial Embezzlement, Power-of-Attorney Forgery & Ghost-Dividend Cash Kiting at Marsh, Stracey, Fauntleroy & Graham (1814–1852)*

A complete, free, open-access forensic accounting reconstruction of the 1824 Berners Street bank collapse in London, built exclusively from pre-1923 public-domain Old Bailey transcripts (`t18241028-97`), Fairburn (1824), Bank of England archives (`1A95/4`), *The London Gazette*, Bleackley (1916), Hilton Price (1890), *Stone v. Marsh* (1827), and *Marsh v. Keating* (1834).

## What This Casebook Shows (Key Findings)

This forensic accounting lab reconstructs the September 1824 collapse of London private bank **Marsh, Stracey, Fauntleroy & Graham** (No. 6 Berners Street) from Old Bailey testimony (`t18241028-97`), Fauntleroy's **7 May 1816 Tin-Box Confession Schedule**, Bank of England archives, and 1825–1852 bankruptcy distributions to show why **partner override and missing third-party confirmations** make custodial embezzlement mathematically self-accelerating:

1. **The £188,187.80 Tin-Box Schedule & The £360,000 Bank of England Loss:** Cross-checking *The Proceedings of the Old Bailey* (`t18241028-97`), *Fairburn* (1824), and the 1846 Marsh-family transcript recovers all **16 verbatim accounts** signed *"Fauntleroy, Berners-street, May 7, 1816"*—summing to **£188,187 16s. 0d. (£188,187.80)**, exceeding the rounded *"above £170,000"* courtroom myth. Adding 6 verified post-1816 indictments and litigated claims (**£27,660.70**, including *Marsh v. Keating* £12,000 and Viscountess Nelson's April 1824 £6,425.70 POA) reaches **£215,848.50**, leaving **£144,151.50** in unscheduled 1816–1824 liquidations to match Bank of England Governor John Horsley Palmer's **£360,000** cumulative loss testimony (1832).
2. **Penny-Exact Test-Indictment Proof & The Ghost-Dividend Death Spiral:** On **1 June 1815**, Fauntleroy forged clerk John Watson's witness signature to liquidate **£5,000** of **Miss Frances Young**'s 3% Consols at **59⅛%** (£2,956.25 gross) less Marsh, Sibbald & Co.'s **50/50 split brokerage** (1/16% = £3 2s. 6d.), crediting exactly **£2,953 2s. 6d. (£2,953.125)** to `H. F.` via Messrs. Martin & Co. To hide the theft, Fauntleroy submitted a **dual dividend list** to the Bank of England (claiming only her remaining **£550** = **£8 5s. 0d.** red-checked warrant) while crediting her passbook for **£5,550** (**£83 5s. 0d.**). Across 18 half-years (Jan 1816–Jul 1824), Miss Young's **£75/half-year** phantom coupon drained **£1,350.00 (45.71% of 1815 cash)**, while the May 1816 portfolio drained **£55,559.64** off-ledger—and replacing Miss Young's Consols at **96¼%** on 22 Oct 1824 cost the Bank **£4,812.50 (+62.96% secular bond-rally squeeze)**.
3. **27-Year Bankruptcy Recovery & Vicarious Liability of Absentee Partners:** Alongside **£50,000** hidden across two pages of the locked *Partners' Private Ledger*, the partnership collapsed in September 1824; seven court-ordered dividends from 1825 to 1852 paid **11s. 2⅛d. in £1** (**£310,386.14** on **£558,686.25** peak proved debt, leaving **44.44% / £248,300.11** permanently lost). In ***Stone v. Marsh*** (1827) and ***Marsh v. Keating*** (1834), courts held the absentee innocent partners civilly liable once forged proceeds entered firm clearing accounts—establishing the direct ancestor of modern **ISA 240**, **ISA 501**, and **Client Money** custody rules.


---

## Repository Structure

```text
1824-fauntleroy-forgery-casebook/
├── README.md                                  # Overview, Key Findings, setup & legal notices
├── LICENSE-PROSE.txt                          # CC BY-NC-SA 4.0 (narrative, PDF, visuals & workbooks)
├── LICENSE-CODE.txt                           # MIT License (Python audit script, CSV & notebook code)
├── .gitignore                                 # Excludes OS and Python/Excel cache files
├── casebook.md                                # Complete 5-section forensic monograph & 3 lab exercises
├── 1824_Fauntleroy_Forgery_Casebook.pdf       # Standalone formatted PDF reading & seminar edition
├── instructor_debrief.md                      # 100-point grading rubric, pitfalls & 120-min seminar plan
├── Fauntleroy_1824_Forensic_Lab.ipynb         # Interactive Jupyter notebook (custody & kiting audit)
├── data/
│   ├── fauntleroy_forgeries_1824.csv          # 23 verified primary records (16 Tin-Box + 6 Post-1816 + 1 Control)
│   └── sources_index.md                       # Pre-1923 bibliography & textual variance log
├── src/
│   └── custody_gap_audit.py                   # Automated custody-gap, split-brokerage & kiting script
├── assets/
│   ├── fauntleroy_kiting_loop.svg             # Vector schematic: Forged POA -> Dual Lists -> 27-Yr Workout
│   ├── chart_1_tin_box_mix.png                # 300-DPI May 7, 1816 security mix & top-5 concentration
│   └── chart_2_ghost_dividend_and_bankruptcy.png # 300-DPI 18-cycle kiting drain & 1825–1852 dividends
└── workbook/
    ├── 1824_fauntleroy_challenge.xlsx         # 5-tab blank-input learner challenge workbook
    └── 1824_fauntleroy_solution_key.xlsx      # Worked 5-tab live-formula solution workbook + 3 charts
```

---

## Quick Start

1. **Run the MIT-licensed custody & ghost-dividend audit script:**
   ```bash
   python3 src/custody_gap_audit.py
   ```
2. **Explore in Jupyter:** Open `Fauntleroy_1824_Forensic_Lab.ipynb` to inspect all 23 primary records and reproduce the Frances Young brokerage and 18-cycle kiting checks.
3. **Complete or inspect the 5-tab Excel workbooks:**
   * Open `workbook/1824_fauntleroy_challenge.xlsx` to fill in the amber-shaded cells across Labs 1–3.
   * Open `workbook/1824_fauntleroy_solution_key.xlsx` in Excel, LibreOffice Calc, or Google Sheets to inspect all live formulas and 3 embedded charts.

---

## Licensing & Australian Legal Notices

### 1. Dual Open License
* **Prose, PDF, Diagrams & Workbook Layouts (`LICENSE-PROSE.txt`):** Licensed under **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)**. Free to read, share, teach from, and adapt non-commercially with attribution; third-party resale is prohibited.
* **Code & Structured CSV Data (`LICENSE-CODE.txt`):** Licensed under the **MIT License**.

### 2. Educational Purpose & Non-Advice Disclaimer
This casebook, its spreadsheets, and its Python script are **historical forensic accounting exercises prepared solely for educational, training, and academic research purposes**. Nothing in this repository constitutes legal, audit, tax, or financial advice.

### 3. Australian Consumer Law Qualification
To the maximum extent permitted by law (including Schedule 2 of the *Competition and Consumer Act 2010* (Cth) — the **Australian Consumer Law**), these materials are provided on an educational reference basis without warranty as to completeness for any specific purpose. Nothing in these notices excludes, restricts, or modifies any right or remedy conferred by the Australian Consumer Law that cannot lawfully be excluded.

### 4. Archival Transparency & Historical Clearance
Every figure derives exclusively from pre-1923 public-domain trial, Bank of England, parliamentary, and bankruptcy records. Four minor source print variances (e.g., *W. Reader* 3% vs. 5%, Lady Nelson £11,595 vs. £11,995, Hilton Price 12s. 6d. vs. Bleackley 11s. 2⅛d., and the Sept 1835 £24,271 2s. 11d. `[VERIFY ALIGNMENT]` line) are explicitly documented rather than smoothed away. All named historical figures died roughly two centuries ago, clearing defamation risk under s 10 of Victoria's *Defamation Act 2005*.

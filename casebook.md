# The Henry Fauntleroy Forgery Scandal (1824): Forensic Accounting Casebook

**Open Forensic Accounting & Internal Controls Lab** | *London (1814–1852)*
**Dual License:** Narrative prose, PDF, SVGs & workbook layouts under **CC BY-NC-SA 4.0**; Python code, CSV dataset & notebook under **MIT License**.

## What This Casebook Shows (Key Findings)

This forensic accounting lab reconstructs the September 1824 collapse of London private bank **Marsh, Stracey, Fauntleroy & Graham** (No. 6 Berners Street) from Old Bailey testimony (`t18241028-97`), Fauntleroy's **7 May 1816 Tin-Box Confession Schedule**, Bank of England archives, and 1825–1852 bankruptcy distributions to show why **partner override and missing third-party confirmations** make custodial embezzlement mathematically self-accelerating:

1. **The £188,187.80 Tin-Box Schedule & The £360,000 Bank of England Loss:** Cross-checking *The Proceedings of the Old Bailey* (`t18241028-97`), *Fairburn* (1824), and the 1846 Marsh-family transcript recovers all **16 verbatim accounts** signed *"Fauntleroy, Berners-street, May 7, 1816"*—summing to **£188,187 16s. 0d. (£188,187.80)**, exceeding the rounded *"above £170,000"* courtroom myth. Adding 6 verified post-1816 indictments and litigated claims (**£27,660.70**, including *Marsh v. Keating* £12,000 and Viscountess Nelson's April 1824 £6,425.70 POA) reaches **£215,848.50**, leaving **£144,151.50** in unscheduled 1816–1824 liquidations to match Bank of England Governor John Horsley Palmer's **£360,000** cumulative loss testimony (1832).
2. **Penny-Exact Test-Indictment Proof & The Ghost-Dividend Death Spiral:** On **1 June 1815**, Fauntleroy forged clerk John Watson's witness signature to liquidate **£5,000** of **Miss Frances Young**'s 3% Consols at **59⅛%** (£2,956.25 gross) less Marsh, Sibbald & Co.'s **50/50 split brokerage** (1/16% = £3 2s. 6d.), crediting exactly **£2,953 2s. 6d. (£2,953.125)** to `H. F.` via Messrs. Martin & Co. To hide the theft, Fauntleroy submitted a **dual dividend list** to the Bank of England (claiming only her remaining **£550** = **£8 5s. 0d.** red-checked warrant) while crediting her passbook for **£5,550** (**£83 5s. 0d.**). Across 18 half-years (Jan 1816–Jul 1824), Miss Young's **£75/half-year** phantom coupon drained **£1,350.00 (45.71% of 1815 cash)**, while the May 1816 portfolio drained **£55,559.64** off-ledger—and replacing Miss Young's Consols at **96¼%** on 22 Oct 1824 cost the Bank **£4,812.50 (+62.96% secular bond-rally squeeze)**.
3. **27-Year Bankruptcy Recovery & Vicarious Liability of Absentee Partners:** Alongside **£50,000** hidden across two pages of the locked *Partners' Private Ledger*, the partnership collapsed in September 1824; seven court-ordered dividends from 1825 to 1852 paid **11s. 2⅛d. in £1** (**£310,386.14** on **£558,686.25** peak proved debt, leaving **44.44% / £248,300.11** permanently lost). In ***Stone v. Marsh*** (1827) and ***Marsh v. Keating*** (1834), courts held the absentee innocent partners civilly liable once forged proceeds entered firm clearing accounts—establishing the direct ancestor of modern **ISA 240**, **ISA 501**, and **Client Money** custody rules.


---

## 1. Custody Architecture & The Berners Street Blind Spot (1792–1824)
Founded in 1792 at No. 6 Berners Street, West End private bank **Marsh, Sibbald & Co.** (later **Marsh, Stracey, Fauntleroy & Graham**) suffered a **£20,000** loss in 1794 and heavy builder-loan illiquidity after 1810. With senior partners **William Marsh** (residing in Kent), **Josias Henry Stracey**, and Colonel **George Edward Graham** largely absentee, managing partner **Henry Fauntleroy** (clerk 1800, partner 1807) held unchecked control over client Bank of England powers of attorney, clearing through City agents **Messrs. Martin & Co.**, and a locked **Partners' Private Ledger** (**£50,000** hidden across two pages, where clerk **James Tyson** testified Fauntleroy inserted lines beneath Graham's £40 entry).

---

## 2. Lab 1 — Forged vs. Genuine Consol Custody Audit
**Workbook Tab:** `1_BoE_Consol_Ledger_Audit` | **Data:** `data/fauntleroy_forgeries_1824.csv`
* **The 7 May 1816 Tin-Box Schedule:** All **16 verbatim lines** sum to **£188,187 16s. 0d. (£188,187.80)**—4% Annuities **£98,050.00** (led by **Lord Aboyne £61,550** = 32.71%), 3% Consols **£83,087.80** (led by **Peter Moore & John Marsh £21,500**), Navy 5% **£4,000.00**, and 5% Annuities **£3,050.00**. Adding 6 post-1816 verified claims (**£27,660.70**) yields **£215,848.50**, leaving **£144,151.50** in unscheduled 1816–1824 liquidations to reach Governor Palmer's **£360,000** gross Bank loss.
* **Frances Young Test-Indictment Proof (`t18241028-97`):** Passbook balance **£5,550.00** vs. genuine Bank register **£550.00** = **£5,000.00** forged on **1 June 1815** (sold to William Flower; clerk **John Watson**'s attestation forged; Bank clerk **Robert Browning, Jun.** witnessed *"I demand to act"*). Gross sale at **59⅛%** (**£2,956.25**) less standard ⅛% brokerage (**-£6.25**) plus Marsh, Sibbald & Co.'s **50/50 split** (**+£3.125**) equals exactly **£2,953.125 (£2,953 2s. 6d.)** credited to `H. F.`.

**Graded Exercise 1 (35 Points):** Complete `1_BoE_Consol_Ledger_Audit` custody gaps, annual coupons, POA classifications, and the 9-step Frances Young proof.

---

## 3. Lab 2 — The Ghost-Dividend & Cash-Kiting Waterfall (1816–1824)
**Workbook Tab:** `2_Dividend_Shortfall_Kiting` | **Script:** `src/custody_gap_audit.py`
* On the July 1824 Bank dividend claim list, Fauntleroy listed Miss Young for **£550** (red-checked by Bank clerks; **£8 5s. 0d.** warrant collected by William Marsh) while crediting her internal passbook for **£5,550** (**£83 5s. 0d.**).
* Across **18 half-years** (Jan 1816–Jul 1824), her **£75.00** semi-annual phantom gap burned **£1,350.00 (45.71% of 1815 cash)**. Across the full May 1816 portfolio (**17 Jan/Jul cycles** @ **£1,422.57** = £24,183.64 + **16 Apr/Oct cycles** @ **£1,961.00** = £31,376.00), off-ledger dividend servicing drained **£55,559.64** (with sensitivities for the *W. Reader* 5% vs. 3% print conflict of **+£1,190.00** and the 1822 Vansittart Navy 5%→4% conversion of **-£100.00**).

**Graded Exercise 2 (30 Points):** Complete `2_Dividend_Shortfall_Kiting` and verify via `python3 src/custody_gap_audit.py`.

---

## 4. Lab 3 — Partnership Insolvency, Restitution & Legal Precedents (1824–1852)
**Workbook Tabs:** `3_Partnership_Solvency_Bridge` & `4_Control_Crosswalk`
* **Arrest, Trial & Replacement Squeeze:** Arrested **10 September 1824**, Fauntleroy was convicted on **30 October 1824** (*"of Uttering only"*) and executed **30 November 1824**. On **22 October 1824**, Bank broker **Benjamin Cole** replaced Miss Young's £5,000 Consols at **96¼%** for **£4,812.50**—a **+£1,859.38 (+62.96%)** secular bond-rally loss.
* **Adjusting Entries & 27-Year Bankruptcy Waterfall:** Off-book restatements total **£465,559.64** (AJE-1 £360,000 BoE loss + AJE-2 £55,559.64 ghost dividends + AJE-3 £50,000 hidden private ledger). Seven court-ordered dividends (7 Feb 1825 – 5 Apr 1852) distributed **11s. 2⅛d. in £1** (**£310,386.14**) on **£558,686.25** peak proved claims, leaving **44.44% (£248,300.11)** permanently lost alongside the £95,000 Bank compromise + £11,000 costs.
* **Landmark Civil Rulings & Modern Crosswalk:** ***Stone v. Marsh*** (1827, 6 B. & C. 551) and ***Marsh v. Keating*** (1834, 2 Cl. & F. 250) established vicarious partner liability for forged proceeds entering firm clearing accounts—mapped to **ISA 240**, **ISA 501**, **SEC Rule 206(4)-2 / ASIC Client Money Rules**, **COSO SoD**, and **IFRS 9** in Tab `4_Control_Crosswalk`.

**Graded Exercise 3 (35 Points):** Complete `3_Partnership_Solvency_Bridge` AJEs and 7-tranche dividend waterfall, and review `4_Control_Crosswalk`.

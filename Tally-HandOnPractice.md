# 🧾 Tally — Hands-On Practice Repository
### *Complete Practice Exercises from Zero to Advanced — TallyPrime & Tally ERP 9*

> **"You learn Tally by doing entries, not by reading about them."**
> This repository contains 8 fully structured practice modules with a fictional company, real business scenarios, step-by-step entry instructions, expected outputs to verify, and common errors to watch for. Complete all modules in order and you will have the equivalent of 6 months of real bookkeeping experience.

---

## 📌 How to Use This Repository

Each module builds on the previous one — do them in order. Never skip ahead.

Before starting any module, read the scenario carefully. Understand what kind of business it is, what transactions are happening, and why. Understanding the context makes the entries intuitive rather than mechanical.

After completing each module, use the Verification Checklist at the end to confirm your Tally data is correct. If any check fails, find and fix the error before moving to the next module.

**The Practice Company:** Throughout all modules, you will build and maintain the complete accounts of a single fictional company — **Sunrise Traders** — a wholesale stationery and office supplies trading business based in Pune, Maharashtra.

**Tools Required:** TallyPrime (Educational Mode) or Tally ERP 9 (Educational Mode). Both are free.

---

## Module 1: Company Setup and Master Creation

**Estimated Time:** 2–3 hours
**Concepts Practiced:** Company creation, ledger creation, group selection, opening balances, stock item setup

---

### The Business

**Sunrise Traders** is a partnership firm dealing in wholesale stationery and office supplies. They buy from manufacturers and distributors and sell to retail shops, schools, and corporate offices.

Business Details:
- **Full Name:** Sunrise Traders
- **Address:** 45, Shivaji Nagar, Pune – 411005, Maharashtra
- **GSTIN:** 27AAECS1234F1Z5 (27 = Maharashtra state code)
- **PAN:** AAECS1234F
- **Financial Year:** April 1, 2024 to March 31, 2025
- **Books Beginning:** April 1, 2024
- **Partners:** Ramesh Sharma and Suresh Gupta

---

### Task 1.1: Create the Company

Open TallyPrime → Alt+K → Create Company.

Enter the following:
| Field | Value |
|-------|-------|
| Company Name | Sunrise Traders |
| Primary Mailing Name | Sunrise Traders |
| Address | 45, Shivaji Nagar, Pune |
| Country | India |
| State | Maharashtra |
| Pin Code | 411005 |
| Telephone | 020-25678901 |
| Email | sunrisetraders@email.com |
| Currency Symbol | ₹ |
| Maintain | Accounts with Inventory |
| Financial Year Beginning | 1-Apr-2024 |
| Books Beginning | 1-Apr-2024 |

Press Ctrl+A to save.

**Enable Features (F11):**
- Maintain Bill-wise Details: **Yes**
- Use Cost Centres: **No** (enable later in Module 7)
- Enable GST: **Yes**
  - GSTIN: 27AAECS1234F1Z5
  - Applicable From: 1-Apr-2024
  - Periodicity of GSTR 1: Monthly

---

### Task 1.2: Create Ledgers

Create each ledger below. Pay careful attention to the Group column — this is the most important field.

**Capital and Partner Accounts:**
| Ledger Name | Group | Opening Balance |
|-------------|-------|----------------|
| Ramesh Sharma – Capital | Capital Account | ₹5,00,000 Cr |
| Suresh Gupta – Capital | Capital Account | ₹5,00,000 Cr |
| Ramesh Sharma – Current A/c | Capital Account | ₹0 |
| Suresh Gupta – Current A/c | Capital Account | ₹0 |

**Bank and Cash Accounts:**
| Ledger Name | Group | Opening Balance |
|-------------|-------|----------------|
| Cash | Cash-in-Hand | ₹45,000 Dr |
| HDFC Bank – Current A/c | Bank Accounts | ₹3,85,000 Dr |
| SBI Bank – Current A/c | Bank Accounts | ₹1,20,000 Dr |

**Customer Ledgers (Sundry Debtors):**

For each customer, enable "Maintain Balances Bill-by-Bill: Yes" and set Default Credit Period as shown.

| Ledger Name | Group | GSTIN | State | Opening Balance | Credit Period |
|-------------|-------|-------|-------|----------------|---------------|
| Patel Book Depot | Sundry Debtors | 27BKZPP1234A1Z1 | Maharashtra | ₹28,500 Dr | 30 Days |
| Sharma Stationery House | Sundry Debtors | 27BKZPS1234B1Z2 | Maharashtra | ₹15,000 Dr | 30 Days |
| MK Office Solutions | Sundry Debtors | 29BKZPM1234C1Z3 | Karnataka | ₹42,000 Dr | 45 Days |
| Delhi Paper Mart | Sundry Debtors | 07BKZPD1234D1Z4 | Delhi | ₹0 | 30 Days |
| Bright Future School | Sundry Debtors | 27BKZPB1234E1Z5 | Maharashtra | ₹8,750 Dr | 60 Days |

**Supplier Ledgers (Sundry Creditors):**

| Ledger Name | Group | GSTIN | State | Opening Balance | Credit Period |
|-------------|-------|-------|-------|----------------|---------------|
| National Paper Mills | Sundry Creditors | 27BKZPN1234F1Z6 | Maharashtra | ₹65,000 Cr | 45 Days |
| Classmate Industries Ltd | Sundry Creditors | 06BKZPC1234G1Z7 | Haryana | ₹38,500 Cr | 30 Days |
| Luxor Writing Instruments | Sundry Creditors | 07BKZPL1234H1Z8 | Delhi | ₹22,000 Cr | 30 Days |
| Kores India Ltd | Sundry Creditors | 27BKZPK1234I1Z9 | Maharashtra | ₹0 | 45 Days |

**Income Ledgers:**
| Ledger Name | Group |
|-------------|-------|
| Sales – Local (Maharashtra) | Sales Accounts |
| Sales – Interstate | Sales Accounts |
| Discount Received | Indirect Income |
| Interest Received | Indirect Income |

**Expense Ledgers:**
| Ledger Name | Group |
|-------------|-------|
| Purchases – Local | Purchase Accounts |
| Purchases – Interstate | Purchase Accounts |
| Freight Inward | Direct Expenses |
| Packing Charges | Direct Expenses |
| Office Rent | Indirect Expenses |
| Electricity Charges | Indirect Expenses |
| Telephone & Internet | Indirect Expenses |
| Staff Salaries | Indirect Expenses |
| Office Expenses | Indirect Expenses |
| Bank Charges | Indirect Expenses |
| Conveyance | Indirect Expenses |
| Advertising | Indirect Expenses |
| Discount Allowed | Indirect Expenses |
| Depreciation | Indirect Expenses |
| Stationary & Printing | Indirect Expenses |

**Tax Ledgers (for GST):**
| Ledger Name | Group | Tax Type |
|-------------|-------|---------|
| CGST Input | Duties & Taxes | CGST |
| SGST Input | Duties & Taxes | SGST |
| IGST Input | Duties & Taxes | IGST |
| CGST Output | Duties & Taxes | CGST |
| SGST Output | Duties & Taxes | SGST |
| IGST Output | Duties & Taxes | IGST |

**Fixed Asset Ledgers:**
| Ledger Name | Group | Opening Balance |
|-------------|-------|----------------|
| Furniture & Fixtures | Fixed Assets | ₹85,000 Dr |
| Computer & Peripherals | Fixed Assets | ₹65,000 Dr |
| Office Equipment | Fixed Assets | ₹35,000 Dr |

**Loan Ledger:**
| Ledger Name | Group | Opening Balance |
|-------------|-------|----------------|
| HDFC Bank – Term Loan | Loans (Liability) | ₹2,00,000 Cr |

---

### Task 1.3: Create Stock Items

First, create Units of Measure:
Go to Inventory Info → Units of Measure → Create.
Create: **Pcs** (Pieces), **Box** (Boxes), **Ream** (Reams), **Doz** (Dozen), **Nos** (Numbers)
Create Compound Unit: **Box of 10 Nos** (1 Box = 10 Nos)

Create Stock Groups:
- Writing Instruments (under Primary)
- Paper Products (under Primary)
- Files and Folders (under Primary)
- Adhesives and Tapes (under Primary)

Create the following Stock Items:

| Stock Item | Stock Group | Unit | GST Rate | HSN Code | Opening Qty | Opening Rate |
|------------|------------|------|---------|---------|------------|-------------|
| Classmate Notebook 200 Pages | Paper Products | Nos | 12% | 4820 | 500 Nos | ₹45 each |
| A4 Copier Paper 75 GSM (Ream) | Paper Products | Ream | 12% | 4802 | 200 Reams | ₹280 each |
| Reynolds Pen Blue | Writing Instruments | Box | 12% | 9608 | 50 Box | ₹120 per box |
| Flair Pen Black | Writing Instruments | Box | 12% | 9608 | 30 Box | ₹110 per box |
| Camlin Pencil HB | Writing Instruments | Box | 12% | 9609 | 40 Box | ₹85 per box |
| Cello Tape 2 inch | Adhesives and Tapes | Nos | 18% | 3919 | 100 Nos | ₹35 each |
| Double Sided Tape | Adhesives and Tapes | Nos | 18% | 3919 | 60 Nos | ₹28 each |
| L-Shape Folder | Files and Folders | Nos | 12% | 3926 | 200 Nos | ₹18 each |
| Box File | Files and Folders | Nos | 12% | 3926 | 80 Nos | ₹95 each |
| Stapler Medium | Writing Instruments | Nos | 18% | 8305 | 25 Nos | ₹180 each |

---

### Module 1 Verification Checklist

After completing all tasks, verify the following:

Open the Trial Balance (Gateway → Display More Reports → Trial Balance or Ctrl+G → "Trial Balance"):

- [ ] Total of all opening Debit balances = Total of all opening Credit balances
- [ ] Sundry Debtors total = ₹94,250 (sum of all customer opening balances)
- [ ] Sundry Creditors total = ₹1,25,500 (sum of all supplier opening balances)
- [ ] Bank Accounts total = ₹5,05,000 (HDFC ₹3,85,000 + SBI ₹1,20,000)
- [ ] Cash balance = ₹45,000
- [ ] Capital Account total = ₹10,00,000
- [ ] Fixed Assets total = ₹1,85,000
- [ ] HDFC Term Loan = ₹2,00,000

Open Stock Summary (Gateway → Inventory Reports → Stock Summary):
- [ ] All 10 stock items appear with correct opening quantities and values

**Common Error to Check:** If the Trial Balance doesn't balance, the most likely cause is an opening balance entered on the wrong side (Dr instead of Cr or vice versa). Check each ledger individually.

---

## Module 2: Recording Basic Transactions — April 2024

**Estimated Time:** 3–4 hours
**Concepts Practiced:** Payment, Receipt, Contra, Journal vouchers — without GST complexity

---

### Background

April 1, 2024 marks the start of Sunrise Traders' new financial year. The opening balances from Module 1 are already in place. Now record the day-to-day transactions for the first two weeks of April.

---

### Transactions — April 2024 (Part 1: Non-Inventory)

Record each transaction carefully. Note the date, voucher type, and narration.

**April 1, 2024**

**Transaction 1:**
Paid office rent for April 2024 by HDFC Bank cheque no. 000101.
Amount: ₹18,000
Voucher Type: **Payment (F5)**
Dr: Office Rent ₹18,000
Cr: HDFC Bank – Current A/c ₹18,000
Narration: "Rent paid for April 2024, Cheque No. 000101"

**Transaction 2:**
Withdrew ₹20,000 cash from HDFC Bank for office petty cash.
Voucher Type: **Contra (F4)**
Dr: Cash ₹20,000
Cr: HDFC Bank – Current A/c ₹20,000
Narration: "Cash withdrawal from HDFC Bank for office expenses"

**April 2, 2024**

**Transaction 3:**
Received payment from Patel Book Depot against their opening balance of ₹28,500. They paid ₹28,000 by NEFT into HDFC Bank and claimed a discount of ₹500.
Voucher Type: **Receipt (F6)**

This is slightly complex — you need to record both the receipt AND the discount. Here is how:
Dr: HDFC Bank ₹28,000
Dr: Discount Allowed ₹500
Cr: Patel Book Depot ₹28,500

In Tally, when entering a Receipt voucher against Patel Book Depot, set the bill reference to their outstanding opening bill. Record the discount as a separate line.
Narration: "Payment received from Patel Book Depot, NEFT, discount ₹500"

**April 3, 2024**

**Transaction 4:**
Paid salary to office staff for March 2024 (previous month's salary due).
Amount: ₹35,000 by HDFC Bank NEFT.
Voucher Type: **Payment (F5)**
Dr: Staff Salaries ₹35,000
Cr: HDFC Bank ₹35,000
Narration: "Salary payment for March 2024"

**Transaction 5:**
Paid electricity bill for March 2024 in cash.
Amount: ₹2,850
Voucher Type: **Payment (F5)**
Dr: Electricity Charges ₹2,850
Cr: Cash ₹2,850
Narration: "MSEDCL electricity bill March 2024, receipt no. E0012345"

**April 5, 2024**

**Transaction 6:**
Received ₹15,000 from Sharma Stationery House against their full opening balance of ₹15,000. Paid by cheque deposited in HDFC Bank.
Voucher Type: **Receipt (F6)**
Dr: HDFC Bank ₹15,000
Cr: Sharma Stationery House ₹15,000
Narration: "Payment received from Sharma Stationery House, Cheque No. 445678"

**April 7, 2024**

**Transaction 7:**
Paid telephone and internet bill for April by bank transfer.
Amount: ₹3,200
Voucher Type: **Payment (F5)**
Dr: Telephone & Internet ₹3,200
Cr: HDFC Bank ₹3,200
Narration: "Airtel broadband and telephone bill April 2024"

**Transaction 8:**
Deposited ₹15,000 cash into HDFC Bank.
Voucher Type: **Contra (F4)**
Dr: HDFC Bank ₹15,000
Cr: Cash ₹15,000
Narration: "Cash deposited into HDFC Bank"

**April 9, 2024**

**Transaction 9:**
Paid ₹22,000 to Luxor Writing Instruments against their full opening balance by NEFT from SBI Bank.
Voucher Type: **Payment (F5)**
Dr: Luxor Writing Instruments ₹22,000
Cr: SBI Bank ₹22,000
Narration: "Payment to Luxor Writing Instruments, NEFT, UTR no. SBI123456"

**April 10, 2024**

**Transaction 10:**
Received a partial payment from MK Office Solutions (Karnataka) — ₹25,000 out of their ₹42,000 outstanding. Bank NEFT into HDFC Bank.
Voucher Type: **Receipt (F6)**
Dr: HDFC Bank ₹25,000
Cr: MK Office Solutions ₹25,000
Narration: "Part payment received from MK Office Solutions, NEFT"

**Transaction 11:**
Paid office miscellaneous expenses in cash — purchased stationery for internal use, ₹850.
Voucher Type: **Payment (F5)**
Dr: Stationary & Printing ₹850
Cr: Cash ₹850
Narration: "Office stationery purchased"

**April 12, 2024**

**Transaction 12:**
Partners decided to invest additional capital. Ramesh Sharma contributed ₹1,00,000 and Suresh Gupta contributed ₹1,00,000 into HDFC Bank.
Voucher Type: **Receipt (F6)** — Two separate entries or one with two debit lines.

Entry 1:
Dr: HDFC Bank ₹1,00,000
Cr: Ramesh Sharma – Capital ₹1,00,000
Narration: "Additional capital introduced by Ramesh Sharma"

Entry 2:
Dr: HDFC Bank ₹1,00,000
Cr: Suresh Gupta – Capital ₹1,00,000
Narration: "Additional capital introduced by Suresh Gupta"

**April 14, 2024**

**Transaction 13:**
Paid HDFC Bank loan EMI of ₹12,500 from HDFC Bank account. The EMI includes ₹10,000 principal repayment and ₹2,500 interest.

You need to split this into two ledgers in one payment voucher:
Dr: HDFC Bank – Term Loan ₹10,000 (reduces the loan liability)
Dr: Bank Interest (create this ledger under Indirect Expenses if not already created) ₹2,500
Cr: HDFC Bank – Current A/c ₹12,500
Narration: "HDFC Term Loan EMI April 2024, including ₹2,500 interest"

**April 15, 2024**

**Transaction 14:**
Received interest on SBI Bank Savings Account: ₹820. Auto-credited by bank.
Voucher Type: **Receipt (F6)**
Dr: SBI Bank ₹820
Cr: Interest Received ₹820
Narration: "Interest credited by SBI Bank, April 2024"

---

### Module 2 Verification Checklist

Open the Day Book for April 1–15, 2024. Verify all 14 transactions appear.

Check individual ledger balances:
- [ ] Cash balance = ₹45,000 + ₹20,000 – ₹2,850 – ₹15,000 – ₹850 = ₹46,300
- [ ] HDFC Bank balance = ₹3,85,000 – ₹18,000 – ₹20,000 + ₹28,000 – ₹35,000 + ₹15,000 – ₹3,200 + ₹15,000 – ₹12,500 + ₹1,00,000 + ₹1,00,000 = ₹5,54,300
- [ ] Patel Book Depot balance = ₹28,500 – ₹28,500 = ₹0
- [ ] Sharma Stationery House balance = ₹15,000 – ₹15,000 = ₹0
- [ ] MK Office Solutions balance = ₹42,000 – ₹25,000 = ₹17,000
- [ ] Luxor Writing Instruments balance = ₹22,000 – ₹22,000 = ₹0
- [ ] HDFC Term Loan balance = ₹2,00,000 – ₹10,000 = ₹1,90,000
- [ ] Staff Salaries in P&L = ₹35,000
- [ ] Office Rent in P&L = ₹18,000

---

## Module 3: Purchase and Sales with GST — April 2024

**Estimated Time:** 4–5 hours
**Concepts Practiced:** Purchase vouchers, Sales vouchers, GST (CGST/SGST/IGST), inventory update, bill-wise tracking

---

### Transactions — Purchases (April 2024)

**April 3, 2024 — Purchase from Local Supplier**

**Transaction P1:**
Purchased from National Paper Mills (Maharashtra — local supplier, intra-state).

| Item | Qty | Rate (before GST) | GST Rate |
|------|-----|------------------|---------|
| A4 Copier Paper 75 GSM (Ream) | 150 Reams | ₹260 per Ream | 12% |
| Classmate Notebook 200 Pages | 300 Nos | ₹38 per Nos | 12% |

Voucher Type: **Purchase (F9)**
Supplier: National Paper Mills
Bill Number: NPM/24-25/001 | Date: April 3, 2024

Calculate manually first to verify Tally's calculation:
A4 Paper: 150 × ₹260 = ₹39,000 + CGST 6% ₹2,340 + SGST 6% ₹2,340 = ₹43,680
Notebooks: 300 × ₹38 = ₹11,400 + CGST 6% ₹684 + SGST 6% ₹684 = ₹12,768
Total Invoice Value: ₹56,448

Tally automatically calculates and posts:
Dr: Purchases – Local ₹50,400 (taxable value total)
Dr: CGST Input ₹3,024
Dr: SGST Input ₹3,024
Cr: National Paper Mills ₹56,448
(Plus inventory: A4 Paper +150 Reams, Notebooks +300 Nos)

**April 6, 2024 — Purchase from Interstate Supplier**

**Transaction P2:**
Purchased from Classmate Industries Ltd (Haryana — interstate supplier).

| Item | Qty | Rate | GST Rate |
|------|-----|------|---------|
| Classmate Notebook 200 Pages | 500 Nos | ₹36 per Nos | 12% |
| Reynolds Pen Blue | 20 Box | ₹100 per Box | 12% |
| Flair Pen Black | 15 Box | ₹95 per Box | 12% |

Bill Number: CI/2024/0456 | Date: April 6, 2024

Calculate:
Notebooks: 500 × ₹36 = ₹18,000
Reynolds Pen: 20 × ₹100 = ₹2,000
Flair Pen: 15 × ₹95 = ₹1,425
Total taxable value = ₹21,425
IGST @ 12% = ₹2,571
Total Invoice Value = ₹23,996

Tally posts:
Dr: Purchases – Interstate ₹21,425
Dr: IGST Input ₹2,571
Cr: Classmate Industries Ltd ₹23,996

**April 8, 2024**

**Transaction P3:**
Purchased from Kores India Ltd (Maharashtra — local).

| Item | Qty | Rate | GST Rate |
|------|-----|------|---------|
| Cello Tape 2 inch | 50 Nos | ₹28 per Nos | 18% |
| Double Sided Tape | 30 Nos | ₹22 per Nos | 18% |
| Stapler Medium | 10 Nos | ₹150 per Nos | 18% |

Bill Number: KORES/2024/789 | Date: April 8, 2024

Calculate:
Cello Tape: 50 × ₹28 = ₹1,400
Double Sided Tape: 30 × ₹22 = ₹660
Stapler: 10 × ₹150 = ₹1,500
Total taxable = ₹3,560
CGST @ 9% = ₹320.40
SGST @ 9% = ₹320.40
Total = ₹4,200.80

Record this entry. Check that Tally rounds fractional amounts appropriately.

**April 10, 2024**

**Transaction P4:**
Paid freight charges to Shiv Transport for delivery of above purchases.
Amount: ₹1,800 cash (no GST — transporter under RCM, ignore RCM for this exercise).
Voucher Type: **Payment (F5)**
Dr: Freight Inward ₹1,800
Cr: Cash ₹1,800
Narration: "Freight charges for April purchases, Shiv Transport"

---

### Transactions — Sales (April 2024)

**April 4, 2024**

**Transaction S1:**
Sold to Sharma Stationery House (Maharashtra — local). Credit sale.

| Item | Qty | Rate (before GST) | GST Rate |
|------|-----|------------------|---------|
| A4 Copier Paper 75 GSM | 80 Reams | ₹340 per Ream | 12% |
| Classmate Notebook 200 Pages | 150 Nos | ₹55 per Nos | 12% |

Invoice Number: ST/24-25/001 | Date: April 4, 2024

Calculate:
A4 Paper: 80 × ₹340 = ₹27,200
Notebooks: 150 × ₹55 = ₹8,250
Taxable total = ₹35,450
CGST 6% = ₹2,127
SGST 6% = ₹2,127
Invoice Total = ₹39,704

Tally posts:
Dr: Sharma Stationery House ₹39,704
Cr: Sales – Local ₹35,450
Cr: CGST Output ₹2,127
Cr: SGST Output ₹2,127

**April 7, 2024**

**Transaction S2:**
Sold to MK Office Solutions (Karnataka — interstate). Credit sale.

| Item | Qty | Rate | GST Rate |
|------|-----|------|---------|
| Reynolds Pen Blue | 10 Box | ₹140 per Box | 12% |
| Flair Pen Black | 8 Box | ₹135 per Box | 12% |
| L-Shape Folder | 100 Nos | ₹24 per Nos | 12% |

Invoice Number: ST/24-25/002 | Date: April 7, 2024

Calculate:
Reynolds Pen: 10 × ₹140 = ₹1,400
Flair Pen: 8 × ₹135 = ₹1,080
Folders: 100 × ₹24 = ₹2,400
Taxable total = ₹4,880
IGST 12% = ₹585.60
Invoice Total = ₹5,465.60

**April 9, 2024**

**Transaction S3:**
Cash sale to a walk-in customer (unregistered, consumer).

| Item | Qty | Rate | GST Rate |
|------|-----|------|---------|
| Cello Tape 2 inch | 5 Nos | ₹45 per Nos | 18% |
| Classmate Notebook 200 Pages | 10 Nos | ₹60 per Nos | 12% |

Invoice: ST/24-25/003 | Date: April 9, 2024

For unregistered/consumer customers, you can use the ledger "Cash" as the party in the Sales voucher, or create a ledger "Cash Sales" under Sundry Debtors.

Calculate:
Cello Tape: 5 × ₹45 = ₹225, CGST+SGST 18% = ₹40.50
Notebooks: 10 × ₹60 = ₹600, CGST+SGST 12% = ₹72
Total received in cash = ₹937.50

Dr: Cash ₹937.50
Cr: Sales – Local ₹825
Cr: CGST Output ₹56.25 (blended, approximate)
Cr: SGST Output ₹56.25

**April 12, 2024**

**Transaction S4:**
Sold to Delhi Paper Mart (Delhi — interstate). Credit sale.

| Item | Qty | Rate | GST Rate |
|------|-----|------|---------|
| A4 Copier Paper 75 GSM | 50 Reams | ₹345 per Ream | 12% |
| Box File | 30 Nos | ₹125 per Nos | 12% |
| Stapler Medium | 5 Nos | ₹250 per Nos | 18% |

Invoice: ST/24-25/004 | Date: April 12, 2024

Calculate each line manually and verify against Tally's output. Note that the Stapler has 18% GST while the others have 12%.

**April 14, 2024**

**Transaction S5:**
Sold to Bright Future School (Maharashtra — local). They are an educational institution (check their GST registration status — registered).

| Item | Qty | Rate | GST Rate |
|------|-----|------|---------|
| Classmate Notebook 200 Pages | 200 Nos | ₹52 per Nos | 12% |
| Reynolds Pen Blue | 15 Box | ₹138 per Box | 12% |
| Camlin Pencil HB | 10 Box | ₹110 per Box | 12% |

Invoice: ST/24-25/005 | Date: April 14, 2024

---

### Module 3 Verification Checklist

After recording all purchases and sales, verify:

**Stock Summary:**
- [ ] A4 Copier Paper: 200 opening + 150 purchased – 80 sold – 50 sold = 220 Reams remaining
- [ ] Classmate Notebooks: 500 opening + 300 + 500 purchased – 150 – 10 – 200 sold = 940 Nos remaining
- [ ] Reynolds Pen: 50 opening + 20 purchased – 10 – 15 sold = 45 Box remaining
- [ ] Box File: 80 opening – 30 sold = 50 Nos remaining

**GST Report — GSTR-1 for April (partial):**
- [ ] Local (Maharashtra) sales appear under B2B section with CGST and SGST
- [ ] Interstate sales (Karnataka, Delhi) appear under B2B section with IGST
- [ ] Cash sale (consumer) appears under B2C section

**Supplier Outstanding:**
- [ ] National Paper Mills outstanding = ₹56,448 (new bill)
- [ ] Classmate Industries outstanding = ₹38,500 (opening) + ₹23,996 (new) = ₹62,496
- [ ] Kores India outstanding = ₹4,200.80 (new)

---

## Module 4: Purchase Returns, Sales Returns, and Month-End — April 2024

**Estimated Time:** 2 hours
**Concepts Practiced:** Debit notes (purchase returns), Credit notes (sales returns), completing a month

---

### Purchase Return

**April 17, 2024**

**Transaction PR1:**
Returned defective stock to Classmate Industries Ltd. 20 Notebooks from the April 6 purchase (Invoice CI/2024/0456) were found defective.

Rate was ₹36 per Nos. GST 12% IGST (interstate).

Taxable value: 20 × ₹36 = ₹720
IGST @ 12% = ₹86.40
Total debit note value = ₹806.40

Voucher Type: **Debit Note (Ctrl+F9)**
Supplier: Classmate Industries Ltd
Reference: CI/2024/0456

Dr: Classmate Industries Ltd ₹806.40
Cr: Purchases – Interstate ₹720 (or Purchase Returns – Interstate)
Cr: IGST Input ₹86.40

Inventory: Classmate Notebooks reduce by 20 Nos.

---

### Sales Return

**April 19, 2024**

**Transaction SR1:**
Sharma Stationery House returned 10 Reams of A4 Paper from Invoice ST/24-25/001. The paper was water-damaged during delivery.

Rate was ₹340 per Ream. GST 12% CGST+SGST (intra-state).

Taxable value: 10 × ₹340 = ₹3,400
CGST @ 6% = ₹204
SGST @ 6% = ₹204
Total credit note value = ₹3,808

Voucher Type: **Credit Note (Ctrl+F8)**
Customer: Sharma Stationery House
Reference: ST/24-25/001

Dr: Sales – Local ₹3,400 (or Sales Returns)
Dr: CGST Output ₹204
Dr: SGST Output ₹204
Cr: Sharma Stationery House ₹3,808

Inventory: A4 Paper increases by 10 Reams (returned to stock).

---

### Month-End Journal Entries

**April 30, 2024**

**Transaction J1 — Depreciation:**
Record depreciation for April 2024.
- Furniture & Fixtures: 10% p.a. → ₹85,000 × 10% / 12 months = ₹708.33 (round to ₹708)
- Computers: 40% p.a. → ₹65,000 × 40% / 12 = ₹2,166.67 (round to ₹2,167)
- Office Equipment: 15% p.a. → ₹35,000 × 15% / 12 = ₹437.50 (round to ₹438)

Voucher Type: **Journal (F7)**
Dr: Depreciation ₹3,313
Cr: Furniture & Fixtures ₹708
Cr: Computer & Peripherals ₹2,167
Cr: Office Equipment ₹438
Narration: "Depreciation for April 2024 @ SLM rates"

**Transaction J2 — Provision for Salaries:**
Salaries for April have not been paid yet (payment will be made in May).
Amount: ₹35,000

Voucher Type: **Journal (F7)**
Dr: Staff Salaries ₹35,000
Cr: Salaries Payable (create this ledger under Current Liabilities) ₹35,000
Narration: "Provision for salaries April 2024 — to be paid in May"

---

### Module 4 Verification Checklist

Check the following reports:

**Trial Balance as of April 30, 2024:**
- [ ] The trial balance must balance (Total Debit = Total Credit)

**Profit and Loss for April 1–30, 2024:**
- [ ] Sales (Local + Interstate) appears on income side
- [ ] Purchases appears on expense side
- [ ] Gross Profit = Sales – Purchases – Direct Expenses ± Stock Change
- [ ] All indirect expenses (Rent, Salaries provision, Electricity, Depreciation, etc.) appear
- [ ] Net Profit = Gross Profit – Indirect Expenses

**Balance Sheet as of April 30, 2024:**
- [ ] Total Assets = Total Liabilities + Capital
- [ ] Sundry Debtors shows all outstanding customer balances
- [ ] Sundry Creditors shows all outstanding supplier balances
- [ ] GST Output liabilities appear under Current Liabilities
- [ ] Reduced fixed asset values (after depreciation)

---

## Module 5: Bill-Wise Settlement and Aging Analysis

**Estimated Time:** 2 hours
**Concepts Practiced:** Bill-by-bill settlement, outstanding reports, aging analysis

---

### Background

Multiple invoices are outstanding. Record the following receipt and payment transactions, applying them against specific bills.

---

### Transactions — May 5–10, 2024

**May 5, 2024**

**Transaction 1:**
Sharma Stationery House makes a payment. They have:
- Invoice ST/24-25/001 outstanding: ₹39,704 – ₹3,808 (credit note) = ₹35,896

They pay ₹35,896 in full by NEFT into HDFC Bank.

Voucher Type: **Receipt (F6)**
Dr: HDFC Bank ₹35,896
Cr: Sharma Stationery House ₹35,896

When selecting Sharma Stationery House as the credit ledger, Tally will show the outstanding bills. Select ST/24-25/001 and apply the full amount against it. After this entry, Sharma Stationery House balance = ₹0.

**May 7, 2024**

**Transaction 2:**
Paid National Paper Mills the full amount of Invoice NPM/24-25/001 by HDFC NEFT.
Amount: ₹56,448

Voucher Type: **Payment (F5)**
Dr: National Paper Mills ₹56,448
Cr: HDFC Bank ₹56,448

Select the specific bill NPM/24-25/001 in the bill allocation. After this, National Paper Mills opening balance (₹65,000) is still outstanding — this payment only cleared the April invoice.

**May 9, 2024**

**Transaction 3:**
MK Office Solutions pays the remaining ₹17,000 of their opening balance plus ₹5,465.60 (Invoice ST/24-25/002) = Total: ₹22,465.60 by NEFT.

Voucher Type: **Receipt (F6)**
Dr: HDFC Bank ₹22,465.60
Cr: MK Office Solutions ₹22,465.60

Allocate: ₹17,000 against opening balance, ₹5,465.60 against ST/24-25/002.

---

### Generate and Analyze Outstanding Reports

After recording the above:

**Bills Receivable Report:**
Path: Gateway → Display More Reports → Statements of Accounts → Outstanding → Receivables

This shows every outstanding invoice for every customer. Look at:
- Which customers have invoices overdue beyond their credit period?
- What is the total outstanding amount?
- Which is the oldest outstanding invoice?

**Debtors Aging Analysis:**
Path: Gateway → Display More Reports → Statements of Accounts → Ageing Analysis → Receivables

Tally groups outstanding by age: 0–30 days, 31–60 days, 61–90 days, 90+ days.

Identify: Bright Future School's invoice from April 14 — is it within their 60-day credit period on May 9? Yes (26 days old). Delhi Paper Mart's April 12 invoice — they have a 30-day credit period, so by May 12 it becomes overdue.

**Exercise:** Write down which customers will have overdue invoices by May 15, 2024. Use the credit periods configured in their ledgers.

---

### Module 5 Verification Checklist

- [ ] Sharma Stationery House balance = ₹0 after May 5 receipt
- [ ] National Paper Mills opening balance ₹65,000 still outstanding (only the April invoice was paid)
- [ ] MK Office Solutions balance = ₹0 after May 9 receipt
- [ ] Bills Receivable report shows Delhi Paper Mart's April invoice and Bright Future School's April invoice as outstanding
- [ ] Aging analysis correctly categorizes all outstanding amounts by age

---

## Module 6: Full Month Simulation — May 2024

**Estimated Time:** 5–6 hours
**Concepts Practiced:** Complete month of operations — all voucher types, GST, inventory

---

### May 2024 Transactions

Record all of the following transactions. Dates and narrations are provided. The GST calculations and voucher types — determine them yourself based on what you have learned.

**May 1:** Paid April salary (provision from April 30 journal entry). ₹35,000 from HDFC Bank. Reverse the provision and record the actual payment.

Step 1 — Reverse the provision:
Journal: Dr Salaries Payable ₹35,000 / Cr Staff Salaries ₹35,000 (reversing the accrual)
Step 2 — Record payment:
Payment: Dr Staff Salaries ₹35,000 / Cr HDFC Bank ₹35,000

**May 1:** Paid May office rent ₹18,000 by HDFC cheque.

**May 3:** Purchased from National Paper Mills (local, 12% GST):
- A4 Copier Paper: 100 Reams @ ₹262 each
- Classmate Notebooks: 400 Nos @ ₹39 each
Bill no: NPM/24-25/015

**May 5:** Sold to Patel Book Depot (local, on credit):
- A4 Copier Paper: 60 Reams @ ₹342
- Classmate Notebooks: 100 Nos @ ₹57
Invoice: ST/24-25/012

**May 7:** Purchased from Kores India Ltd (local, 18% GST):
- Cello Tape 2 inch: 80 Nos @ ₹27
- L-Shape Folder: 200 Nos @ ₹15 (12% GST)
Bill no: KORES/2024/912

**May 9:** Cash sale to unregistered customer:
- Reynolds Pen Blue: 2 Box @ ₹145
- Flair Pen Black: 3 Box @ ₹140
- Cello Tape: 3 Nos @ ₹48

**May 12:** Received full payment from Bright Future School for April invoice. NEFT into HDFC Bank. ₹(calculate based on your April S5 entry).

**May 14:** Paid Classmate Industries Ltd ₹38,500 (opening balance). SBI Bank NEFT.

**May 15:** Sold to Delhi Paper Mart (interstate):
- Classmate Notebooks: 300 Nos @ ₹58
- Box File: 20 Nos @ ₹128
Invoice: ST/24-25/015

**May 16:** Delhi Paper Mart pays their April invoice (ST/24-25/004) in full. NEFT into HDFC Bank.

**May 18:** Received ₹5,000 from a new customer, Royal Stationery Mart (create ledger — Maharashtra, registered, credit period 30 days) as advance payment. HDFC Bank NEFT. Record as receipt against "Advance from Customer" — create this ledger under Current Liabilities.

**May 20:** Sold to Royal Stationery Mart (local) and adjusted the ₹5,000 advance:
- Camlin Pencil HB: 20 Box @ ₹112
- L-Shape Folder: 50 Nos @ ₹25
Invoice: ST/24-25/018 | Total = calculate. Adjust ₹5,000 advance, balance by credit.

**May 22:** Paid telephone bill ₹3,450 HDFC Bank.

**May 24:** Paid electricity ₹3,100 in cash.

**May 25:** Conveyance expenses paid in cash ₹650.

**May 26:** Returned 10 Reams of A4 Paper to National Paper Mills from May 3 purchase (damaged on delivery). Reference bill NPM/24-25/015.

**May 28:** Received 15 Notebooks returned by Patel Book Depot from ST/24-25/012 (slightly misprinted cover).

**May 29:** Advertising expense ₹4,500 paid by HDFC Bank (to a local printer for flyers).

**May 30:** Bank charges debited by HDFC Bank ₹350. Record as journal entry:
Dr: Bank Charges ₹350 / Cr: HDFC Bank ₹350

**May 31:** Depreciation for May (same as April: ₹3,313). Journal entry.

**May 31:** Salary provision for May: ₹35,000. Journal entry.

---

### Module 6 Verification Checklist

After completing all May entries:

- [ ] Day Book for May shows all transactions in chronological order
- [ ] Trial Balance balances
- [ ] Stock levels make sense (no negative stock on any item)
- [ ] All outstanding bills in the Bills Receivable report are within credit period (or identify which are overdue)
- [ ] GST Output ledgers have accumulated balances (total CGST/SGST/IGST collected on sales less returns)
- [ ] P&L for April–May shows two months of activity

---

## Module 7: Cost Centres and Budget Tracking

**Estimated Time:** 2–3 hours
**Concepts Practiced:** Cost centres, budgets, variance analysis

---

### Enabling Cost Centres

Gateway → F11 → Accounting Features → Maintain Cost Centres: **Yes**
Also enable: Use Pre-Defined Cost Centre Allocations in Transactions: Yes

### Creating Cost Centres

Create the following Cost Centres:
- **Administration** (under Primary)
- **Sales & Marketing** (under Primary)
- **Warehouse & Operations** (under Primary)

### Allocating Expenses to Cost Centres

From this point forward, when recording certain expense vouchers, Tally will prompt you to allocate the amount to a cost centre. Allocate as follows:
- Office Rent → 60% Administration, 40% Sales & Marketing
- Staff Salaries → Allocate based on department of the employee
- Electricity → 50% Administration, 50% Warehouse & Operations
- Advertising → 100% Sales & Marketing
- Conveyance → 70% Sales & Marketing, 30% Warehouse

Go back and add cost centre allocation to the May entries where possible.

### Creating Budgets

Gateway → Accounts Info → Budgets → Create.

Create a budget named "FY 2024-25 Annual Budget":
| Ledger | Annual Budget | Monthly Budget |
|--------|--------------|----------------|
| Sales – Local | ₹24,00,000 | ₹2,00,000 |
| Sales – Interstate | ₹12,00,000 | ₹1,00,000 |
| Staff Salaries | ₹4,20,000 | ₹35,000 |
| Office Rent | ₹2,16,000 | ₹18,000 |
| Electricity | ₹48,000 | ₹4,000 |
| Advertising | ₹1,20,000 | ₹10,000 |

### Viewing Budget vs Actual

Gateway → Display More Reports → Statements of Accounts → Budget Variance.

This report compares actual figures against budgeted. For April and May:
- Is actual Sales vs Budget on track?
- Which expenses are over budget?
- What does the variance tell the business owner?

Write a brief 5-sentence analysis of Sunrise Traders' performance against budget based on what you see.

---

## Module 8: Bank Reconciliation and GST Filing Preparation

**Estimated Time:** 2–3 hours
**Concepts Practiced:** Bank reconciliation, GST reports, preparing for filing

---

### Bank Reconciliation — May 2024

You have the following (fictional) HDFC Bank statement for May 2024. Compare it against your HDFC Bank ledger in Tally and perform a reconciliation.

**Fictional HDFC Bank Statement (May 2024 — partial):**
| Date | Description | Debit | Credit | Balance |
|------|------------|-------|--------|---------|
| May 1 | Salary NEFT | 35,000 | | |
| May 1 | Rent Cheque 000102 | 18,000 | | |
| May 3 | NEFT from MK Office Solutions | | 22,465.60 | |
| May 5 | NEFT from Sharma Stationery | | 35,896 | |
| May 7 | NEFT to National Paper Mills | 56,448 | | |
| May 12 | NEFT from Bright Future School | | (your figure) | |
| May 14 | NEFT to Classmate Industries | 38,500 | | |
| May 22 | Telephone NEFT | 3,450 | | |
| May 29 | Advertising NEFT | 4,500 | | |
| May 30 | Bank Charges | 350 | | |

**Notice:** May 16 Delhi Paper Mart NEFT is NOT in the bank statement (the bank will process it the next day — it was received on May 31 and credited on June 1).

Perform reconciliation in Tally:
Gateway → Banking → Bank Reconciliation → HDFC Bank – Current A/c

Mark each transaction that appears in both Tally AND the bank statement. The Delhi Paper Mart receipt will appear in Tally but not in the bank statement — this is your reconciling item.

The BRS should show:
- Balance as per Tally: ₹X
- Less: Cheques issued but not cleared: ₹0
- Add: Receipts in Tally not credited in bank: ₹(Delhi Paper Mart amount)
- Balance as per Bank Statement: ₹Y (should match Tally balance adjusted for the above)

---

### GST Filing Preparation

Generate the GSTR-1 report for April 2024:
Gateway → Display More Reports → Statutory Reports → GST → GSTR-1

Verify the following sections are correctly populated:
- [ ] **B2B (Business to Business):** All invoices to registered GST customers appear here with their GSTIN
- [ ] **B2C Large:** Any single invoice to an unregistered customer above ₹2.5 lakhs (interstate) — likely none for us
- [ ] **B2C Small:** Cash sales and small unregistered sales
- [ ] **CDNR (Credit/Debit Notes):** The credit note to Sharma Stationery House appears
- [ ] **HSN Summary:** All stock items grouped by HSN code with quantities and values

Generate GSTR-3B figures for April:
- Total Output Tax (CGST + SGST + IGST)
- Total Input Tax Credit (CGST Input + SGST Input + IGST Input)
- Net GST Payable = Output Tax – Input Tax Credit

**Exercise:** Calculate manually what GST Sunrise Traders owes to the government for April. Compare with Tally's GSTR-3B.

---

### Final Portfolio Exercise

After completing all 8 modules, generate and export the following reports for April and May 2024 combined:

1. Profit and Loss Account
2. Balance Sheet as of May 31, 2024
3. Trial Balance as of May 31, 2024
4. Stock Summary as of May 31, 2024
5. Debtors Aging Analysis
6. Creditors Outstanding
7. GSTR-1 for April (PDF)
8. Cost Centre-wise Expense Report

These 8 reports together represent a complete financial picture of Sunrise Traders for the period. A professional accountant presenting monthly MIS (Management Information System) reports to the business owner would present exactly these.

---

## 🔑 Master Reference: Keyboard Shortcuts

| Action | TallyPrime | Tally ERP 9 |
|--------|-----------|-------------|
| Go To (smart navigation) | Ctrl+G | Not available |
| Contra Voucher | F4 | F4 |
| Payment Voucher | F5 | F5 |
| Receipt Voucher | F6 | F6 |
| Journal Voucher | F7 | F7 |
| Sales Voucher | F8 | F8 |
| Purchase Voucher | F9 | F9 |
| Credit Note | Ctrl+F8 | Ctrl+F8 |
| Debit Note | Ctrl+F9 | Ctrl+F9 |
| Change Date | F2 | F2 |
| Change Period | Alt+F2 | Alt+F2 |
| Accept/Save | Ctrl+A or Enter | Ctrl+A |
| Cancel/Go Back | Escape | Escape |
| Create Master on the Fly | Alt+C | Alt+C |
| Company Features | F11 | F11 |
| Configuration | F12 | F12 |
| Backup | Alt+F3 → Backup | F3 → Backup |
| Switch Company | F3 | F3 |
| Delete Voucher | Alt+D | Alt+D |
| Alter Voucher | Enter on the voucher | Enter on the voucher |
| Print | Alt+P | Alt+P |
| Export | Alt+E | Alt+E |
| Day Book | Ctrl+G → "Day Book" | Gateway → Day Book |
| Balance Sheet | Ctrl+G → "Balance Sheet" | Gateway → Balance Sheet |
| Profit & Loss | Ctrl+G → "P&L" | Gateway → P&L |
| Trial Balance | Ctrl+G → "Trial Balance" | Gateway → Trial Balance |
| Stock Summary | Ctrl+G → "Stock Summary" | Gateway → Stock Summary |

---

## 🗂️ Opening Balance Quick Reference

When entering opening balances, remember:

| Account Type | Opening Balance Side |
|-------------|---------------------|
| Customer (Debtor) | **Debit** |
| Supplier (Creditor) | **Credit** |
| Bank Account | **Debit** |
| Cash | **Debit** |
| Capital | **Credit** |
| Loans Taken | **Credit** |
| Loans Given | **Debit** |
| Fixed Assets | **Debit** |
| Stock/Inventory | **Debit** |
| Outstanding Expenses (Payable) | **Credit** |
| Prepaid Expenses | **Debit** |
| Income Received in Advance | **Credit** |

---

## ❌ Common Entry Errors and How to Fix Them

**Error 1: Wrong amount entered.**
Open the Day Book → find the voucher → press Enter to open → correct the amount → Ctrl+A to save.

**Error 2: Wrong ledger selected.**
Same as above — open the voucher, change the ledger.

**Error 3: Entered in wrong financial year.**
The voucher date was typed incorrectly — e.g., typed 2023 instead of 2024. Open the voucher, press F2 to change the date, correct it, save.

**Error 4: Used wrong voucher type (e.g., used Journal instead of Payment).**
You cannot change a voucher's type after creation. Delete the incorrect voucher (Alt+D) and re-enter it with the correct voucher type.

**Error 5: Forgot to apply GST.**
If a purchase or sales entry was saved without GST lines, open the voucher, scroll to the tax section, add the GST ledgers and amounts, save.

**Error 6: Bill-wise details not matching.**
If you applied a receipt to the wrong bill, open the receipt voucher, go to the bill allocation section, and re-allocate to the correct bill.

**Error 7: Negative stock.**
Tally allows negative stock in Educational Mode. If you see negative stock, it means you sold more than you had — check if a purchase entry was missed or if the opening stock was entered incorrectly.

---

## 📊 Self-Assessment: Are You Ready?

After completing all 8 modules, test yourself with these questions. If you can answer all of them confidently, you have genuine Tally proficiency.

1. A customer returns ₹5,000 of goods from a previous invoice. What voucher type do you use? What are the debit and credit entries?

2. You need to record interest charged by the bank — no cash moves, it is simply debited from your account. What do you see in the bank statement and how do you record it in Tally?

3. What is the difference between a Contra voucher and a Journal voucher? Give an example of each.

4. A customer pays ₹48,000 against an invoice of ₹50,000 and takes a ₹2,000 discount. How do you record this receipt?

5. You bought goods worth ₹1,00,000 from a supplier in another state. GST rate is 18%. What is the total invoice amount? Which GST ledgers are debited?

6. Your Trial Balance is not balancing — debits are ₹500 more than credits. What are three possible causes and how do you find the error?

7. A stock item shows negative balance in the Stock Summary. What does this mean and how do you fix it?

8. What is the difference between CGST+SGST and IGST? When does each apply?

9. How do you record salary that is due but not yet paid at month-end?

10. You want to know which customers have invoices overdue for more than 45 days. Which report do you use and where do you find it in Tally?

---

*Document Version 1.0 | Created for GitHub Repository | February 2026*
*Practice company "Sunrise Traders" is entirely fictional. All data is for educational purposes only.*
*Complete all 8 modules in order for maximum learning effectiveness.*

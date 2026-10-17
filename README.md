# NgernKob: an income and expense tracker for Thai users

One file · runs in your browser · works offline · your data stays on your own device (localStorage). No server and no sign-up.

**How to use:** double-click `NgernKob.html` to open it in your browser. The app starts in Thai; click **EN** at the top right to switch to English. To try it out, go to ⚙️ **Settings** → **✨ Load sample data**, then use **🗑 Erase everything** before you start recording your own money.

---

## Features

| # | Feature | Details |
|---|---------|---------|
| 1 | Record income, expenses and transfers | A floating ＋ button, a large amount keypad, and icon categories you pick with one tap |
| 2 | Thai-style categories | Food & drink (rice-and-curry shops) · Convenience store · Coffee & tea · Transport (BTS, MRT, motorbike taxis) · Utilities · Merit & donation · Family support · Lottery · Car payment |
| 3 | Buddhist Era calendar | Full and short Thai month names, fixed-date public holidays in red, and a heat map of daily spending |
| 4 | Multiple wallets | 12 Thai banks plus TrueMoney, Paotang, ShopeePay, LINE Pay, cash and credit cards (with credit limit and payment due date) |
| 5 | Slip and PromptPay QR reader | Upload a slip image or scan it with the camera. The app decodes the EMVCo TLV payload, checks the CRC-16, picks out the PromptPay phone number, national ID or e-wallet ID, and reads the slip-verification mini QR (sending bank and reference number). You can also paste the slip text. It then guesses the category for you |
| 6 | Personal income tax calculator | Progressive brackets from 0% to 35%, the 50% expense deduction (up to 100,000 baht), 23 allowances with their limits, and the combined caps: retirement funds 500,000 in total, life and health insurance 100,000, donations up to 10%. Amounts over a cap are trimmed automatically, with a warning |
| 7 | Deductions tagged on real transactions | Tick 🧾 when you record an expense (Easy E-Receipt, insurance premiums, SSF/RMF/Thai ESG, donations) and the amount flows into the tax page by itself |
| 8 | Tax-saving tips | Shows how much more you can still put into tax-saving funds, and roughly how many baht that would save at your tax rate |
| 9 | Government benefits and social security | Half-Half co-pay · Domestic travel co-pay · State welfare card · SSO sections 33, 39 and 40 · Universal healthcare. Set the limit for each entitlement, and the app counts what you have used from transactions tagged 🏛️ |
| 10 | Budgets and the 50/30/20 rule | Set a budget per category, see warning bars as you near the limit, and get a **Safe to spend / day** figure for the rest of the month |
| 11 | Savings goals | Set a target and a deadline, and the app tells you how much to save each month |
| 12 | Bills and instalments | Electricity, rent, car payments and credit cards, sorted by due date. The **Paid** button records the payment straight away |
| 13 | Annual report | A 12-month chart, spending by category, savings rate, and CSV export (UTF-8 with BOM, so Thai text shows correctly in Excel) |
| 14 | Thai/English and dark mode | Switch the whole app's language in one click |
| 15 | Backup and restore | A full backup of all your data as one JSON file |

## A note on tax

Allowance figures follow the rules for tax years 2568/2569 BE (2025/2026): personal 60,000 · spouse 60,000 · children 30,000 to 60,000 · parents 30,000 each · social security 9,000 · life insurance 100,000 · own health insurance 25,000 · parents' health insurance 15,000 · annuity life insurance 200,000 · SSF 200,000 · RMF 500,000 · Thai ESG/ESGX 300,000 · home loan interest 100,000 · Easy E-Receipt 50,000 (all in baht). Limits and schemes change every year, so every field can be edited, and you should confirm the figures with the Revenue Department (rd.go.th) before you file. The app is a planning tool, not tax advice.

## Known limitations

- Lunar holidays (Makha Bucha, Visakha Bucha, Khao Phansa) fall on different dates each year, so they are not included yet.
- Automatic bank account syncing is not possible from a single HTML file (it needs a backend and open banking), so the app reads slips and QR codes instead.
- Verifying slips against a bank's API needs a merchant key held on a server. This app only reads and decodes slips on your device.

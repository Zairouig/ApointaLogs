# Release Notes

---

# 🇸🇰 Apointa v1.16 — Slovenčina

> **Dátum vydania:** 6. mája 2026
> **Verzia:** `v1.16.0`

---

## 🧾 Fakturačný systém — kompletný remake

### ✨ Nové funkcie

- **Nový formulár faktúry** sekcie: Faktúra → Nastavenie → Dodávateľ → Odberateľ → Položky
- **Dynamické položky faktúry** — neobmedzený počet riadkov, každý s vlastnou:
  - _Jednotkovou cenou_, _množstvom_, _mernou jednotkou_
  - _Sadzbou DPH_ (0 % / 5 % / 10 % / 19 % / 20 % / 23 % / vlastná)
  - _Prepínačom s DPH / bez DPH_ — automatický prepočet základu a DPH
  - _Zľavou na položku_ v %
  - _Duplikovaním_ riadku jedným kliknutím
- **Quick select zo služieb** — pridaj existujúce služby a add-ony priamo do faktúry jedným kliknutím
- **QR kód — Pay by Square** — slovenský štandard pre platbu mobilným bankingom, generuje sa automaticky pri bankovom prevode
- **Logo a pečiatka** — nahranie obrázka do PDF faktúry
- **Dve šablóny PDF** — _Moderný_ (farebný header) a _Jednoduchý_ (čistý minimalistický)
- **Farba faktúry** — 4 predvolené farby + vlastná HEX hodnota, živý náhľad šablóny
- **Séria číslovania** — vlastná šablóna napr. `{rok}{mesiac}{cislo}` → `2026050001`
- **Všetky typy faktúr** — Faktúra bez DPH, Faktúra s DPH, Zálohová, Proforma, Dobropis, Prenesená daňová povinnosť
- **Symboly platby** — Variabilný, Konštantný, Špecifický symbol, Evidenčné číslo
- **Forma úhrady** — Bankový prevod, Hotovosť, Karta, PayPal, Dobierka, Vzájomný zápočet, Registračná pokladnica
- **Zaokrúhľovanie** — Žiadne / 10 centov / 50 centov / Celé čísla
- **Zľava na celú faktúru** — percentuálna zľava aplikovaná na celkový súčet
- **Poznámka k faktúre** — voliteľný text zobrazený v PDF
- **Vystavil** — meno osoby zobrazené v pätičke

### 📋 Zoznam faktúr

- Nová stránka `/dashboard/appky/invoices` — história všetkých vystavených faktúr
- Stiahnuť PDF, zmazať faktúru
- Sumár celkovej sumy všetkých faktúr

### 🔗 Prefill z rezervácie

- Tlačidlo **"Vystaviť faktúru"** priamo v zozname rezervácií
- Automaticky predvyplní: meno zákazníka, email, telefón, názov služby, cenu a menu

### 🔒 Feature Gate

- Fakturácia je dostupná od plánu **Starter** a vyššie
- Free tier vidí upgrade screen s prehľadom funkcií plánu

### 🌍 Lokalizácia

- Kompletné translation keys pre **SK, CS, EN, DE, UK**
- PDF faktúra podporuje všetkých 5 jazykov

---

## 📊 Pokročilé štatistiky — feature gate

- Štatistiky uzamknuté pre Free a Starter plán
- Prístup od **Growth** plánu a vyššie

---

## 🛠 Opravy a vylepšenia

---

# 🇬🇧 Apointa v1.16 — English

> **Release date:** May 6, 2026
> **Version:** `v1.16.0`

---

## 🧾 Invoicing System — Complete Rebuild

### ✨ New Features

- **New invoice form**sections: Invoice → Settings → Supplier → Customer → Line Items
- **Dynamic line items** — unlimited rows, each with:
  - _Unit price_, _quantity_, _unit of measure_
  - _VAT rate_ (0% / 5% / 10% / 19% / 20% / 23% / custom)
  - _VAT inclusive / exclusive toggle_ — automatic base and VAT recalculation
  - _Per-item discount_ in %
  - _One-click row duplication_
- **Quick select from services** — add existing services and add-ons directly to the invoice with one click
- **QR code — Pay by Square** — Slovak mobile banking payment standard, auto-generated for bank transfer invoices
- **Logo and stamp** — upload images embedded in the PDF invoice
- **Two PDF templates** — _Modern_ (colored header) and _Simple_ (clean minimalist)
- **Invoice color** — 4 preset colors + custom HEX value, live template preview
- **Numbering series** — custom template e.g. `{rok}{mesiac}{cislo}` → `2026050001`
- **All invoice types** — Invoice without VAT, Invoice with VAT, Advance, Proforma, Credit Note, Reverse Charge
- **Payment symbols** — Variable, Constant, Specific symbol, Reference number
- **Payment method** — Bank transfer, Cash, Card, PayPal, COD, Mutual offset, POS terminal
- **Rounding** — None / 10 cents / 50 cents / Whole numbers
- **Global invoice discount** — percentage discount applied to the total
- **Invoice note** — optional text displayed in the PDF
- **Issued by** — person's name shown in the footer

### 📋 Invoice List

- New page `/dashboard/appky/invoices` — history of all issued invoices
- Download PDF, delete invoice
- Total amount summary across all invoices

### 🔗 Booking Prefill

- **"Create invoice"** button directly in the booking list
- Automatically prefills: customer name, email, phone, service name, price and currency

### 🔒 Feature Gate

- Invoicing is available from the **Starter** plan and above
- Free tier sees an upgrade screen with plan feature overview

### 🌍 Localization

- Complete translation keys for **SK, CS, EN, DE, UK**
- PDF invoice supports all 5 languages

---

## 📊 Advanced Analytics — Feature Gate

- Analytics locked for Free and Starter plans
- Access from **Growth** plan and above

---

## 🛠 Bug Fixes & Improvements

---

*Apointa v1.16 — Built with ❤️ in Slovakia*

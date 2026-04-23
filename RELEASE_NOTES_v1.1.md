# Apointa v1.1 — Release Notes

**Dátum vydania / Release date:** 23. apríl 2026

---

## 🔐 PIN ochrana pre Gift Cards a Produkty / PIN Protection for Gift Cards & Products

Zákazník zadáva bezpečnostný PIN pri kúpe. Provider ho overuje pri uplatnení alebo vydaní objednávky. PIN sa ukladá ako bcrypt hash — nikdy v plaintext.

Customers set a security PIN during purchase. Providers verify it during redemption or order pickup. PINs are stored as bcrypt hashes — never in plaintext.

- Povinný PIN field pri kúpe gift card a produktu / Mandatory PIN field on gift card and product purchase
- PIN doručený zákazníkovi emailom v plaintext / PIN delivered to customer via email in plaintext
- Dashboard: modal pre overenie PIN pri redemption a prevzatí / Dashboard: PIN verification modal on redemption and pickup
- Možnosť obísť overenie s auditným logom (redeemed_without_pin / picked_up_without_pin) / Option to bypass verification with audit log
- Zaznamenanie worker_id pri každej akcii / Worker ID logged on every action

---

## 🎫 Google Wallet — Loyalty karta na Success page / Google Wallet Loyalty Card on Success Page

Po dokončení rezervácie sa zobrazí tlačidlo "Add to Google Wallet" ak zákazník má loyalty kartu pre danú prevádzku.

After completing a booking, an "Add to Google Wallet" button appears if the customer has a loyalty card for that location.

- Automatické vytvorenie Google Wallet objektu ak neexistuje / Auto-creation of Google Wallet object if missing
- Uloženie google_wallet_object_id do DB po vytvorení / Saves google_wallet_object_id to DB after creation
- Button sa zobrazí len ak karta existuje / Button only shown if loyalty card exists

---

## 🐛 Opravy / Bug Fixes

- Opravený join `locations → customization_settings` na Gift Card success page / Fixed `locations → customization_settings` join on Gift Card success page
- Odstránený nesprávny join cez `profiles` / Removed incorrect join via `profiles`
- Vyčistené debug logy z production kódu / Cleaned up debug logs from production code

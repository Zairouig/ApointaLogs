**SK:**

---

**## v1.13 — Google Wallet, Expiration Reminders & Informational Webs**

**Vydané:** 30. apríla 2026

---

**### 🎫 Google Wallet — Loyalty Card Redesign**
Vernostná karta v Google Wallet bola kompletne prepísaná z `LoyaltyObject` na `GenericObject` pre lepší layout a kontrolu nad dizajnom. Karta teraz zobrazuje:
- Meno zákazníka, prevádzku a tier (Silver / Gold ✦ / Diamond ✦✦)
- QR kód s čitateľným alternateText
- Čierne pozadie, čistý minimalistický štýl
- Logo prevádzky uploadovateľné priamo z loyalty settings

Upload rozhranie pre logo loyalty karty pridané do dashboard → Eshop → Vernostný program.

> ⚠️ **Poznámka:** Plný redesign tier vizuálov (Silver/Gold/Diamond hero image) a level-up animácie prídu v ďalšej verzii. Testovanie API momentálne neumožňuje pokročilejšie úpravy. Riešiť sa bude naraz s Apple Developer účtom pre Apple Wallet a Apple Calendar integráciu.

---

**### ⚠️ Expiration Smart Reminders**
Nová Supabase Edge Function `send-grace-reminders` beží každý deň o 8:00 UTC a posiela inteligentné pripomienky pri neúspešnej platbe:
- **Deň 2** (5 dní do konca): "Platba stále neprešla — nestráť prístup k PRO funkciám"
- **Deň 5** (2 dni do konca): urgentná pripomienka
- **Deň 6** (1 deň do konca): posledná šanca

Emaily sú plne lokalizované (SK/EN/CS/DE/UK) a obsahujú správny branding. In-app notifikácia sa zobrazí súčasne s emailom.

Email template `payment-failed.tsx` prepísaný do štýlu ostatných provider emailov — logo, detailsBox, dynamická farba urgentnosti.

---

**### 🌐 Informational Webs**
Pridané dve nové verejné stránky:

**`/customers`** — vysvetlenie zákazníckeho portálu:
- Čo môže zákazník robiť (správa rezervácií, história, loyalty, darčekové poukážky)
- Mockup zákazníckeho portálu `/my-reservations`
- Sekcia pre Apointa poskytovateľov — čo im zákaznícky portál prináša (–40% no-show, 3× retencia, +28% opakovaných rezervácií)

**`/how-it-works`** — 3-krokový flow pre obe strany:
- Pre prevádzky: Nastaviť → Zdieľať link → Rásť s dátami
- Pre zákazníkov: Nájsť prevádzku → Rezervovať → Dostávať pripomienky

Obe stránky plne i18n (SK/EN/CS/DE/UK), rovnaký dizajn štýl ako landing page.

**`/for/[vertical]`** — cenník sekcia aktualizovaná na FREE / STARTER 9.99€ / GROWTH 24.99€. Navbar rozšírený o linky "Ako to funguje" a "Pre zákazníkov".

---

**EN:**

---

**## v1.13 — Google Wallet, Expiration Reminders & Informational Webs**

**Released:** April 30, 2026

---

**### 🎫 Google Wallet — Loyalty Card Redesign**
The loyalty card in Google Wallet was completely rewritten from `LoyaltyObject` to `GenericObject` for better layout control. The card now displays:
- Customer name, business name and tier (Silver / Gold ✦ / Diamond ✦✦)
- QR code with readable alternateText
- Black background, clean minimalist style
- Business logo uploadable directly from loyalty settings

Logo upload UI added to Dashboard → Eshop → Loyalty Program.

> ⚠️ **Note:** Full tier visual redesign (Silver/Gold/Diamond hero images) and level-up animations are coming in a future version. The current testing environment does not allow more advanced customizations. This will be handled together with the Apple Developer account for Apple Wallet and Apple Calendar integration.

---

**### ⚠️ Expiration Smart Reminders**
New Supabase Edge Function `send-grace-reminders` runs daily at 8:00 UTC and sends intelligent reminders on failed payment:
- **Day 2** (5 days left): "Payment still failed — don't lose access to PRO features"
- **Day 5** (2 days left): urgent reminder
- **Day 6** (1 day left): last chance

Emails are fully localized (SK/EN/CS/DE/UK) with proper branding. In-app notification fires simultaneously with the email.

`payment-failed.tsx` email template rewritten to match other provider email styles — logo, detailsBox, dynamic urgency color.

---

**### 🌐 Informational Webs**
Two new public pages added:

**`/customers`** — customer portal explanation:
- What customers can do (manage bookings, history, loyalty, gift cards)
- `/my-reservations` portal mockup
- Section for Apointa providers — what the customer portal brings them (–40% no-show, 3× retention, +28% repeat bookings)

**`/how-it-works`** — 3-step flow for both sides:
- For providers: Set up → Share link → Grow with data
- For customers: Find a business → Book → Get reminders

Both pages fully i18n (SK/EN/CS/DE/UK), matching landing page design style.

**`/for/[vertical]`** — pricing section updated to FREE / STARTER 9.99€ / GROWTH 24.99€. Navbar extended with "How it works" and "For customers" links.

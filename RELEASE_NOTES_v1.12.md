**SK:**

---

**## v1.12 — Brandované emaily, SMS kredity & Expiration flow**

**Vydané:** 29. apríla 2026

---

**### 🎨 Brandovaný odosielateľ emailov**
Všetky emaily zákazníkom teraz odchádzajú od nakonfigurovaného odosielateľa prevádzky (napr. `Hanicka <recipesquad@apointa.sk>`) namiesto predvoleného Apointa sendera. Platí pre potvrdenia rezervácií, pripomienky, zrušenia, darčekové poukážky, eshop objednávky a waiting list emaily. Ak odosielateľ nie je nakonfigurovaný, použije sa `Apointa <noreply@apointa.sk>`.

---

**### 💬 SMS kredity — opakované dopĺňanie**
SMS kredity sa teraz automaticky pridávajú pri každej obnove fakturačného cyklu:
- Starter mesačne: +10 kreditov
- Starter ročne: +120 kreditov
- Growth mesačne: +25 kreditov
- Growth ročne: +300 kreditov

Kredity sa pridávajú aj pri novom predplatnom cez `customer.subscription.created`.

---

**### 📅 Kalendár — zobrazenie mena workera**
Sloty v kalendári teraz zobrazujú meno priradeného pracovníka namiesto mena zákazníka. Ak nie je priradený žiadny pracovník, zobrazí sa meno zákazníka.

---

**### ⚠️ Expiration flow pri neúspešnej platbe**
Kompletný grace period flow pre zlyhané platby:
- Webhook `invoice.payment_failed` nastaví účet na `past_due` + aktivuje 7-dňovú grace period
- Dashboard banner s odpočtom a progress barom počas grace periody
- Deň 7: Edge Function `process-expired-subscriptions` (pg_cron, beží každý deň o 3:00 UTC) downgraduje účet na Free, zruší Stripe subscription, pošle email + in-app notifikáciu

---

**### 🐛 Opravy chýb**
- Opravený handler `invoice.paid` pre nový formát Stripe API `2026-02-25.clover` — subscription ID sa teraz správne číta z `invoice.parent.subscription_details.subscription`
- Opravený `revalidatePath` v `waitingListActions.ts` spôsobujúci chybu počas renderu na stránke kalendára
- Opravený chýbajúci prop `staffName` a prekladový kľúč pre subject v `booking-cancelled-by-provider-customer`

---

**EN:**

---

**## v1.12 — Branded Emails, SMS Credits & Expiration Flow**

**Released:** April 29, 2026

---

**### 🎨 Branded Email Sender**
All customer-facing emails now use the provider's configured sender name and email prefix (e.g. `Hanicka <recipesquad@apointa.sk>`) instead of the default Apointa sender. Applies to booking confirmations, reminders, cancellations, gift cards, shop orders, and waiting list emails. Falls back to `Apointa <noreply@apointa.sk>` if sender settings are not configured.

---

**### 💬 SMS Credits — Recurring Top-up**
SMS credits are now automatically added on every billing cycle renewal:
- Starter monthly: +10 credits
- Starter annual: +120 credits
- Growth monthly: +25 credits
- Growth annual: +300 credits

Credits are also added on new subscription creation via `customer.subscription.created`.

---

**### 📅 Calendar — Worker Name Display**
Calendar event slots now show the assigned worker's name instead of the customer name. Falls back to customer name if no worker is assigned.

---

**### ⚠️ Subscription Expiration Flow**
Full grace period flow for failed payments:
- `invoice.payment_failed` webhook sets account to `past_due` + activates 7-day grace period
- Dashboard banner with countdown + progress bar shown during grace period
- Day 7: `process-expired-subscriptions` Edge Function (pg_cron, runs daily at 3:00 UTC) downgrades account to Free, cancels Stripe subscription, sends email + in-app notification

---

**### 🐛 Bug Fixes**
- Fixed `invoice.paid` handler for new Stripe API format `2026-02-25.clover` — subscription ID now correctly read from `invoice.parent.subscription_details.subscription`
- Fixed `revalidatePath` in `waitingListActions.ts` causing render-time error on calendar page
- Fixed `booking-cancelled-by-provider-customer` missing `staffName` prop and subject translation key

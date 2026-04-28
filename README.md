# Apointa v1.12 — Upcoming / Pripravujeme

**Plánované vydanie / Planned release:** Soon

---

## 🟢 Quick Implementations

### Branded sender email
Emaily budú chodiť od `barber@apointa.sk` namiesto `noreply@apointa.sk`.
Provider si nastaví meno odosielateľa v dashboarde.

Emails will be sent from `businessname@apointa.sk` instead of `noreply@apointa.sk`.
Providers can configure the sender name in the dashboard.

### Zabudnuté heslo pre zákazníkov / Forgot Password for Customers
Reset hesla priamo z customer portálu `/my-reservations`.
Password reset directly from the customer portal `/my-reservations`.

### Cenník — update textácie / Pricing Page Copy Update
Preformulovanie plánov a popisov funkcií na hlavnej stránke.
Reformulated plan descriptions and feature copy on the main page.

### Autoscroll po výbere času /  Autoscroll after time slot have been chosen

---

## 🟡 Nové funkcie / New Features

### Zľavové kódy / Discount Codes
Provideri môžu vytvárať zľavové kódy (percentuálne alebo fixné).
Zákazník zadá kód pri rezervácii alebo v eshope.
Nastaviteľný počet použití, expirácia, minimálna suma.

Providers can create discount codes (percentage or fixed amount).
Customers apply the code during booking or in the shop.
Configurable usage limit, expiration, and minimum order value.

### Welcome guide po upgrade / Post-Upgrade Welcome Guide
Po prechode na platený plán sa zobrazí onboarding checklist:
pridaj pracovníka, nastav služby, aktivuj online platby, kúp SMS kredity.

After upgrading to a paid plan, an onboarding checklist appears:
add a worker, set up services, activate online payments, buy SMS credits.

### SMS kredity pri upgrade / SMS Credits on Upgrade
Automatické pridelenie bonus SMS kreditov po upgrade podľa plánu.
Starter: 20 kreditov / Growth: 50 kreditov / Enterprise: 100 kreditov.

Automatic bonus SMS credits granted on plan upgrade.
Starter: 20 credits / Growth: 50 credits / Enterprise: 100 credits.

---

## 🔴 Väčšie funkcie / Major Features

### 7-dňový expiration flow / 7-Day Grace Period
Po vypršaní predplatného:
- Countdown banner v dashboarde s možnosťou exportu zákazníkov (CSV)
- Denné emailové upozornenia
- Po 7 dňoch: downgrade na Free, odstránenie workerov (okrem ownera),
  vypnutie online platieb
- Poukážky a produkty zostanú aktívne pre existujúcich zákazníkov

After subscription expires:
- Countdown banner in dashboard with option to export customers (CSV)
- Daily email reminders
- After 7 days: downgrade to Free, removal of workers (except owner),
  online payments disabled
- Gift cards and products remain active for existing customers

---

*Poradie a dátumy sa môžu zmeniť podľa spätnej väzby. / Order and dates subject to change based on feedback.*

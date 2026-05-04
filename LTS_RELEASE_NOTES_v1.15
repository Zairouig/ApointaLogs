Apointa v1.15 — Release Notes
🇸🇰 Slovensky
### 🚀 Nové funkcie
#Mailing

Nová sekcia Mailing v sidebar pod SMS
Mass mailing — pošli email všetkým alebo vybraným klientom
Filter príjemcov podľa štítkov alebo manuálny výber
Personalizácia cez tagy {{first_name}}, {{full_name}}
Preview emailu pred odoslaním
História odoslaných mailov
Sender name/prefix podľa nastavení prevádzky
Dostupné len pre Growth a Enterprise plán

#QR kód & Booking link

Nový widget na dashboarde s booking linkom prevádzky
QR kód s Apointa logom v strede (Revolut štýl)
Copy link button
Stiahnutie QR kódu ako PNG

#Quick Share — Story generátor

Generuj Instagram/Facebook story kartu s QR kódom
Natívny share sheet na mobile (iOS Safari, Android Chrome)
Story obsahuje meno prevádzky, QR kód a booking link
Desktop fallback — stiahne PNG

#Quick Actions

Nový tab bar na dashboarde pod KPI kartami
Rýchly prístup: Waitlist, Príjmy & výdavky, Objednávky, Recenzie, Dochádzka

#Resend voucher

Preposlanie darčekovej poukážky emailom klientovi
Dostupné v zozname objednávok aj v scan detaile
Automaticky vygeneruje nové PDF s QR kódom


###🔧 Vylepšenia
Analytics

Opravený výpočet príjmov pracovníkov (CONFIRMED + FINISHED)
Opravená logika nových vs. vracajúcich sa klientov
Opravený CSV export (UTF-8 BOM, diakritika, správna štruktúra)
Opravený scroll na mobile

#Performance

Spline lazy load — Speed Index 3.4s → 2.1s

#Bezpečnosť

Migrácia z hCaptcha na Cloudflare Turnstile

#Auth & Onboarding

Opravený auth callback — locale prefix v confirmation linku
Welcome email po registrácii (lokalizovaný SK/EN/CS/DE/UK)
Onboarding reminder sequence (deň 1, 7, 14)
Nový používateľ dostane role: provider automaticky
Database webhook pre create-profile Edge Function

#Monitoring

UptimeRobot monitoring (5 min interval)
Sentry error tracking


###🐛 Opravené bugy

Login redirectoval na /my-reservations namiesto /dashboard pre nových providerov
Auth callback 404 bez locale prefixu
create-profile webhook sa spúšťal 4x naraz
Heatmap farby — nesprávny výpočet obsadenosti po migrácii na public_availability
Mobile sidebar scroll zablokovaný
Mailing client — React hooks error pri navigácii



🇬🇧 English
### 🚀 New Features
#Mailing

New Mailing section in sidebar under SMS
Mass mailing — send email to all or selected clients
Filter recipients by label or manual selection
Personalization via {{first_name}}, {{full_name}} tags
Email preview before sending
Sent email history
Sender name/prefix based on business settings
Available on Growth and Enterprise plan only

#QR Code & Booking Link

New dashboard widget with business booking link
QR code with Apointa logo in the center (Revolut style)
Copy link button
Download QR code as PNG

#Quick Share — Story Generator

Generate Instagram/Facebook story card with QR code
Native share sheet on mobile (iOS Safari, Android Chrome)
Story includes business name, QR code and booking link
Desktop fallback — downloads PNG

#Quick Actions

New tab bar on dashboard below KPI cards
Quick access: Waitlist, Income & expenses, Orders, Reviews, Attendance

#Resend Voucher

Resend gift card to client via email
Available in order list and scan detail
Automatically generates new PDF with QR code


###🔧 Improvements
Analytics

Fixed worker revenue calculation (CONFIRMED + FINISHED)
Fixed new vs. returning clients logic
Fixed CSV export (UTF-8 BOM, diacritics, correct structure)
Fixed mobile scroll

#Performance

Spline lazy load — Speed Index 3.4s → 2.1s

#Security

Migration from hCaptcha to Cloudflare Turnstile (free)

#Auth & Onboarding

Fixed auth callback — locale prefix in confirmation link
Welcome email after registration (localized SK/EN/CS/DE/UK)
Onboarding reminder sequence (day 1, 7, 14)
New user automatically gets role: provider
Database webhook for create-profile Edge Function

#Monitoring

UptimeRobot monitoring (5 min interval)
Sentry error tracking


###🐛 Bug Fixes

Login redirected to /my-reservations instead of /dashboard for new providers
Auth callback 404 without locale prefix
create-profile webhook fired 4x simultaneously
Heatmap colors — incorrect occupancy calculation after migration to public_availability
Mobile sidebar scroll blocked
Mailing client — React hooks error on navigation

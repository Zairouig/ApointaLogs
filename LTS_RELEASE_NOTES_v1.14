## v1.14 — Statistics & Analytics + Recurring Finance
Vydané: 1. Máj 2026

### 📊 Analytics modul — MVP
Nová sekcia Štatistiky v dashboarde — palubná doska podnikania kde za 20 sekúnd vidíš či ideš rovno, do kopca, alebo ti z motora kvapká tržba.
Prehľad — celkové tržby, rezervácie, noví klienti, zobrazenia profilu, konverzný pomer, stratené tržby zo zrušení a no-show. Porovnanie s predchádzajúcim obdobím s percentuálnou zmenou.
Rezervácie — trend podľa dní, rozloženie podľa dňa v týždni, vyťaženosť podľa hodiny dňa.
Tržby — graf podľa dní, tržby podľa služby, tržby podľa zamestnanca.
Klienti — noví vs. vracajúci sa (správna logika — porovnáva s celou históriou, nie len predchádzajúcim obdobím), pomer v pie charte.
Služby — najpopulárnejšie služby, počet rezervácií, počet zrušení per služba.
Zamestnanci — výkon, počet rezervácií, tržby per zamestnanec.
Export CSV — plne lokalizovaný, UTF-8 BOM pre správnu diakritiku v Exceli, štruktúrovaný (prehľad + služby + zamestnanci).
Filtrovanie podľa období: dnes, včera, tento/minulý týždeň, tento/minulý mesiac, posledných 30/90 dní, tento rok.
✨ Enterprise upsell tab — "Viac?" tab s prehľadom pokročilých funkcií (heatmapy, marketingové zdroje, loyalty metriky, PDF export, vlastné reporty) a priamym kontaktom na Apointa tím.

### 💰 Recurring Finance — Opakované záznamy
Finančný modul rozšírený o podporu opakovaných príjmov a výdavkov.
Pri pridávaní záznamu možno zapnúť "Opakovaný záznam" a zvoliť interval: každý týždeň / mesiac / rok. Záznamy sa generujú automaticky každú noc o 3:00 UTC cez Supabase Edge Function process-recurring-financie + pg_cron — funguje nezávisle od aktivity používateľa.
Ak používateľ vynechá viac období, všetky chýbajúce záznamy sa dogenerujú spätne. Duplicity sú ošetrené. Opakované záznamy sú označené modrým "Recurring" badge v zozname.

### 🔧 Opravy a vylepšenia

Total Earnings KPI na hlavnom dashboarde opravený — teraz fetchuje priamo z bookings.total_price namiesto financie_zaznamy
Financie modul hybridný — auto príjmy z rezervácií (read-only, badge "Auto") + manuálne záznamy + výdavky
Analytics klienti — opravená logika nových vs. vracajúcich sa klientov (historické porovnanie namiesto period-over-period)
Analytics tržby — zahŕňajú CONFIRMED aj FINISHED rezervácie
CSV export — UTF-8 BOM, bodkočiarka ako separator, quoted fields, memory leak fix


EN:

## v1.14 — Statistics & Analytics + Recurring Finance
Released: 1st May 2026

### 📊 Analytics module — MVP
New Statistics section in the dashboard — a business cockpit where you can see in 20 seconds whether you're on track, growing, or losing revenue.
Overview — total revenue, bookings, new clients, profile views, conversion rate, lost revenue from cancellations and no-shows. Period-over-period comparison with percentage change.
Bookings — daily trend, distribution by day of week, occupancy by hour of day.
Revenue — daily chart, revenue by service, revenue by staff member.
Clients — new vs. returning (correct logic — compares against full history, not just the previous period), ratio in pie chart.
Services — most popular services, booking count, cancellations per service.
Staff — performance, booking count, revenue per staff member.
CSV export — fully localized, UTF-8 BOM for correct characters in Excel, structured (overview + services + staff).
Period filters: today, yesterday, this/last week, this/last month, last 30/90 days, this year.
✨ Enterprise upsell tab — "More?" tab with an overview of advanced features (heatmaps, marketing sources, loyalty metrics, PDF export, custom reports) and direct contact to the Apointa team.

### 💰 Recurring Finance
Finance module extended with support for recurring income and expenses.
When adding a record, toggle "Recurring entry" and choose an interval: every week / month / year. Records are generated automatically every night at 3:00 UTC via Supabase Edge Function process-recurring-financie + pg_cron — works independently of user activity.
If a user misses multiple periods, all missing records are back-generated. Duplicates are handled. Recurring records are marked with a blue "Recurring" badge in the list.

### 🔧 Fixes & improvements

Total Earnings KPI on the main dashboard fixed — now fetches directly from bookings.total_price instead of financie_zaznamy
Finance module hybrid — auto income from bookings (read-only, "Auto" badge) + manual records + expenses
Analytics clients — fixed new vs. returning client logic (historical comparison instead of period-over-period)
Analytics revenue — includes both CONFIRMED and FINISHED bookings
CSV export — UTF-8 BOM, semicolon separator, quoted fields, memory leak fix

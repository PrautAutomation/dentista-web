# Mockup fotografie — NEPOUŽÍVAT V OSTRÉM PROVOZU

Tyhle fotky jsou **vygenerované**. Slouží výhradně k tomu, aby si lékař uměl
web představit — jak vypadá hero, jak sedí portréty v sekci O nás.

**Do ostrého webu nesmí.** Brand guidelines trvají na skutečných fotkách
a vygenerovaná „ordinace", která takhle nevypadá, je u zdravotnického
zařízení problém důvěry, ne kosmetická věc.

## Jak je nahradit

1. Skutečné fotky uložit do `../assets/logo/` (nebo kamkoliv, cesty se upraví
   v `web/tools/prepare-photos.mjs`)
2. Upravit mapování v `JOBS` v tom skriptu
3. `npm run photos` — zmenší a převede do WebP
4. Složku `mockup/` smazat a v `home-page.ts` přepsat cestu

## Proč WebP

Zdrojové PNG mají po ~2 MB. Tři takové v hero znamenají 6 MB, což je na
mobilu několik sekund čekání. Po převodu má celá sada 505 kB místo 11,3 MB.

## Známý nedostatek

Křeslo má na různých fotkách různou barvu (vínová vs. modrá) — vzniklo to
generováním po dávkách. U placeholderů to neřešíme, u skutečných fotek to
problém nebude.

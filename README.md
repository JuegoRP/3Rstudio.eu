# 3rstudio.eu

Web nezávislého herního studia **3R Studio** — Indie Games & Creative Tech. Jeden člověk z ČR: hry, aplikace a experimenty, postavené s pomocí automatizace a AI týmu.

Statický web (vanilla HTML/CSS/JS, bez frameworku). Hostován na Hetzner VPS přes Caddy, auto-deploy z této `main` větve.

## Stránky

| Soubor | Obsah |
|---|---|
| `index.html` | Studio hub — mega-menu projektů, showcase, časová osa, o studiu, kontakt |
| `conflux.html` | Detail hry CONFLUX (narativní karetní hra) |
| `gream.html` | Detail hry Gream (vzdělávací mobilní hra) |
| `blog.html` | Blog — rozcestník článků |
| `blog-post.html` | Šablona jednotlivého článku |
| `clicker/index.html` | Drobná webová hra / experiment |

## Design

- Tmavé téma, černá + žlutá, mega-menu inspirované Riot Games
- Dvojjazyčnost CZ/EN

## Projekty (jak je web prezentuje)

PC hry: **CONFLUX** (priorita), RECHO, Threshold · Mobile: **Gream** (priorita), Blind Roll, The 1% Focus, Thread the Needle, 100-Year Canvas, Exactly · Experimenty: PULSE · Vize: 3Cue. Celkem „11 projektů ve vývoji".

## Stav (k 2026-06-11)

**Hotovo:** deploy, HTTPS, auto-deploy, Cloudflare, mega-menu, showcase, časová osa, detailové stránky CONFLUX a Gream.

**Zbývá / k ověření:**
- [ ] **Google Analytics má placeholder `G-XXXXXXXXXX`** — měření neběží, doplnit reálné ID
- [ ] **Sjednotit pozici CONFLUXu**: menu uvádí „CONFLUX · Steam", ale strategie je **Itch.io první**, Steam až po ověření zájmu — sjednotit napříč webem
- [ ] **Gream termín**: web slibuje „App Store + Play, srpen 2026", reálně posunuto na **Q4 2026** (srpen = jen CONFLUX) — upravit
- [ ] Press kit a kompletní detailové stránky zbývajících her
- [ ] První blog článek (sekce „Blog" připravená, prázdná)

## Reálný stav her (zdroj pravdy)

Stav a úkoly her se řídí jejich repozitáři: `JuegoRP/Conflux` (TODO.md, TODO_pribehy.md) a `JuegoRP/Gream` (TODO.md) + `projects.json` v admin systému. CONFLUX je ve fázi beta-polish (kampaň 10 aktů napsaná, 163 kartových artů), Gream má hotovou EN+CZ lokalizaci.

## Deploy

Push do `main` → automatický deploy na VPS (Caddy servíruje statické soubory). Žádný build krok.

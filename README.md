# MRNKA – web (čištění a renovace střech a fasád)

Statický jednostránkový web. Žádný build, žádné závislosti – stačí `index.html` a složka `assets/`.

## Nasazení na GitHub Pages

1. Vytvoř nový repozitář na GitHubu (např. `mrnka-web`).
2. Nahraj obsah této složky (`index.html`, složku `assets/`, `.nojekyll`) do kořene repozitáře.
   - Přes web: *Add file → Upload files* → přetáhni soubory → *Commit*.
   - Nebo přes git:
     ```bash
     git init
     git add .
     git commit -m "MRNKA web"
     git branch -M main
     git remote add origin https://github.com/UZIVATEL/mrnka-web.git
     git push -u origin main
     ```
3. V repozitáři otevři **Settings → Pages**.
4. V sekci *Build and deployment* zvol **Source: Deploy from a branch**, větev **main**, složka **/ (root)**, a ulož.
5. Za chvíli web poběží na `https://UZIVATEL.github.io/mrnka-web/`.

> Soubor `.nojekyll` zajišťuje, že GitHub Pages nasadí soubory tak, jak jsou.

## Vlastní doména
V *Settings → Pages → Custom domain* zadej doménu (např. `www.mrnka.cz`) a u registrátora nastav DNS (CNAME na `UZIVATEL.github.io`).

## Co ještě doplnit (zástupné údaje)
- Telefony, e-mail, IČO, adresa (v hlavičce, patičce a formuláři)
- Čísla ve statistikách (`XX`, `XXX`…)
- Skutečné texty a jména recenzí + celkové hodnocení
- Portrét a podpis zakladatele (sekce „O nás")
- Napojení formulářů na e-mail / CRM (teď jen ukázka)

## Struktura
```
index.html        – celá stránka (HTML + CSS + JS v jednom)
assets/           – logo a fotografie
.nojekyll         – vypnutí Jekyll zpracování
```

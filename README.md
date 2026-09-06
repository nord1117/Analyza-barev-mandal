#  Analýza barevného složení mandal (Python -> Excel -> Power BI)

##  O projektu
Tento projekt vznikl z touhy propojit kreativní koníček (vybarvování mandal) s moderními nástroji datové analytiky. Cílem bylo vytvořit automatizovaný proces, který dokáže transformovat vizuální data (fotografie) na strukturovaná data, analyzovat je a přehledně vizualizovat pro koncového uživatele.

Projekt simuluje reálný firemní proces (tzv. **data pipeline**): od sběru syrových dat, přes jejich zpracování algoritmem strojového učení, uložení do tabulky, až po finální business reporting.

---

## 🔎 Co v projektu analyzuji a proč?
* **Podíl dominantních barev:** Zjišťuji, jaká barva (vyjádřená v HEX kódech) má v konkrétní mandale největší procentuální zastoupení.
* **Analýza nálady a trendů:** Sledování barevné palety může v praxi sloužit k analýze psychologického stavu nebo nálady autora v čase (např. zda v období stresu převládají jiné barvy než v období klidu).
* **Byznysový přesah:** Tento proces čištění obrazu a extrakce barev se v praxi využívá v e-commerce (automatické štítkování produktů podle barev z fotek), v módním průmyslu nebo při kontrole kvality výroby.

---

##  Použité technologie a kroky v projektu

###  Python (Sběr a zpracování dat)
Vytvořila jsem skript, který automaticky projde složku s fotografiemi mandal a aplikuje na ně následující postup:
* **PIL (Pillow):** Načtení a optimalizace velikosti obrázků.
* **Scikit-learn (K-Means):** Použití algoritmu strojového učení (shlukování) pro segmentaci obrazu a nalezení 5 nejvíce dominantních barev z milionů pixelů.
* **Numpy & Pandas:** Výpočet procentuálního podílu každé barvy a seřazení dat do strukturované tabulky (DataFrame).
* Výstup byl exportován do souboru `Mandaly_vystup.xlsx`.

###  Excel (Kontrola dat)
* Provedena lidská kontrola a verifikace dat před importem do vizualizačního nástroje.
* Zaokrouhlení a příprava čistých hodnot pro reporting.

###  Power BI (Business Intelligence & Reporting)
* **Power Query:** Import dat a transformace datových typů.
* **Interaktivní Dashboard:** Vytvoření reportu, kde uživatel pomocí průřezu (Sliceru) zvolí konkrétní mandalu a prstencový graf mu okamžitě ukáže její přesné barevné složení a poměry.

---

##  Výsledek
Výsledkem je plně funkční, interaktivní dashboard, který dokáže dynamicky filtrovat data pro jednotlivé obrazy. Projekt úspěšně prokazuje schopnost propojit pokročilé programování v Pythonu s tradičními business nástroji jako Excel a Power BI.

#  # Analýza barevného složení mandal

**Python → Excel → Power BI**

Osobní datový projekt, ve kterém propojuji kreativní koníček s praktickými nástroji datové analytiky.

Cílem projektu je převést fotografie vybarvených mandal na strukturovaná data, analyzovat jejich barevné složení a výsledky následně zobrazit v interaktivním Power BI reportu.

## Co projekt řeší

Pro jednotlivé fotografie mandal:

* načtu a zpracovávám obrazová data,
* pomocí algoritmu **K-Means** identifikuji dominantní barvy,
* vypočítám jejich procentuální zastoupení,
* výsledná data uložím do Excelu,
* data zkontroluji a připravím pro reporting,
* v Power BI vytvořím interaktivní vizualizaci.

Projekt tak ukazuje celý proces od zpracování vstupních dat až po jejich vizualizaci.

## Použité technologie

### Python

* **Pillow** – načtení a základní zpracování obrázků
* **NumPy** – práce s obrazovými daty
* **Pandas** – zpracování a strukturování dat
* **Scikit-learn / K-Means** – identifikace dominantních barev

### Excel

* kontrola výsledných dat
* zaokrouhlení a příprava hodnot pro další zpracování

### Power BI

* import dat
* **Power Query**
* transformace dat
* interaktivní dashboard
* filtrování jednotlivých mandal pomocí sliceru
* vizualizace barevného zastoupení

## Výsledek

Výsledkem je interaktivní Power BI report, ve kterém lze vybrat konkrétní mandalu a zobrazit její barevné složení a procentuální zastoupení jednotlivých dominantních barev.

Projekt mi umožnil prakticky si vyzkoušet propojení **Pythonu, práce s daty, Excelu, Power Query a Power BI** v jednom celku.

## Struktura projektu

* `analyza.ipynb` – Python analýza
* `data_mandaly_vystup.xlsx` – zpracovaná data
* `Mandaly.pbix` – Power BI report
* `Obrazky/` – vstupní obrazová data

## Co projekt demonstruje

* zpracování a čištění dat
* automatizaci opakující se práce pomocí Pythonu
* práci s tabulkovými daty
* základní aplikaci algoritmu K-Means
* transformaci dat v Power Query
* tvorbu interaktivního reportu v Power BI
* propojení více nástrojů v rámci jednoho analytického projektu



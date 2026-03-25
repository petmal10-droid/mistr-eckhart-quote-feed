# GitHub Pages zdroj pro citát dne

Tahle složka obsahuje nejjednodušší variantu centrálního online zdroje pro aplikaci.

## Co nahrát na GitHub
Nahraj do repozitáře alespoň soubor:
- `quote-of-day.json`

## Jak to zprovoznit
1. Vytvoř GitHub repozitář.
2. Nahraj obsah této složky do repozitáře.
3. V GitHubu otevři `Settings` > `Pages`.
4. Jako source nastav větev `main` a root složku `/ (root)`.
5. Po publikaci dostaneš URL ve tvaru:
   `https://tvuj-ucet.github.io/nazev-repozitare/quote-of-day.json`

## Co vložit do aplikace
V souboru `app/src/main/java/com/example/dailydemello/MainActivity.kt` nahraď hodnotu `QUOTE_ENDPOINT` skutečnou URL.

Příklad:
`private const val QUOTE_ENDPOINT = "https://tvuj-ucet.github.io/nazev-repozitare/quote-of-day.json"`

## Jak měnit citát každý den
Každé ráno uprav hodnoty v `quote-of-day.json`:
- `date`
- `text`
- případně `author`

A změnu pushni na GitHub. Po krátké chvíli bude nový citát dostupný všem uživatelům.

## Doporučení
- používej datum ve formátu `YYYY-MM-DD`
- nech `timezone` jako `Europe/Prague`
- vždy drž jen jeden aktivní citát dne v tomto souboru

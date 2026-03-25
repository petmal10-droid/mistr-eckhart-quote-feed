# GitHub Pages zdroj pro citát dne

Repozitář teď umí měnit `quote-of-day.json` automaticky každý den přes GitHub Actions.

## Co je v repozitáři
- `quote-of-day.json`: aktuální citát dne pro aplikaci
- `quotes.json`: seznam citátů, ze kterého se každý den vybírá
- `.github/workflows/daily-quote.yml`: automatizace denní změny

## Jak automatika funguje
- workflow běží každý den ráno pro časové pásmo `Europe/Prague`
- vybere další citát ze souboru `quotes.json`
- přepíše `quote-of-day.json`
- commitne změnu zpět do repozitáře
- GitHub Pages pak nabídne nový citát aplikaci všem uživatelům

## Kde měnit citáty
Uprav soubor `quotes.json`.

## URL pro aplikaci
`https://petmal10-droid.github.io/mistr-eckhart-quote-feed/quote-of-day.json`

## Ruční spuštění
Na GitHubu můžeš workflow spustit i ručně přes `Actions` > `Daily Quote Update` > `Run workflow`.

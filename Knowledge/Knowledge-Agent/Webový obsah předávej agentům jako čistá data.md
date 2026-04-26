# Webový obsah předávej agentům jako čistá data

## Trigger
- web scraping
- lead generation
- analýza mnoha URL

## Core rule
- Pokud web scraping vrací šum → předej agentovi extrahovaná strukturovaná data místo HTML

## Decision rules
- Pokud scraping vrací šum nebo chybějící obsah → použij extrakční vrstvu
- Pokud agent analyzuje mnoho URL → nekrm ho syrovým HTML
- Pokud web blokuje jeden zdroj vyhledávání → použij alternativní cestu
- Čistá data snižují tokenovou spotřebu
- Strukturovaný výstup zvyšuje přesnost následné analýzy
- Syrové HTML zvyšuje šum a náklady

## Use for
- lead generation
- průzkumu trhu
- extrakci kontaktů
- ukládání webových zdrojů do raw vrstvy

## Avoid
- Posílat agentovi celé chaotické HTML stránky místo extrahovaného obsahu


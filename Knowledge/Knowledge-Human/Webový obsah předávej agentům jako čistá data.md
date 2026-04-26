---
updated: 2026-04-26
created: 2026-04-26
typ: princip
puvod:
  - youtube
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - pracovni-hypoteza
stav: kandidat
duvera: medium
overeno_v_praxi: false
review_poznamka: "Pattern převzatý ze zdrojů; použij jako kandidáta, ne jako dogma, a ověř proti aktuálnímu úkolu."
oblast:
  - tools-skills-mcp-cli
  - research-a-znalostni-baze
  - tokeny-a-naklady
pouzij_kdy:
  - web scraping
  - lead generation
  - analýza mnoha URL
nastroje:
  - Firecrawl
  - Firecrawl MCP
  - scraping CLI
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]]"
  - "[[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]"
  - "[[AI System/Knowledge/Knowledge-Human/Velký výzkum deleguj do specializované vrstvy|Velký výzkum deleguj do specializované vrstvy]]"
zdroje:
  - "[[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]"
  - "[[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]]"
---

# Webový obsah předávej agentům jako čistá data

## Kontext
Použij, když agent potřebuje čerpat informace z webů, které nejsou optimalizované pro strojové čtení. Čistá data jsou lepší vstup než syrové HTML plné šumu.

## Princip
Webový HTML obsah je často plný reklam, cookie bannerů, lazy-loadingu a JavaScriptu. Před analýzou ho převeď na čistá strukturovaná data.

## Heuristiky

Decision trigger:
- Když scraping vrací šum nebo chybějící obsah → použij extrakční vrstvu.
- Když agent analyzuje mnoho URL → nekrm ho syrovým HTML.
- Když web blokuje jeden zdroj vyhledávání → použij alternativní cestu.

Pravidla:
- Čistá data snižují tokenovou spotřebu.
- Strukturovaný výstup zvyšuje přesnost následné analýzy.
- Syrové HTML zvyšuje šum a náklady.

## Použij při
- lead generation
- průzkumu trhu
- extrakci kontaktů
- ukládání webových zdrojů do raw vrstvy

## Použij s
- Firecrawl nebo jinou extrakční vrstvou
- [[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|úzkou CLI automatizací]]
- raw uložením extrahovaného obsahu
- kontrolou kvality dat před syntézou

## Související
- [[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]]
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]
- [[AI System/Knowledge/Knowledge-Human/Velký výzkum deleguj do specializované vrstvy|Velký výzkum deleguj do specializované vrstvy]]

## Zdroje
- [[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]
- [[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Posílat agentovi celé chaotické HTML stránky místo extrahovaného obsahu.


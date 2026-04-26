---
created: 2026-04-26
updated: 2026-04-26
typ: workflow
puvod:
  - youtube
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - pracovni-hypoteza
stav: kandidat
duvera: medium
overeno_v_praxi: false
review_poznamka: "Pattern převzatý ze zdroje; největší hodnotu má u dlouhodobých projektů a pravidelné práce s agentem."
oblast:
  - ai-agent-workflow
  - research-a-znalostni-baze
  - tools-skills-mcp-cli
pouzij_kdy:
  - dlouhodobý projekt
  - denní práce s agentem
  - ztráta kontextu mezi dny
nastroje:
  - scheduled tasks
  - Obsidian
  - Markdown
  - Claude skills
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]]"
  - "[[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]"
  - "[[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]"
zdroje:
  - "[[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]"
---

# Denní rekap ukládej do pracovní paměti

## Kontext
Použij, když agent pracuje na projektu více dní a kontext se ztrácí mezi chaty, úkoly a plánovanými běhy.

## Princip
Na konci dne ulož stručný rekap: co bylo dodáno, co se změnilo, co je rozpracované, blokery, rozhodnutí a priority na další den.

## Heuristiky

Decision trigger:
- Když projekt běží déle než jeden den → ukládej denní rekap.
- Když agent dělá scheduled tasks → zaznamenej jejich výstupy.
- Když vzniknou rozhodnutí nebo blokery → přenes je do pracovní paměti.

Pravidla:
- Denní rekap snižuje ztrátu kontextu.
- Markdown note zvyšuje přenositelnost mezi agenty.
- Rekap bez priorit na další den má nižší akční hodnotu.

## Použij při
- dlouhodobém vývoji aplikace
- obsahovém workflow
- výzkumných projektech
- práci s více paralelními agenty

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|živým kontextem]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|naplánovaným během]]
- Obsidian daily notes
- checklistem blokery / dodáno / zítra

## Související
- [[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]]
- [[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]

## Zdroje
- [[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: workflow pro projekty, kde stojí za to udržet kontinuitu.

## Kdy nepoužít
- Když jde o krátký jednorázový úkol.
- Když rekap jen duplikuje existující task tracker bez nové hodnoty.

## Anti-pattern
- Nechat výsledky dne jen v chatu a další den znovu rekonstruovat stav projektu.

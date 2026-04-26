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
  - tokeny-a-naklady
  - tools-skills-mcp-cli
  - ai-agent-workflow
pouzij_kdy:
  - volba mezi MCP a CLI
  - úzká opakovatelná automatizace
  - snižování context overheadu
nastroje:
  - Playwright CLI
  - Claude Code
  - MCP
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]"
  - "[[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|Automatizační skripty proměňuj ve skills]]"
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|Nástroje přidávej až podle měřítka]]"
zdroje:
  - "[[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]]"
---

# CLI automatizace šetří tokeny oproti MCP

## Kontext
Použij, když vybíráš mezi MCP serverem a CLI nástrojem pro agentickou automatizaci. Je to praktické zejména u [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|browser QA]], kde specializovaný příkaz často stačí.

## Princip
CLI nástroj často spotřebuje méně kontextu než MCP s mnoha nástroji a popisy. Pokud agent umí bezpečně volat CLI, preferuj CLI pro úzké, opakovatelné úkoly.

## Heuristiky

Decision trigger:
- Když MCP zabírá hodně kontextu → zvaž CLI alternativu.
- Když úkol vyžaduje úzkou automatizaci → použij specializovaný CLI skript.
- Když řešení lze vyjádřit jako shell příkaz → nepoužívej těžší agentické workflow.
- Když potřebuješ širokou interaktivní integraci → MCP může dávat větší smysl.

Pravidla:
- Mnoho MCP nástrojů zvyšuje tokenovou režii.
- CLI snižuje kontextovou stopu opakovaných operací.
- CLI skript zvyšuje reprodukovatelnost deterministických lokálních operací.
- Výběr nástroje má vyvažovat tokeny, výkon a spolehlivost.

## Použij při
- browser automation
- web scrapingu
- lokálních kontrolách projektu
- automatizaci opakovaných příkazů

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|měřením tokenového rozpočtu]]
- úzkými CLI skripty uloženými v repu
- skills pro opakované postupy
- MCP jen tam, kde je potřeba širší integrace

## Související
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]
- [[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|Automatizační skripty proměňuj ve skills]]
- [[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|Nástroje přidávej až podle měřítka]]

## Zdroje
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
- Připojit velký MCP server kvůli úkolu, který vyřeší jeden úzký CLI příkaz nebo skript.

---
created: 2026-04-26
updated: 2026-04-26
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
  - coding-agenti
  - ai-agent-workflow
  - tools-skills-mcp-cli
pouzij_kdy:
  - zakládání agentického projektu
  - práce s více výstupy
  - odkazování souborů v chatu
nastroje:
  - Codex
  - Claude Code
  - Finder
  - Markdown
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]"
  - "[[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|Kontext drž mimo konkrétní AI nástroj]]"
  - "[[AI System/Knowledge/Knowledge-Human/Paralelní agentické chaty řiď přes plán a stav|Paralelní agentické chaty řiď přes plán a stav]]"
zdroje:
  - "[[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]"
---

# Projektový adresář používej jako pracovní hranici agenta

## Kontext
Použij, když agent vytváří soubory, dokumenty, spreadsheety, aplikace nebo assety. Projektový adresář určuje, kde agent pracuje, co může snadno zmínit a jak se výstupy později dohledají.

## Princip
Každý větší agentický workflow začni ve vlastním projektovém adresáři. Ukládej do něj výstupy, plán, zdroje a související chaty tak, aby šly znovu otevřít a referencovat.

## Heuristiky

Decision trigger:
- Když úkol vytvoří více souborů → založ samostatný projektový adresář.
- Když agent potřebuje navazovat mezi chaty → udržuj výstupy ve stejné složce.
- Když projekt mizí ze sidebaru → hledej ho přes složku nebo search, nepanikař.

Pravidla:
- Projektová složka snižuje chaos mezi výstupy.
- File mentions fungují lépe, když agent pracuje ve správném adresáři.
- Chat není jediný zdroj pravdy; výstupy mají ležet v souborech.

## Použij při
- výzkumném projektu
- tvorbě decku, reportu nebo spreadsheetu
- vývoji webové nebo mobilní aplikace
- práci s více souběžnými chaty

## Použij s
- `plan.md` nebo checklistem v kořeni projektu
- `outputs/` pro generované dokumenty
- `assets/` pro obrázky, videa a design podklady
- [[AI System/Knowledge/Knowledge-Human/Paralelní agentické chaty řiď přes plán a stav|paralelními chaty nad jednou složkou]]

## Související
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]
- [[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|Kontext drž mimo konkrétní AI nástroj]]
- [[AI System/Knowledge/Knowledge-Human/Paralelní agentické chaty řiď přes plán a stav|Paralelní agentické chaty řiď přes plán a stav]]

## Zdroje
- [[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Pouštět dlouhý agentický projekt v obecné složce a nechat výstupy rozházené mezi chatem, Downloads a náhodnými adresáři.


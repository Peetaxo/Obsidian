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
  - claude-code
  - coding-agenti
  - tokeny-a-naklady
pouzij_kdy:
  - velké codebase
  - opakované dotazy nad repozitářem
  - snížení tokenů při onboardingu agenta
nastroje:
  - Graphify
  - Claude Code
  - knowledge graph
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]"
  - "[[AI System/Knowledge/Knowledge-Human/Model routing podle náročnosti úkolu|Model routing podle náročnosti úkolu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Velký výzkum deleguj do specializované vrstvy|Velký výzkum deleguj do specializované vrstvy]]"
zdroje:
  - "[[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]"
---

# Knowledge graph používej pro velké codebase

## Kontext
Použij, když agent opakovaně odpovídá na otázky nad rozsáhlým codebase. [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet]] se zlepší, pokud agent nemusí každou session mapovat repo od nuly.

## Princip
Velké codebase je vhodné převést na dotazovatelný knowledge graph. Graph zrychlí navigaci vztahů mezi soubory, importy, komunitami a klíčovými uzly.

## Heuristiky

Decision trigger:
- Když repo má stovky souborů → zvaž knowledge graph.
- Když agent opakovaně pálí tokeny na mapování codebase → vytvoř index vztahů.
- Když repo má méně než několik desítek souborů → graph overhead se nemusí vyplatit.

Pravidla:
- Knowledge graph snižuje náklady na opakované otázky nad velkým repem.
- Hub uzly pomáhají najít architektonicky důležité soubory.
- Malý projekt nepotřebuje těžkou indexační vrstvu.

## Použij při
- orientaci ve velkém repozitáři
- onboarding dotazech nad codebase
- hledání architektonických závislostí
- opakované práci agenta ve stejném projektu

## Použij s
- Graphify nebo podobným indexem vztahů
- krátkým README pro dotazování graphu
- model routingem podle složitosti úkolu
- pravidelnou obnovou indexu po větším refaktoru

## Související
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]
- [[AI System/Knowledge/Knowledge-Human/Model routing podle náročnosti úkolu|Model routing podle náročnosti úkolu]]
- [[AI System/Knowledge/Knowledge-Human/Velký výzkum deleguj do specializované vrstvy|Velký výzkum deleguj do specializované vrstvy]]

## Zdroje
- [[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Nechat agenta v každé nové session znovu procházet velké repo bez uložené mapy vztahů.


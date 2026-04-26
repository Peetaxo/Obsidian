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
  - research-a-znalostni-baze
  - tokeny-a-naklady
  - ai-agent-workflow
pouzij_kdy:
  - mnoho PDF nebo videí
  - rozsáhlá rešerše
  - dotazování velkého korpusu
nastroje:
  - NotebookLM
  - knowledge graph
  - Obsidian
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Persistentní wiki místo jednorázového RAG|Persistentní wiki místo jednorázového RAG]]"
  - "[[AI System/Knowledge/Knowledge-Human/Knowledge graph používej pro velké codebase|Knowledge graph používej pro velké codebase]]"
  - "[[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]"
zdroje:
  - "[[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]"
---

# Velký výzkum deleguj do specializované vrstvy

## Kontext
Použij, když agent potřebuje pracovat s desítkami až stovkami zdrojů pro výzkum nebo rešerši. Aktivní kontext agenta nemá nést celý korpus.

## Princip
Rozsáhlý zdrojový korpus nepatří celý do aktivního kontextu agenta. Vytvoř specializovanou výzkumnou vrstvu, kterou agent dotazuje a výsledky ukládá zpět jako znalost.

## Heuristiky

Decision trigger:
- Když výzkum obsahuje mnoho PDF, videí nebo článků → použij externí notebook nebo index.
- Když dotaz vyžaduje jen odpověď z korpusu → dotazuj výzkumnou vrstvu.
- Když výzkum vytvoří opakovaně použitelný závěr → ulož ho do wiki.

Pravidla:
- Externí výzkumná vrstva snižuje kontextovou zátěž.
- Agent má kurátorovat notebooky podle cíle, ne jen sbírat zdroje.
- Výsledky výzkumu musí proudit zpět do persistentní wiki.

## Použij při
- rešerši přes mnoho YouTube videí
- práci s PDF zdroji
- přípravě prezentací
- tvorbě tematického výzkumného korpusu

## Použij s
- NotebookLM nebo dotazovatelným indexem
- [[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|ukládáním závěrů zpět do wiki]]
- raw složkou pro primární zdroje
- indexem pro výsledné principy

## Související
- [[AI System/Knowledge/Knowledge-Human/Persistentní wiki místo jednorázového RAG|Persistentní wiki místo jednorázového RAG]]
- [[AI System/Knowledge/Knowledge-Human/Knowledge graph používej pro velké codebase|Knowledge graph používej pro velké codebase]]
- [[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]

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
- Cpát celý rozsáhlý korpus do jedné agentické session místo použití dotazovatelné mezivrstvy.


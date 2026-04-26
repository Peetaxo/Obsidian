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
review_poznamka: "Pattern převzatý ze zdrojů; použij jako kandidáta, ne jako dogma, a ověř proti aktuálnímu úkolu."
oblast:
  - tools-skills-mcp-cli
  - ai-agent-workflow
  - research-a-znalostni-baze
pouzij_kdy:
  - opakovaný report
  - plánovaná automatizace
  - skill s API nebo pluginem
nastroje:
  - Codex automations
  - skills
  - plugins
  - API
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|Automatizační skripty proměňuj ve skills]]"
  - "[[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]"
  - "[[AI System/Knowledge/Knowledge-Human/Denní rekap ukládej do pracovní paměti|Denní rekap ukládej do pracovní paměti]]"
  - "[[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]]"
zdroje:
  - "[[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]"
  - "[[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]"
---

# Automatizace stavěj až z odladěného skillu

## Kontext
Použij, když se má opakovaný postup spouštět podle času nebo události: měsíční report, týdenní recap, příprava dokumentu, draft postů nebo kontrola dat.

## Princip
Nejdřív postup odlaď ručně jako skill nebo workflow, potom z něj udělej automatizaci. Automatizace má používat ověřené nástroje, jasný výstup a testovací běh.

## Heuristiky

Decision trigger:
- Když stejný skill spouštíš pravidelně → zvaž automation.
- Když workflow potřebuje API key → nejdřív otestuj skill ručně.
- Když automatizace posílá email, post nebo externí akci → nastav kontrolu nebo omezení.

Pravidla:
- Odladěný skill snižuje riziko špatné automatizace.
- Testovací běh musí ověřit výstup i oprávnění.
- Automatizace bez jasného logu se špatně ladí.

## Použij při
- měsíčním reportu z YouTube transkriptů
- týdenním kalendářním recapu
- plánování social postů
- pravidelném výzkumném nebo QA workflow

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|pluginem pro přístup ke službě]]
- [[AI System/Knowledge/Knowledge-Human/Denní rekap ukládej do pracovní paměti|denním rekapem výstupů a blockerů]]
- API klíčem uloženým mimo veřejný výstup
- testovacím během před zapnutím
- logem posledního běhu a výstupu

## Související
- [[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|Automatizační skripty proměňuj ve skills]]
- [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]
- [[AI System/Knowledge/Knowledge-Human/Denní rekap ukládej do pracovní paměti|Denní rekap ukládej do pracovní paměti]]
- [[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]]

## Zdroje
- [[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]
- [[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Hned naplánovat automatizaci nad neověřeným promptem a zjistit chyby až po tom, co odešle špatný výstup.

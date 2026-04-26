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
  - ai-agent-workflow
  - coding-agenti
  - claude-code
pouzij_kdy:
  - více souběžných agentických tasků
  - dlouhé běhy agentů
  - multitasking v Codexu nebo Claude Code
nastroje:
  - Codex
  - Claude Code
  - plan.md
  - checklist
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Projektový adresář používej jako pracovní hranici agenta|Projektový adresář používej jako pracovní hranici agenta]]"
  - "[[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]"
zdroje:
  - "[[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]"
---

# Paralelní agentické chaty řiď přes plán a stav

## Kontext
Použij, když jeden projekt obsahuje několik nezávislých výstupů: aplikaci, landing page, deck, video, databázi nebo automatizace. Agenti běží déle, takže efektivita stojí na správném rozdělení a sledování stavu.

## Princip
Paralelizuj jen úkoly s jasným vlastnictvím a společným plánem. Každý chat pojmenuj podle výstupu, průběžně kontroluj stav a sdílené rozhodnutí ukládej do projektu.

## Heuristiky

Decision trigger:
- Když projekt má více nezávislých výstupů → rozděl je do samostatných chatů.
- Když úkoly sahají do stejných souborů → nejdřív stanov pořadí nebo ownership.
- Když agent běží dlouho → přepni pozornost na jiný připravený task a vrať se přes checklist.

Pravidla:
- Paralelní chaty zvyšují throughput.
- Sdílený plán snižuje ztrátu kontextu mezi chaty.
- Neřízené paralelní editace zvyšují riziko konfliktů.

## Použij při
- souběžné tvorbě appky, webu, decku a videa
- dlouhých research nebo build taskech
- práci nad jedním projektovým adresářem
- iteraci marketingových assetů a produktu současně

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Projektový adresář používej jako pracovní hranici agenta|projektovým adresářem]]
- jedním `plan.md` nebo checklistem
- pojmenovanými chaty podle výstupu
- pravidlem: jeden chat vlastní jeden hlavní výstup

## Související
- [[AI System/Knowledge/Knowledge-Human/Projektový adresář používej jako pracovní hranici agenta|Projektový adresář používej jako pracovní hranici agenta]]
- [[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]

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
- Spustit mnoho agentů nad stejnými soubory bez plánu, pojmenování chatů a vlastnictví výstupů.


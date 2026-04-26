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
  - ai-agent-workflow
pouzij_kdy:
  - dlouhodobá údržba wiki
  - delegace bookkeepingu
  - lidská kurace zdrojů
nastroje:
  - Claude Code
  - Obsidian
  - lokální markdown
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]"
  - "[[AI System/Knowledge/Knowledge-Human/Obsidian jako UI nad markdown wiki|Obsidian jako UI nad markdown wiki]]"
  - "[[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# LLM jako správce wiki člověk jako kurátor

## Kontext
Použij, když je cílem dlouhodobě udržovat znalostní bázi bez ručního bookkeepingu. Člověk má vybírat směr a agent má držet strukturu.

## Princip
Člověk vybírá zdroje, směr zkoumání a otázky. LLM provádí údržbu: shrnutí, propojení, aktualizace, filing a kontrolu konzistence.

## Heuristiky

Decision trigger:
- Když práce vyžaduje údržbu vazeb a souborů → deleguj ji na LLM.
- Když je potřeba rozhodnout důležitost zdroje → zapoj člověka.
- Když vzniká nový směr výzkumu → člověk určí prioritu.

Pravidla:
- LLM snižuje náklady na údržbu wiki.
- Člověk zvyšuje kvalitu výběru zdrojů a otázek.
- Bookkeeping je vhodná práce pro agenta, ne pro ruční proces.

## Použij při
- osobní znalostní bázi
- týmové interní wiki
- výzkumných projektech
- opakované syntéze poznámek

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|lokálním markdownem]]
- pravidelným lintem vazeb
- lidským schvalováním nových témat
- logem změn

## Související
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]
- [[AI System/Knowledge/Knowledge-Human/Obsidian jako UI nad markdown wiki|Obsidian jako UI nad markdown wiki]]
- [[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]

## Zdroje
- [[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Očekávat, že člověk bude dlouhodobě ručně udržovat všechny odkazy, souhrny a rozpory.


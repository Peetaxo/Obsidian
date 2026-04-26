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
  - ai-agent-workflow
  - research-a-znalostni-baze
pouzij_kdy:
  - návrh nové wiki
  - větší restrukturalizace
  - nejasný účel znalostní báze
nastroje:
  - Claude Code plan mode
  - Obsidian
  - schema checklist
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Třívrstvá architektura znalostní báze|Třívrstvá architektura znalostní báze]]"
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|Nástroje přidávej až podle měřítka]]"
  - "[[AI System/Knowledge/Knowledge-Human/LLM jako správce wiki člověk jako kurátor|LLM jako správce wiki člověk jako kurátor]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Plan mode před návrhem znalostní báze

## Kontext
Použij před založením nebo větší restrukturalizací wiki. Plan mode pomáhá vyjasnit účel, zdroje a hranice dřív, než agent začne vytvářet soubory.

## Princip
Před implementací znalostní báze má agent vyjasnit účel, jazyk, typy zdrojů, způsoby ingesce a strukturu. Dobrý plán snižuje pozdější chaos ve wiki.

## Heuristiky

Decision trigger:
- Když vzniká nová wiki → nejdřív projdi plánovací otázky.
- Když se mění účel wiki → aktualizuj schema a strukturu.
- Když není jasné, jaké zdroje budou přibývat → nezačínej implementací.

Pravidla:
- Účel wiki určuje strukturu složek.
- Typy zdrojů určují metadata a workflow ingesce.
- Jazyk obsahu má odpovídat budoucím dotazům a zdrojům.

## Použij při
- zakládání Obsidian vaultu
- návrhu workflow pro agenta
- rozhodování o složkách a metadatech
- přípravě wiki pro konkrétní projekt

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Třívrstvá architektura znalostní báze|třívrstvou architekturou]]
- seznamem typů zdrojů
- pravidly pro raw a knowledge vrstvu
- následným indexem a logem

## Související
- [[AI System/Knowledge/Knowledge-Human/Třívrstvá architektura znalostní báze|Třívrstvá architektura znalostní báze]]
- [[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|Nástroje přidávej až podle měřítka]]
- [[AI System/Knowledge/Knowledge-Human/LLM jako správce wiki člověk jako kurátor|LLM jako správce wiki člověk jako kurátor]]

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
- Nechat agenta rovnou generovat strukturu bez vyjasnění účelu, zdrojů a způsobu používání.


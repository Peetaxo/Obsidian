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
  - research-a-znalostni-baze
  - ai-agent-workflow
pouzij_kdy:
  - údržba agentické paměti
  - neplatné odkazy v kontextu
  - změny projektu nebo brandu
nastroje:
  - Obsidian
  - Markdown
  - lint checklist
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]"
  - "[[AI System/Knowledge/Knowledge-Human/Index a log jako navigační paměť|Index a log jako navigační paměť]]"
  - "[[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]"
zdroje:
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
---

# Kontext udržuj jako živý dokument

## Kontext
Použij, když agentická paměť, konfigurační soubory nebo knowledge báze začínají zastarávat. Kontext má hodnotu jen tehdy, když odpovídá aktuální realitě projektu.

## Princip
Kontextové soubory nejsou jednorázové nastavení. Průběžně je aktualizuj, maž neplatné odkazy a doplňuj nové rozcestníky podle skutečných workflow.

## Heuristiky

Decision trigger:
- Když agent použije starý odkaz nebo pravidlo → oprav kontextový dokument.
- Když se změní brand, projekt nebo workflow → aktualizuj rozcestníky.
- Když knowledge báze roste → spusť lint a zkontroluj zastaralost.

Pravidla:
- Živý kontext zvyšuje kvalitu budoucích odpovědí.
- Neplatný kontext může být horší než žádný kontext.
- Údržba kontextu je opakovaný proces, ne setup na začátku projektu.

## Použij při
- údržbě `AGENTS.md`, `CLAUDE.md` nebo skillů
- aktualizaci brand manuálu
- přesunu zdrojů mezi nástroji
- kontrole knowledge báze po větší změně

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|pravidelným lintem]]
- logem změn
- kontrolou neexistujících wiki odkazů
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|skilly-rozcestníky]]

## Související
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]
- [[AI System/Knowledge/Knowledge-Human/Index a log jako navigační paměť|Index a log jako navigační paměť]]
- [[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]

## Zdroje
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Brát kontextové soubory jako hotové jednou provždy a nechat agenta opakovat zastaralé instrukce.


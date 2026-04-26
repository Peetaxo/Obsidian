---
updated: 2026-04-26
created: 2026-04-26
typ: princip
puvod:
  - youtube
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - overene-v-tomto-vaultu
stav: overeno
duvera: high
overeno_v_praxi: true
review_poznamka: "Pattern je převzatý ze zdrojů a zatím ověřený hlavně při správě tohoto vaultu; mimo tento kontext ho znovu posuď."
oblast:
  - research-a-znalostni-baze
  - ai-agent-workflow
pouzij_kdy:
  - ukládání transkriptů
  - import primárních zdrojů
  - pozdější reingesce
nastroje:
  - Obsidian
  - Web Clipper
  - lokální markdown
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Třívrstvá architektura znalostní báze|Třívrstvá architektura znalostní báze]]"
  - "[[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|Traceabilita wiki stránek ke zdrojům]]"
  - "[[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Kompletní raw zdroje bez zkracování

## Kontext
Použij při ukládání přepisů videí, článků, schůzek nebo jiných primárních zdrojů. Raw vrstva je zdroj pravdy pro pozdější revizi a nové syntézy.

## Princip
Raw zdroj musí obsahovat kompletní původní informaci. Agent nesmí nahrazovat raw obsah zkráceným souhrnem nebo odkazem na chybějící část.

## Heuristiky

Decision trigger:
- Když ukládáš transkript → ověř, že je kompletní.
- Když agent vytvoří raw soubor se zkrácenou částí → doplň plný text.
- Když raw odkazuje na jiný nedostupný soubor → považuj zdroj za nekompletní.

Pravidla:
- Kompletní raw zdroj zvyšuje ověřitelnost znalostí.
- Zkrácený raw zdroj snižuje schopnost pozdější reingesce.
- Raw vrstva má uchovat fakta, ne interpretaci.

## Použij při
- YouTube transkriptech
- automatických titulcích
- přepisech schůzek
- importu webových článků

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Třívrstvá architektura znalostní báze|oddělenou raw vrstvou]]
- frontmatterem raw zdroje
- odkazem na původní URL
- následnou syntézou do krátkých knowledge bloků

## Související
- [[AI System/Knowledge/Knowledge-Human/Třívrstvá architektura znalostní báze|Třívrstvá architektura znalostní báze]]
- [[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|Traceabilita wiki stránek ke zdrojům]]
- [[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]

## Zdroje
- [[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]

## Review
- Stav: Ověřeno v tomto vaultu.
- Důvěra: high.
- Ověření v praxi: Použito při organizaci a údržbě AI System knowledge báze.
- Použij jako: stabilnější lokální pravidlo, ale při jiném projektu znovu ověř kontext.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Uložit do raw vrstvy jen shrnutí, výtah nebo poznámku „transkript zkrácen“.


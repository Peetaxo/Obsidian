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
  - hromadné zpracování zdrojů
  - import více YouTube transkriptů
  - kontrola konzistence wiki
nastroje:
  - Obsidian
  - lokální markdown
  - lint checklist
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]"
  - "[[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]"
  - "[[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|Traceabilita wiki stránek ke zdrojům]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Batch ingesce vyžaduje následný lint

## Kontext
Použij, když agent zpracovává více videí, článků nebo zdrojů najednou. Batch režim urychlí práci, ale musí skončit [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|lintem znalostní báze]], jinak rychle vzniknou slabé odkazy a duplicity.

## Princip
Batch ingesce šetří čas, ale snižuje dohled nad kvalitou struktury. Po hromadném zpracování je nutné zkontrolovat úplnost raw zdrojů, duplicity, špatné zařazení a odkazy.

## Heuristiky

Decision trigger:
- Když zpracuješ více zdrojů najednou → spusť lint wiki.
- Když agent vytvoří nové kategorie bez jasného důvodu → zkontroluj strukturu.
- Když výstupy vypadají nekonzistentně → oprav schema nebo pravidla ingesce.

Pravidla:
- Batch zvyšuje rychlost ingesce.
- Batch snižuje průběžnou supervizi.
- Následný lint snižuje dlouhodobý strukturální dluh.

## Použij při
- zpracování více YouTube videí
- importu starších článků
- migraci poznámek
- automatickém vytváření tematických stránek

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|traceabilitou ke zdrojům]]
- kontrolou YAML frontmatteru
- kontrolou neexistujících wiki odkazů
- aktualizací [[AI System/Knowledge/Knowledge-Human/Index a log jako navigační paměť|indexu a logu]]

## Související
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]
- [[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]
- [[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|Traceabilita wiki stránek ke zdrojům]]

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
- Hromadně ingestovat zdroje a bez kontroly předpokládat, že vzniklá wiki struktura je správná.


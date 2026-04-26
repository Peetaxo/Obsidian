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
  - wiki rychle roste
  - po větší ingesci
  - kontrola odkazů a rozporů
nastroje:
  - Obsidian Graph view
  - lokální skript
  - lint checklist
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Batch ingesce vyžaduje následný lint|Batch ingesce vyžaduje následný lint]]"
  - "[[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]]"
  - "[[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|Traceabilita wiki stránek ke zdrojům]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
---

# Pravidelný lint znalostní báze

## Kontext
Použij, když wiki roste a hrozí rozpory, zastaralost, osiřelé stránky nebo chybějící vazby. Lint je údržbová smyčka nad [[AI System/Knowledge/Knowledge-Human/Persistentní wiki místo jednorázového RAG|persistentní wiki]].

## Princip
Znalostní báze potřebuje pravidelnou kontrolu kvality. Lint hledá rozpory, zastaralá tvrzení, chybějící stránky, slabé odkazy a mezery ve znalostech.

## Heuristiky

Decision trigger:
- Když wiki rychle roste → spusť lint.
- Když se zdroje časově překrývají nebo odporují → zkontroluj rozpory.
- Když se pojem často opakuje bez vlastní stránky → vytvoř kandidáta na nový blok.

Pravidla:
- Orphan stránky snižují navigovatelnost.
- Zastaralá tvrzení snižují důvěryhodnost wiki.
- Chybějící odkazy snižují využitelnost syntézy.

## Použij při
- pravidelné údržbě wiki
- kontrole po větší ingesci
- přípravě znalostí pro rozhodování
- hledání dalších výzkumných otázek

## Použij s
- kontrolou YAML frontmatteru
- kontrolou raw zdrojů
- kontrolou neexistujících wiki odkazů
- Graph view pro huby a osiřelé stránky

## Související
- [[AI System/Knowledge/Knowledge-Human/Batch ingesce vyžaduje následný lint|Batch ingesce vyžaduje následný lint]]
- [[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]]
- [[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|Traceabilita wiki stránek ke zdrojům]]

## Zdroje
- [[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]

## Review
- Stav: Ověřeno v tomto vaultu.
- Důvěra: high.
- Ověření v praxi: Použito při organizaci a údržbě AI System knowledge báze.
- Použij jako: stabilnější lokální pravidlo, ale při jiném projektu znovu ověř kontext.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Přidávat nové stránky bez kontroly konzistence a propojení.

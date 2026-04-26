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
  - hodnotná odpověď v chatu
  - nové rozhodovací pravidlo
  - opakovaně použitelná syntéza
nastroje:
  - Obsidian
  - lokální markdown
  - Claude Code
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Persistentní wiki místo jednorázového RAG|Persistentní wiki místo jednorázového RAG]]"
  - "[[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]"
  - "[[AI System/Knowledge/Knowledge-Human/Index a log jako navigační paměť|Index a log jako navigační paměť]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Dotazy ukládej zpět jako znalosti

## Kontext
Použij, když dotaz vytvoří hodnotnou analýzu, srovnání, rozhodnutí nebo nový vztah mezi pojmy. Tím se z chatu stává vstup do [[AI System/Knowledge/Knowledge-Human/Persistentní wiki místo jednorázového RAG|persistentní wiki]].

## Princip
Dobrá odpověď nemá zmizet v historii chatu. Pokud má budoucí hodnotu, ulož ji zpět do wiki jako novou nebo aktualizovanou stránku.

## Heuristiky

Decision trigger:
- Když odpověď obsahuje opakovaně použitelnou analýzu → ulož ji do wiki.
- Když dotaz odhalí nový vztah mezi pojmy → přidej odkaz nebo nový blok.
- Když výstup slouží jako rozhodnutí → zaznamenej ho jako znalost.

Pravidla:
- Uložený dotaz zvyšuje kumulaci znalostí.
- Chat historie je slabé místo pro dlouhodobou paměť.
- Výstupy z průzkumu mají stejnou hodnotu jako ingesce zdrojů.

## Použij při
- srovnávacích tabulkách
- návrhových rozhodnutích
- syntézách přes více zdrojů
- objevech vzniklých během konverzace

## Použij s
- krátkým knowledge blokem místo dlouhého souhrnu
- [[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|traceabilitou ke zdrojům]]
- aktualizací indexu
- log záznamem změny

## Související
- [[AI System/Knowledge/Knowledge-Human/Persistentní wiki místo jednorázového RAG|Persistentní wiki místo jednorázového RAG]]
- [[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]
- [[AI System/Knowledge/Knowledge-Human/Index a log jako navigační paměť|Index a log jako navigační paměť]]

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
- Nechat hodnotné analýzy jen v chatu a při dalším dotazu je znovu vytvářet.


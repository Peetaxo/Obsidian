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
  - knowledge blok z raw zdroje
  - ověření tvrzení
  - syntéza více videí
nastroje:
  - Obsidian wiki odkazy
  - YAML frontmatter
  - lokální markdown
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Kompletní raw zdroje bez zkracování|Kompletní raw zdroje bez zkracování]]"
  - "[[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]"
  - "[[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Traceabilita wiki stránek ke zdrojům

## Kontext
Použij, když wiki stránka vzniká z raw zdroje nebo kombinuje více zdrojů. Každý praktický princip má být dohledatelný zpět k primárnímu materiálu.

## Princip
Každá zpracovaná wiki stránka má být dohledatelná zpět k raw zdroji. Odkazy na zdroj zvyšují kontrolovatelnost, důvěru a možnost pozdější revize.

## Heuristiky

Decision trigger:
- Když vytvoříš stránku z videa → přidej odkaz na raw přepis.
- Když syntéza kombinuje více zdrojů → uveď relevantní zdroje.
- Když odpověď cituje tvrzení → dohledávej ho přes raw nebo zpracovanou stránku.

Pravidla:
- Traceabilita snižuje riziko halucinací.
- Odkaz na raw zdroj zrychluje kontrolu tvrzení.
- Syntéza bez zdrojů snižuje důvěryhodnost wiki.

## Použij při
- tvorbě wiki stránek z videí
- aktualizaci tematických stránek
- odpovídání na dotazy s citacemi
- kontrole sporných tvrzení

## Použij s
- `zdroje` ve YAML frontmatteru
- sekcí `## Zdroje`
- raw linkem s cestou do `AI System/Raw`
- lintem, který hlídá chybějící zdroje

## Související
- [[AI System/Knowledge/Knowledge-Human/Kompletní raw zdroje bez zkracování|Kompletní raw zdroje bez zkracování]]
- [[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]

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
- Vytvořit znalostní stránku bez informace, odkud její tvrzení pochází.


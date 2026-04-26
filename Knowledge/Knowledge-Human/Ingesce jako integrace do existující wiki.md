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
  - nový raw zdroj
  - aktualizace existující znalosti
  - propojení více zdrojů
nastroje:
  - Obsidian
  - lokální markdown
  - Claude Code
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|Traceabilita wiki stránek ke zdrojům]]"
  - "[[AI System/Knowledge/Knowledge-Human/Persistentní wiki místo jednorázového RAG|Persistentní wiki místo jednorázového RAG]]"
  - "[[AI System/Knowledge/Knowledge-Human/Batch ingesce vyžaduje následný lint|Batch ingesce vyžaduje následný lint]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Ingesce jako integrace do existující wiki

## Kontext
Použij, když přidáváš nový článek, přepis, poznámky nebo jiný zdroj do znalostního systému. Cílem je integrovat poznatek do sítě, ne vytvořit izolovaný souhrn.

## Princip
Ingesce není jen vytvoření souhrnu. Nový zdroj má aktualizovat související stránky, vazby, rozpory a stav celé wiki.

## Heuristiky

Decision trigger:
- Když nový zdroj opakuje známé téma → aktualizuj existující stránku.
- Když nový zdroj přidává nový pojem → vytvoř nový znalostní blok.
- Když nový zdroj odporuje starému tvrzení → označ rozpor.

Pravidla:
- Ingesce má zasáhnout všechny relevantní stránky.
- Nový souhrn bez propojení snižuje hodnotu wiki.
- Rozpory zvyšují potřebu explicitní poznámky nebo revize.

## Použij při
- zpracování videí
- zpracování článků
- přidávání výzkumných zdrojů
- aktualizaci existující znalosti

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|odkazy na raw zdroje]]
- kandidáty na nové knowledge bloky
- sekcí `Související`
- následným lintem po větší dávce

## Související
- [[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|Traceabilita wiki stránek ke zdrojům]]
- [[AI System/Knowledge/Knowledge-Human/Persistentní wiki místo jednorázového RAG|Persistentní wiki místo jednorázového RAG]]
- [[AI System/Knowledge/Knowledge-Human/Batch ingesce vyžaduje následný lint|Batch ingesce vyžaduje následný lint]]

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
- Uložit nový zdroj jako izolovaný souhrn bez aktualizace souvisejících znalostí.


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
  - opakované otázky nad zdroji
  - syntéza z více zdrojů
  - dlouhodobá paměť projektu
nastroje:
  - Obsidian
  - lokální markdown
  - Claude Code
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]"
  - "[[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]"
  - "[[AI System/Knowledge/Knowledge-Human/Velký výzkum deleguj do specializované vrstvy|Velký výzkum deleguj do specializované vrstvy]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Persistentní wiki místo jednorázového RAG

## Kontext
Použij, když znalosti vznikají z více zdrojů a mají se opakovaně používat v čase. Wiki má ukládat syntézu, ne jen znovu vyhledávat fragmenty.

## Princip
LLM nemá při každém dotazu znovu skládat znalosti z raw fragmentů. Má průběžně udržovat persistentní wiki, kde se syntéza kumuluje.

## Heuristiky

Decision trigger:
- Když odpověď vyžaduje syntézu více zdrojů → vytvoř nebo aktualizuj wiki stránku.
- Když poznatek bude znovu použit → ulož ho jako trvalý znalostní blok.
- Když se dotaz vrací opakovaně → převeď odpověď na rozhodovací princip.

Pravidla:
- Persistentní wiki snižuje opakované vyvozování.
- Aktualizovaná syntéza zvyšuje konzistenci odpovědí.
- Izolované raw vyhledávání zvyšuje riziko ztráty kontextu.

## Použij při
- dlouhodobém výzkumu
- osobní znalostní bázi
- práci s opakovanými otázkami
- rozhodování nad více zdroji

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|ukládáním hodnotných dotazů]]
- [[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|traceabilitou ke zdrojům]]
- atomickými knowledge bloky
- indexem podle oblastí

## Související
- [[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]
- [[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]
- [[AI System/Knowledge/Knowledge-Human/Velký výzkum deleguj do specializované vrstvy|Velký výzkum deleguj do specializované vrstvy]]

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
- Spoléhat jen na RAG nad raw dokumenty bez ukládání výsledné syntézy.


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
  - browser-automation
  - ai-agent-workflow
  - tools-skills-mcp-cli
pouzij_kdy:
  - desktop aplikace bez API
  - export z UI nástroje
  - agent ovládá myš a klávesnici
nastroje:
  - Codex computer use
  - browser use
  - Canva
  - Finder
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]"
  - "[[AI System/Knowledge/Knowledge-Human/Přihlášené browser session izoluj a superviduj|Přihlášené browser session izoluj a superviduj]]"
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]"
zdroje:
  - "[[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]]"
  - "[[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]"
---

# Computer use omez jasnou hranicí úkolu

## Kontext
Použij, když agent musí ovládat desktop aplikaci nebo webové UI, které nemá vhodné API. Typicky jde o exporty, přesuny souborů, práci v Canvě, Finderu nebo podobných nástrojích.

## Princip
Computer use dávej agentovi jen s jasným cílem, hranicí a kontrolou výsledku. Je silné pro UI-only úkoly, ale rizikovější než API nebo lokální souborová operace.

## Heuristiky

Decision trigger:
- Když existuje spolehlivé API nebo CLI → preferuj ho před computer use.
- Když úkol vyžaduje klikání v desktop UI → použij computer use s konkrétním cílem.
- Když agent může provést nevratnou akci → spusť supervidovaný nebo potvrzovací režim.

Pravidla:
- Computer use zvyšuje dosah agenta mimo kód.
- UI automatizace je křehčí než API.
- Jasná hranice úkolu snižuje riziko nežádoucích akcí.

## Použij při
- exportu decku z Canvy
- stažení nebo přesunu souboru přes UI
- kontrole výsledku v desktop aplikaci
- propojení více aplikací bez API

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Přihlášené browser session izoluj a superviduj|supervizí přihlášených session]]
- screenshoty před a po akci
- read-only nebo minimálními oprávněními, kde to jde
- explicitním seznamem zakázaných akcí

## Související
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]
- [[AI System/Knowledge/Knowledge-Human/Přihlášené browser session izoluj a superviduj|Přihlášené browser session izoluj a superviduj]]
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]

## Zdroje
- [[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]]
- [[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Nechat agenta volně ovládat desktop bez jasného cíle, vizuální kontroly a hranice oprávnění.


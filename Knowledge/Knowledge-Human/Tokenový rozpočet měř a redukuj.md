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
  - tokeny-a-naklady
  - claude-code
  - tools-skills-mcp-cli
pouzij_kdy:
  - vysoká spotřeba tokenů
  - limity Claude Code
  - audit skills a MCP
nastroje:
  - Code Burn
  - Caveman
  - Claude Code
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]]"
  - "[[AI System/Knowledge/Knowledge-Human/Náklady modelu měř podle dokončené úlohy|Náklady modelu měř podle dokončené úlohy]]"
  - "[[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]]"
zdroje:
  - "[[AI System/Raw/YouTube/3 New Claude Code Repos Will 100x Your Next Project.md]]"
  - "[[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]"
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
  - "[[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]]"
---

# Tokenový rozpočet měř a redukuj

## Kontext
Použij, když agent naráží na limity, zpomalení nebo vysoké náklady. Nejprve zjisti, co spotřebu zvyšuje, a teprve potom zkracuj instrukce, skills nebo nástroje.

## Princip
Nejdřív zjisti, kam tokeny mizí, potom redukuj největší zdroje plýtvání. Častými viníky jsou přebujelé instrukce, staré skills, velké MCP servery a zbytečně dlouhé odpovědi.

## Heuristiky

Decision trigger:
- Když často narážíš na limity → audituj spotřebu tokenů.
- Když instrukční soubory bobtnají → zkrať je na rozhodovací pravidla.
- Když skill nebo MCP není potřeba → odpoj ho z aktivního kontextu.

Pravidla:
- Měření předchází optimalizaci.
- Kratší odpovědi snižují cenu i latenci.
- Nepoužívaný kontext zvyšuje náklady každé session.

## Použij při
- ladění Claude Code setupu
- správě skills a MCP nástrojů
- zkracování systémových instrukcí
- opakované agentické práci

## Použij s
- Code Burn pro audit spotřeby
- Caveman pro zkrácení odpovědí
- [[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI místo velkého MCP]]
- kontrolou, jaké memories a instrukce se přidávají do kontextu
- model routingem u rutinních úkolů

## Související
- [[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]]
- [[AI System/Knowledge/Knowledge-Human/Náklady modelu měř podle dokončené úlohy|Náklady modelu měř podle dokončené úlohy]]
- [[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]]

## Zdroje
- [[AI System/Raw/YouTube/3 New Claude Code Repos Will 100x Your Next Project.md]]
- [[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]
- [[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Řešit limity náhodným mazáním bez zjištění, co tokeny skutečně spotřebovává.

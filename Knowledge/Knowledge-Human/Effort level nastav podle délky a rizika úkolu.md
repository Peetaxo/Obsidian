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
  - coding-agenti
  - tokeny-a-naklady
  - ai-agent-workflow
pouzij_kdy:
  - nastavení reasoning effort
  - dlouhé agentické tasky
  - tool-heavy práce
nastroje:
  - Codex
  - Claude Code
  - reasoning effort
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Model routing podle náročnosti úkolu|Model routing podle náročnosti úkolu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Náklady modelu měř podle dokončené úlohy|Náklady modelu měř podle dokončené úlohy]]"
  - "[[AI System/Knowledge/Knowledge-Human/Paralelní agentické chaty řiď přes plán a stav|Paralelní agentické chaty řiď přes plán a stav]]"
zdroje:
  - "[[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]]"
  - "[[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]"
---

# Effort level nastav podle délky a rizika úkolu

## Kontext
Použij, když agentický nástroj dovoluje volit effort nebo reasoning úroveň. Cílem není vždy nejvyšší nastavení, ale vhodná úroveň pro délku, riziko a potřebu nástrojů.

## Princip
Nízký nebo střední effort používej pro rutinní a dobře ohraničené kroky. Vysoký effort nech pro dlouhé, rizikové, multi-file nebo silně tool-heavy úkoly.

## Heuristiky

Decision trigger:
- Když úkol trvá minuty a má jasný výstup → začni medium/low.
- Když úkol může běžet hodinu, zasahuje více částí systému nebo vyžaduje plánování → zvaž high.
- Když agent dělá zbytečně dlouhé úvahy u rutiny → sniž effort.

Pravidla:
- Vyšší effort zvyšuje šanci na lepší plán, ale také náklady a latenci.
- Dlouhý agentický task potřebuje přesnější zadání a stabilní intent.
- Effort je součást routingu, ne náhrada dobrého promptu.

## Použij při
- nastavování Codex/Claude Code tasku
- tvorbě dokumentů, decků a spreadsheetů
- multi-file refaktoru
- orchestraci více souběžných agentů

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Model routing podle náročnosti úkolu|model routingem]]
- [[AI System/Knowledge/Knowledge-Human/Náklady modelu měř podle dokončené úlohy|měřením ceny dokončené úlohy]]
- explicitním definition of done
- průběžnou kontrolou dlouhých tasků

## Související
- [[AI System/Knowledge/Knowledge-Human/Model routing podle náročnosti úkolu|Model routing podle náročnosti úkolu]]
- [[AI System/Knowledge/Knowledge-Human/Náklady modelu měř podle dokončené úlohy|Náklady modelu měř podle dokončené úlohy]]
- [[AI System/Knowledge/Knowledge-Human/Paralelní agentické chaty řiď přes plán a stav|Paralelní agentické chaty řiď přes plán a stav]]

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
- Používat nejvyšší effort pro každý dotaz a pak řešit pomalost nebo náklady bez měření.


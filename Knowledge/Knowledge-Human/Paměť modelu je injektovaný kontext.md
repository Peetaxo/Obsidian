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
  - ai-agent-workflow
  - tokeny-a-naklady
  - research-a-znalostni-baze
pouzij_kdy:
  - práce s AI memory
  - rozdíl mezi modelem a aplikací
  - vysvětlování tokenové spotřeby
nastroje:
  - ChatGPT memory
  - Claude memory
  - Claude Code
  - Codex
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]"
  - "[[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|Kontext drž mimo konkrétní AI nástroj]]"
  - "[[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]"
zdroje:
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
---

# Paměť modelu je injektovaný kontext

## Kontext
Použij, když řešíš, proč se stejný model chová jinak v ChatGPT, Claude, OpenRouteru nebo agentickém nástroji. Rozdíl často není v modelu, ale v tom, jaká aplikace mu před dotazem přidá kontext.

## Princip
Model se běžnou konverzací nedotrénuje. „Paměť“ aplikace jsou uložené informace, které se při další odpovědi znovu vloží do kontextového okna.

## Heuristiky

Decision trigger:
- Když stejný dotaz dává jinou odpověď v běžném a anonymním chatu → zkontroluj skrytý kontext.
- Když krátký dotaz spotřebuje hodně tokenů → hledej připojené memories, instrukce nebo nástroje.
- Když chceš přenositelnost paměti → ulož ji mimo uzavřenou aplikaci.

Pravidla:
- Aplikační memory zvyšuje personalizaci.
- Skrytý kontext může zvyšovat tokenovou spotřebu.
- Špatně uložená memory může opakovat nežádoucí preference.

## Použij při
- ladění rozdílů mezi chatovacími aplikacemi
- auditu personalizovaných odpovědí
- návrhu agentické paměti
- vysvětlování, proč samotný model není celý systém

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|tokenovým auditem]]
- anonymním/dočasným chatem jako kontrolním experimentem
- [[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|tool-agnostic správou kontextu]]
- lokální memory vrstvou pro agenty

## Související
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]
- [[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|Kontext drž mimo konkrétní AI nástroj]]
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]

## Zdroje
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Předpokládat, že model se v komerčním chatu průběžně dotrénoval na uživatele, a ignorovat aplikační kontext.


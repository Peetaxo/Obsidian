---
created: 2026-04-26
updated: 2026-04-26
typ: princip
puvod:
  - web
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - pracovni-hypoteza
stav: kandidat
duvera: medium
overeno_v_praxi: false
review_poznamka: "Pattern převzatý z webového návodu; nejvíc hodnoty má u Figma/code syncu, kde agent potřebuje přesné cíle změn."
oblast:
  - design-a-frontend
  - coding-agenti
  - tools-skills-mcp-cli
pouzij_kdy:
  - Figma to code sync
  - změny po sekcích
  - design tokens
nastroje:
  - Figma MCP
  - Figma Variables
  - Claude Code
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Figma používej jako vizuální mezivrstvu mezi kódem a designem|Figma používej jako vizuální mezivrstvu mezi kódem a designem]]"
  - "[[AI System/Knowledge/Knowledge-Human/Design reference převáděj na systémové specifikace|Design reference převáděj na systémové specifikace]]"
  - "[[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]"
zdroje:
  - "[[AI System/Raw/Web/Figma → Claude.md]]"
---

# Design změny synchronizuj po sekcích a přes pojmenované vrstvy

## Kontext
Použij, když agent čte Figma soubor a má propsat změny do kódu. Čím přesnější je rozsah a pojmenování, tím menší je riziko špatné interpretace.

## Princip
Synchronizuj design změny po konkrétních sekcích, používej smysluplné názvy vrstev a mapuj Figma variables na kódové design tokeny.

## Heuristiky

Decision trigger:
- Když Figma soubor obsahuje mnoho pages nebo frames → pracuj jen s konkrétním framem.
- Když agent neví, co se změnilo → popiš změny explicitně.
- Když používáš Figma variables → mapuj je na CSS custom properties nebo theme tokens.

Pravidla:
- Menší rozsah snižuje chyby při syncu.
- Pojmenované vrstvy zvyšují přesnost změn.
- Variables snižují drift mezi designem a kódem.

## Použij při
- propsání Figma změn do React/Tailwind UI
- redesignu hero, navigation nebo CTA sekce
- mapování barev, spacingu a typografie
- přípravě responzivní verze

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Figma používej jako vizuální mezivrstvu mezi kódem a designem|Figma/code workflow]]
- screenshotem aktuálního stavu
- CSS custom properties
- mobile framem ve Figmě

## Související
- [[AI System/Knowledge/Knowledge-Human/Figma používej jako vizuální mezivrstvu mezi kódem a designem|Figma používej jako vizuální mezivrstvu mezi kódem a designem]]
- [[AI System/Knowledge/Knowledge-Human/Design reference převáděj na systémové specifikace|Design reference převáděj na systémové specifikace]]
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]

## Zdroje
- [[AI System/Raw/Web/Figma → Claude.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: přesnostní pravidlo pro Figma MCP a code sync.

## Kdy nepoužít
- Když změna nemá vizuální dopad.
- Když design není ve Figmě strukturovaný a rychlejší je ruční úprava v kódu.

## Anti-pattern
- Poslat agentovi celý Figma soubor a čekat přesné propsání změn bez názvů vrstev, rozsahu a mobile stavu.

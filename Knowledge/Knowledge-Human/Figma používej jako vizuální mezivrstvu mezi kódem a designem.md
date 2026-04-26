---
created: 2026-04-26
updated: 2026-04-26
typ: workflow
puvod:
  - web
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - pracovni-hypoteza
stav: kandidat
duvera: medium
overeno_v_praxi: false
review_poznamka: "Pattern převzatý z webového návodu; použij jako kandidáta pro design-heavy weby, ne jako náhradu běžného frontend QA."
oblast:
  - design-a-frontend
  - ai-agent-workflow
  - tools-skills-mcp-cli
pouzij_kdy:
  - design-heavy landing page
  - iterace mezi kódem a Figmou
  - human design review
nastroje:
  - Figma MCP
  - Claude Code
  - Computer Use
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Design změny synchronizuj po sekcích a přes pojmenované vrstvy|Design změny synchronizuj po sekcích a přes pojmenované vrstvy]]"
  - "[[AI System/Knowledge/Knowledge-Human/Design reference převáděj na systémové specifikace|Design reference převáděj na systémové specifikace]]"
  - "[[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]"
zdroje:
  - "[[AI System/Raw/Web/Figma → Claude.md]]"
---

# Figma používej jako vizuální mezivrstvu mezi kódem a designem

## Kontext
Použij, když agent umí vytvořit frontend základ, ale finální vizuální ladění má proběhnout ve Figmě člověkem.

## Princip
Nech agenta vytvořit funkční základ v kódu, přenést vybraný UI rozsah do Figmy, nechat člověka upravit design a až potom promítnout změny zpět do kódu.

## Heuristiky

Decision trigger:
- Když je vizuální kvalita důležitější než rychlé vygenerování kódu → vlož do workflow Figmu.
- Když designer potřebuje upravit layout, barvy nebo typografii → upravuj ve Figmě, ne v promptu.
- Když změny z Figmy jdou zpět do kódu → ověř výsledek v browseru.

Pravidla:
- Figma mezivrstva zvyšuje kvalitu vizuální iterace.
- Kódový základ musí být funkční před přenosem do Figmy.
- Browser preview po návratu z Figmy snižuje riziko rozbité responzivity.

## Použij při
- tvorbě landing page
- redesignu webové sekce
- klientském design review
- ladění vizuálního systému nad existujícím kódem

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Design změny synchronizuj po sekcích a přes pojmenované vrstvy|pojmenovanými vrstvami a sekčním syncem]]
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|browser QA]]
- Figma MCP
- lokálním preview serverem

## Související
- [[AI System/Knowledge/Knowledge-Human/Design změny synchronizuj po sekcích a přes pojmenované vrstvy|Design změny synchronizuj po sekcích a přes pojmenované vrstvy]]
- [[AI System/Knowledge/Knowledge-Human/Design reference převáděj na systémové specifikace|Design reference převáděj na systémové specifikace]]
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]

## Zdroje
- [[AI System/Raw/Web/Figma → Claude.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: workflow pro design-heavy projekty s jasným QA krokem.

## Kdy nepoužít
- Když jde o jednoduchý interní UI bez design review.
- Když Figma změny nejsou lépe strukturované než zdrojový kód.

## Anti-pattern
- Přenést celý design do Figmy, upravit ho ručně a pak přeskočit browser kontrolu po propsání zpět do kódu.

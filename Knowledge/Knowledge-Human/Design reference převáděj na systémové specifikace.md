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
  - design-a-frontend
  - claude-code
  - tools-skills-mcp-cli
pouzij_kdy:
  - redesign podle reference
  - tvorba frontend promptu
  - extrakce motion a interaction states
nastroje:
  - Design Extract
  - Awesome Design MD
  - Claude Code
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]"
  - "[[AI System/Knowledge/Knowledge-Human/Brand styl drž jako sdílený skill|Brand styl drž jako sdílený skill]]"
  - "[[AI System/Knowledge/Knowledge-Human/Webový obsah předávej agentům jako čistá data|Webový obsah předávej agentům jako čistá data]]"
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|Nástroje přidávej až podle měřítka]]"
zdroje:
  - "[[AI System/Raw/YouTube/3 New Claude Code Repos Will 100x Your Next Project.md]]"
  - "[[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]"
  - "[[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]"
---

# Design reference převáděj na systémové specifikace

## Kontext
Použij, když agent navrhuje web nebo aplikaci podle existující vizuální inspirace. Reference musí skončit jako konkrétní pravidla, ne jako vágní estetický dojem.

## Princip
Vizuální reference má být převedena na konkrétní design systém: typografii, komponenty, motion jazyk, responzivní chování, interakční stavy a brand voice.

## Heuristiky

Decision trigger:
- Když zadání říká „udělej to jako tento web“ → extrahuj design pravidla.
- Když UI působí genericky → dodej agentovi konkrétní design systém.
- Když reference obsahuje animace → popiš motion jazyk, ne jen screenshot.

Pravidla:
- Konkrétní design pravidla zvyšují kvalitu UI výstupu.
- Motion a interaction states jsou součást designu.
- Šablona je startovní bod, ne finální značka.

## Použij při
- tvorbě landing page
- redesignu aplikace
- napodobení vizuálního stylu
- tvorbě promptu pro frontend agenta

## Použij s
- Design Extract nebo Awesome Design MD reportem
- [[AI System/Knowledge/Knowledge-Human/Brand styl drž jako sdílený skill|brand style skillem]]
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|browser QA]] pro ověření výsledku
- komponentovým checklistem
- screenshoty referencí a výsledku

## Související
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]
- [[AI System/Knowledge/Knowledge-Human/Brand styl drž jako sdílený skill|Brand styl drž jako sdílený skill]]
- [[AI System/Knowledge/Knowledge-Human/Webový obsah předávej agentům jako čistá data|Webový obsah předávej agentům jako čistá data]]
- [[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|Nástroje přidávej až podle měřítka]]

## Zdroje
- [[AI System/Raw/YouTube/3 New Claude Code Repos Will 100x Your Next Project.md]]
- [[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]
- [[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Zadávat agentovi jen vágní „ať to vypadá moderně“ bez konkrétních design parametrů.

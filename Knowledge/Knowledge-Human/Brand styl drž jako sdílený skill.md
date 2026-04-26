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
review_poznamka: "Pattern převzatý ze zdroje; použij jako kandidáta pro opakované vizuální výstupy a ověř proti brandu projektu."
oblast:
  - design-a-frontend
  - tools-skills-mcp-cli
  - ai-agent-workflow
pouzij_kdy:
  - opakované HTML dashboardy
  - konzistentní vizuální výstupy
  - brand manuál ve skillech
nastroje:
  - Claude skills
  - Markdown
  - HTML dashboards
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Design reference převáděj na systémové specifikace|Design reference převáděj na systémové specifikace]]"
  - "[[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Opakované výstupy bal do deliverable skillů|Opakované výstupy bal do deliverable skillů]]"
zdroje:
  - "[[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]"
---

# Brand styl drž jako sdílený skill

## Kontext
Použij, když agent opakovaně generuje vizuální výstupy: dashboardy, PDF, explainery, carousely nebo HTML reporty. Styl nemá být pokaždé znovu popsaný v promptu.

## Princip
Brand a vizuální pravidla drž jako samostatný style skill nebo markdown manuál, který ostatní výstupní skilly používají jako společný zdroj.

## Heuristiky

Decision trigger:
- Když agent generuje více výstupů ve stejném brandu → vytvoř sdílený style skill.
- Když výstupy vypadají nekonzistentně → odděl pravidla stylu od konkrétního úkolu.
- Když má projekt design systém → odkaž ho ze skillu místo kopírování do promptu.

Pravidla:
- Sdílený styl snižuje opakované promptování.
- Jedno místo pro barvy, typografii a komponenty zvyšuje konzistenci.
- Style skill nesmí nahrazovat kontrolu konkrétního výstupu.

## Použij při
- tvorbě HTML dashboardu
- generování PDF guide
- vizuálních explainerech
- konzistentních marketingových assetech

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Design reference převáděj na systémové specifikace|design specifikací]]
- [[AI System/Knowledge/Knowledge-Human/Opakované výstupy bal do deliverable skillů|deliverable skilly]]
- screenshoty referencí
- brand manuálem projektu

## Související
- [[AI System/Knowledge/Knowledge-Human/Design reference převáděj na systémové specifikace|Design reference převáděj na systémové specifikace]]
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]]
- [[AI System/Knowledge/Knowledge-Human/Opakované výstupy bal do deliverable skillů|Opakované výstupy bal do deliverable skillů]]

## Zdroje
- [[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu pro opakované brandované výstupy.

## Kdy nepoužít
- Když jde o jednorázový experiment bez potřeby konzistence.
- Když styl ještě není schválený a potřebuje exploraci.

## Anti-pattern
- Kopírovat stejný brand prompt do každého úkolu a nechat jednotlivé skilly driftovat.

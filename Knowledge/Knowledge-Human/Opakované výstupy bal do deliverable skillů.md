---
created: 2026-04-26
updated: 2026-04-26
typ: workflow
puvod:
  - youtube
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - pracovni-hypoteza
stav: kandidat
duvera: medium
overeno_v_praxi: false
review_poznamka: "Pattern převzatý ze zdroje; vhodný pro výstupy, které se opakují a mají stabilní formát."
oblast:
  - ai-agent-workflow
  - design-a-frontend
  - tools-skills-mcp-cli
pouzij_kdy:
  - opakovaný PDF guide
  - vizuální explainer
  - marketingový carousel
  - HTML dashboard
nastroje:
  - Claude skills
  - Markdown
  - HTML
  - image API
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Brand styl drž jako sdílený skill|Brand styl drž jako sdílený skill]]"
  - "[[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]"
zdroje:
  - "[[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]"
---

# Opakované výstupy bal do deliverable skillů

## Kontext
Použij, když agent často vytváří stejný typ artefaktu: PDF guide, vizuální explainer, carousel, dashboard nebo report.

## Princip
Opakovaný výstup převeď na deliverable skill, který definuje vstup, strukturu, styl, kontrolu kvality, formát souborů a hranici publikování.

## Heuristiky

Decision trigger:
- Když stejný výstup promptuješ opakovaně → vytvoř deliverable skill.
- Když výstup potřebuje brand styl → napoj ho na sdílený style skill.
- Když výstup publikuje ven → odděl tvorbu od schválení nebo plánování.

Pravidla:
- Deliverable skill zvyšuje konzistenci výstupu.
- Pevná struktura snižuje opakované ladění promptu.
- Publikační konektor zvyšuje riziko, pokud chybí kontrola.

## Použij při
- tvorbě PDF lead magnetu
- vizuálním vysvětlení komplexního tématu
- generování carouselů
- interních HTML reportech

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Brand styl drž jako sdílený skill|brand style skillem]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|automation až po testu]]
- [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|publikačním konektorem]]
- kontrolním checklistem výstupu

## Související
- [[AI System/Knowledge/Knowledge-Human/Brand styl drž jako sdílený skill|Brand styl drž jako sdílený skill]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]
- [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]

## Zdroje
- [[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pattern pro opakované artefakty, ne pro jednorázové poznámky.

## Kdy nepoužít
- Když výstup nemá stabilní formát.
- Když je rychlejší jednorázový prompt bez budoucího opakování.

## Anti-pattern
- Znovu vymýšlet prompt pro každý PDF, carousel nebo dashboard místo stabilního deliverable skillu.

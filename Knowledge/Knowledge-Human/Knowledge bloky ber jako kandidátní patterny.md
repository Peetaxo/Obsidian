---
created: 2026-04-26
updated: 2026-04-26
typ: princip
puvod:
  - konverzace
  - agenticka-synteza
povaha:
  - systemove-pravidlo-vaultu
  - review-proces
stav: overeno
duvera: high
overeno_v_praxi: true
review_poznamka: "Lokální pravidlo pro práci s touto knowledge bází; zavedeno jako ochrana proti nekritickému přebírání YouTube patternů."
oblast:
  - research-a-znalostni-baze
  - ai-agent-workflow
pouzij_kdy:
  - výběr relevantních patternů
  - review knowledge báze
  - prevence knowledge debt
nastroje:
  - Obsidian
  - YAML frontmatter
  - lint checklist
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]"
  - "[[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]"
  - "[[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]]"
zdroje:
  - "[[AI System/log.md]]"
---

# Knowledge bloky ber jako kandidátní patterny

## Kontext
Použij vždy, když agent vybírá knowledge bloky pro konkrétní úkol. Většina bloků vzniká ze zdrojů od jiných tvůrců, takže má sloužit jako inspirace a rozhodovací materiál, ne jako automaticky správný postup.

## Princip
Knowledge blok je pracovní hypotéza: nejdřív posuď kontext, riziko a režii, potom ho teprve aplikuj. Pattern se stává silnějším pravidlem až po ověření v praxi.

## Heuristiky

Decision trigger:
- Když blok má `stav: kandidat` → použij ho jen po explicitním posouzení vhodnosti.
- Když se pattern osvědčí v projektu → aktualizuj `overeno_v_praxi`, `stav` a review poznámku.
- Když se pattern opakovaně nehodí → označ ho jako slabý, uprav omezení nebo navrhni archivaci.

Pravidla:
- Kandidátní patterny rozšiřují možnosti, ale nesmí řídit práci naslepo.
- Ověření v praxi zvyšuje důvěru víc než popularita videa.
- Neužitečné bloky vytvářejí knowledge debt a mají být sloučeny, zúženy nebo vyřazeny.

## Použij při
- vývoji webové aplikace
- výběru agentického workflow
- pravidelném lintu knowledge báze
- rozhodování, jestli nový poznatek stojí za samostatný blok

## Použij s
- `stav: kandidat | overeno | slabe | archivovat`
- `duvera: low | medium | high`
- `overeno_v_praxi: true | false`
- sekcí `Review`
- sekcí `Kdy nepoužít`

## Související
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]
- [[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]
- [[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]]

## Zdroje
- [[AI System/log.md]]

## Review
- Stav: Ověřeno v tomto vaultu.
- Důvěra: high.
- Ověření v praxi: Použito jako nová metadata a review sekce napříč knowledge bází.
- Použij jako: základní pravidlo pro aplikaci cizích patternů v praxi.

## Kdy nepoužít
- Když jde o čistě faktický zdroj, který nemá být aplikován jako workflow nebo rozhodovací pravidlo.
- Když už existuje tvrdé projektové rozhodnutí, které má před kandidátním patternem vyšší prioritu.

## Anti-pattern
- Zacházet s každým YouTube tipem jako s ověřenou best practice bez testu v konkrétním projektu.


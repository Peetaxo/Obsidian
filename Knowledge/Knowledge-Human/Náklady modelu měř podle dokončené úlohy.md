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
  - tokeny-a-naklady
  - ai-agent-workflow
  - coding-agenti
pouzij_kdy:
  - výběr modelu
  - porovnání nákladů
  - dlouhé agentické úkoly
nastroje:
  - Codex
  - Claude Code
  - model eval
  - token audit
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]"
  - "[[AI System/Knowledge/Knowledge-Human/Model routing podle náročnosti úkolu|Model routing podle náročnosti úkolu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]]"
zdroje:
  - "[[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]]"
---

# Náklady modelu měř podle dokončené úlohy

## Kontext
Použij, když porovnáváš modely nebo effort nastavení pro reálnou práci. Cena za milion tokenů sama o sobě nestačí, protože dražší model může úkol dokončit rychleji, s méně retry a s menším celkovým kontextem.

## Princip
Model hodnoť podle kvality výsledku, času dokončení, počtu retry a celkové tokenové spotřeby na dokončenou úlohu. Ne podle jednotkové ceny tokenu izolovaně.

## Heuristiky

Decision trigger:
- Když nový model vypadá dražší → otestuj ho na stejné úloze proti levnějšímu modelu.
- Když levný model potřebuje mnoho oprav → započítej retry do ceny.
- Když výstup vyžaduje lidské přepracování → počítej to jako náklad, ne jako úsporu.

Pravidla:
- Vyšší cena tokenu nemusí znamenat vyšší cenu úlohy.
- Retry zvyšují cenu, latenci i lidský dohled.
- Kvalita, čas a tokeny musí být měřené na stejném zadání.

## Použij při
- výběru modelu pro reporty, dokumenty nebo coding úkoly
- rozhodování mezi low/medium/high effort
- benchmarku agentů pro firemní workflow
- optimalizaci nákladů na dlouhé tasky

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|tokenovým auditem]]
- side-by-side evalem stejného promptu
- měřením času do použitelného výsledku
- checklistem kvality výstupu

## Související
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]
- [[AI System/Knowledge/Knowledge-Human/Model routing podle náročnosti úkolu|Model routing podle náročnosti úkolu]]
- [[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]]

## Zdroje
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
- Vybrat model jen podle nejnižší ceny za token a ignorovat kvalitu, čas, retry a lidské opravy.


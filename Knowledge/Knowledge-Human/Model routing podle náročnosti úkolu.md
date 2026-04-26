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
  - claude-code
  - tokeny-a-naklady
  - ai-agent-workflow
pouzij_kdy:
  - optimalizace nákladů
  - různé náročnosti úkolů
  - tool-heavy práce
nastroje:
  - Claude Code Router
  - Claude Code
  - levnější modely
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]"
  - "[[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Náklady modelu měř podle dokončené úlohy|Náklady modelu měř podle dokončené úlohy]]"
zdroje:
  - "[[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]"
  - "[[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]]"
---

# Model routing podle náročnosti úkolu

## Kontext
Použij, když chceš snížit náklady agentické práce bez ztráty kvality u náročných úkolů. Routing je užitečný až po základním [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|měření tokenů]].

## Princip
Ne každý krok vyžaduje nejsilnější model. Jednoduché úkoly směruj na levnější modely, komplexní refaktory a tool-heavy práci nech na silném modelu.

## Heuristiky

Decision trigger:
- Když úkol nevyžaduje hluboké uvažování → použij levnější model.
- Když úkol zahrnuje multi-file refaktor nebo složité tool calling → použij silný model.
- Když routing rozbíjí tools nebo skills → vrať se na kompatibilní backend.

Pravidla:
- Routing snižuje cenu rutinních kroků.
- Slabší modely mohou selhat na tool calling a komplexních změnách.
- Cena, latence a spolehlivost jsou trade-off.

## Použij při
- opakovaných jednoduchých úkolech
- generování drobných souborů
- agentických workflow s různou náročností
- optimalizaci nákladů Claude Code setupu

## Použij s
- Claude Code Routerem
- tokenovým auditem před změnou routingu
- effort nastavením podle rizika úkolu
- fallbackem na silný model
- oddělením rutinních a rizikových kroků

## Související
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]
- [[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]]
- [[AI System/Knowledge/Knowledge-Human/Náklady modelu měř podle dokončené úlohy|Náklady modelu měř podle dokončené úlohy]]

## Zdroje
- [[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]]
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
- Posílat multi-file refaktor nebo citlivé tool-heavy operace na náhodný levný model.

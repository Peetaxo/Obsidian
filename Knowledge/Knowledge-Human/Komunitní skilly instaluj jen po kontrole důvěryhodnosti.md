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
review_poznamka: "Bezpečnostní pattern převzatý ze zdroje; před použitím přizpůsob konkrétním oprávněním a prostředí."
oblast:
  - tools-skills-mcp-cli
  - ai-agent-workflow
pouzij_kdy:
  - instalace komunitního skillu
  - skill directory
  - neznámý uploader
nastroje:
  - Claude skills
  - skill directories
  - plugins
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]"
  - "[[AI System/Knowledge/Knowledge-Human/Skill katalog audituj pravidelně|Skill katalog audituj pravidelně]]"
zdroje:
  - "[[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]"
---

# Komunitní skilly instaluj jen po kontrole důvěryhodnosti

## Kontext
Použij, když agent nebo člověk hledá skill v komunitním katalogu. Skill je instrukce, která může ovlivnit práci agenta, nástroje i soubory.

## Princip
Před instalací komunitního skillu zkontroluj autora, reputaci, počet použití, rozsah oprávnění a čitelnost instrukcí.

## Heuristiky

Decision trigger:
- Když skill pochází z neznámého zdroje → neinstaluj ho bez kontroly.
- Když skill žádá široká oprávnění → zkontroluj scope a izolaci.
- Když existuje skill od důvěryhodného autora → preferuj ho před anonymním.

Pravidla:
- Komunitní katalog zrychluje hledání skillů.
- Neznámý skill zvyšuje bezpečnostní riziko.
- Menší oprávnění snižují dopad škodlivého nebo chybného skillu.

## Použij při
- instalaci skillu z veřejného katalogu
- hledání náhrady za vlastní workflow
- review agentického setupu
- auditu pluginů a skillů

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|minimálním oprávněním]]
- [[AI System/Knowledge/Knowledge-Human/Skill katalog audituj pravidelně|skill auditem]]
- sandboxem nebo testovacím projektem
- ručním přečtením `SKILL.md`

## Související
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]
- [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]
- [[AI System/Knowledge/Knowledge-Human/Skill katalog audituj pravidelně|Skill katalog audituj pravidelně]]

## Zdroje
- [[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: bezpečnostní default při práci s cizími skilly.

## Kdy nepoužít
- Když skill vznikl interně a prošel review.
- Když běží v izolovaném experimentu bez přístupu k citlivým datům.

## Anti-pattern
- Instalovat anonymní skill jen proto, že řeší aktuální problém rychleji než vlastní postup.

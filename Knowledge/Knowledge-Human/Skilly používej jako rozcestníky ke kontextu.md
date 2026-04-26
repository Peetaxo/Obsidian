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
  - tools-skills-mcp-cli
  - ai-agent-workflow
  - design-a-frontend
pouzij_kdy:
  - opakované workflow se stejným kontextem
  - brand manuál nebo projektová paměť
  - agent se má sám zorientovat
nastroje:
  - Claude skills
  - Codex skills
  - Markdown
  - CLAUDE.md
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]"
  - "[[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Skill katalog audituj pravidelně|Skill katalog audituj pravidelně]]"
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]"
zdroje:
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
  - "[[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]"
  - "[[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]"
---

# Skilly používej jako rozcestníky ke kontextu

## Kontext
Použij, když agent opakovaně potřebuje stejný projektový, brandový nebo workflow kontext. Skill nemusí obsahovat všechna data; často má hlavně říct, kde je agent najde.

## Princip
Skill může fungovat jako navigační mapa ke kontextu: kdy ho použít, jaké soubory načíst, jaké nástroje otevřít a jaký výstup očekávat.

## Heuristiky

Decision trigger:
- Když agent u stejného typu úkolu pokaždé hledá stejné podklady → vytvoř skill-rozcestník.
- Když by vložení všeho kontextu zahltilo okno → dej agentovi cestu, ne celý obsah.
- Když existuje brand manuál, předchozí výstupy nebo projektová pravidla → odkaž je ze skillu.

Pravidla:
- Skill snižuje opakované vysvětlování kontextu.
- Rozcestník snižuje potřebu cpát všechno do promptu.
- Kontextové skilly potřebují pravidelnou údržbu odkazů.

## Použij při
- tvorbě grafiky podle brand manuálu
- práci s design systémem
- opakovaných projektových reportech
- agentickém onboardingu do projektu

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|přenositelnou kontextovou vrstvou]]
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|nástroji pro získání kontextu]]
- [[AI System/Knowledge/Knowledge-Human/Skill katalog audituj pravidelně|katalogem a auditem skillů]]
- projektovým `README`, `CLAUDE.md` nebo `AGENTS.md`
- lintem neplatných odkazů ve skillech

## Související
- [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]
- [[AI System/Knowledge/Knowledge-Human/Skill katalog audituj pravidelně|Skill katalog audituj pravidelně]]
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]

## Zdroje
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]
- [[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]
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
- Dávat do skillu celý knowledge dump místo krátké instrukce, kdy a odkud načíst relevantní kontext.

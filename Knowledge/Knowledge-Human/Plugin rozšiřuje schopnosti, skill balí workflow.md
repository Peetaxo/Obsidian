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
pouzij_kdy:
  - volba mezi pluginem a skillem
  - integrace externí služby
  - reusable workflow
nastroje:
  - Codex plugins
  - Claude skills
  - MCP
  - API
  - Zapier MCP
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Komunitní skilly instaluj jen po kontrole důvěryhodnosti|Komunitní skilly instaluj jen po kontrole důvěryhodnosti]]"
  - "[[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]"
zdroje:
  - "[[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]"
  - "[[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]"
---

# Plugin rozšiřuje schopnosti, skill balí workflow

## Kontext
Použij, když se rozhoduješ, jestli agent potřebuje nový nástroj, konektor, MCP nebo jen opakovatelný postup. Názvosloví se mezi nástroji liší, ale role je prakticky rozlišitelná.

## Princip
Plugin nebo MCP přidává agentovi novou schopnost přístupu ke službě. Skill balí konkrétní způsob, jak tuto schopnost použít pro opakovaný úkol.

## Heuristiky

Decision trigger:
- Když agent nemá přístup ke službě → potřebuje plugin, MCP nebo API integraci.
- Když agent přístup má, ale pokaždé neví postup → vytvoř skill.
- Když workflow kombinuje více nástrojů → skill popíše pořadí a výstup.

Pravidla:
- Plugin řeší schopnost.
- Skill řeší postup.
- Dobrý skill může obalit plugin, MCP nebo API do stabilního workflow.

## Použij při
- napojení kalendáře, emailu, Figmy nebo Typefully
- tvorbě YouTube researcher workflow
- balení MCP do použitelného agentického postupu
- vysvětlování rozdílu mezi tools, skills a plugins

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|kontextovými nástroji]]
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|skilly jako rozcestníky]]
- [[AI System/Knowledge/Knowledge-Human/Komunitní skilly instaluj jen po kontrole důvěryhodnosti|kontrolou důvěryhodnosti cizích skillů]]
- testem minimálních oprávnění
- dokumentací vstupu, výstupu a fallbacku

## Související
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]]
- [[AI System/Knowledge/Knowledge-Human/Komunitní skilly instaluj jen po kontrole důvěryhodnosti|Komunitní skilly instaluj jen po kontrole důvěryhodnosti]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]

## Zdroje
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
- Instalovat další plugin, když problém je jen chybějící postup, nebo psát skill, když agent vůbec nemá potřebný přístup.

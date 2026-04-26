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
  - tools-skills-mcp-cli
  - research-a-znalostni-baze
  - ai-agent-workflow
pouzij_kdy:
  - volba nového toolingu
  - škálování wiki nebo workflow
  - rozhodování o MCP/pluginu
nastroje:
  - Obsidian
  - Dataview
  - MCP
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]"
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
---

# Nástroje přidávej až podle měřítka

## Kontext
Použij při rozhodování, jestli znalostní systém potřebuje vyhledávač, pluginy, frontmatter nebo další tooling. Začni jednoduchou strukturou a přidávej nástroje až podle reálného limitu.

## Princip
Začni jednoduchou markdown wiki a indexem. Pokročilé nástroje přidávej až tehdy, když velikost nebo typ práce překročí možnosti jednoduché struktury.

## Heuristiky

Decision trigger:
- Když index stačí najít relevantní stránky → nepřidávej další vyhledávací vrstvu.
- Když wiki naroste na stovky stránek → zvaž lokální search nebo MCP nástroj.
- Když potřebuješ dynamické přehledy → zvaž frontmatter a Dataview.

Pravidla:
- Předčasný tooling zvyšuje komplexitu.
- Jednoduchý markdown snižuje tření při startu.
- Nástroje mají řešit konkrétní limit, ne abstraktní možnost.

## Použij při
- zakládání nové wiki
- škálování existující wiki
- rozhodování o Obsidian pluginech
- přidávání CLI nebo MCP nástrojů

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|lokálním markdownem]]
- indexem jako prvním navigačním nástrojem
- frontmatterem až ve chvíli, kdy pomáhá filtrovat
- měřením nákladů nového nástroje

## Související
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]]

## Zdroje
- [[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Budovat složité vyhledávání nebo metadata dřív, než wiki narazí na konkrétní problém.

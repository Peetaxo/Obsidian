---
updated: 2026-04-26
created: 2026-04-26
typ: princip
puvod:
  - youtube
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - overene-v-tomto-vaultu
stav: overeno
duvera: high
overeno_v_praxi: true
review_poznamka: "Pattern je převzatý ze zdrojů a zatím ověřený hlavně při správě tohoto vaultu; mimo tento kontext ho znovu posuď."
oblast:
  - research-a-znalostni-baze
  - tools-skills-mcp-cli
pouzij_kdy:
  - lidské procházení wiki
  - graph view a canvas
  - lokální knowledge base
nastroje:
  - Obsidian
  - Graph view
  - Web Clipper
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]"
  - "[[AI System/Knowledge/Knowledge-Human/LLM jako správce wiki člověk jako kurátor|LLM jako správce wiki člověk jako kurátor]]"
  - "[[AI System/Knowledge/Knowledge-Human/Index a log jako navigační paměť|Index a log jako navigační paměť]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Obsidian jako UI nad markdown wiki

## Kontext
Použij, když chce člověk znalostní bázi nejen generovat agentem, ale i pohodlně procházet. Obsidian dává lokálním markdown souborům lidské rozhraní.

## Princip
Obsidian funguje jako uživatelské rozhraní nad lokální markdown wiki. Agent spravuje soubory, člověk prochází odkazy, graf, canvas a obsah.

## Heuristiky

Decision trigger:
- Když chceš vizualizovat vazby → použij Graph view.
- Když chceš rychle importovat webový obsah → použij Web Clipper.
- Když chceš pracovat s prezentací z wiki → zvaž Marp.

Pravidla:
- Obsidian zvyšuje čitelnost lokální wiki.
- Graph view pomáhá odhalit huby, duplicity a osiřelé stránky.
- Web Clipper zrychluje ukládání raw zdrojů.

## Použij při
- procházení znalostní báze
- kontrole propojení témat
- ukládání článků a YouTube transkriptů
- tvorbě prezentací z markdown obsahu

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|lokální markdown wiki]]
- wiki odkazy a aliasy
- indexem jako vstupním bodem
- graph view pro audit propojení

## Související
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]
- [[AI System/Knowledge/Knowledge-Human/LLM jako správce wiki člověk jako kurátor|LLM jako správce wiki člověk jako kurátor]]
- [[AI System/Knowledge/Knowledge-Human/Index a log jako navigační paměť|Index a log jako navigační paměť]]

## Zdroje
- [[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]

## Review
- Stav: Ověřeno v tomto vaultu.
- Důvěra: high.
- Ověření v praxi: Použito při organizaci a údržbě AI System knowledge báze.
- Použij jako: stabilnější lokální pravidlo, ale při jiném projektu znovu ověř kontext.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Používat markdown wiki jen jako skrytou databázi bez lidsky pohodlného rozhraní.


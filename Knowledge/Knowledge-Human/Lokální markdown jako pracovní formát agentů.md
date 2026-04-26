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
  - ai-agent-workflow
pouzij_kdy:
  - agentická knowledge base
  - časté čtení a editace znalostí
  - volba mezi lokálním souborem a vzdáleným nástrojem
nastroje:
  - Markdown
  - Obsidian
  - git
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Obsidian jako UI nad markdown wiki|Obsidian jako UI nad markdown wiki]]"
  - "[[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]]"
  - "[[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|Kontext drž mimo konkrétní AI nástroj]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
---

# Lokální markdown jako pracovní formát agentů

## Kontext
Použij, když vybíráš úložiště znalostí, se kterým má pravidelně pracovat AI agent. Lokální soubory snižují tření oproti nástrojům, které musí agent ovládat přes vzdálenou integraci.

## Princip
Lokální markdown soubory jsou pro agenty rychlejší a jednodušší než vzdálené nástroje ovládané přes MCP nebo API. Wiki má být čitelná člověkem a přímo editovatelná agentem.

## Heuristiky

Decision trigger:
- Když agent potřebuje často číst a upravovat znalosti → preferuj lokální markdown.
- Když práce přes MCP zpomaluje workflow → přesuň pracovní vrstvu do souborů.
- Když chceš verzování a přenositelnost → použij git nad markdown vaultem.

Pravidla:
- Lokální soubory snižují latenci agentické práce.
- Markdown snižuje závislost na konkrétní aplikaci.
- Vzdálené databáze zvyšují integrační tření.

## Použij při
- volbě mezi Obsidianem a Notionem
- návrhu agentické knowledge base
- práci s velkým množstvím poznámek
- nastavování lokálního workflow s gitem

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Obsidian jako UI nad markdown wiki|Obsidianem jako UI]]
- git verzováním
- YAML frontmatterem
- wiki odkazy mezi atomickými bloky
- [[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|tool-agnostic správou kontextu]]

## Související
- [[AI System/Knowledge/Knowledge-Human/Obsidian jako UI nad markdown wiki|Obsidian jako UI nad markdown wiki]]
- [[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]]
- [[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|Kontext drž mimo konkrétní AI nástroj]]

## Zdroje
- [[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]

## Review
- Stav: Ověřeno v tomto vaultu.
- Důvěra: high.
- Ověření v praxi: Použito při organizaci a údržbě AI System knowledge báze.
- Použij jako: stabilnější lokální pravidlo, ale při jiném projektu znovu ověř kontext.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Stavět primární pracovní znalostní vrstvu v nástroji, ke kterému agent přistupuje pomalu nebo křehce.

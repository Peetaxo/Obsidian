# Lokální markdown jako pracovní formát agentů

## Trigger
- agentická knowledge base
- časté čtení a editace znalostí
- Volíš mezi lokálním souborem a vzdáleným nástrojem

## Core rule
- Pokud agent opakovaně čte a upravuje znalosti → používej lokální markdown jako pracovní vrstvu

## Decision rules
- Pokud agent potřebuje číst a upravovat znalosti → použij lokální markdown
- Pokud práce přes MCP zpomaluje workflow → přesuň pracovní vrstvu do souborů
- Pokud chceš verzování a přenositelnost → použij git nad markdown vaultem
- Lokální soubory snižují latenci agentické práce
- Markdown snižuje závislost na konkrétní aplikaci
- Vzdálené databáze zvyšují integrační tření

## Use for
- volbě mezi Obsidianem a Notionem
- návrhu agentické knowledge base
- práci s velkým množstvím poznámek
- nastavování lokálního workflow s gitem

## Avoid
- Stavět primární pracovní znalostní vrstvu v nástroji, ke kterému agent přistupuje pomalu nebo křehce


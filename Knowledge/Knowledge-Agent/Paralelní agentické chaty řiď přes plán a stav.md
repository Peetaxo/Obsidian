# Paralelní agentické chaty řiď přes plán a stav

## Trigger
- více souběžných agentických tasků
- dlouhé běhy agentů
- multitasking v Codexu nebo Claude Code
- Codex

## Core rule
- Pokud úkoly nemají jasné vlastnictví a společný plán → neparalelizuj je

## Decision rules
- Pokud projekt má více nezávislých výstupů → rozděl je do samostatných chatů
- Pokud úkoly sahají do stejných souborů → nejdřív stanov pořadí nebo ownership
- Pokud agent běží dlouho → přepni pozornost na jiný připravený task a vrať se přes checklist
- Paralelní chaty zvyšují throughput
- Sdílený plán snižuje ztrátu kontextu mezi chaty
- Neřízené paralelní editace zvyšují riziko konfliktů

## Use for
- souběžné tvorbě appky, webu, decku a videa
- dlouhých research nebo build taskech
- práci nad jedním projektovým adresářem
- iteraci marketingových assetů a produktu současně

## Avoid
- Spustit mnoho agentů nad stejnými soubory bez plánu, pojmenování chatů a vlastnictví výstupů


# Computer use omez jasnou hranicí úkolu

## Trigger
- desktop aplikace bez API
- export z UI nástroje
- Agent ovládá myš a klávesnici

## Core rule
- Pokud existuje spolehlivé API nebo CLI → použij ho před computer use

## Decision rules
- Pokud existuje spolehlivé API nebo CLI → použij ho před computer use
- Pokud úkol vyžaduje klikání v desktop UI → použij computer use s konkrétním cílem
- Pokud agent provést nevratnou akci → spusť supervidovaný nebo potvrzovací režim
- Computer use zvyšuje dosah agenta mimo kód
- UI automatizace je křehčí než API
- Jasná hranice úkolu snižuje riziko nežádoucích akcí

## Use for
- exportu decku z Canvy
- stažení nebo přesunu souboru přes UI
- kontrole výsledku v desktop aplikaci
- propojení více aplikací bez API

## Avoid
- Nechat agenta volně ovládat desktop bez jasného cíle, vizuální kontroly a hranice oprávnění


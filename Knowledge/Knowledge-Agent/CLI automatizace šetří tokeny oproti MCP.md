# CLI vs MCP pro efektivní automatizaci

## Trigger
- volba mezi MCP a CLI
- úzká nebo opakovaná automatizace
- MCP přidává vysoký context overhead
- potřeba lokální kontroly nebo skriptování

## Core rule
- Pokud úkol řeší jeden příkaz nebo skript → použij CLI místo MCP

## Decision rules
- Pokud úloha = 1 nástroj, 1 akce → použij CLI
- Pokud úloha = opakovaný postup → napiš CLI skript
- Pokud MCP přidává mnoho nástrojů → použij CLI
- Pokud řešení lze vyjádřit jako shell příkaz → nepoužívej AI workflow
- Pokud úloha = multi-step integrace → použij MCP
- MCP zvyšuje tokenovou režii
- CLI skript zvyšuje reprodukovatelnost

## Use for
- build / test / lint
- web scraping
- browser automation
- shell skripty
- datové transformace

## Avoid
- MCP pro úkol řešitelný jedním příkazem
- MCP pro deterministické lokální operace
- dlouhé prompty místo skriptů


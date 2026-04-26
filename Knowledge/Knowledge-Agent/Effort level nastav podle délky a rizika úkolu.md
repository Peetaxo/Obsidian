# Effort level nastav podle délky a rizika úkolu

## Trigger
- nastavení reasoning effort
- dlouhé agentické tasky
- tool-heavy práce
- Codex

## Core rule
- Pokud úkol zasahuje více částí systému nebo vyžaduje plánování → použij vyšší effort

## Decision rules
- Pokud úkol trvá minuty a má jasný výstup → začni medium/low
- Pokud úkol běží dlouho, zasahuje více částí systému nebo vyžaduje plánování → použij high
- Pokud agent dělá zbytečně dlouhé úvahy u rutiny → sniž effort
- Vyšší effort zvyšuje šanci na lepší plán, ale také náklady a latenci
- Dlouhý agentický task potřebuje přesnější zadání a stabilní intent
- Effort je součást routingu, ne náhrada dobrého promptu

## Use for
- nastavování Codex/Claude Code tasku
- tvorbě dokumentů, decků a spreadsheetů
- multi-file refaktoru
- orchestraci více souběžných agentů

## Avoid
- Používat nejvyšší effort pro každý dotaz a pak řešit pomalost nebo náklady bez měření


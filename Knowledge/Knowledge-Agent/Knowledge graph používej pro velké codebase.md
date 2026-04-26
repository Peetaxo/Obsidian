# Knowledge graph používej pro velké codebase

## Trigger
- velké codebase
- opakované dotazy nad repozitářem
- snížení tokenů při onboardingu agenta

## Core rule
- Pokud repo generuje opakované onboarding dotazy → vytvoř dotazovatelný graph nebo index vztahů

## Decision rules
- Pokud repo má stovky souborů → použij knowledge graph
- Pokud agent opakovaně pálí tokeny na mapování codebase → vytvoř index vztahů
- Pokud repo má méně než několik desítek souborů → graph overhead nepoužívej
- Knowledge graph snižuje náklady na opakované otázky nad velkým repem
- Hub uzly pomáhají najít architektonicky důležité soubory
- Malý projekt nepotřebuje těžkou indexační vrstvu

## Use for
- orientaci ve velkém repozitáři
- onboarding dotazech nad codebase
- hledání architektonických závislostí
- opakované práci agenta ve stejném projektu

## Avoid
- Nechat agenta v každé nové session znovu procházet velké repo bez uložené mapy vztahů


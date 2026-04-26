# Tokenový rozpočet měř a redukuj

## Trigger
- Vysoká spotřeba tokenů
- limity Claude Code
- audit skills a MCP

## Core rule
- Pokud narážíš na limity → změř spotřebu a redukuj největší zdroje context overheadu

## Decision rules
- Pokud narážíš na limity → audituj spotřebu tokenů
- Pokud instrukční soubory bobtnají → zkrať je na rozhodovací pravidla
- Pokud skill nebo MCP není potřeba → odpoj ho z aktivního kontextu
- Měření předchází optimalizaci
- Kratší odpovědi snižují cenu i latenci
- Nepoužívaný kontext zvyšuje náklady každé session

## Use for
- ladění Claude Code setupu
- správě skills a MCP nástrojů
- zkracování systémových instrukcí
- opakované agentické práci

## Avoid
- Řešit limity náhodným mazáním bez zjištění, co tokeny skutečně spotřebovává


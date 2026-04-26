# Skilly používej jako rozcestníky ke kontextu

## Trigger
- opakované workflow se stejným kontextem
- brand manuál nebo projektová paměť
- Agent se má sám zorientovat

## Core rule
- Pokud agent opakovaně hledá stejný kontext → vytvoř skill-rozcestník

## Decision rules
- Pokud agent u stejného typu úkolu pokaždé hledá stejné podklady → vytvoř skill-rozcestník
- Pokud by vložení všeho kontextu zahltilo okno → dej agentovi cestu, ne celý obsah
- Pokud existuje brand manuál, předchozí výstupy nebo projektová pravidla → odkaž je ze skillu
- Skill snižuje opakované vysvětlování kontextu
- Rozcestník snižuje potřebu cpát všechno do promptu
- Kontextové skilly potřebují pravidelnou údržbu odkazů

## Use for
- tvorbě grafiky podle brand manuálu
- práci s design systémem
- opakovaných projektových reportech
- agentickém onboardingu do projektu

## Avoid
- Dávat do skillu celý knowledge dump místo krátké instrukce, kdy a odkud načíst relevantní kontext


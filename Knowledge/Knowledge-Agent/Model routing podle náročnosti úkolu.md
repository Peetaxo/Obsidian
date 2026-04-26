# Model routing podle náročnosti úkolu

## Trigger
- optimalizace nákladů
- různé náročnosti úkolů
- tool-heavy práce

## Core rule
- Pokud úkol nevyžaduje hluboké uvažování ani složité tool calling → použij levnější model

## Decision rules
- Pokud úkol nevyžaduje hluboké uvažování → použij levnější model
- Pokud úkol zahrnuje multi-file refaktor nebo složité tool calling → použij silný model
- Pokud routing rozbíjí tools nebo skills → vrať se na kompatibilní backend
- Routing snižuje cenu rutinních kroků
- Slabší model zvyšuje riziko selhání u tool calling a komplexních změn
- Cena, latence a spolehlivost jsou trade-off

## Use for
- opakovaných jednoduchých úkolech
- generování drobných souborů
- agentických workflow s různou náročností
- optimalizaci nákladů Claude Code setupu

## Avoid
- Posílat multi-file refaktor nebo citlivé tool-heavy operace na náhodný levný model


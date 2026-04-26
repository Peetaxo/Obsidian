# Ingesce udržuje Human i Agent vrstvu

## Trigger
- nový raw YouTube zdroj
- aktualizace knowledge báze
- změna human knowledge bloku
- příprava promptu pro agenta

## Core rule
- Pokud vznikne nebo se změní human knowledge blok → vytvoř nebo aktualizuj odpovídající agent blok

## Decision rules
- Pokud human blok nemá praktickou rozhodovací hodnotu → agent blok negeneruj
- Pokud agent blok obsahuje odkazy, metadata nebo review → přepiš ho
- Human vrstva drží kontext, zdroje a review
- Agent vrstva drží jen rozhodovací hodnotu
- Agent blok je odvozenina, ne druhý zdroj pravdy
- Agent blok musí jít vložit přímo do promptu

## Use for
- zpracování nového YouTube transkriptu
- aktualizace existujícího principu
- lint knowledge báze
- příprava promptu pro agenta

## Avoid
- aktualizovat jen human vrstvu
- agent blok s frontmatterem nebo zdroji
- promptový blok bez rozhodovací hodnoty


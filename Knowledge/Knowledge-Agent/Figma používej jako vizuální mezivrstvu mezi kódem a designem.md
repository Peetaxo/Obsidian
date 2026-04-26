# Figma používej jako vizuální mezivrstvu mezi kódem a designem

## Trigger
- design-heavy landing page
- člověk má ladit vizuál ve Figmě
- agent má propsat design zpět do kódu
- po změně následuje browser QA

## Core rule
- Pokud vizuální kvalita vyžaduje lidský design review → vlož mezi kód a implementaci Figmu

## Decision rules
- Pokud agent vytvoří funkční základ → přenes vybraný UI rozsah do Figmy
- Pokud designer mění layout, barvy nebo typografii → upravuj ve Figmě
- Pokud změny jdou zpět do kódu → ověř výsledek v browseru
- Figma mezivrstva zvyšuje kvalitu vizuální iterace
- Kódový základ musí být funkční před přenosem do Figmy
- Browser preview snižuje riziko rozbité responzivity

## Use for
- landing page
- redesign webové sekce
- klientské design review
- vizuální ladění nad kódem

## Avoid
- Figma sync bez browser kontroly
- celý design workflow jen přes prompt
- přenos nefunkčního UI do Figmy

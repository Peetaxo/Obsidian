# Design změny synchronizuj po sekcích a přes pojmenované vrstvy

## Trigger
- Figma to code sync
- mnoho frames nebo pages
- agent neví co se změnilo
- design používá variables

## Core rule
- Pokud agent propsuje Figma změny do kódu → omez rozsah a používej pojmenované vrstvy

## Decision rules
- Pokud Figma soubor obsahuje mnoho pages → pracuj s konkrétním framem
- Pokud sync míří na UI sekci → uveď přesný název sekce
- Pokud agent neví změny → popiš změny explicitně
- Pokud používáš Figma variables → mapuj je na CSS custom properties
- Menší rozsah snižuje chyby syncu
- Pojmenované vrstvy zvyšují přesnost implementace

## Use for
- React/Tailwind UI změny
- redesign hero nebo CTA sekce
- mapování barev a spacingu
- responzivní úpravy

## Avoid
- celý Figma soubor jako vstup
- nepojmenované vrstvy
- sync bez mobile frame

# Denní rekap ukládej do pracovní paměti

## Trigger
- projekt běží více dní
- agent pracuje přes více chatů
- vznikly blokery nebo rozhodnutí
- denní práce má pokračování

## Core rule
- Pokud projekt pokračuje další den → ulož stručný rekap do pracovní paměti

## Decision rules
- Pokud agent dokončil výstupy → zapiš co bylo dodáno
- Pokud se změnil projektový stav → zapiš změny
- Pokud existují blokery → zapiš blokery a další krok
- Pokud vznikly priority → zapiš priority na další den
- Denní rekap snižuje ztrátu kontextu
- Markdown note zvyšuje přenositelnost mezi agenty

## Use for
- dlouhodobý vývoj aplikace
- výzkumné projekty
- obsahové workflow
- paralelní agentické práce

## Avoid
- nechávat stav jen v chatu
- rekap bez dalších kroků
- denní automatizace bez kontroly hodnoty výstupu

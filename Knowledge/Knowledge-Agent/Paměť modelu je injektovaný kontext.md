# Paměť modelu je injektovaný kontext

## Trigger
- Práce s AI memory
- rozdíl mezi modelem a aplikací
- vysvětlování tokenové spotřeby

## Core rule
- Pokud chování modelu vypadá personalizovaně → hledej injektovaný kontext, ne dotrénování modelu

## Decision rules
- Pokud stejný dotaz dává jinou odpověď v běžném a anonymním chatu → zkontroluj skrytý kontext
- Pokud krátký dotaz spotřebuje hodně tokenů → hledej připojené memories, instrukce nebo nástroje
- Pokud chceš přenositelnost paměti → ulož ji mimo uzavřenou aplikaci
- Aplikační memory zvyšuje personalizaci
- Skrytý kontext zvyšuje tokenovou spotřebu
- Špatně uložená memory opakuje nežádoucí preference

## Use for
- ladění rozdílů mezi chatovacími aplikacemi
- auditu personalizovaných odpovědí
- návrhu agentické paměti
- vysvětlování, proč samotný model není celý systém

## Avoid
- Předpokládat, že model se v komerčním chatu průběžně dotrénoval na uživatele, a ignorovat aplikační kontext


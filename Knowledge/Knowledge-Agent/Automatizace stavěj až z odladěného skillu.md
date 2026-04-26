# Automatizace stavěj až z odladěného skillu

## Trigger
- opakovaný report
- plánovaná automatizace
- skill s API nebo pluginem

## Core rule
- Nejdřív postup odlaď ručně jako skill nebo workflow, potom z něj udělej automatizaci

## Decision rules
- Pokud stejný skill spouštíš pravidelně → použij automation
- Pokud workflow potřebuje API key → nejdřív otestuj skill ručně
- Pokud automatizace posílá email, post nebo externí akci → nastav kontrolu nebo omezení
- Odladěný skill snižuje riziko špatné automatizace
- Testovací běh musí ověřit výstup i oprávnění
- Automatizace bez jasného logu se špatně ladí

## Use for
- měsíčním reportu z YouTube transkriptů
- týdenním kalendářním recapu
- plánování social postů
- pravidelném výzkumném nebo QA workflow

## Avoid
- Hned naplánovat automatizaci nad neověřeným promptem a zjistit chyby až po tom, co odešle špatný výstup


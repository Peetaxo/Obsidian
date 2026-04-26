# Třívrstvá architektura znalostní báze

## Trigger
- Návrh knowledge báze
- oddělení zdrojů od syntézy
- pravidla pro agenta

## Core rule
- Pokud buduješ knowledge base → odděl raw zdroje, syntézu a pravidla agenta

## Decision rules
- Pokud ukládáš nový zdroj → dej ho do raw vrstvy
- Pokud vytváříš opakovaně použitelnou znalost → dej ji do wiki vrstvy
- Pokud měníš workflow LLM → uprav schema pravidel
- Raw zdroje jsou neměnný zdroj pravdy
- Wiki je pracovní syntéza, kterou LLM udržuje
- Schema mění chování agenta napříč budoucími sezeními

## Use for
- zakládání nové wiki
- migraci poznámek do strukturovaného systému
- nastavování pravidel pro LLM agenta
- oddělování zdrojů od interpretací

## Avoid
- Míchat původní zdroje, syntézy a instrukce do jedné složky bez jasných hranic


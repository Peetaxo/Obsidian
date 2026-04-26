---
updated: 2026-04-26
created: 2026-04-26
typ: princip
puvod:
  - youtube
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - overene-v-tomto-vaultu
stav: overeno
duvera: high
overeno_v_praxi: true
review_poznamka: "Pattern je převzatý ze zdrojů a zatím ověřený hlavně při správě tohoto vaultu; mimo tento kontext ho znovu posuď."
oblast:
  - research-a-znalostni-baze
  - ai-agent-workflow
pouzij_kdy:
  - návrh knowledge báze
  - oddělení zdrojů od syntézy
  - pravidla pro agenta
nastroje:
  - Obsidian
  - lokální markdown
  - Claude Code
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Kompletní raw zdroje bez zkracování|Kompletní raw zdroje bez zkracování]]"
  - "[[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]"
  - "[[AI System/Knowledge/Knowledge-Human/Plan mode před návrhem znalostní báze|Plan mode před návrhem znalostní báze]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Třívrstvá architektura znalostní báze

## Kontext
Použij při návrhu osobní nebo týmové znalostní báze řízené LLM. Oddělení vrstev chrání raw zdroje a zároveň dovoluje agentovi volně upravovat pracovní syntézu.

## Princip
Odděl raw zdroje, LLM-generovanou wiki a schema pravidel. Každá vrstva má jinou odpovědnost a jiné riziko změny.

## Heuristiky

Decision trigger:
- Když ukládáš nový zdroj → dej ho do raw vrstvy.
- Když vytváříš opakovaně použitelnou znalost → dej ji do wiki vrstvy.
- Když měníš workflow LLM → uprav schema pravidel.

Pravidla:
- Raw zdroje jsou neměnný zdroj pravdy.
- Wiki je pracovní syntéza, kterou LLM udržuje.
- Schema mění chování agenta napříč budoucími sezeními.

## Použij při
- zakládání nové wiki
- migraci poznámek do strukturovaného systému
- nastavování pravidel pro LLM agenta
- oddělování zdrojů od interpretací

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Kompletní raw zdroje bez zkracování|kompletní raw vrstvou]]
- atomickými knowledge bloky
- indexem a logem
- pravidelným lintem kvality

## Související
- [[AI System/Knowledge/Knowledge-Human/Kompletní raw zdroje bez zkracování|Kompletní raw zdroje bez zkracování]]
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]
- [[AI System/Knowledge/Knowledge-Human/Plan mode před návrhem znalostní báze|Plan mode před návrhem znalostní báze]]

## Zdroje
- [[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]

## Review
- Stav: Ověřeno v tomto vaultu.
- Důvěra: high.
- Ověření v praxi: Použito při organizaci a údržbě AI System knowledge báze.
- Použij jako: stabilnější lokální pravidlo, ale při jiném projektu znovu ověř kontext.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Míchat původní zdroje, syntézy a instrukce do jedné složky bez jasných hranic.


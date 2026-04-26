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
  - orientace ve wiki
  - evidence změn knowledge báze
  - rychlý výběr relevantních bloků
nastroje:
  - Obsidian
  - index.md
  - log.md
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]"
  - "[[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]"
  - "[[AI System/Knowledge/Knowledge-Human/LLM jako správce wiki člověk jako kurátor|LLM jako správce wiki člověk jako kurátor]]"
zdroje:
  - "[[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]]"
---

# Index a log jako navigační paměť

## Kontext
Použij, když wiki potřebuje být snadno prohledatelná a zpětně dohledatelná bez složité infrastruktury. Index je vstupní bod pro člověka i agenta; log je stopa změn.

## Princip
`index.md` slouží jako obsahová mapa wiki. `log.md` slouží jako chronologická paměť operací a změn.

## Heuristiky

Decision trigger:
- Když přidáš nebo změníš stránku → aktualizuj index.
- Když proběhne ingesce, dotaz nebo lint → přidej záznam do logu.
- Když hledáš relevantní znalosti → začni indexem.

Pravidla:
- Index zrychluje výběr relevantních stránek.
- Log pomáhá pochopit poslední vývoj wiki.
- Konzistentní prefixy v logu zvyšují strojovou čitelnost.

## Použij při
- navigaci v menší a střední markdown wiki
- dohledávání posledních změn
- odpovídání na dotazy nad wiki
- budování základu před pokročilým vyhledáváním

## Použij s
- oblastmi v YAML frontmatteru
- jednovětými anotacemi u odkazů
- append-only logem
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|pravidelným lintem]]

## Související
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]
- [[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]]
- [[AI System/Knowledge/Knowledge-Human/LLM jako správce wiki člověk jako kurátor|LLM jako správce wiki člověk jako kurátor]]

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
- Nechat wiki růst bez centrální mapy obsahu a chronologie změn.


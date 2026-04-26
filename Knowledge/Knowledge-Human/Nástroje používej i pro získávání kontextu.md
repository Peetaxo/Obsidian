---
created: 2026-04-26
updated: 2026-04-26
typ: princip
puvod:
  - youtube
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - pracovni-hypoteza
stav: kandidat
duvera: medium
overeno_v_praxi: false
review_poznamka: "Pattern převzatý ze zdrojů; použij jako kandidáta, ne jako dogma, a ověř proti aktuálnímu úkolu."
oblast:
  - tools-skills-mcp-cli
  - ai-agent-workflow
  - research-a-znalostni-baze
pouzij_kdy:
  - agent potřebuje externí kontext
  - MCP nebo konektor k datům
  - read-only přístup ke službám
nastroje:
  - MCP
  - GitHub
  - Notion
  - NotebookLM
  - Figma
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|Nástroje přidávej až podle měřítka]]"
  - "[[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]"
  - "[[AI System/Knowledge/Knowledge-Human/Computer use omez jasnou hranicí úkolu|Computer use omez jasnou hranicí úkolu]]"
zdroje:
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
  - "[[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]"
---

# Nástroje používej i pro získávání kontextu

## Kontext
Použij, když agent potřebuje najít relevantní informace v GitHubu, Notionu, Figma souborech, kalendáři, NotebookLM nebo dalších službách. Nástroj není jen ruka pro akci, ale i cesta ke kontextu.

## Princip
Nástroje připojuj tam, kde agentovi bezpečně zpřístupní relevantní kontext. U citlivých služeb preferuj nejmenší nutná oprávnění a read-only režim.

## Heuristiky

Decision trigger:
- Když agent opakovaně žádá stejný externí kontext → přidej řízený konektor nebo rozcestník.
- Když nástroj slouží jen hypoteticky → nepřidávej ho do aktivního kontextu.
- Když služba obsahuje citlivá data → začni read-only přístupem.

Pravidla:
- Kontextové nástroje snižují ruční kopírování informací.
- Každý připojený nástroj zvyšuje oprávnění, údržbu a často i tokenovou režii.
- Přístup k datům má být omezený podle rizika úkolu.

## Použij při
- napojení agenta na GitHub nebo issue tracker
- práci s firemní wiki
- hledání brand podkladů ve Figmě
- dotazování výzkumného notebooku

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|přidáváním nástrojů podle měřítka]]
- oprávněními podle principu nejmenšího přístupu
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|skillem, který říká, kde hledat]]
- tokenovým auditem po připojení většího MCP

## Související
- [[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|Nástroje přidávej až podle měřítka]]
- [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]
- [[AI System/Knowledge/Knowledge-Human/Computer use omez jasnou hranicí úkolu|Computer use omez jasnou hranicí úkolu]]

## Zdroje
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]
- [[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Dávat agentovi široké zápisové přístupy jen proto, aby si mohl přečíst kontext.

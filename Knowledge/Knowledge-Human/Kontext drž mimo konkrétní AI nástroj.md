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
  - ai-agent-workflow
  - research-a-znalostni-baze
  - tools-skills-mcp-cli
pouzij_kdy:
  - přenositelnost kontextu
  - prevence vendor lock-in
  - sdílení kontextu mezi agenty
nastroje:
  - Markdown
  - Obsidian
  - git
  - Notion
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]"
  - "[[AI System/Knowledge/Knowledge-Human/Obsidian jako UI nad markdown wiki|Obsidian jako UI nad markdown wiki]]"
  - "[[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]"
zdroje:
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
---

# Kontext drž mimo konkrétní AI nástroj

## Kontext
Použij, když má kontext sloužit déle než jedna aplikace nebo jeden agent. Hodí se pro osobní i firemní znalosti, které mají přežít změnu modelu, editoru nebo chatovacího nástroje.

## Princip
Klíčový kontext ukládej do přenositelných souborů nebo systémů, které může číst více agentů. AI aplikace na něj jen nasměruj, místo aby byla jediným místem paměti.

## Heuristiky

Decision trigger:
- Když kontext bude potřebovat více nástrojů → ulož ho do lokální nebo exportovatelné vrstvy.
- Když znalost drží jen ChatGPT/Claude memory → zvaž kopii ve vlastní wiki.
- Když nový agent potřebuje onboarding → dej mu rozcestník ke kontextu.

Pravidla:
- Přenositelný kontext snižuje vendor lock-in.
- Lokální soubory zrychlují práci agentů nad častým kontextem.
- Uzavřená memory ztěžuje migraci i audit.

## Použij při
- nastavování osobní AI paměti
- firemní knowledge base
- práci přes více agentů
- migraci mezi AI nástroji

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|lokálním markdownem]]
- git verzováním
- Notionem jako zálohou nebo lidským UI
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|skilly jako rozcestníky]]

## Související
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]]
- [[AI System/Knowledge/Knowledge-Human/Obsidian jako UI nad markdown wiki|Obsidian jako UI nad markdown wiki]]
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]]

## Zdroje
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Nalít veškerý dlouhodobý kontext do jedné chatovací aplikace a pak ho neumět exportovat ani auditovat.


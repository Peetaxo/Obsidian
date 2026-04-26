---
created: 2026-04-26
updated: 2026-04-26
typ: workflow
puvod:
  - youtube
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - pracovni-hypoteza
stav: kandidat
duvera: medium
overeno_v_praxi: false
review_poznamka: "Pattern převzatý ze zdroje; hodí se až ve chvíli, kdy počet skillů vytváří orientační nebo duplicitní problém."
oblast:
  - tools-skills-mcp-cli
  - ai-agent-workflow
  - research-a-znalostni-baze
pouzij_kdy:
  - mnoho nainstalovaných skillů
  - duplicity skillů
  - agent neví který skill použít
nastroje:
  - Claude skills
  - scheduled tasks
  - Markdown
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]"
  - "[[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]"
zdroje:
  - "[[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]"
---

# Skill katalog audituj pravidelně

## Kontext
Použij, když se počet skillů zvětší natolik, že agent nebo člověk ztrácí přehled, co existuje, co se překrývá a co je rozbité.

## Princip
Skill knihovna potřebuje katalog a audit stejně jako wiki: seznam skillů, kategorie, příkazy, stav, duplicity a doporučené úpravy.

## Heuristiky

Decision trigger:
- Když máš mnoho skillů → vytvoř skill dashboard.
- Když se skilly překrývají → spusť audit duplicit.
- Když dashboard používáš pravidelně → automatizuj jeho refresh.

Pravidla:
- Katalog zrychluje výběr správného skillu.
- Audit snižuje skill sprawl.
- Scheduled refresh snižuje ruční údržbu katalogu.

## Použij při
- správě osobní knihovny skillů
- review agentického setupu
- přípravě promptu pro opakované workflow
- kontrole duplicitních nebo rozbitých skillů

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|skill rozcestníky]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|scheduled refresh]]
- lintem knowledge báze
- dashboardem se stavem a kategoriemi

## Související
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]]
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]

## Zdroje
- [[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pattern pro prevenci skill sprawl, ne jako povinný dashboard pro malý setup.

## Kdy nepoužít
- Když máš jen pár stabilních skillů.
- Když audit zabere víc času než ruční orientace.

## Anti-pattern
- Instalovat další skilly bez katalogu, bez auditu a bez mazání překryvů.

---
updated: 2026-04-26
created: 2026-04-26
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
  - browser-automation
  - tools-skills-mcp-cli
pouzij_kdy:
  - opakovaná browser automatizace
  - reusable QA workflow
  - scraping nebo reporty bez API
nastroje:
  - Playwright CLI
  - Claude Code
  - skills
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]"
  - "[[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]"
zdroje:
  - "[[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]]"
  - "[[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]]"
  - "[[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]]"
---

# Automatizační skripty proměňuj ve skills

## Kontext
Použij, když agent opakovaně vykonává stejný browser, scraping nebo QA postup. Největší návratnost má u postupů, které už byly odladěné přes [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|browser automation]] a budou se vracet v dalších projektech.

## Princip
Jednorázový automatizační skript má být po odladění převeden na skill nebo opakovatelný pracovní postup. Skill stabilizuje kroky a snižuje znovuvymýšlení.

## Heuristiky

Decision trigger:
- Když skript úspěšně řeší opakovaný úkol → zabal ho jako skill.
- Když agent musí znovu psát podobný browser skript → vytvoř reusable postup.
- Když skript selže na UI detailu → uprav skill o novou zkušenost.

Pravidla:
- Skill zvyšuje konzistenci opakovaných automatizací.
- Odladěný skript je lepší základ než nový prompt od nuly.
- Selhání skriptu má aktualizovat postup, ne zůstat jen v chatu.

## Použij při
- browser QA
- lead scraping workflow
- práci s interními portály
- pravidelných kontrolách a reportech

## Použij s
- [[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizací]]
- [[AI System/Knowledge/Knowledge-Human/Přihlášené browser session izoluj a superviduj|supervidovanými browser session]]
- Playwright skripty uloženými v projektu
- krátkým runbookem: setup, spuštění, očekávaný výstup, fallback

## Související
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]]
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]]

## Zdroje
- [[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]]
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
- Psát pro stejný úkol pokaždé nový automatizační skript bez ukládání naučeného postupu.

---
created: 2026-04-26
updated: 2026-04-26
typ: workflow
puvod:
  - konverzace
  - agenticka-synteza
povaha:
  - systemove-pravidlo-vaultu
  - workflow-ingesce
stav: overeno
duvera: high
overeno_v_praxi: true
review_poznamka: "Lokální pravidlo pro budoucí ingesci raw zdrojů: human vrstva je zdroj pravdy, agent vrstva je kompilovaný runtime výstup."
oblast:
  - research-a-znalostni-baze
  - ai-agent-workflow
pouzij_kdy:
  - nový raw YouTube zdroj
  - aktualizace knowledge báze
  - příprava znalostí pro agentické použití
nastroje:
  - Obsidian
  - Markdown
  - Knowledge-Human
  - Knowledge-Agent
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]"
  - "[[AI System/Knowledge/Knowledge-Human/Knowledge bloky ber jako kandidátní patterny|Knowledge bloky ber jako kandidátní patterny]]"
  - "[[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]"
zdroje:
  - "[[AI System/log.md]]"
---

# Ingesce udržuje Human i Agent vrstvu

## Kontext
Použij při každém novém raw zdroji. Human vrstva má sloužit člověku, Obsidianu, review a traceabilitě; agent vrstva má sloužit jako krátký prompt-friendly runtime výstup.

## Princip
Každá ingesce musí aktualizovat dvě vrstvy: `Knowledge-Human` jako zdroj pravdy a `Knowledge-Agent` jako komprimovaný agentický blok bez metadat, odkazů, zdrojů a dlouhého vysvětlování.

## Heuristiky

Decision trigger:
- Když vznikne nebo se změní human knowledge blok → vytvoř nebo aktualizuj odpovídající agent blok.
- Když je human blok `stav: slabe` nebo `archivovat` → agent blok negeneruj nebo ho označ k odstranění.
- Když agent blok obsahuje odkazy, metadata nebo review → zkrať ho znovu.

Pravidla:
- Human vrstva zachovává kontext, zdroje a review.
- Agent vrstva zachovává jen rozhodovací hodnotu.
- Agent blok je odvozenina, ne druhý zdroj pravdy.
- Agent blok musí být execution-grade: krátký, rozhodovací a použitelný přímo při implementaci kódu.

## Použij při
- zpracování nového YouTube transkriptu
- aktualizaci existujícího principu
- pravidelném lintu knowledge báze
- přípravě promptu pro agenta

## Použij s
- formátem `Trigger / Core rule / Decision rules / Use for / Avoid`
- limitem 120-180 slov na agent blok
- tvrdými pravidly typu `Pokud X → udělej Y`
- kontrolou, že agent blok neobsahuje wiki odkazy
- aktualizací `AI System/index.md` a `AI System/log.md`

## Související
- [[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]]
- [[AI System/Knowledge/Knowledge-Human/Knowledge bloky ber jako kandidátní patterny|Knowledge bloky ber jako kandidátní patterny]]
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]]

## Zdroje
- [[AI System/log.md]]

## Review
- Stav: Ověřeno v tomto vaultu.
- Důvěra: high.
- Ověření v praxi: Zavedeno jako nová struktura `Knowledge-Human` a `Knowledge-Agent`.
- Použij jako: povinný workflow pro budoucí raw ingesce.

## Kdy nepoužít
- Když se upravuje pouze raw soubor bez tvorby knowledge výstupu.
- Když jde o archivní nebo slabý blok, který nemá být použit agenty.

## Anti-pattern
- Aktualizovat jen human poznámku a zapomenout vytvořit krátkou agentickou verzi pro reálné použití v promptu.

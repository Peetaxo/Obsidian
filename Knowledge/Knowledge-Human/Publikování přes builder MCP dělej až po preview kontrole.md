---
created: 2026-04-26
updated: 2026-04-26
typ: workflow
puvod:
  - web
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - pracovni-hypoteza
stav: kandidat
duvera: medium
overeno_v_praxi: false
review_poznamka: "Pattern převzatý z webového návodu; používej opatrně, protože publikování přes builder mění externí stav."
oblast:
  - design-a-frontend
  - tools-skills-mcp-cli
  - ai-agent-workflow
pouzij_kdy:
  - Webflow MCP
  - Framer MCP
  - publikování webu
  - externí deployment
nastroje:
  - Webflow MCP
  - Framer MCP
  - Vercel
  - Netlify
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]"
  - "[[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]"
  - "[[AI System/Knowledge/Knowledge-Human/Computer use omez jasnou hranicí úkolu|Computer use omez jasnou hranicí úkolu]]"
zdroje:
  - "[[AI System/Raw/Web/Figma → Claude.md]]"
---

# Publikování přes builder MCP dělej až po preview kontrole

## Kontext
Použij, když agent dokáže publikovat web přes Webflow, Framer, Vercel nebo Netlify. Publikování je externí akce, takže patří až za ověření.

## Princip
Deploy přes builder MCP spusť až po lokálním preview, kontrole responzivity, potvrzení cílového projektu a jasném mapování komponent.

## Heuristiky

Decision trigger:
- Když agent má publikovat web ven → nejdřív ověř lokální preview.
- Když deploy míří do Webflow nebo Frameru → explicitně mapuj komponenty, classes a breakpointy.
- Když publishing může přepsat existující projekt → vyžádej potvrzení.

Pravidla:
- Preview kontrola snižuje riziko publikování rozbité verze.
- Builder MCP zvyšuje dosah agenta mimo lokální kód.
- Jasný site/project ID snižuje riziko deploye na špatné místo.

## Použij při
- deploy landing page do Webflow
- přenos komponent do Frameru
- publikování z GitHubu na Vercel
- klientském předání webu

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|browser QA]]
- potvrzením cílového projektu
- checklistem breakpointů
- rollback plánem

## Související
- [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]]
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]
- [[AI System/Knowledge/Knowledge-Human/Computer use omez jasnou hranicí úkolu|Computer use omez jasnou hranicí úkolu]]

## Zdroje
- [[AI System/Raw/Web/Figma → Claude.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: bezpečnostní workflow pro agentické publikování.

## Kdy nepoužít
- Když výstup zůstává jen lokální prototyp.
- Když agent nemá ověřená oprávnění nebo správný cílový projekt.

## Anti-pattern
- Nechat agenta publikovat do Webflow nebo Frameru bez preview, potvrzení cíle a kontroly mobilní verze.

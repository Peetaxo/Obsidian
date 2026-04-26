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
  - browser-automation
  - design-a-frontend
  - ai-agent-workflow
pouzij_kdy:
  - frontend QA
  - lokální webová aplikace
  - ověření uživatelského toku
nastroje:
  - Playwright CLI
  - Claude Code
  - screenshots
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|Automatizační skripty proměňuj ve skills]]"
  - "[[AI System/Knowledge/Knowledge-Human/Computer use omez jasnou hranicí úkolu|Computer use omez jasnou hranicí úkolu]]"
  - "[[AI System/Knowledge/Knowledge-Human/Přihlášené browser session izoluj a superviduj|Přihlášené browser session izoluj a superviduj]]"
zdroje:
  - "[[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]]"
  - "[[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]]"
---

# Browser automation jako QA smyčka

## Kontext
Použij, když agent staví nebo upravuje webovou aplikaci a potřebuje ověřit reálné chování v prohlížeči. Hodí se hlavně tam, kde statická kontrola nestačí a výsledek závisí na klikání, formulářích nebo navigaci.

## Princip
Browser automation má spustit aplikaci, projít uživatelský tok, zachytit chyby, opravit kód a test zopakovat. QA má být iterativní smyčka, ne jednorázová ruční kontrola.

## Heuristiky

Decision trigger:
- Když workflow závisí na klikání, formulářích nebo navigaci → spusť browser QA.
- Když agent najde chybu v UI toku → oprav kód a zopakuj průchod.
- Když potřebuješ audit viditelného stavu → ukládej screenshoty.

Pravidla:
- Reálný browser odhalí chyby, které statická kontrola mine.
- Screenshoty zvyšují auditovatelnost UI testu.
- Test-oprava-test smyčka snižuje riziko regresí v toku.

## Použij při
- formulářích po krocích
- e2e kontrole webové aplikace
- testování onboarding flow
- ověření lokálního frontend serveru

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|opakovatelným QA skillem]]
- Playwright test script
- headed módem při rizikových akcích
- screenshoty před a po opravě

## Související
- [[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|Automatizační skripty proměňuj ve skills]]
- [[AI System/Knowledge/Knowledge-Human/Computer use omez jasnou hranicí úkolu|Computer use omez jasnou hranicí úkolu]]
- [[AI System/Knowledge/Knowledge-Human/Přihlášené browser session izoluj a superviduj|Přihlášené browser session izoluj a superviduj]]

## Zdroje
- [[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]]
- [[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Považovat hotový kód za ověřený bez průchodu v reálném browseru.

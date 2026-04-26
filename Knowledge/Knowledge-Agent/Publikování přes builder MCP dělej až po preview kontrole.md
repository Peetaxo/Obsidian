# Publikování přes builder MCP dělej až po preview kontrole

## Trigger
- Webflow nebo Framer deploy
- publikování webu ven
- agent mění externí projekt
- hotový lokální preview build

## Core rule
- Pokud agent publikuje mimo lokální repo → nejdřív ověř preview a cílový projekt

## Decision rules
- Pokud agent má deployovat web → spusť lokální preview kontrolu
- Pokud deploy míří do builderu → mapuj komponenty, classes a breakpointy
- Pokud publikování přepíše projekt → vyžádej potvrzení
- Pokud chybí site/project ID → nepublikuj
- Preview kontrola snižuje riziko rozbité verze
- Builder MCP zvyšuje dopad chyb mimo kód

## Use for
- Webflow deploy
- Framer komponenty
- Vercel nebo Netlify publish
- klientské předání webu

## Avoid
- deploy bez preview
- neověřený cílový projekt
- publikování bez rollback plánu

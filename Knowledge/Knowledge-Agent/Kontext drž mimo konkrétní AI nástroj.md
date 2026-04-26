# Kontext drž mimo konkrétní AI nástroj

## Trigger
- přenositelnost kontextu
- prevence vendor lock-in
- sdílení kontextu mezi agenty

## Core rule
- Pokud kontext potřebuje více agentů nebo nástrojů → ulož ho do přenositelné vrstvy

## Decision rules
- Pokud kontext bude potřebovat více nástrojů → ulož ho do lokální nebo exportovatelné vrstvy
- Pokud znalost drží jen ChatGPT/Claude memory → použij kopii ve vlastní wiki
- Pokud nový agent potřebuje onboarding → dej mu rozcestník ke kontextu
- Přenositelný kontext snižuje vendor lock-in
- Lokální soubory zrychlují práci agentů nad častým kontextem
- Uzavřená memory ztěžuje migraci i audit

## Use for
- nastavování osobní AI paměti
- firemní knowledge base
- práci přes více agentů
- migraci mezi AI nástroji

## Avoid
- Nalít veškerý dlouhodobý kontext do jedné chatovací aplikace a pak ho neumět exportovat ani auditovat


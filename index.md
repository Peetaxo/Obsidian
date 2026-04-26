# AI System index

Hlavní vstupní bod pro rychlý výběr použitelných principů, workflow a nástrojových patternů z raw AI zdrojů.

Knowledge má dvě vrstvy:
- `AI System/Knowledge/Knowledge-Human/` - zdroj pravdy pro člověka, review, odkazy a raw traceabilitu.
- `AI System/Knowledge/Knowledge-Agent/` - krátké agentické bloky bez metadat, odkazů a zdrojů, určené pro prompt/runtime použití.

## Review a kvalita knowledge
- [[AI System/Knowledge/Knowledge-Human/Ingesce udržuje Human i Agent vrstvu|Ingesce udržuje Human i Agent vrstvu]] - Při každém novém raw zdroji aktualizuje human i agent vrstvu.
- [[AI System/Knowledge/Knowledge-Human/Knowledge bloky ber jako kandidátní patterny|Knowledge bloky ber jako kandidátní patterny]] - Určuje, že převzaté patterny jsou hypotézy k posouzení, ne automatické příkazy.
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]] - Hledá slabé, duplicitní, zastaralé nebo neověřené bloky.
- [[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]] - Připomíná, že platnost kontextu a odkazů se musí průběžně udržovat.

## AI agent workflow
- [[AI System/Knowledge/Knowledge-Human/LLM jako správce wiki člověk jako kurátor|LLM jako správce wiki člověk jako kurátor]] - Rozděluje práci mezi lidskou kuraci zdrojů a agentickou údržbu wiki.
- [[AI System/Knowledge/Knowledge-Human/Paměť modelu je injektovaný kontext|Paměť modelu je injektovaný kontext]] - Připomíná, že aplikační memory je text vložený do kontextového okna, ne dotrénování modelu.
- [[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|Kontext drž mimo konkrétní AI nástroj]] - Chrání dlouhodobou paměť před zamčením do jedné aplikace.
- [[AI System/Knowledge/Knowledge-Human/Plan mode před návrhem znalostní báze|Plan mode před návrhem znalostní báze]] - Použij před větší strukturální změnou nebo návrhem nové wiki.
- [[AI System/Knowledge/Knowledge-Human/Projektový adresář používej jako pracovní hranici agenta|Projektový adresář používej jako pracovní hranici agenta]] - Drží agentické výstupy, soubory a chaty v jedné dohledatelné složce.
- [[AI System/Knowledge/Knowledge-Human/Paralelní agentické chaty řiď přes plán a stav|Paralelní agentické chaty řiď přes plán a stav]] - Umožňuje souběžnou práci agentů bez ztráty přehledu a ownershipu.
- [[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|Automatizační skripty proměňuj ve skills]] - Převádí odladěné skripty na opakovatelné postupy.
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]] - Dává agentovi cestu k relevantním souborům a nástrojům místo velkého prompt dumpu.
- [[AI System/Knowledge/Knowledge-Human/Skill katalog audituj pravidelně|Skill katalog audituj pravidelně]] - Udržuje přehled o nainstalovaných skillech, duplicitách a jejich použití.
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]] - Plánované běhy staví až nad ručně ověřeným workflow.
- [[AI System/Knowledge/Knowledge-Human/Denní rekap ukládej do pracovní paměti|Denní rekap ukládej do pracovní paměti]] - Převádí dodávky, změny, blokery a priority dne do trvalého kontextu.
- [[AI System/Knowledge/Knowledge-Human/Opakované výstupy bal do deliverable skillů|Opakované výstupy bal do deliverable skillů]] - Dává opakovaným artefaktům stabilní strukturu, styl, formát a kontrolu publikování.
- [[AI System/Knowledge/Knowledge-Human/Dotazy ukládej zpět jako znalosti|Dotazy ukládej zpět jako znalosti]] - Zachytává hodnotné odpovědi z chatu jako budoucí znalost.

## Claude Code / coding produktivita
- [[AI System/Knowledge/Knowledge-Human/Knowledge graph používej pro velké codebase|Knowledge graph používej pro velké codebase]] - Zrychluje opakované dotazy nad rozsáhlým repozitářem.
- [[AI System/Knowledge/Knowledge-Human/Model routing podle náročnosti úkolu|Model routing podle náročnosti úkolu]] - Směruje jednoduché a složité kroky na vhodně silné modely.
- [[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]] - Volí reasoning effort podle délky, rizika a nároků na nástroje.
- [[AI System/Knowledge/Knowledge-Human/Projektový adresář používej jako pracovní hranici agenta|Projektový adresář používej jako pracovní hranici agenta]] - Nastavuje lokální hranici práce pro coding i knowledge výstupy.
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]] - Nejdřív měří spotřebu tokenů, potom redukuje největší zdroje plýtvání.

## Browser automation
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]] - Ověřuje UI přes reálný browser v cyklu test-oprava-test.
- [[AI System/Knowledge/Knowledge-Human/Computer use omez jasnou hranicí úkolu|Computer use omez jasnou hranicí úkolu]] - Používá ovládání desktopu jen pro jasně ohraničené UI-only úkoly.
- [[AI System/Knowledge/Knowledge-Human/Přihlášené browser session izoluj a superviduj|Přihlášené browser session izoluj a superviduj]] - Řeší bezpečné použití cookies, login handoffu a headed režimu.
- [[AI System/Knowledge/Knowledge-Human/Webový obsah předávej agentům jako čistá data|Webový obsah předávej agentům jako čistá data]] - Převádí webový šum do strukturovaného vstupu pro agenta.

## Tokeny a náklady
- [[AI System/Knowledge/Knowledge-Human/Paměť modelu je injektovaný kontext|Paměť modelu je injektovaný kontext]] - Pomáhá vysvětlit, proč i krátký dotaz může nést skrytý kontext a tokenovou režii.
- [[AI System/Knowledge/Knowledge-Human/Náklady modelu měř podle dokončené úlohy|Náklady modelu měř podle dokončené úlohy]] - Porovnává modely podle kvality, času, retry a tokenů na hotový výstup.
- [[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu|Effort level nastav podle délky a rizika úkolu]] - Brání zbytečnému používání nejvyššího reasoning nastavení.
- [[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]] - Volí úzký CLI nástroj místo velkého MCP, když to stačí.
- [[AI System/Knowledge/Knowledge-Human/Tokenový rozpočet měř a redukuj|Tokenový rozpočet měř a redukuj]] - Audituj limity, skills, MCP a instrukce před optimalizací.
- [[AI System/Knowledge/Knowledge-Human/Velký výzkum deleguj do specializované vrstvy|Velký výzkum deleguj do specializované vrstvy]] - Nepřenáší celý korpus do aktivního kontextu agenta.

## Design a frontend
- [[AI System/Knowledge/Knowledge-Human/Design reference převáděj na systémové specifikace|Design reference převáděj na systémové specifikace]] - Převádí inspiraci na typografii, komponenty, motion a stavy.
- [[AI System/Knowledge/Knowledge-Human/Brand styl drž jako sdílený skill|Brand styl drž jako sdílený skill]] - Ukládá brand pravidla jako sdílený style skill pro konzistentní vizuální výstupy.
- [[AI System/Knowledge/Knowledge-Human/Opakované výstupy bal do deliverable skillů|Opakované výstupy bal do deliverable skillů]] - Balí PDF, explainery, carousely a dashboardy do opakovatelných výstupních workflow.
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]] - Dává frontend změnám ověřovací smyčku v prohlížeči.

## Research a znalostní báze
- [[AI System/Knowledge/Knowledge-Human/Knowledge bloky ber jako kandidátní patterny|Knowledge bloky ber jako kandidátní patterny]] - Chrání wiki před nekritickým přebíráním cizích workflow.
- [[AI System/Knowledge/Knowledge-Human/Třívrstvá architektura znalostní báze|Třívrstvá architektura znalostní báze]] - Odděluje raw zdroje, pracovní wiki a schema pravidel.
- [[AI System/Knowledge/Knowledge-Human/Kompletní raw zdroje bez zkracování|Kompletní raw zdroje bez zkracování]] - Chrání raw vrstvu jako kompletní zdroj pravdy.
- [[AI System/Knowledge/Knowledge-Human/Ingesce jako integrace do existující wiki|Ingesce jako integrace do existující wiki]] - Nový zdroj začleňuje do existujících bloků a vazeb.
- [[AI System/Knowledge/Knowledge-Human/Persistentní wiki místo jednorázového RAG|Persistentní wiki místo jednorázového RAG]] - Ukládá syntézu tak, aby se nemusela pokaždé znovu vyvozovat.
- [[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj|Kontext drž mimo konkrétní AI nástroj]] - Udržuje dlouhodobou paměť přenositelnou mezi agenty a aplikacemi.
- [[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument|Kontext udržuj jako živý dokument]] - Bere memory a konfigurační soubory jako průběžně udržovaný systém.
- [[AI System/Knowledge/Knowledge-Human/Denní rekap ukládej do pracovní paměti|Denní rekap ukládej do pracovní paměti]] - Udržuje kontinuitu dlouhodobých projektů mezi dny a chaty.
- [[AI System/Knowledge/Knowledge-Human/Traceabilita wiki stránek ke zdrojům|Traceabilita wiki stránek ke zdrojům]] - Drží odkaz z každého principu zpět na raw zdroj.
- [[AI System/Knowledge/Knowledge-Human/Batch ingesce vyžaduje následný lint|Batch ingesce vyžaduje následný lint]] - Po hromadném importu kontroluje kvalitu vazeb a struktury.
- [[AI System/Knowledge/Knowledge-Human/Pravidelný lint znalostní báze|Pravidelný lint znalostní báze]] - Hledá rozpory, chybějící odkazy a kandidáty na nové bloky.
- [[AI System/Knowledge/Knowledge-Human/Index a log jako navigační paměť|Index a log jako navigační paměť]] - Udržuje mapu obsahu a chronologii změn.

## Tools / skills / MCP / CLI
- [[AI System/Knowledge/Knowledge-Human/Lokální markdown jako pracovní formát agentů|Lokální markdown jako pracovní formát agentů]] - Preferuje editovatelné lokální soubory pro agentickou práci.
- [[AI System/Knowledge/Knowledge-Human/Obsidian jako UI nad markdown wiki|Obsidian jako UI nad markdown wiki]] - Používá Obsidian jako lidské rozhraní nad markdownem.
- [[AI System/Knowledge/Knowledge-Human/Nástroje přidávej až podle měřítka|Nástroje přidávej až podle měřítka]] - Přidává pluginy a vyhledávání až při konkrétním limitu.
- [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu|Nástroje používej i pro získávání kontextu]] - Připojuje služby primárně jako řízené zdroje kontextu, často read-only.
- [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow|Plugin rozšiřuje schopnosti, skill balí workflow]] - Rozlišuje přístup ke službě od opakovatelného postupu.
- [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu|Skilly používej jako rozcestníky ke kontextu]] - Popisuje, kdy skill naviguje agenta k podkladům místo ukládání všech dat do promptu.
- [[AI System/Knowledge/Knowledge-Human/Komunitní skilly instaluj jen po kontrole důvěryhodnosti|Komunitní skilly instaluj jen po kontrole důvěryhodnosti]] - Brání instalaci neznámých skillů bez kontroly autora, oprávnění a instrukcí.
- [[AI System/Knowledge/Knowledge-Human/Skill katalog audituj pravidelně|Skill katalog audituj pravidelně]] - Pomáhá řídit rostoucí knihovnu skillů jako auditovatelný systém.
- [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu|Automatizace stavěj až z odladěného skillu]] - Převádí opakované skilly do plánovaných běhů až po testu.
- [[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]] - Pomáhá rozhodnout, kdy stačí CLI místo MCP.

## Raw zdroje
- [[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]] - Claude skills pro dashboard style, skill katalog, audit, PDF guide, denní rekap, Obsidian daily note, carousely a konektory.
- [[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]] - Codex projekty, soubory, pluginy, skilly, automations, multitasking a produkční workflow.
- [[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]] - Task-based model eval, effort nastavení, browser/computer use a knowledge work v Codexu.
- [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]] - Kontext jako hlavní páka kvality AI práce, tool-agnostic paměť, MCP a skilly pro navigaci.
- [[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]] - Browser automation, Playwright CLI, QA smyčky a přihlášené session.
- [[AI System/Raw/YouTube/LLM Wiki od Karpathyho AI agent spravující vaší knowledge base.md]] - Lokální LLM wiki, Obsidian, raw/wiki vrstvy a agentická údržba.
- [[AI System/Raw/YouTube/Top 5 Claude Code Skills... 100,000+ github stars.md]] - Graphify, Firecrawl, design skills, model routing a výzkumné vrstvy.
- [[AI System/Raw/YouTube/3 New Claude Code Repos Will 100x Your Next Project.md]] - Caveman, Code Burn a Design Extract pro Claude Code produktivitu.

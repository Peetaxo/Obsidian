# AI System log

## [2026-04-26] audit | Akční schema knowledge bloků
- Proveden audit `AI System/Raw/YouTube/` a `AI System/Knowledge/Knowledge-Human/`.
- Všechny existující knowledge bloky převedeny na akční formát s YAML frontmatterem, oblastmi použití, nástroji, souvisejícími bloky, raw zdroji a sekcí `Použij s`.
- Doplněny cílené Obsidian wiki odkazy mezi nejsilněji souvisejícími principy.
- Vytvořen hlavní vstupní bod [[AI System/index.md]] a tento append-only log.


## [2026-04-26] konvence | Odstranění prefixu [AI] z knowledge souborů
- Knowledge soubory v AI System/Knowledge/Knowledge-Human/ přejmenovány podle názvu principu bez prefixu [AI].
- Do YAML frontmatteru knowledge bloků doplněna metadata created a updated.
- Opraveny Obsidian odkazy a index tak, aby mířily na nové stabilní názvy.

## [2026-04-26] ingesce | Kontext je často důležitější než AI model nebo nástroj
- Zpracován raw zdroj [[AI System/Raw/YouTube/Kontext je často důležitější než AI model nebo nástroj Coffee break s Filipem.md]].
- Přidány knowledge bloky [[AI System/Knowledge/Knowledge-Human/Paměť modelu je injektovaný kontext]], [[AI System/Knowledge/Knowledge-Human/Kontext drž mimo konkrétní AI nástroj]], [[AI System/Knowledge/Knowledge-Human/Nástroje používej i pro získávání kontextu]], [[AI System/Knowledge/Knowledge-Human/Skilly používej jako rozcestníky ke kontextu]] a [[AI System/Knowledge/Knowledge-Human/Kontext udržuj jako živý dokument]].
- Aktualizovány vazby v existujících blocích o lokálním markdownu, tokenovém rozpočtu, nástrojích, lintu a skillech.

## [2026-04-26] ingesce | Codex full course a GPT 5.5 v Codexu
- Zpracovány raw zdroje [[AI System/Raw/YouTube/Codex Full Course 2026 The NEW Best AI Coding Tool.md]] a [[AI System/Raw/YouTube/GPT 5.5 + Codex Just Became the Best Model Ever.md]].
- Přidány knowledge bloky [[AI System/Knowledge/Knowledge-Human/Náklady modelu měř podle dokončené úlohy]], [[AI System/Knowledge/Knowledge-Human/Effort level nastav podle délky a rizika úkolu]], [[AI System/Knowledge/Knowledge-Human/Projektový adresář používej jako pracovní hranici agenta]], [[AI System/Knowledge/Knowledge-Human/Paralelní agentické chaty řiď přes plán a stav]], [[AI System/Knowledge/Knowledge-Human/Automatizace stavěj až z odladěného skillu]], [[AI System/Knowledge/Knowledge-Human/Plugin rozšiřuje schopnosti, skill balí workflow]] a [[AI System/Knowledge/Knowledge-Human/Computer use omez jasnou hranicí úkolu]].
- Aktualizovány vazby v indexu a existujících blocích pro model routing, tokeny, browser QA, tools a skilly.

## [2026-04-26] schema | Review a stav knowledge bloků
- Do knowledge bloků doplněna review metadata `puvod`, `povaha`, `stav`, `duvera`, `overeno_v_praxi` a `review_poznamka`.
- Doplněny sekce `Review` a `Kdy nepoužít`, aby bylo jasné, že většina YouTube patternů je kandidát k posouzení, ne dogma.
- Přidán princip [[AI System/Knowledge/Knowledge-Human/Knowledge bloky ber jako kandidátní patterny]] a nová sekce review v [[AI System/index.md]].

## [2026-04-26] schema | Human a Agent knowledge vrstvy
- Současná human knowledge přesunuta do `AI System/Knowledge/Knowledge-Human/` jako zdroj pravdy pro člověka, review, odkazy a raw traceabilitu.
- Vytvořena `AI System/Knowledge/Knowledge-Agent/` jako kompilovaná agentická vrstva bez metadat, odkazů, zdrojů a review poznámek.
- Přidán workflow [[AI System/Knowledge/Knowledge-Human/Ingesce udržuje Human i Agent vrstvu]], aby budoucí raw ingesce vždy aktualizovala human i agent vrstvu.

## [2026-04-26] agent-schema | Execution-grade agent bloky
- Agent blok [[AI System/Knowledge/Knowledge-Agent/CLI automatizace šetří tokeny oproti MCP]] převeden na ostřejší execution-grade formát pro implementaci kódu.
- Do human pravidla [[AI System/Knowledge/Knowledge-Human/Ingesce udržuje Human i Agent vrstvu]] doplněno, že agent vrstva má být krátká, rozhodovací a použitelná přímo v promptu při programování.

## [2026-04-26] agent-schema | Přepsání celé Knowledge-Agent vrstvy
- Všech 38 agent bloků v `AI System/Knowledge/Knowledge-Agent/` sjednoceno do execution-grade formátu: trigger, core rule, decision rules, use for a avoid.
- Z agent vrstvy odstraněny generické avoid věty, samostatné tool položky v triggeru, měkké formulace, metadata, odkazy, zdroje a review obsah.
- Ověřeno, že agent bloky jsou krátké promptové odvozeniny human vrstvy a každý blok má maximálně 180 slov.

## [2026-04-26] ingesce | 9 Claude Skills I Can’t Live Without
- Zpracován raw zdroj [[AI System/Raw/YouTube/9 Claude Skills I Can’t Live Without (steal them).md]].
- Přidány human i agent bloky [[AI System/Knowledge/Knowledge-Human/Brand styl drž jako sdílený skill]], [[AI System/Knowledge/Knowledge-Human/Skill katalog audituj pravidelně]], [[AI System/Knowledge/Knowledge-Human/Komunitní skilly instaluj jen po kontrole důvěryhodnosti]], [[AI System/Knowledge/Knowledge-Human/Denní rekap ukládej do pracovní paměti]] a [[AI System/Knowledge/Knowledge-Human/Opakované výstupy bal do deliverable skillů]].
- Aktualizovány vazby v blocích o skillech, automatizaci, pluginech a design specifikacích a doplněn hlavní index.

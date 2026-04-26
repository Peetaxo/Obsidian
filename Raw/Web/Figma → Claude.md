![🖥️ Page icon](https://notion-emojis.s3-us-west-2.amazonaws.com/prod/svg-twitter/1f5a5-fe0f.svg)

Pro tebe od @ [blazek.design](http://blazek.design/) — sleduj pro další šablony, AI workflow a kreativní tech obsah

Co se v tomhle návodu naučíš:

Jak propojit Claude s Figmou přes Figma MCP.

Jak nechat Claude postavit web a překopírovat ho do Figmy.

Jak upravit design ve Figmě a nechat Claude propagovat změny zpět do kódu.

Jak napojit Webflow nebo Framer MCP a publishnout web rovnou z Claude.

Jak celý workflow využívá Computer Use — Claude kliká, otevírá okna a pracuje za tebe.

#### O co jde — big picture

Představ si tohle: řekneš Claude, co chceš. On to postaví. Ty si to otevřeš ve Figmě, upravíš vizuál jak potřebuješ — fonty, barvy, spacing, layout. Pak řekneš Claude, ať tvoje změny propíše do kódu. Živá verze webu se aktualizuje. Bez toho, abys napsal jediný řádek.

Celé to funguje díky třem věcem: Figma MCP, Computer Use a volitelně Webflow / Framer MCP pro finální deployment.

Tohle není sci-fi. Tohle je workflow, které můžeš rozjet dneska.

Chceš se naučit stavět weby s AI a vydělávat tím reálné peníze?

Připojil jsem pro tebe bezplatný webinář — „Jak díky AI získáš 100 tis. Kč / měs. tvorbou webů“. Ukážu ti, jak celej workflow funguje v praxi, jaké nástroje používat a jak začít odevzdávat weby klientům — i když jsi nikdy nekodil.

[Zaregistruj se zdarma na webinář](https://www.education.socialmind.cz/webinar-webdesigner)

## Část 1 — Setup

#### Co budeš potřebovat

Než začneš, ujisti se, že máš tyhle věci:

Claude Pro / Team — potřebuješ přístup ke Claude Code (terminálová verze Claude).

Figma — účet + otevřený projekt, do kterého chceš designovat.

Node.js — nainstalovaný na počítači (potřeba pro MCP servery).

Volitelně: Webflow nebo Framer účet — pokud chceš deploy rovnou do builderu.

#### Krok 1 — Instalace Figma MCP

Figma MCP je propojení mezi Claude a tvým Figma souborem. Umožňuje Claude číst design, kopírovat komponenty a propíše změny.

\# 1. Otevři terminál a nainstaluj Figma MCP server npm install -g @anthropic-ai/figma-mcp # 2. Spusť server s tvým Figma API tokenem figma-mcp --token=TVUJ\_FIGMA\_TOKEN

Kde najdeš Figma API token?

Figma → Settings → Account → Personal access tokens → Generate new token. Zkopíruj ho a ulož na bezpečné místo.

Pokud používáš Claude Desktop, můžeš MCP přidat přímo v nastavení:

// claude\_desktop\_config.json { "mcpServers": { "figma": { "command": "figma-mcp", "args": \["--token=TVUJ\_FIGMA\_TOKEN"\] } } }

#### Krok 2 — Instalace Webflow nebo Framer MCP (volitelné)

Pokud chceš, aby Claude deployoval rovnou do Webflow nebo Framer:

Webflow MCP:

npm install -g @anthropic-ai/webflow-mcp webflow-mcp --token=TVUJ\_WEBFLOW\_API\_TOKEN

Framer MCP:

npm install -g @anthropic-ai/framer-mcp framer-mcp --token=TVUJ\_FRAMER\_API\_TOKEN

Důležité: MCP servery pro Webflow a Framer se průběžně aktualizují. Vždy zkontroluj aktuální dokumentaci na GitHubu pro nejnovější setup instrukce. Konkrétní příkazy se mohou lišit.

## Část 2 — Workflow krok za krokem

#### Krok 1 — Nech Claude postavit základ (15–30 min)

Otevři Claude Code a popiš, co chceš. Čím přesnější budeš, tím lepší výsledek.

Postav mi landing page pro fiktivní AI SaaS produkt. - Hero sekce s headlinem, podnadpisem a CTA tlačítkem - Features sekce — 3 karty s ikonami - Testimonial sekce — 2 recenze - Pricing — 3 sloupce - Footer s linky Tech stack: Next.js + Tailwind CSS Design styl: minimalistický, tmavý, se subtilními gradienty Primární barva: #6C5CE7 Font: Inter

Claude vygeneruje kompletní kód a spustí ti lokální preview. Zkontroluj v prohlížeči, že základ vypadá rozumně.

Pro tip: Přidej i design system prompt (z naší šablony „Obecný prompt & toolkit") — AI pak drží konzistentní vizuál od začátku.

#### Krok 2 — Překopíruj do Figmy (5 min)

Teď přijde kouzlo. Řekni Claude:

Překopíruj aktuální verzi landing page do mého Figma souboru. Figma file URL: \[vlož link na tvůj Figma soubor\] Chci: - Celou landing page jako jednotlivé sekce (frames) - Zachovat hierarchii vrstev - Pojmenovat vrstvy smysluplně (hero-section, features-card, atd.)

Claude pomocí Figma MCP a Computer Use vytvoří v tvém Figma souboru strukturované framy, které odpovídají tomu, co vygeneroval v kódu. Můžeš přenést celou stránku, jen jednotlivé sekce, nebo i specifické komponenty i s variables.

#### Krok 3 — Uprav design ve Figmě (30–60 min)

Teď jsi ve svém živlu. Otevři Figmu a uprav si vše podle sebe:

Spacing — uprav mezery mezi sekcemi, padding karet.

Fonty — změň font family, váhu, velikosti.

Barvy — posuň paletu, přidej gradient, uprav kontrast.

Layout — přehoď pořadí sekcí, změň grid na 2 sloupce místo 3.

Obsah — přepiš texty, přidej reálné copy.

Prostě dělej to, co děláš normálně ve Figmě. Žádná omezení.

#### Krok 4 — Propíš změny zpět do kódu (10–15 min)

Hotovo s designem? Řekni Claude:

Podívej se na můj aktualizovaný Figma soubor a propíš změny do kódu. Co jsem změnil: - Zvětšil spacing mezi sekcemi na 96px - Změnil primární barvu na #4F46E5 - Font je teď Space Grotesk místo Inter - Hero sekce má nový layout — text vlevo, obrázek vpravo - Přidal jsem novou CTA sekci před footer Zachovej responsivitu a existující animace.

Claude si přečte tvůj Figma soubor přes MCP, porovná změny a aktualizuje kód. Živá verze webu se aktualizuje — bez toho, abys otevřel editor kódu.

Jak to funguje pod kapotou?

Claude používá Computer Use — doslova vidí obrazovku, kliká, otevírá okna a pracuje za tebe. V kombinaci s Figma MCP umí číst strukturu tvého designu, styly, variables a propsat je přímo do kódu tvého projektu.

#### Krok 5 — Deploy do Webflow / Framer (15–20 min)

Pokud máš napojený Webflow nebo Framer MCP, řekni Claude:

Pro Webflow:

Nasaď aktuální verzi webu do mého Webflow projektu. Webflow site ID: \[tvé site ID\] Mapuj komponenty na Webflow třídy. Zachovej responzivní breakpointy.

Pro Framer:

Překopíruj aktuální kód do Frameru jako komponenty. Framer project URL: \[tvůj Framer projekt\] Použij Framer layout (Stack, Frame) místo HTML divů. Zachovej animace a interakce.

Nechceš builder? Klidně deployni přímo na Vercel nebo Netlify — Claude to umí taky. Stačí říct: „Pusni to na Vercel z mého GitHub repa."

## Část 3 — Tipy pro praxi

#### Iterační smyčka — opakuj dokola

Tohle workflow není lineární. Je to smyčka:

Claude postaví → Figma úprava → Claude propíše → kontrola → Figma úprava → Claude propíše → …

Každý průchod ti zabere minuty, ne hodiny. Po 3–4 iteracích máš web, který vypadá, jako bys na něm pracoval týden.

#### Power tipy

Pracuj po sekcích. Neptej se „překopíruj celý web". Řekni „překopíruj hero sekci a navigation".

Pojmenovávej vrstvy ve Figmě.

hero-headline

,

cta-button

,

feature-card-1

— Claude pak přesně ví, co je co.

Používej Figma Variables. Pokud definuješ barvy a spacing jako variables, Claude je převede na CSS custom properties 1:1.

Dej Claude screenshot, když ztrácí kontext. „Takhle vypadá aktuální verze. Drž se toho."

Neřeš kód. Celý point tohohle workflow je, že se kódu nemusíš dotknout. Nech to na Claude.

#### Čemu se vyhnout

Neposílej celý Figma soubor s 50 stránkami. Claude se ztratí. Sdílej konkrétní frame nebo page.

Nedělej manuální změny v kódu vedle Claude. Budete si přepisovat práci. Buď jdeš přes Figmu, nebo přes Claude — ne obojí najednou.

Nepřeskakuj preview. Po každém „propíši změny" zkontroluj výsledek v prohlížeči, než jdeš dál.

Nezapomeň na mobilní verzi. Ve Figmě si nachystej i mobile frame — Claude pak responsivitu zvládne lépe.

Celý workflow na časové ose:

Setup MCP serverů — 10 min (jednorázově)

Claude postaví základ — 15–30 min

Překopírování do Figmy — 5 min

Design úpravy ve Figmě — 30–60 min

Propagace změn do kódu — 10–15 min

Iterace (2–3 průchody) — 30–45 min

Deploy — 15–20 min

Celkem: ~2–3 hodiny od nuly k živému webu s custom designem.

Chceš se naučit designovat a stavět weby s AI od A do Z?

Aktuálně máme otevřený waitlist na třetí edici, již 2× vyprodaného kurzu Webdesigner 3.0. Naučíš se designovat, pracovat ve Figmě, stavět weby pomocí AI i běžných builderů (Webflow, Framer atp.), a hlavně — odevzdávat pro klienty a vydělávat. Tohle není teorie. Je to cesta k reálným penězům.

Chceš další workflow, šablony a recepty jako je tenhle? Sleduj [@blazek.design](http://blazek.design/) na Instagramu — cinematické webové šablony, AI-powered kreativní workflow a design engineering obsah, který nevypadá jako AI slop. Nové šablony přibývají pravidelně.
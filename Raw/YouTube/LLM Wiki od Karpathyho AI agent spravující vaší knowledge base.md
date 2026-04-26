---
title: "LLM Wiki od Karpathyho: AI agent spravující vaší knowledge base"
source: "https://www.youtube.com/watch?v=bRIOjTScO-s"
author:
  - "[[Filip Oborník | AI s rozumem]]"
published: 2026-04-17
created: 2026-04-26
description: "Ukážu vám koncept LLM Wiki od Andreje Karpathyho – způsob, jak si pomocí Obsidianu, Markdown souborů a Claude Code vybudovat lokální knowledge base, se kterou efektivně spolupracují AI agenti. Společn"
tags:
  - "clippings"
---
![](https://www.youtube.com/watch?v=bRIOjTScO-s)

Ukážu vám koncept LLM Wiki od Andreje Karpathyho – způsob, jak si pomocí Obsidianu, Markdown souborů a Claude Code vybudovat lokální knowledge base, se kterou efektivně spolupracují AI agenti. Společně si ji postavíme krok za krokem a podíváme se, jak funguje v praxi.  
  
Odkaz na LLM Wiki specifikaci od Andreje Karpathyho:  
\- https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f  
(někteří mají problém se stažením, proto přikládám i kopii na stažení z google disku - https://drive.google.com/file/d/1riprklDE4iEKCSjPQcn8CvCW0u1MhiZ9/view?usp=sharing)  
  
\-----------------  
  
💬 Připojte se do ZDARMA AI Discord komunity přes https://discord.gg/mgrgyZuJuv .  
Diskutujeme zde zajimavé novinky, diskutujeme různá témata a sdílíme užitečné rady, tipy a zkušenosti ze světa AI.  
  
\-----------------  
  
🎙️ Sledujte také podcast o technologiích a AI: https://deeplink.show, kde s kolegou Jindřichem rozebíráme témata ze světa technologií, AI a businessu.  
  
\-----------------  
  
🚀 Nabízím AI konzultace, školení a mentoring v oblasti AI: https://filipobornik.cz  
  
\-----------------  
  
🎓 Pro pravidelné vzdělávání v oblasti umělé inteligence je tu AI univerzita, se kterou spolupracuji.  
Stal jsem se ambasadorem pro Vibe Coding. AI univerzita ale nejsou jen já, ale celá řada lektorů a odborníků na AI.  
Vyzkoušejte se slevou za 47 Kč na první týden přes můj odkaz:  
🔗 https://www.chatbuilders.cz/univerzita/?fr\_code=jfjoauvn  
(slevový kód "jfjoauvn" se uplatní až při objednávce)  
  
\-----------------  
  
ℹ️ Pokud vás zajímá více o umělé inteligence a chcete se o ní dozvědět více bez zbytečného humbuku a hlavně s rozumem,  
odebírejte YouTube kanál AI s rozumem nebo navštivte web https://aisrozumem.cz.  
  
\-----------------  
  
#aisrozumem #umelainteligence #ai #karpathy #obsidian #claudecode #knowledgebase #markdown #vibecoding #aiagenti  
  
\-----------------  
  
00:00 Úvod – kdo je Andrej Karpathy a co je LLM Wiki  
01:43 Princip LLM Wiki a proč Notion nestačí  
03:29 Obsidian jako základ knowledge base  
04:45 Spuštění Claude Code a zadání úkolu  
06:30 Použití Karpathyho specifikace jako promptu  
07:05 Plan mode a brainstorming se Superpowers pluginem  
11:08 Struktura složek: RAW, Wiki, Projekt  
15:48 Ukázka vygenerované Wiki a propojení témat  
19:45 Jak správně vkládat zdroje podle Karpathyho  
21:16 Obsidian Web Clipper a další tipy  
22:45 Graph view – vizualizace znalostí  
24:14 Shrnutí a proč je lokální přístup silný

## Transcript

### Úvod – kdo je Andrej Karpathy a co je LLM Wiki

**0:00** · Andreje Karpatyho dost možná znáte a pokud ne, tak ho doporučuju sledovat třeba na Twitteru X, protože má velmi zajímavý projekty a velmi zajímavý pointy. Pro ty, který ho neznají, tak je to jeden ze spoluzakladatelů nebo spoluzakládajících členů Open AI a bývalý Head of AI v Tesle, kde měl spoustu let na starosti právě vývoj AI systémů pro autonomní vozidla. A pokud na vás nefungujou jména, ale spíš praktický věci, tak tenhleten člověk přišel teďka s konceptem takzvaný LLM wiky. Není to nic novýho.

**0:29** · Je to způsob, jak konsolidovat svoje znalosti pomocí Markown souborů, používat k tomu obsidián jako takový uživatelský rozhraní a vlastně pomocí AI agentů zprocesovávat tady ty znalosti, roztřizovat je a vytvářet mezi nima spojení a vlastně lokálně si budovat nějakou knowledge base. Pokud zrovna řešíte, jak si vybudovat nějakou vlastní knowledge base, který se dá jednoduše číst a pracovat s ní s AI agentama, tak tohle může bejt jedno ze zajímavejch řešení.

**0:58** · Já už jsem to zmiňoval třeba v podcastu Coffee Break s Philipem, ale používám často Notion jako knowledge base a ten je skvělej. Je to hezký uživatelský rozhraní, dá se s ním krásně pracovat, jsou tam různý databáze a podobně, ale má jednu obrovskou nevýhodu a to, že aby s ním AI agenti mohli pracovat, tak s ním musej pracovat přes takzvaný MCP a je to prostě extrémně pomalý. oproti tomu, když agent pracuje s lokálníma Markown souborama.

**1:22** · No a proto bych chtěl dneska společně s váma si postavit takovou jednoduchou LLM wiki podle Andreje Karpatyho a pokud se mi osvědčí, tak ji dál rozšiřovat a třeba ideálně vymyslet nějaký způsob, jak jí propojit s Nošem. Nicméně tak či jonak pojďme se podívat, co je to len wiky od Andreje Karpatyho, jak si ji nastavit a jak ji používat. Celý to začalo tady tím tweetem nebo Xkem, jak se tomu dneska říká.

### Princip LLM Wiki a proč Notion nestačí

**1:48** · Zkrátka postem na sociální síti XD Andrej Karpaty zmiňuje, jakým způsobem on používá takzvanou LLM lokální knowledge base. A ta premise je taková, že aby se nějaká knowledge base jednoduše udržovala, tak je potřeba to zpracování dat a to udržování udělat co nejjednodušší, protože ve chvíli, kdy bude záviset na vás jako člověku, tak to nikdy nebude tak efektivní, protože na to budem zapomínat, data budou zastarávat, nebudou se dělat ty propojení mezi nima a vkládání novejch informací bude poměrně složitý.

**2:19** · Andrej Karpate na to jde poměrně chytře. Ta jeho myšlenka je, že všechny nový věci se budou sypat do nějaký složky, třeba RA a jazykovej model nebo AI agent, tak bude inkrementálně kompilovat ty znalosti, který tam přicházejí a zařazovat je do tý viky.

**2:35** · To znamená, že vezme si třeba ty nový články, nový poznatky, záznamy ze schůzek a tak dál, zpracuje je a vlastně vloží je do tý viky nějaký sumarizovaný podobě. vytvoří tam různý prolinky, aby bylo jasný, jak ty vazby mezi nima vlastně fungujou a vytvoří z nich takzvaný MD fily.

**2:53** · On se hodně zaměřuje na různý webový články, nicméně já bych si tu wiki rád ohnul pro různý use casy, nejenom pro webový články, ale třeba pro svůj YouTube kanál, kde bych chtěl mít nějakej ton of voice, jakým způsobem funguju. Zároveň bych pak si chtěl vytvořit oddělenou wiki třeba pro svoje podnikání, pro různý konzultace, který dělám s klientama a potom třeba i nějakou knowledge base právě, jak tady naznačuje Karpaty, kdy si budu schraňovat nějaký

**3:20** · informace z internetu a budovat si nějakou vlastní tu knowledge base, kde mám uložený nějaký data. První věc, kterou k tomu budem potřebovat, tak je obsidián. Obsidianá není nic jinýho než velice propracovanej a hezkej markdown editor s pár funkcema navíc. co vám nabídne úplně v základu. Máte tady možnost si přidat nějaký volt do nějaký složky. Tam máte různý vlastně poznámky formátovaný markdownu. Můžete si mezi nima tvořit takzvaný grafy.

### Obsidian jako základ knowledge base

**3:47** · To znamená řeší se tam nějaké závislosti a zároveň si tam v canvasu můžete tvořit nějaký diagramy. Tohleto je všechno úplně zadarmo. Pokud si chcete zaplatit, tak platíte jenom za takzvanej syn a to 4 dolar, když platíte ročně nebo 5 dolarů měsíčně. No a ten syn dělá to, že vlastně vy si můžete ten Markdown propojit ve více zařízeních a můžete používat i mobilní apku, což za mě může bejt jako velmi zajímavý.

**4:13** · Já ten sync zatím budu řešit přes GitHub jako normální repozitář. později pak budu řešit, jak ho třeba zpřístupnit právě i z mobilní app. Už mám nápad, že bych ho pravděpodobně dal na MacBook a tam měl vlastně kovorka přes dispatch, aby si mohl do toho Obsidian Voltu šahat a zároveň si tam bude periodicky vlastně povat ten git repozitář a tak nějak jako obejdu vlastně tady to placení, ale uvidíme, možná doiteruju k tomu, že budu chtít řešit i tady ten syn, ale to samozřejmě uvidíme, jak se to bude rozvíjet. Nicméně potřebuju obsidián.

### Spuštění Claude Code a zadání úkolu

**4:47** · Obsidiá, když si stáhnete, tak vás vyzve k tomu, abyste si vytvořili nějaký nový trezor. Buď to můžete i rychlým startem, ale já začnu tady vytvořením trezoru. To pojmenuju AI s rozumem a umístění. Tak si tady dám procházet a půjdu do vlastně tady Filip. A už jsem si tady připravil složku CBU. Tole ještě teda smažu. To už jsem tady měl připravené. A nechám to v té složce CBU. A ono se vám tam vytvoří podsložka, která se jmenuje stejně jako jméno toho trezoru. Takže když teďka kliknu vytvořit, tak tady vidíte, že už mám připravenej ten obsidián.

**5:20** · A když si kliknu pravým a zobrazit ve Finderu, tak když se podíváte, tak Philip CBU a tady mám pak AI s rozumem a mám tady to vítejte MD. A to je vlastně tadyc ten zápis. Tole si teďka zavřu, potřebovat to nebudu a otevřu si terminál ghosty.

**5:38** · Dám si ho takhle na stranu vedle obsidiánu a v rámci ghosty tak si spustím clóda. A to je další dílek skládačky, kterj potřebujem. Potřebujem nějakýho AI agenta, kterej nám dokáže v tý složce pracovat. No a teďka už jenom tomu agentovi je nadiktuju, k čemu budu tu Wiki chtít potřebovat. Tvým cílem je implementovat mi vlastní Viky pro můj projekt AI s rozumem, kterj je edukační a slouží ke vzdělávání ve oblasti umělý inteligence. Tvořím videa na YouTube, blogový články, LinkedIn posty a další věci, přednášky a tak dál.

**6:09** · Zkrátka potřebuju někde konsolidovat jakž svoje historický znalosti a historický věci, který jsem udělal, nějaký zajímavý témata a články a pracovat s nima v kontextu tady toho projektu. Ještě jsem si tady doplnil jenom odkaz a nějaký spelling a teďka se přesunu do lmwiky.

### Použití Karpathyho specifikace jako promptu

**6:30** · To je soubor, který Andrej Karpaty poskytnul a který slouží vlastně jako takový PRD Product requirement document, kterej specifikuje, jak ta wiki má fungovat. Můžete si ho přečíst. Odkaz máte dole v popisku videa. No, ale my použijem to jako prompt pro našeho agenta. On to tady Andrej Karpaty vlastně i píše, že je designovaný, aby byl copy pastennut do LLM agenta, aby vám tu Vicky společně s váma vytvořil.

**6:55** · Takže já to tady vložím a doplním tady, že wiki a její fungování tvořne na základě této specifikace a vložím to sem. Zapínám plan modóe, protože plan mode za mě je jako vždycky dobrá volba, protože se vás ten agent doptá na různý otázky a zkrátka umožní vám ten ty věci vytvořit trošku líp. Tady si můžete všimnout, že používám plugin Superpwers na brainstorming. Mimochodem ho doporučuje. Je velmi zajímavej.

### Plan mode a brainstorming se Superpowers pluginem

**7:16** · Eh, zase uděláme na něj někdy v budoucnu video, ale dokáže vlastně trošku víc donutit Cloud koda, aby se ptal na detailnější otázky. případně vám trošku líp umí navrhovat EU UI a tak dál. Teďka vidíte, že tady máme nějakej planning, kterj probíhá. Budem odpovídat na nějaký otázky. První, co, tak se nás ptá, jestli jestli bude česky. E, v tuhletu chvíli asi budem potřebovat, aby byla v češtině, protože chci tam dávat transkripty i YouTube videí, chci s tím pracovat trošku pokročilejc.

**7:46** · Takže i přesto, že mi to vlastně nedoporučuje, že angličtina je lepší pro zpracování, tak se vydáme tou češtinou. Opět odpovídám prostě jenom aáčko. Uvidíme, co se ptá dál. Jaké typy zdrojů budeš do Viky přidávat? E, vlastní obsah, cizí články a zdroje, oboje přibližně stejně.

**8:03** · Trošku mu to upřesním, že primárně tady budou vlastní zdroje, ale inspirace o zodostatní, články z webu. Zároveň tu budou třeba moje myšlenky o směřování projektu a na co se zaměřovat. Eh, uvidíme. Ta Viky zase bude to nějakej jako živej dokument, se kterým budeme žít, takže bude se to vylepšovat. Eh, k čemu Viki primárně využiješ? Bude to přehled všeho, jak tvorba novýho psadu, přehled audit, zpráva a tak dál. Zkrátka budem to používat tak nějak ke všemu.

**8:30** · Todle všechno tomu agentovi pomáhá pochopit ten náš záměr. Jaký jsou hlavní tématický oblasti se rozumem, jak strukturovat wiky, například IL modely nástroje pro firmy, tutoriály. Zatím mu řeknu, že tady budou YouTube videa, knowledge base, kurzy a webináře a postupně budem rozšiřovat, aby se na to připravil. Zase tu knowledge base můžete časem jako restrukturovat, trošku jí upravit, není nic vytesaný do kamene, takže jako je dobrý to jako vlastně nastavit co nejlíp do začátku, ale není to nutnost.

**9:01** · Tady todle je věc z toho pluginu Superpavoru, že mi chce vizuálně ukázat, jak by to vypadalo. To tady přeskočíme, to my úplně nepotřebujem. A ptá se mě, jak budem přidávat data kombinací ideálně. Eh, buďto URL paste textu do chatu nebo soubory do složky.

**9:18** · Tam bych to viděl opravdu prostě taky, jak říkám kombinací. Tak už jsme se dostali k tomu, že budeme mít tři přístupy nějaký, který si můžem vybrat.

**9:30** · Takže pojďme se na to podívat. Vše v jedné složce minimum podadresářů.

**9:34** · Funguje dobře do 50 souborů. Potom jsou tady nějaký delší rozdělení. To si myslím, že bude vlastně jako lepší. A plně tagovaná struktura data viewu.

**9:44** · Buchá složka stránek plus bohatý Mlátor na každé stránce. i doporučeně je přístup B. Mně se to taky líbí. Eh, takže dáme přístup B, ať je to trošku jednodušší, ale zároveň je to trošku formátovaný a dá se tam přidávat víc věcí, protože tady by nám to přestalo fungovat nad nějakejch 50 stránek.

**10:03** · Samozřejmě to nějakej odhad toho agenta, ale myslím si, že je to dobrá volba to takhle líp strukturovat. Já si tady na chvilku roztáhnu terminál a podíváme se, jak to teda bude vypadat. Bude tady schéma instrukce, nějaký katalog, lok operací.

**10:18** · RA to budou zdrojový soubory, přepisy videí, coffee break episod a tak dál.

**10:22** · Jsou to zkrátka nějaký Ro soubory, se kterýma se bude pracovat. A pak je tady Wiki. To je vlastně nějaká konsolidovaná část těch znalostí. Ono to vlastně jako odpovídá do jistý míry, když se podíváte, ale vlastně tady to se bude referencovat pravděpodobně pak do toho RA. Uvidíme, jak s tím, jak s tím ten agent bude chtít pak pracovat. Ro je imutabilní, to znamená, že tam LM nikdy nezasahuje, takže tam budem vlastně jako dávat ty naše R data, ze kterých se bude vycházet.

**10:49** · Eh, ono tam ten agent bude zasahovat, protože tam bude zapisovat, ale neznamená to, že ty data tam bude upravovat. Pak je ta wiki a potom tady je projekt. To je místo pro metaobsah strategie, kam projekt směřuje a tak dál. Sup. Tak jo. Ano, pokračuji.

### Struktura složek: RAW, Wiki, Projekt

**11:08** · Tak a jdeme dál. Design formáty stránek.

**11:11** · Tak teďka nám to tady navrhuje, jak by to mohlo vlastně jako vypadat, že to bude nějaký typ, video, podcast, témata, se kterých se to týká, eh, nějaký stavy.

**11:20** · To vlastně nevím, jestli tam budem potřebovat, ale asi jo, vlastně, protože publikováno, že je to na YouTube a v přípravě, že s tím budem teprve o tom přemýšlet. stručnej souhrn, Filipův pohled, související témata, navazující video. Todle jsou nástroje, wiky témata, to jsou nějaký jasně, to jsou koncepty.

**11:40** · Wiki kurzy, wiki projekt, volnější formát, jen formátem typ. Ten ta struktura mi sedí. Jenom ještě zkusíme doplnit, že by bylo dobrý se odkazovat přímo na ty zdroje, který jsou vlastně v tý R složce. Tady opět něco, co se dá případně jako dodělat, ale tady by to ten agent e dohledával poměrně složitě.

**11:59** · Máme tady kód MD, e, kde budou nějaký konfigurace, eh jak má vypadat workflow inest, to znamená, jak zpracovávat ty data a nějaký konvence pojmenovávání. To vypadá v pohodě. Schéma vypadá dobře a zatím to necháme. Takže mu řeknem pokračuj. Myslím si, že zatím to vypadá dobře. Tak jak to bude vypadat při každodenní použití? Inest přidání nového zdroje. Elm pak projde pět kroků a aktualizuje wiki a ohlásí, co změnil. To dává smysl.

**12:30** · A já se pak budu moct zeptat, co jsem zřískal o Cloud Opus ve svých videích. Která témata mi ve Wiki chybí pro plánovaný kurz u AI agentech.

**12:39** · Dej mi přehled všech nástrojů, co jsem zrecenzoval a tak dál. S tím, že ten agent bude schopný syntetizovat ty data.

**12:46** · Lint to znamená, že vlastně projde eh ty indexy, najde nějaký mezery stránky, co tam nejsou, protože tady máme ten index, to je katalog všech těch Wiky stránky a my ho potřebujeme aktualizovat. Takže todle bude řešit ten link a log to už je jenom nějakej záznam. Za mě to vypadá dobře. Říkáme ano, pokračuj, pojďme vytvořit implementační plán. Tak a máme připravenou specifikaci. El Viky Filip provozuje vzdělávací projekt, tvoří YouTube videa, coffee break, shorts, blogový články, LinkedIn a přednášky.

**13:15** · Potřebuje konsolidovat historické a nové znalosti v češtině ten vlastně plán tady vypadá velmi dobře. Takže yes, auto accept edits a necháme agenta, aby nám zapracoval tu implementaci. A máme vytvořenej Obsidian volt, assets RAW, články a tak dál.

**13:33** · Viky, clot. Tady je vlastně popsáno, jak to má fungovat.

**13:38** · jak má clot zpracovávat ty data, jo? A vy vidíte, že to tady můžu vyloženě jenom poslat tomu agentovi a po ingestu odhlásí, kde je nová Wiki stránka, které stránky byly aktualizovány a proč.

**13:51** · Případné otázky nebo zjištěné mezery.

**13:53** · Jasně, workflow a zeptá se. Já si tady spustím Clouda ještě v novým okně, aby opravdu nemoh čerpat e z těch instrukcí, co jsme měli tady a řeknu mu, ať zpracuje posledních pět videí na YouTube AI s rozumem, ať použije nástroj YouTube DLP. a ještě mu trošku pomůžem. Vložím mu sem URL, protože to standardní fungování bude, že já si tady vkládám ty

**14:16** · data sem do toho RAW a on je odsaď zpracovává, ale já nechci teďka to tady ručně řešit, takže vlastně já ho donutím, aby si do těch rozložek ty data dostal sám a potom já s ním budu pracovat. Tak teďka stahuje h titulky pro všech těch pět videí. Koukám, že nakonec využil jinej nástroj, protože mu ten YouTube DLP nefungoval. Nicméně už stahuje všechny ty titulky. Vypadá to, že se to daří a uvidíme, kam nám to teďka uloží. Jasně, vytvoří row soubory, wikičánky a teďka spouští paralelně ten processing. Tak jo.

**14:47** · E, pojďme se podívat, co se tady děje v tom obsidiánu. Zatím tady ještě není, ale teďka si teprve jede načíst ty data. Tak a už vidíte, že se nám tady vytváří první přepis. Jo, tady koukám, že je automatický přepis. Nevím, proč je tady napsáno přepis zkrácen. Tady koukám, první věc, co se mi moc nelíbí, že eh se tady odkazuje na tydlety zdrojový soubory.

**15:10** · Tak já mu tady ještě doplním přepisy a řeknu mu, ať tam dává kompletní přepisy, protože to úplně nechcem, aby nám to tady zkracoval nebo se odkazoval do jinejch souborů, takže to nám ještě bude muset doplnit. Tak už nám je sem dává, takže super. Máme tady všechno. Konečně se na to nevyflák a nebyl línej. Tak to se někdy mimochodem s agentama děje. Já nevím proč se to děje, ale zkrátka to, že někdy se vyfláknul na to, aby tam dali všechny informace, tak mně přijde, že třeba ukódování je taková běžná věc a je potřeba si na to dávat zkrátka pozor.

**15:43** · Tak máme už tady e vlastně všechny ty přepisy a už vidíme, že se nám tady tvoří ta wiki. Máme tady cloud code Figma plugin. Když se podíváme, tak témata jsou Figma, Cloud Code, Vibe Designing, Link Carousel, stav je publikováno, odkaz na ten rdjovej soubor, kterej je vlastně tady, nějaký YouTube ID, typ a další věci. Eh, o čem to je?

### Ukázka vygenerované Wiki a propojení témat

**16:05** · Klíčový body, eh, chgpt, open claw, jasně, ostatní zajímavý postřehy, budování kontextu, přepínání nástrojů, plánování videa o tom, proč je Nusa přen škodí a další související témata. A teďka když se podívám, tak je tady vytvořenej nástroj přímo v knowledge base KB open claw.

**16:26** · Zatím tam nic k němu nedoplnil, ale když se podíváte, tak on vlastně jako prochází a vytváří ty tu knowledge base k tomu, co je to cloud kode, co je to vlastně notebook elm a další věci a vytvoří vlastně pro linky mezi nima. Tak teďka vytvoří KBY s tématama paralelně. Takže on teďka vlastně vleze do těch KB stránek, který tady připravuje a má cloud kód mezi tématama.

**16:55** · AI agenti, cloud kode, agentic nástroj od Antropicu, jak o tom Philip mluví, primární nástroj, klíčový use casy, profesní vývoj, deep research, analýzy dat Figma Design atd. atd, související videa a KB články. Todle je velmi zajímavý. Tady opět téma AI agenti, jak o tom Filip mluví ve svým obsahu.

**17:16** · Reaktivní, proaktivní agenty. Insight.

**17:19** · Cílem je nedělat z agentu prodloužený ruce, ale rovnocenný kolegy. Už tohle je za mě jako velmi působivý. A tady vidíte, že eh si vytváří vlastně ten ta naše knowledge base nebo ten agent to, jakým způsobem bude strukturovat ty věci. Takže třeba Fedma plugin, co to je, kde ho najde, když se podíváme, jestli je to on opravdu. Aha, 404.

**17:41** · Mimochodem zajímá funkce od Figmy. Tak to budem pak muset mu vynadat, že to nemá úplně správně, ale uvidíme. Třeba se ty znalostiš konsolidujou. Ale co mě na tom baví, je, že vlastně tady teďka ten agent vytváří různý vztahy mezi těma datama, co Karpaty zmiňuje. Tak a koukám, že máme hotovo. Tak se na to můžem podívat, jak se nám to roztřídil.

**18:03** · Máme tady, co bylo zpracováno, nějaký videa. Jasně. Coffee break video. Eh, v RW máme ty zdrojový videa. Eh, potom když se podíváme do indexu, tak tady máme ten mapping na ty jednotlivý soubory. Máme tady ty YouTube videa, nějaký přepisy. Eh, je vidět, že tady jsou klíčový vlastnosti, Filipů, pohled, zdroj. Můžem se prokliknout do toho Ro.

**18:27** · A co je zajímavý, tak tady jsou různý témata. Jasně, AI agenti, vibe coding a další. Co mě jakoby překvapuje, je to rozdělení mezi e KB a tématama. Ty témata jsou samozřejmě to, jak já o tom mluvím, vývoj toho tématu, jak jsem o tom třeba jako mluvil v nějakejch částech. Eh, potom třeba bych čekal, že ten cloud kód bude popsanej i tady. To je zase něco na doladění. Todle jsou věci, se kterejma si v tý Viki budete hrát, budete je propojovat.

**18:56** · Když se ptám, jak mluvím o proaktivní AI, tak agent se vlastně podívá. První, co, tak jste viděli, že si přečet ten index HTML a teďka tady vidí, že o proaktivní AI mluž kontextu agentur sám iniciuje práci. Hlavní příklad: Open claw, sleduje YouTube trendy, navrhuje témata videí, spouští code review, filozofický rámec, kterej předávám. Agenti nemají být prodloužený ruce, ale rovnocení kolegové, kterým delegujem celý odpovědnosti. Eh, mentální zátěž, parní context switching, vyčerpávající sesupovat agenty a tak dál.

**19:26** · A tady vidíte, že cituje, odkaď vlastně bral ty informace. Co Karpaty doporučuje, jak s tou Viky pracovat, vkládat tam ty zdroje do RAW nebo nechat agenta je tam vložit?

**19:37** · A Karpaty sám tady říká, že preferuje JR to jeden po druhým, čte ty summeries, čekuje ty updatey a vlastně snaží se směřovat to lm, aby ty data ukládalo tak, jak on chce. Zároveň ale můžete bečovat tychesty, to znamená dávat je do, jako jsem to udělal já třeba tady ty YouTube videa, ale je to méně supervizovaný a ty výstupy nemusí bejt kvalitní. To je třeba to, že z nějakého důvodu rozdělil Clotko do témat a ne do knowledge base. Todle by třeba za mě chtělo ještě poladit.

### Jak správně vkládat zdroje podle Karpathyho

**20:06** · Potom je ta query čast, kde se ptáte na otázky a vlastně ten agent sám prochází ty markdowny, porovnává, je schopnej pak pomocí nějakejch pluginů tvořit nějaký další věci. K tomu se ještě za chvilku dostanem a pokud najde něco zajímavýho, tak vy tu novou informaci můžete vrátit zpátky do Viky. Třeba hele, todle si zapamatuj, že to je ta správná interpretace. No a potom poslední věc je ten Lind.

**20:29** · To je vlastně to, co jsem zmiňoval, že tady je ten index a je potřeba ho nějakým způsobem přeformulovat, třeba ho někdy aktualizovat, protože tam třeba budou zapomenutý nějaký stránky. Co tady Karpate ještě zmiňuje, tak je, že za nějakou dobu člověk možná narazí na to, že ten ta index složka nebo ten index soubor je moc velkej a proto je potřeba tam přidat nějakej proper search.

**20:52** · Zmiňuje tady plugin GMD, kterej vlastně poskytuje vector search nad markdown dokumentama, což mi přijde velmi super.

**20:59** · Takže si ho můžete nainstalovat, vlastně ho používat a trošku vylepšit ten search, aby nespolíhal jenom na ten index soubor v tom obsidiánu. Co je super, tak tenhle nástroj má i CLI, což já už jsem o tom mluvil, že je to efektivnější metoda než MCP server, ale můžete použít i to klasický MCP. A pak jsou tady nějaký typy a triky. Můžete používat Obsidian Webclipper. To je, když se podíváte na ten nástroj, tak vy ho můžete si přidat takhle do prohlížeče. Já si ho takhle přidám a pak ho najdu tady v rozšířeních.

### Obsidian Web Clipper a další tipy

**21:26** · A když si na něj kliknu, tak tady v settings se můžu podívat a on mi řekne, do jakýho voltu to mám e přidávat. Já si tady zadám AI s rozumem. A teďka když půjdu zpátky třeba tady a spustím si ten obsidian highlighter, tak vidíte, že on už mi tady navrhuje, že mi to rovnou uloží do AI s rozumem. No a vy už pak jenom si tady kliknete, dáte uložit do obsidiánu a tady už vidíte, že mám ten volt AI s rozumem, nějaký ty data.

**21:53** · Můžu použít ještě highlightera, který mi vlastně umožní vybrat nějaký jako jenom zajímavý věci. Takže třeba tydle tips and tricks a můžu si dát jenom, že chci klipnout ty highlighty. E, to znamená, že můžu vybrat jenom nějaký části. Když se pak přesunu tady zpátky, dám add to obsidian, ono mi to vždycky spustí tu apku obsidian.

**22:14** · A teď jsem tady v LM Viki a ono mi to přidalo do clippings, tak já už si to pak jenom přehodím tady třeba do články a potom to můžu nechat inestnout, aby to vlastně ten agent zpracoval. Dají se tady nastavit nějaký další věci, třeba jako properties, který se mají vyplňovat a další věci. To už je pak na vás, jak s tím pluginem budete pracovat. Dalším typem je, abyste si ukládali eh ty soubory nebo obrázky lokálně, aby se k nim byl schopnej ten agent dostat.

**22:42** · Zároveň obsidianá graph view, to jsme si ještě neukazovali, tak obsidianá tady nabízí takzvanej graf.

### Graph view – vizualizace znalostí

**22:50** · Ten si můžete zobrazit takhle. No a vy se můžete podívat, jak ty informace společně souvisej. Jo, LLM wiki zatím není s něčím zařazená, ale když si tady vytáhnu Figma plugin, tak se můžete podívat, že souvisí s cloud kódem, clod aplikace průvodce, cloud kód Figma plugin, vibe coding, cloud kód a tak dál. Zároveň, když si tady vemu cloud kód, tak souvisí s nějakjma tématama, který tady mám.

**23:12** · A samozřejmě já tadyc ty eh vlastnosti nebo tady ty delší věci, tak jsem schopnej tady nechat konsolidovat, protože třeba teďka tady vidíte, že e vibe coding, tak ne napřímo a jo, souvisí s cloud codem, tak v tom případě cloud code je tady dvakrát z nějakého důvodu, ale tydlety věci já jsem schopnej pak nechávat vlastně trošku konsolidovat toho agenta, aby je

**23:35** · zpracoval, jo, takže vidím tady open clow, v jakejch epizodách jsem o něm mluvil, nějaký napojení a další věci, takže tenhle grafoj view může bejt Tady je to velmi zajímavá pomůcka, která vám pomůže vizualizovat tu vaši knowledge base. Zároveň existuje takový rozšíření, který se jmenuje MARP a nechá nebo umožní vám tvořit eh vlastně slide deck, což znamená tak jako prezentace přímo z toho vašeho obsahu.

**23:55** · Data viw, tak to je pak nějaký datový pohledy nad těma e datama vašima. a Vicky, tak je vlastně lokální soubor, je to git repo, takže vy si to můžete komitnout a dát to třeba do nějakýho GitHubu a pracovat s tím jako s projektem normálně, kterej byste programovali. Tohle byla taková rychlá ukázka Viky, se kterou přišel Andrej Karpaty, lmky. Je to opravdu jen takový nastínění, co se to snaží dělat, proč to v tom obsidiánu může fungovat a jak by se to dalo strukturovat.

### Shrnutí a proč je lokální přístup silný

**24:23** · Já si s tím teďka v následujících týdnech budu pravděpodobně hrát a jsem zvědavej, kam mě to posune, protože já třeba jsem ještě paralelně předtím, než vyšla tady ta LLM wiki nebo tady ten přístup, tak jsem si začal tvořit svůj vlastní nástroj, vektorovou databázi, kde mám vlastně veškerej obsah svejch videí a jsem schopnej z nich čerpat. Ale tohle mi možná přijde trošku zajímavější, protože zaprvý to nikde nemusím hostovat, běží to lokálně a zároveň e je to propojený s mnohem více datama a nemusím to jako složitě programovat.

**24:54** · Jsou to prostě markdown soubory. Jsem sám strašně zvědavej, ne, taký limity narazím, jak se mi to bude používat a jak se mi s tím obecně bude pracovat, ale tenhleten koncept mít vlastně nějakou knowledge base, do který ten agent může zapisovat a můžu s ní nějak jako pracovat, tak mi přijde velmi silnej. A to, že je to lokálně, tak přidává obrovskou hodnotu, protože ty AI agenti jsou schopní s lokálníma souborama pracovat mnohem efektivnějc.

**25:18** · Dejte mi vědět do komentáře, co si o LLM Viki myslíte. Jestli tady ten přístup vám dává smysl, nebo jestli jste ho třeba už zkoušeli a jakou s tím máte zkušenost. Já sám jsem zvědavej. Tak říkám, nemůžu to zatím doporučit, ale ten přístup mi přijde minimálně zajímavej. Já se jmenuju Filip Oborník z projektu AI s rozumem. Díky moc, že jste se dívali. Budu se na vás těšit u dalšího dílu podcastu Coffee Break nebo u dalšího videa na YouTube a nebo u podcastu Deep Show, kterj najdete na YouTube, Spotify a dalších podcastovejch platformách pod názvem Deepling Show.

**25:45** · No nebo pochopitelně v naší Discord komunitě AI s rozumím, která je úplně zadarmo. Ještě jednou díky moc, mějte se krásně a budu se na vás těšit opět příště.
![](https://www.youtube.com/watch?v=orkQdaic_Nk)

## Transcript

### Úvod a dnešní téma

**0:00** · Krásný den. Vítejte u dalšího dílu podcastu Coffee Break s Filipem. Doufám, že pijete taky něco dobrého. Já tady mám obět dneska kávu a dnešním tématem je kontext. A to vlastně z pohledu toho, jak to funguje, je to, že nějaký nástroje a modely o vás vědí víc věcí, než nějaký jiný, jak s kontextem pracovat a jak k němu přistupovat.

**0:21** · Zkrátka to nastavení tý hlavy, jak s ním vlastně jako pracovat. Pro začátek si myslím, že jako extrémně důležitý si říct, jak to funguje, když model si o vás něco pamatuje. Někdy se setkávám s dojmem toho, že když si povídám s nějakým AI modelem, tak vlastně on se učí z toho, jak já si s ním povídám. To ale není pravda. Žádnej z dnešních komerčních modelů tak neumí na základě konverzace, kterou s ním mám, se vlastně jako dotrénovat a přizpůsobovat se mě na míru.

### Jak modely "pamatují"

**0:52** · Jsou tady různý pokusy, jakým jak to dělat. tady to učení eh zaběhu svěch konverzací přesně pro vás, ale to není v tuhletu chvíli jako aktuální pro ty konzumerský modely, to znamená ty modely, který normálně používáme.

### Model jako bezstavová krabička

**1:08** · Zkrátka funguje to tak, že ten AI model je prostě jakási krabička a do ní jde nějakej vstup a z ní jde výstup a ten model nemá žádný jako stav, je bezstavový. To znamená, že on si o vás vlastně nic moc nepamatuje, jenom prostě to, co šlo dovnitř a to, co ven. Pomiňme pro některý, kdo jste pokročilejší, třeba kehšování, tam to je trošku složitější, ale zkrátka ten model si není schopnej zapamatovat, že jste se včera nebo předevčírem o něco o čem bavili. Na základě toho se přizpůsobit a odpovědět vám.

**1:39** · To, jak nějaký aplikace jako je či GPT nebo Cloud a další jako docílej tady toho efektu, že to vypadá, že si o vás něco pamatuje, že když mu řeknete,"Hele, kdo jsem," tak on vám napíše vy: "Jo, ty jsi Filip, děláš projekty aj s rozumem" atd. atd. Tak to funguje tak, že ten model sám o sobě si nic neukládá, ale ten nástroj, který je postavenj kolem toho modelu, tak si ukládá určitý střípky informací o vás a

### Jak ChatGPT simuluje paměť

**2:07** · můžete si to představit jako normální textový soubory nebo jako Word dokumenty. Budíš. Ono ve výsledku to jsou opravdu jenom texťáky, který se někde jako ukládají, ale jsou to nějaký útržky informací, který někde naš jako jsi našel nebo spíš konsolidoval během toho, co jste si bavili.

**2:23** · Takže například vy budete mít nějaký dlouhej chat, budete se bavit o nějakém vašem podnikání a Open AI například, tak na pozadí bude dělat to, že bude se ten chat analyzovat a zjistí třeba aha, tak Philip se věnuje tady AI s rozumem projektu a tudletu informaci si uloží do paměti opravdu fakt do nějaký databáze nebo jako texťák nějakej si to můžete představit fakt jenom tady to jako textově.

**2:47** · A příště, když si s tím modelem jdu povídat, tak ten model ještě předtím, než dostane tu moji otázku, na kterou se ptám, tak se předto díky tý aplikaci, čpt, ve kterým si to běží, tak se před to vlastně jako přilepí nějaký tady ty informace, který o mně ví. Takže to pak vypadá, že je tam nějakej systémovej prompt. Pak je tam tady jsou údaje, co víš o uživateli. Filip Oborník dělá projekt, já se rozumím, bla bla bla.

**3:13** · A teď začíná ta naše konverzace a vlastně já se ptám modelu na něco a on už ale všechny tydlety informace v rámci toho promptu vlastně dostal. Eh, jasně, někdy je to složitější. Ve chvíli, kdy těch informací je hodně, ty nástroje uměj vyhledávat třeba i v historickejch četech, tak tam pak jsou nějaký složitější techniky, ale ve výsledku všechno to funguje tak, že se to natáhne do toho kontextovýho okna.

**3:36** · A proto třeba někdy, když ty nástroje používáte, tak máte pocit, že ta konzumace těch tokenů je jako větší, než když jste napsali ahoj a najednou to sežrou spoustu tokenů, tak je to kvůli tomu, že se tam natáhnul tady ten kontext. Eh, funguje to úplně podobně v AI agentech, jako je Cloud COD, Codex a delší. Ty zas nepoužívají tady ty memories, ale eh nebo oni mají taky vlastní systém memories, tam se to jako ukládá vyloženě na disk ty soubory, případně je konfigurujete pomocí Cloud MD a dalších jako souborů.

### Kontextové okno a tokeny

**4:06** · Ale ta důležitá věc, kterou si z toho odnýst, je modely jsou bezstavový a fakt si nepamatujou to, co jste si s nima povídali. Do budoucna to tak možná bude, teď to tak není. No a todle podle mě otvírá tu debatu o tom, jak vlastně pracovat s tím kontextem, protože zkuste si schválně jít třeba do nástroje openrouter.ai a vyzkoušet si tam různý modely.

### Experiment s OpenRouterem

**4:30** · A tu samou otázku, co napíšete do chat GPT, který používáte pravidelně, nebo pokud používáte Clouda, tak to napište tam, tak dejte úplně stejnýmu modelu v tom Open routeru a uvidíte, že dostanete úplně jinou odpověď. nebo zkuste možná ještě jednodušší anonymní režim nebo ten režim dočasnýho chatu, který má jak cloud, tak i chat GPT. Napište tu samou otázku do toho anonymního chatu a pak i do toho klasickýho a uvidíte, že ty odpovědi budou jako úplně jiný.

**4:57** · Tak a v tu chvíli vlastně to ukazuje ten efekt toho, že když ten model nemá přístup k tomu kontextu, tak je vlastně ty ty odpovědi nebudou tak personalizovaný.

**5:12** · Nechci říct kvalitní, protože někdy zase ten kontext, který mu dáte nebo ke kterýmu má přístup, tak může ovlivňovat tu kvalitu těch vašich odpovědí. Pokud ten vlastně jako nástroj si uloží někde v memories, že vy máte rádi, že ten model se k vám chová hezky a přikivuje vám, tak on vám bude i nadále přikyovat, což nemusí bejt to, co vy chcete. Takže na todle je důležitý myslet, že ty odpovědi v těch klasickejch četěch těch nástrojů jsou ovlivněný tím kontextem, co už tam je.

**5:38** · No, ale jak s tím kontextem vlastně pracovat, když chci třeba používat CGPTa nebo další systémy, zkrátka nechci bejt zavřenej v nějakém jednom ekosystému.

### AI agenti a lokální knowledge base

**5:53** · Když používáte ty chatovací asistenty, tak tam je to extrémně složitý, protože oni mají vlastní systémy, jak pracovat s těma e vzpomínkama, jak pracovat vlastně s těma eh uloženejma datama, takže tam je opravdu jako velmi složitý přenášet informace. Nicméně ve chvíli, kdy přejdete do světa AI agentů, který běžej u vás na počítači, Cloud COD, Codex, RZ Cowork, eh, a další jako agenti, který běží u vás na počítači, tak tam se to dá dělat poměrně jednoduše.

**6:22** · A funguje to tak, že vlastně vy necháte toho agenta zapisovat všechny tydlety věci do nějakýho souboru. Eh, typicky to může bejt TXT nebo Markdown. Markdown je lepší, je trošku jako formátovanější, dá se líp číst, dá se tam zdůrazňovat nějaký věci. No a vy ho necháte to zapisovat do těhle textových souborů.

**6:42** · Vlastně postupně, jak používáte toho agenta, tak si budujete takzvanou knowledge base, memory, paměť, mozek, záleží, jak tomu budete chtít říkat, ale zkrátka postupně inkrementálně si jako zlepšujete ten kontext, co mu poskytujete. A je to pak hodně e o tom vlastně si odladit tady ten styl.

**6:59** · Pro každýho bude trošku jako jinej, ale před pár týdny, tak Andrej Karpaty, tak pokud to neznáte, spoluzakladatel Open AI a taky Head of AI v Tesle bejvalej, tak zveřejnil na GitHubu něco, čemu říká, čím se to jmenuje LLM Vicky, eh, nebo AI Wiki, odkaz vám dám do popisku a tam

### LLM Wiki od Karpathyho

**7:22** · vlastně ukazuje to, jak on by si strukturoval nějakou knowledge base nebo jak on s tím pracuje a má vlastně Marko soubory. v nějakým nějaký složce, má to nějak rozstrukturovaný podle toho, jak potřebuje a nechává AI agenty, aby z těch konverzací, co společně mají nebo z nějakejch článků, co třeba jako ho zaujali a tak dál, tak si tvořili takzvaný memories, doptávali se ho na nějaký nejasnosti a konsolidovali vlastně tu paměť.

**7:47** · E, malá taková odbočka, pokud jste sledovali únik clot kódu, tak jedna z věcí, co se tam hodně řešila, tak je modelos a jeho funkce Autodream. nebo Dream, kde vlastně ten model běží na pozadí, i když vy nepoužíváte cloud kóda a konsoliduje ten kontext, přemjšlí nad ním a vlastně tak nějak jako vytváří si nějakou lepší strukturu. Tak tadyc ta vlastně LLM wiki tak je jako dosti podobná eh tomuhle.

**8:18** · Akorát to děláte vlastně jako vědomě, tam to ta je designovaný, že to poběží na pozadí. Takže jako ta práce s tím kontextem je vidět, že se začíná jako dostávat nebo začíná se jí dávat velká pozornost, protože to je opravdu to, co pak odlišuje ty kvalitní odpovědi od těch nekvalitních, protože dneska ty modely, ty Frontier modely jsou opravdu na dosti podobný úrovni a vy jim potřebujete dát ten kvalitní kontext.

### Důležitost správy kontextu

**8:43** · Eh, já budu dělat video na YouTube, jak si vytvořit tady tu LLM paměť, eh, kterou má Andrej Karpaty, nebo možná už na YouTubu je. Pokud je, tak odkaz máte zase dole v popisku videa a tak tam bude třeba zajímavý sledovat, jak se s tím kontextem dá pracovat jako pokročilejc.

**8:59** · Nicméně ve chvíli, kdy pracujete s těma agentama, máte to uložený na disku u vás, tak není jednodušší ho to synchronizovat přes obsidián nebo Google disk nebo si to nahrát do GitHub repozitáře, tvořit z toho různý pluginy a tak dál a zkrátka eh mít tu vaši knowledge base přenositelnou.

**9:17** · Další možností je to mít třeba jako v notionu. Já používám taky často notion, ale ten má jednu obrovskou nevýhodu. Je zkrátka pro ten nástroj strašně pomalý si do toho notionu šahat a vlastně získávat ty data z něj v porovnání s tím, když to máte zapsaný přímo na disku v nějakejch Markdown souborech nebo v texťích.

**9:35** · Takže já teďka řeším to, jakým způsobem tu svojí paměť jako vyřešit, aby jsem jí poskytnul agentům lokálně, aby s ním fungovali rychle, ale zároveň abych to měl zálohovaný třeba právě pomocí toho notionu, protože mě zas jako velmi vyhovuje. A to mě dostává trošku jako k třetímu bodu, proč to řeším takhle, proč třeba to všechno naleju do Clouda a je do jeho paměti.

**9:59** · A to je vlastně jako další myšlenka tohodle videa a ta je taková, že se snažím být tool agnostik a tak se k tomu př snažím přistupovat v rámci zprávy celýho svýho kontextu. Tool agnostic znamená to, že nechci se uzavřít do nějakýho ekosystému. Já bych mohl spolíhat na třeba aplikaci Clot desktopovou a říkat muelehe ulož si todle do memories a tak dál. Ale pak pro mě bude strašně těžký tu platformu opustit.

### Proč být tool agnostik

**10:25** · Takže já na spoustu práce s kontextem, tak používám cloud koda nebo cororka, protože ty běžej u mě lokálně na počítači a snažím se je instruovat, aby veškerý znalosti buďto ukládaly do notionu nebo do lokálních souborů. To znamená, že když pak přijde nějaký super duper AI agent někdy v budoucnu, tak já mu ho jenom nasměruju, hele, tady máš kontext, nějak si s tím pracuj, ale nebudu muset řešit to, že to musím nějak složitě vydolovávat z toho či GPT nebo z clóu, což nikdy stejně tak kvalitně neuděláte.

**10:57** · Na druhou stranu to chce trošku víc práce, když si ten kontakt spravujete sami, ale myslím, že se to vyplatí a to je opravdu ta myšlenka toho bejt tool agnostic. eh zkrátka jako přemýšlet, kde ten kontext máte a jak se k němu chováte, protože myslím si, že v budoucnu to bude důležitější víc než kdy předtím, protože ty agenti se dneska jako extrémně zlepšujou a ve chvíli, kdy vy jste

**11:23** · schopný tam nalejt dostatečně relevantní kontext, tak ty odpovědi jsou prostě víc personalizovaný a víc vám to jde na ruku.

### Nástroje jako zdroj kontextu (MCP)

**11:31** · To ještě mě přivádí k další myšlence, protože jedna věc jsou tady ty soubory, ty lokální vlastně ukládání toho kontextu, konfigurační soubory a tak, ale druhá část tý práce s tím kontextem, která jde s tím vlastně jako rukou dvorce, tak je jsou nástroje.

**11:48** · Eh, možná to zní trošku jako ne nebo jak to říct, jako nezní to jako, že to s tím tolik souvisí, ale já vnímám nástroje, že slouží ke dvoum věcem, těm agentům. Buďto k provádění úkolu, to se nás v tomhleom tématu jako tolik netýká, a nebo právě k získávání kontextu. Takže kromě toho, že máte nějaký kontext lokálně nebo v tom nástroji, tak zároveň ale můžete připojit další služby.

**12:12** · Já typicky připojuju GitHub, připojuju Notion, připojuju Notebook Lem a další vlastně jako služby a umožňuju tomu AI agentovi se do nich napojit, získat si kontext, kterej vlastně potřebuje bez toho, aniž bych já mu eh musel říkat. A to je podle mě jako delší extrémně důležitá věc.

**12:35** · Dejte těm agentům přístup tam. kde se jim může hodit. Samozřejmě řeďte ty přístupy. Já třeba do kalendáře, tak má jenom read only přístup a podobný věci, aby moh nemohl vlastně jako nadělat paseku. Ale zkrátka tady ty kontexty jsou za mě eh tak jako důležitý.

**12:52** · \[odkašlání\] Takže ten přístup k tomu kontextu můžete řešit nejenom těma lokálníma souborama, ale i právě nějakýma toama, MCP, který vám umožňuj se tam napojit.

**13:05** · Tak když bych to měl shrnout, samozřejmě je důležitý pořád si vybírat nástroje, modely atd, ale za mě teď je a bude extrémně důležitej ten kontext, takže zkuste nad tím přemýšlet takhle, ať už to děláte pro sebe nebo třeba ve firmě, tak jak sdílet ten kontext, jak ten kontext dostat do těch nástrojů a ideálně se nezamknout do nějakýho jednoho nástroje tím, že tam nalejete všechny data, protože pak se vám bude těžko odcházet. To je ta hlavní message.

### Investice do kontextu se vyplatí

**13:35** · Prostě přemýšlejte nad tím kontextem jako to, co má vobrovskou hodnotu a myslím si, že se jako vyplatí investovat čas do toho, abyste si vytvořili tu zprávu toho svýho kontextu. Protože copak jako se děje? Já když budu chtít řešit nějaký třeba nový video nebo grafiku pro AI s rozumem, tak já nemusím tomu Moslemelu znova vysvětlovat. Já jsem Filip Oborník, dělám AI s rozumem.

**14:02** · Tady najdeš můj brand manuál ve Figmě.

**14:05** · Tady najdeš v Notionu popisy toho, co dělám. Tady je můj web. Tady je design systém a tak dál. Nemusím to vysvětlovat. Já mu jenom řeknu:„Hele, prosím tě, pojďme vytvořit tady grafiku pro thumbnail, pro nový video nebo návrh. A on už sám je schopnej si říct, aha, potřebuju asi nějakým způsobem vyřešit thumbnail. To znamená, potřebuju design guide, potřebuju se podívat na předchozí thumbnaily, vím, kde je najdu, protože to mám v těch konfiguračních souborch. Díky nástrojům si můžu šáhnout do Figmy, takže si tam něco můžu stáhnout a zkrátka ví, kde to najít.

### Skilly pro navigaci kontextem

**14:37** · Ještě taková doplňovačka k tomu. Vy samozřejmě spoustu takovejdlech promptů třeba budete psát jako častějc a je dobrý třeba si na to tvořit skilly. To znamená eh pomoct tomu modelu eh najít ten kontext. Zase skilly můžou sloužit ke spoustě věcí. Máte to jako prompt šablony a další věci, ale zároveň mu můžete tím pomoct najít kontext, protože skill třeba v clóu, tak funguje tak, že on si ho může ten agent zavolat sám. A jako obdobná věc existuje v ostatních AI agentech.

**15:08** · Já teďka používám Cloda, ale protože ho používám prostě dnes a denně, ale jako podobný koncepty jsou i v jinejch AI agentech, tak vlastně vy tomu v tom skillu můžete nadefinovat, hele, tenhle skill použij, když si chceš zjistit brand manuál třeba nebo zjistit nějaký prostě věci ohledně vizuálu brandu. No a v tom skillu pak budete mít prompt, kterej řekne, hele, načti si tady ten soubor, kde jsou prostě uvedený barvičky a další brand guidelines. V tomhletom souboru pak bude rozsník.

**15:35** · Hele, když potřebuješ thumbnaily, tak jsou tady. Když potřebuješ tohle, tak je to támhle. A zkrátka budujete takovou mapičku, takovou mind mapu toho, kam se ten model má podívat a on si prostě najde cloud MD třeba, jo, tu hlavní konfiguraci. Tam bude napsáno, pokud řešíš e něco s designem, tak tady je odkaz na skill eh brand manuál, nebo to tomu modelu samo samo jako dojde. To už záleží, on si ho jako spustí, nebo to může bejt nějakej soubor, on to nemusí bejt skill. Jo, jako eh těch cest je tam spousta.

**16:06** · To je zas na nějaký úplně jiný video, ale zkrátka jako nasměrováváte model, aby on se prokousával tím kontextem, protože vy nejste schopný vzít veškerý kontext a nalejt ho do kontextýho okna. To nebude fungovat efektivně, ani to prostě dělat nechcete, ale zároveň musíte tomu modelu dát nějakou cestičku, jak se tam prokousat.

**16:24** · Takže za mě je dobrý ten kontext jako strukturovat, ať už nějaký složkový struktuře, rozcestníkama do těch nástrojů a tak dál.

### Kontext jako živý dokument

**16:33** · Zároveň je dobrý přemýšlet nad tím kontextem a těma konfiguračníma soubora, že to jsou živý dokumenty. To znamená, budete je pořád upravovat, budou vznikat nový, budou se stávat nevalidníma, budou tam neplatný odkazy.

**16:48** · Takže zase je potřeba ten kontext vnímat, že je to taková nekončící hra nebo spíš nekončící údržba, ale vyplatí se to. Takže začteno, potrženo.

**17:01** · Kontext je extrémně důležitá věc při práci s AI a myslím si, že bude důležitější a důležitější. A pokud už teďka si nastavíte správný fungování s vaším kontextem, tak vám to pomůže.

**17:13** · Cílem toho podcastu nebylo tak nějak jako říct přesný metody, protože ono se to opravdu liší pro každý nástroje, který používáte, jaký máte workflow, jestli máte tým, jestli jste sami. A těch jako proměnnejch je tam prostě celá řada. Ale zkrátka ta myšlenka byla nastínit vám, proč ten kontext je důležitj, jak fungujou trošku ty jazykový modelyy, že jsou vlastně bezstavový, že byste se tím měli zabývat a vlastně jako naznačit nějaký cestičky, kudy by to mohlo jít.

### Závěr a pozvánka

**17:42** · To je za mě všechno pro tady tu epizodu podcastu Coffee break. Já se jmenuju Filip Oborník z projektu AI s rozmem.

**17:47** · Budu rád, když mi dáte vědět do komentáře, jak třeba kontext, ať už na projektech vlastních nebo třeba firemní nebo osobní řešíte vy. Jestli to řešíte v těch nástrojích jako takovejch, nebo se snažíte bejt právě tool a gnostik, abyste se nezamkli do nějakýho ekosystému a řešíte to v rámci nějakejch agentů. Zkrátka k tomu kontextu přistupujete, můžete mi to napsat do komentáře dole pod video nebo podcast a nebo můžete se přidat do naší komunity AI s rozumem na Discordu, kde můžem tedy ty témata probírat taky.

**18:18** · A v neposlední řadě bych vás rád pozval k poslechu dalšího podcastu, nejenom Coffee breaku, ale i podcastu Deepling Show, kterej tvořím se svým kolegou Jindřichem a bavíme se o různejch tématech ze světa AI. Jsou tam různý pohledy. Můj víc technickej, Jindřichů zase víc tak jako produktovej a byznysovej a zároveň plánujem si v blízký době zvát hosty. Takže se máte určitě na co těšit.

**18:45** · E ten podcast najdete na YouTube, Spotify a dalších podcastovejch platformách pod názvem Deeplink Show. Díky moc, že jste poslouchali, že jste se dívali. Eh, mějte se krásně a budu se na vás těšit u dalšího videa.